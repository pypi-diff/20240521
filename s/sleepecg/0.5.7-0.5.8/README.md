# Comparing `tmp/sleepecg-0.5.7.tar.gz` & `tmp/sleepecg-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepecg-0.5.7.tar", last modified: Thu Feb  8 08:37:14 2024, max compression
+gzip compressed data, was "sleepecg-0.5.8.tar", last modified: Tue May 21 09:38:43 2024, max compression
```

## Comparing `sleepecg-0.5.7.tar` & `sleepecg-0.5.8.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.024023 sleepecg-0.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.004023 sleepecg-0.5.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-08 08:36:54.000000 sleepecg-0.5.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.004023 sleepecg-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-08 08:36:54.000000 sleepecg-0.5.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-08 08:36:54.000000 sleepecg-0.5.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-08 08:36:54.000000 sleepecg-0.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-08 08:36:54.000000 sleepecg-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-02-08 08:36:54.000000 sleepecg-0.5.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-02-08 08:36:54.000000 sleepecg-0.5.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-08 08:36:54.000000 sleepecg-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-08 08:36:54.000000 sleepecg-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-02-08 08:37:14.024023 sleepecg-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-08 08:36:54.000000 sleepecg-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.008023 sleepecg-0.5.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.008023 sleepecg-0.5.7/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/api/classification.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/api/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/api/datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/api/feature_extraction.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/api/heartbeat_detection.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/api/plot.md
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/classification.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/configuration.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.008023 sleepecg-0.5.7/docs/css/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/feature_extraction.md
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/heartbeat_detection.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.008023 sleepecg-0.5.7/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)    65092 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/img/ecgrecord_plot.svg
--rw-r--r--   0 runner    (1001) docker     (127)    72215 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/img/gudb_pearson.svg
--rw-r--r--   0 runner    (1001) docker     (127)   255311 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/img/hypnogram.svg
--rw-r--r--   0 runner    (1001) docker     (127)    38376 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/img/ltdb_runtime_logscale.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60774 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/img/mitdb_metrics.svg
--rw-r--r--   0 runner    (1001) docker     (127)    66358 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/img/plot_ecg.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32231 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/img/wrn-gru-mesa-weighted.svg
--rw-r--r--   0 runner    (1001) docker     (127)    31357 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/img/wrn-gru-mesa.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.012023 sleepecg-0.5.7/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/plot.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.000023 sleepecg-0.5.7/docs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.000023 sleepecg-0.5.7/docs/templates/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.000023 sleepecg-0.5.7/docs/templates/python/material/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.012023 sleepecg-0.5.7/docs/templates/python/material/docstring/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/templates/python/material/docstring/parameters.html
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/templates/python/material/docstring/returns.html
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-08 08:36:54.000000 sleepecg-0.5.7/docs/templates/python/material/docstring/yields.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.012023 sleepecg-0.5.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.012023 sleepecg-0.5.7/examples/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/benchmark/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/benchmark/benchmark_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/benchmark/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/benchmark/plot_benchmark_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/benchmark/requirements-benchmark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.012023 sleepecg-0.5.7/examples/classifiers/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/classifiers/wrn_gru_mesa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/classifiers/wrn_gru_mesa_weighted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-08 08:36:54.000000 sleepecg-0.5.7/examples/classifiers/ws_gru_mesa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-08 08:36:54.000000 sleepecg-0.5.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-02-08 08:36:54.000000 sleepecg-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-08 08:36:54.000000 sleepecg-0.5.7/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 08:37:14.024023 sleepecg-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-08 08:36:54.000000 sleepecg-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.012023 sleepecg-0.5.7/sleepecg/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/_heartbeat_detection.c
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/_heartbeat_detection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19356 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.016023 sleepecg-0.5.7/sleepecg/classifiers/
--rw-r--r--   0 runner    (1001) docker     (127)   775585 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/classifiers/wrn-gru-mesa-weighted.zip
--rw-r--r--   0 runner    (1001) docker     (127)   764383 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/classifiers/wrn-gru-mesa.zip
--rw-r--r--   0 runner    (1001) docker     (127)   775057 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/classifiers/ws-gru-mesa.zip
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.020023 sleepecg-0.5.7/sleepecg/data/
--rw-r--r--   0 runner    (1001) docker     (127)   166750 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/data/ecg.npz
--rw-r--r--   0 runner    (1001) docker     (127)    26643 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    27467 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/heartbeats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.020023 sleepecg-0.5.7/sleepecg/io/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/io/ecg_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    29277 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/io/gudb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/io/nsrr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/io/physionet.py
--rw-r--r--   0 runner    (1001) docker     (127)    24243 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/io/sleep_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.020023 sleepecg-0.5.7/sleepecg/test/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/test/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/test/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/test/test_heartbeat_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/test/test_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/test/test_sleep_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-02-08 08:36:54.000000 sleepecg-0.5.7/sleepecg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 08:37:14.020023 sleepecg-0.5.7/sleepecg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-02-08 08:37:13.000000 sleepecg-0.5.7/sleepecg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-08 08:37:14.000000 sleepecg-0.5.7/sleepecg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 08:37:13.000000 sleepecg-0.5.7/sleepecg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-08 08:37:13.000000 sleepecg-0.5.7/sleepecg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-08 08:37:13.000000 sleepecg-0.5.7/sleepecg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.780413 sleepecg-0.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.764413 sleepecg-0.5.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-21 09:38:35.000000 sleepecg-0.5.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.764413 sleepecg-0.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-21 09:38:35.000000 sleepecg-0.5.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-21 09:38:35.000000 sleepecg-0.5.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 09:38:35.000000 sleepecg-0.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-21 09:38:35.000000 sleepecg-0.5.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-21 09:38:35.000000 sleepecg-0.5.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-21 09:38:35.000000 sleepecg-0.5.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-21 09:38:35.000000 sleepecg-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-21 09:38:43.780413 sleepecg-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-21 09:38:35.000000 sleepecg-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.768413 sleepecg-0.5.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.768413 sleepecg-0.5.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/api/classification.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/api/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/api/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/api/feature_extraction.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/api/heartbeat_detection.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/api/plot.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/classification.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/configuration.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.768413 sleepecg-0.5.8/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/feature_extraction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/heartbeat_detection.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.768413 sleepecg-0.5.8/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    65092 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/img/ecgrecord_plot.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    72215 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/img/gudb_pearson.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   255311 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/img/hypnogram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    38376 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/img/ltdb_runtime_logscale.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60774 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/img/mitdb_metrics.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    66358 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/img/plot_ecg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32231 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/img/wrn-gru-mesa-weighted.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    31357 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/img/wrn-gru-mesa.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.768413 sleepecg-0.5.8/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/plot.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.760413 sleepecg-0.5.8/docs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.760413 sleepecg-0.5.8/docs/templates/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.760413 sleepecg-0.5.8/docs/templates/python/material/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.772413 sleepecg-0.5.8/docs/templates/python/material/docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/templates/python/material/docstring/parameters.html
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/templates/python/material/docstring/returns.html
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-21 09:38:35.000000 sleepecg-0.5.8/docs/templates/python/material/docstring/yields.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.772413 sleepecg-0.5.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.772413 sleepecg-0.5.8/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/benchmark/benchmark_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/benchmark/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/benchmark/plot_benchmark_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/benchmark/requirements-benchmark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.772413 sleepecg-0.5.8/examples/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/classifiers/wrn_gru_mesa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/classifiers/wrn_gru_mesa_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-21 09:38:35.000000 sleepecg-0.5.8/examples/classifiers/ws_gru_mesa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-21 09:38:35.000000 sleepecg-0.5.8/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-21 09:38:35.000000 sleepecg-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-21 09:38:35.000000 sleepecg-0.5.8/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:38:43.780413 sleepecg-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-21 09:38:35.000000 sleepecg-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.764413 sleepecg-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.772413 sleepecg-0.5.8/src/sleepecg/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/_heartbeat_detection.c
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/_heartbeat_detection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.776413 sleepecg-0.5.8/src/sleepecg/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)    59729 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/classifiers/wrn-gru-mesa-weighted.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    59765 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/classifiers/wrn-gru-mesa.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    59741 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/classifiers/ws-gru-mesa.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.776413 sleepecg-0.5.8/src/sleepecg/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   166750 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/data/ecg.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27467 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/heartbeats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.776413 sleepecg-0.5.8/src/sleepecg/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/io/ecg_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/io/gudb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/io/nsrr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/io/physionet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24224 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/io/sleep_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-21 09:38:35.000000 sleepecg-0.5.8/src/sleepecg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.776413 sleepecg-0.5.8/src/sleepecg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-21 09:38:43.000000 sleepecg-0.5.8/src/sleepecg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-21 09:38:43.000000 sleepecg-0.5.8/src/sleepecg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:38:43.000000 sleepecg-0.5.8/src/sleepecg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-21 09:38:43.000000 sleepecg-0.5.8/src/sleepecg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:38:43.000000 sleepecg-0.5.8/src/sleepecg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:43.776413 sleepecg-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 09:38:35.000000 sleepecg-0.5.8/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-21 09:38:35.000000 sleepecg-0.5.8/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-21 09:38:35.000000 sleepecg-0.5.8/tests/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-21 09:38:35.000000 sleepecg-0.5.8/tests/test_heartbeat_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-21 09:38:35.000000 sleepecg-0.5.8/tests/test_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-05-21 09:38:35.000000 sleepecg-0.5.8/tests/test_sleep_readers.py
```

### Comparing `sleepecg-0.5.7/.github/workflows/release.yml` & `sleepecg-0.5.8/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     name: Pre-commit checks
     runs-on: ubuntu-22.04
     steps:
     - uses: actions/checkout@v4
     - uses: actions/setup-python@v5
       with:
         python-version: '3.12'
-    - uses: pre-commit/action@v3.0.0
+    - uses: pre-commit/action@v3.0.1
 
 
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
 
     strategy:
       matrix:
         os: [ubuntu-22.04, windows-2022, macos-14]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.16.5
+        uses: pypa/cibuildwheel@v2.18.0
 
       - uses: actions/upload-artifact@v4
         with:
           name: artifact-${{ matrix.os }}
           path: ./wheelhouse/*.whl
 
 
@@ -68,11 +68,11 @@
     steps:
       - uses: actions/download-artifact@v4
         with:
           pattern: artifact-*
           merge-multiple: true
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.11
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `sleepecg-0.5.7/.github/workflows/test.yml` & `sleepecg-0.5.8/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name: Pre-commit checks
     runs-on: ubuntu-22.04
     steps:
     - uses: actions/checkout@v4
     - uses: actions/setup-python@v5
       with:
         python-version: '3.12'
-    - uses: pre-commit/action@v3.0.0
+    - uses: pre-commit/action@v3.0.1
 
 
   test:
     needs: [pre-commit]
     name: Test on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
 
@@ -36,13 +36,13 @@
       matrix:
         os: [ubuntu-22.04, windows-2022, macos-14]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Build wheels and run pytest
-        uses: pypa/cibuildwheel@v2.16.5
+        uses: pypa/cibuildwheel@v2.18.0
 
       - uses: actions/upload-artifact@v4
         with:
           name: artifact-${{ matrix.os }}
           path: ./wheelhouse/*.whl
```

### Comparing `sleepecg-0.5.7/CHANGELOG.md` & `sleepecg-0.5.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## [0.5.8] - 2024-05-21
+### Changed
+- Switch to Keras 3 classifiers ([#217](https://github.com/cbrnr/sleepecg/pull/217) by [Clemens Brunner](https://github.com/cbrnr))
+
 ## [0.5.7] - 2024-02-08
 ### Added
 - Add support for Python 3.12 ([#207](https://github.com/cbrnr/sleepecg/pull/207) by [Clemens Brunner](https://github.com/cbrnr))
 
 ## [0.5.6] - 2023-12-22
 ### Changed
 - Use [edfio](https://github.com/the-siesta-group/edfio) for reading and writing EDF files ([#195](https://github.com/cbrnr/sleepecg/pull/195) by [Florian Hofer](https://github.com/hofaflo))
```

### Comparing `sleepecg-0.5.7/CONTRIBUTING.md` & `sleepecg-0.5.8/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,21 +92,21 @@
 in the project or package root. The tests for the C extension can be excluded using
 ```
 pytest -m "not c_extension"
 ```
 
 ## Releases
 Follow these steps to release a new version of SleepECG:
-- In `sleepecg/__init__.py` remove the `-dev` suffix in `__version__`.
+- In `src/sleepecg/__init__.py` remove the `-dev` suffix in `__version__`.
     - In case of a patch release, modify the version number accordingly.
 - In `CHANGELOG.md`, update `## [UNRELEASED] - YYYY-MM-DD` to contain the version number and current date.
 - Commit these changes as `Prepare vX.Y.Z release` and push.
 - [Create a new release](https://github.com/cbrnr/sleepecg/releases/new) on GitHub.
     - Create a new tag where the target version is prefixed with a `v`, e.g. `v0.4.0`.
     - Use the tag as the release title.
     - Mention the most important changes in the release description and include a link to the changelog.
 - This triggers the [`release.yml`](https://github.com/cbrnr/sleepecg/blob/main/.github/workflows/release.yml) workflow, which builds the wheels and publishes the package on [PyPI](https://pypi.org/project/sleepecg).
 
 This concludes the new release. Now prepare the source for the next planned release as follows:
-- Update `__version__` in `sleepecg/__init__.py` to the next planned version and append `-dev`.
+- Update `__version__` in `src/sleepecg/__init__.py` to the next planned version and append `-dev`.
 - Start a new section at the top of `CHANGELOG.md` titled `## [UNRELEASED] - YYYY-MM-DD`.
 - Commit these changes as `Prepare vX.Y.Z-dev` and push.
```

### Comparing `sleepecg-0.5.7/LICENSE` & `sleepecg-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/PKG-INFO` & `sleepecg-0.5.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: sleepecg
-Version: 0.5.7
+Version: 0.5.8
 Summary: A package for sleep stage classification using ECG data
 Author-email: Florian Hofer <hofaflo@gmail.com>, Clemens Brunner <clemens.brunner@gmail.com>
 License: BSD 3-Clause
 Project-URL: homepage, https://github.com/cbrnr/sleepecg
 Project-URL: documentation, https://sleepecg.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/cbrnr/sleepecg
 Project-URL: changelog, https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md
 Keywords: sleep,ecg,qrs,peak
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
@@ -22,40 +25,34 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: PyYAML>=5.4.0
 Requires-Dist: requests>=2.25.0
 Requires-Dist: scipy>=1.7.0
 Requires-Dist: tqdm>=4.60.0
 Provides-Extra: full
-Requires-Dist: edfio>=0.1.1; extra == "full"
+Requires-Dist: edfio>=0.4.0; extra == "full"
 Requires-Dist: joblib>=1.0.0; extra == "full"
 Requires-Dist: matplotlib>=3.5.0; extra == "full"
-Requires-Dist: numba>=0.59.0; extra == "full"
-Requires-Dist: tensorflow>=2.7.0; python_version < "3.12" and extra == "full"
+Requires-Dist: numba>=0.59.1; extra == "full"
+Requires-Dist: tensorflow>=2.16.1; extra == "full"
 Requires-Dist: wfdb>=3.4.0; extra == "full"
 Provides-Extra: dev
-Requires-Dist: edfio>=0.1.1; extra == "dev"
-Requires-Dist: joblib>=1.0.0; extra == "dev"
-Requires-Dist: matplotlib>=3.5.0; extra == "dev"
-Requires-Dist: mkdocs-material>=8.4.0; extra == "dev"
-Requires-Dist: mkdocstrings-python>=0.7.1; extra == "dev"
+Requires-Dist: sleepecg[doc]; extra == "dev"
+Requires-Dist: sleepecg[full]; extra == "dev"
 Requires-Dist: mypy>=0.991; extra == "dev"
-Requires-Dist: numba>=0.59.0; extra == "dev"
 Requires-Dist: pre-commit>=2.13.0; extra == "dev"
 Requires-Dist: pytest>=6.2.0; extra == "dev"
-Requires-Dist: ruff>=0.1.8; extra == "dev"
+Requires-Dist: ruff>=0.4.0; extra == "dev"
 Requires-Dist: setuptools>=56.0.0; extra == "dev"
-Requires-Dist: tensorflow>=2.7.0; python_version < "3.12" and extra == "dev"
-Requires-Dist: wfdb>=3.4.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: mkdocs-material>=8.4.0; extra == "doc"
 Requires-Dist: mkdocstrings-python>=0.8.2; extra == "doc"
 Provides-Extra: cibw
-Requires-Dist: edfio>=0.1.1; extra == "cibw"
-Requires-Dist: numba>=0.59.0; extra == "cibw"
+Requires-Dist: edfio>=0.4.0; extra == "cibw"
+Requires-Dist: numba>=0.59.1; extra == "cibw"
 Requires-Dist: wfdb>=3.4.0; extra == "cibw"
 
 ![Python](https://img.shields.io/pypi/pyversions/sleepecg.svg?logo=python&logoColor=white)
 [![PyPI](https://img.shields.io/pypi/v/sleepecg)](https://pypi.org/project/sleepecg/)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/sleepecg.svg?label=conda-forge)](https://anaconda.org/conda-forge/sleepecg)
 [![Docs](https://readthedocs.org/projects/sleepecg/badge/?version=latest)](https://sleepecg.readthedocs.io/en/stable/index.html)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05411/status.svg)](https://doi.org/10.21105/joss.05411)
@@ -116,25 +113,25 @@
 
 
 ### Dependencies
 
 SleepECG requires Python ≥ 3.9 and the following packages:
 
 - [numpy](https://numpy.org/) ≥ 1.20.0
+- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
 - [requests](https://requests.readthedocs.io/en/latest/) ≥ 2.25.0
 - [scipy](https://scipy.org/) ≥ 1.7.0
 - [tqdm](https://tqdm.github.io/) ≥ 4.60.0
-- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
 
 Optional dependencies provide additional features:
 
-- [edfio](https://github.com/the-siesta-group/edfio/) ≥ 0.1.1 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
+- [edfio](https://github.com/the-siesta-group/edfio/) ≥ 0.4.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
 - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
 - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
-- [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-- [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
+- [numba](https://numba.pydata.org/) ≥ 0.59.1 (JIT-compiled heartbeat detector)
+- [tensorflow](https://www.tensorflow.org/) ≥ 2.16.1 (sleep stage classification with Keras models)
 - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
 
 
 ### Contributing
 
 The [contributing guide](https://github.com/cbrnr/sleepecg/blob/main/CONTRIBUTING.md) contains detailed instructions on how to contribute to SleepECG.
```

### Comparing `sleepecg-0.5.7/README.md` & `sleepecg-0.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,25 @@
 
 
 ### Dependencies
 
 SleepECG requires Python ≥ 3.9 and the following packages:
 
 - [numpy](https://numpy.org/) ≥ 1.20.0
+- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
 - [requests](https://requests.readthedocs.io/en/latest/) ≥ 2.25.0
 - [scipy](https://scipy.org/) ≥ 1.7.0
 - [tqdm](https://tqdm.github.io/) ≥ 4.60.0
-- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
 
 Optional dependencies provide additional features:
 
-- [edfio](https://github.com/the-siesta-group/edfio/) ≥ 0.1.1 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
+- [edfio](https://github.com/the-siesta-group/edfio/) ≥ 0.4.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
 - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
 - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
-- [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-- [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
+- [numba](https://numba.pydata.org/) ≥ 0.59.1 (JIT-compiled heartbeat detector)
+- [tensorflow](https://www.tensorflow.org/) ≥ 2.16.1 (sleep stage classification with Keras models)
 - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
 
 
 ### Contributing
 
 The [contributing guide](https://github.com/cbrnr/sleepecg/blob/main/CONTRIBUTING.md) contains detailed instructions on how to contribute to SleepECG.
```

### Comparing `sleepecg-0.5.7/docs/classification.md` & `sleepecg-0.5.8/docs/classification.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/configuration.md` & `sleepecg-0.5.8/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/datasets.md` & `sleepecg-0.5.8/docs/datasets.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/examples.md` & `sleepecg-0.5.8/docs/examples.md`

 * *Files 0% similar despite different names*

```diff
@@ -165,16 +165,16 @@
 ## Using a built-in classifier
 
 ```python
 import matplotlib.pyplot as plt
 
 from sleepecg import load_classifier, plot_hypnogram, read_slpdb, stage
 
-# the model was built with tensorflow 2.7, running on higher versions might create warnings
-# but should not influence the results
+# the model was built with tensorflow 2.16.1, running on higher versions might create
+# warnings, but should not influence the results
 clf = load_classifier("ws-gru-mesa", "SleepECG")
 
 # load record
 # `ws-gru-mesa` performs poorly for most SLPDB records, but it works well for slp03
 rec = next(read_slpdb("slp03"))
 
 # predict stages and plot hypnogram
```

### Comparing `sleepecg-0.5.7/docs/feature_extraction.md` & `sleepecg-0.5.8/docs/feature_extraction.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/heartbeat_detection.md` & `sleepecg-0.5.8/docs/heartbeat_detection.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/img/ecgrecord_plot.svg` & `sleepecg-0.5.8/docs/img/ecgrecord_plot.svg`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/img/gudb_pearson.svg` & `sleepecg-0.5.8/docs/img/gudb_pearson.svg`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/img/hypnogram.svg` & `sleepecg-0.5.8/docs/img/hypnogram.svg`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/img/ltdb_runtime_logscale.svg` & `sleepecg-0.5.8/docs/img/ltdb_runtime_logscale.svg`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/img/mitdb_metrics.svg` & `sleepecg-0.5.8/docs/img/mitdb_metrics.svg`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/img/plot_ecg.svg` & `sleepecg-0.5.8/docs/img/plot_ecg.svg`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/img/wrn-gru-mesa-weighted.svg` & `sleepecg-0.5.8/docs/img/wrn-gru-mesa-weighted.svg`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/img/wrn-gru-mesa.svg` & `sleepecg-0.5.8/docs/img/wrn-gru-mesa.svg`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/index.md` & `sleepecg-0.5.8/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 ## Changelog
 Check out the [changelog](https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md) to learn what we added, changed, or fixed.
 
 ## Dependencies
 SleepECG requires Python ≥ 3.9 and the following packages:
 
 - [numpy](https://numpy.org/) ≥ 1.20.0
+- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
 - [requests](https://requests.readthedocs.io/en/latest/) ≥ 2.25.0
 - [scipy](https://scipy.org/) ≥ 1.7.0
 - [tqdm](https://tqdm.github.io/) ≥ 4.60.0
-- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
 
 Optional dependencies provide additional features:
 
-- [edfio](https://github.com/the-siesta-group/edfio/) ≥ 0.1.1 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
+- [edfio](https://github.com/the-siesta-group/edfio/) ≥ 0.4.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
 - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
 - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
-- [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-- [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
+- [numba](https://numba.pydata.org/) ≥ 0.59.1 (JIT-compiled heartbeat detector)
+- [tensorflow](https://www.tensorflow.org/) ≥ 2.16.1 (sleep stage classification with Keras models)
 - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
 
 ## Installation
 SleepECG is available on PyPI and can be installed with [pip](https://pip.pypa.io/en/stable/):
 
 ```
 pip install sleepecg
```

### Comparing `sleepecg-0.5.7/docs/plot.md` & `sleepecg-0.5.8/docs/plot.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/templates/python/material/docstring/parameters.html` & `sleepecg-0.5.8/docs/templates/python/material/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/templates/python/material/docstring/returns.html` & `sleepecg-0.5.8/docs/templates/python/material/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/docs/templates/python/material/docstring/yields.html` & `sleepecg-0.5.8/docs/templates/python/material/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/examples/benchmark/README.md` & `sleepecg-0.5.8/examples/benchmark/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 # Heartbeat detection benchmarks
+
 This example reproduces the benchmarks shown in the [docs](https://sleepecg.readthedocs.io/en/latest/heartbeat_detection.html).
 
 ## Usage
+
 To run the benchmark, create a virtual environment and install the requirements with:
+
 ```
 pip install -r requirements-benchmark.txt
 ```
 
 Then execute
+
 ```
 python benchmark_detectors.py [<benchmark>]
 ```
+
 where the optional `[<benchmark>]` argument is a top-level key in `config.yml` (see section [Configuration](#configuration)). Possible values are `runtime`, `metrics`, and `rri_similarity`. If not provided, the `runtime` benchmark is executed.
 
 Plots can be created by executing
+
 ```
 python plot_benchmark_results.py <results.csv>
 ```
+
 which will save the plot to `<results>.svg` at the same location as `<results>.csv`. Plot types and labels for the provided benchmarks are selected based on the filename, so renaming may lead to errors.
 
 
 ## Configuration
+
 A benchmark configuration is specified below a unique top-level key in `config.yml`.
+
 |Key|Type|Default|Description|
 |---|----|--------|-----------|
 |`data_dir`|`str`|`'~/.sleepecg/datasets'`|Path where all datasets are stored. Required files will be downloaded if they don't exist.|
 |`outfile_dir`|`str`|`'.'`|Path where the evaluation results should be stored.|
 |`db_slug`|`str`||Which dataset to use for evaluation. Possible values: [`mitdb`](https://physionet.org/content/mitdb/1.0.0/), [`ltdb`](https://physionet.org/content/ltdb/1.0.0/), [`gudb`](https://github.com/berndporr/ECG-GUDB).|
 |`export_records`|`bool`|`False`|Whether to export all records from a benchmark as text files (in `outfile_dir`).|
 |`detectors`|`list[str]`||Detectors to be evaluated. For possible options, see [`utils.detector_dispatch`](https://github.com/cbrnr/sleepecg/blob/main/examples/benchmark/utils.py#L51-L94).|
 |`signal_lengths`|`list[int]`||Length in minutes to which each ECG signal should be sliced. If a signal is too short, it is skipped.|
 |`max_distance`|`float`|`0.1`|Maximum temporal distance in seconds between detected and annotated beats to count as a successful detection.|
 |`suppress_warnings`|`bool`|`False`|Whether to suppress warnings during detector execution.|
 |`calc_rri_similarity`|`bool`|`False`|Whether to calculate similarity measures between detected and annotated RR intervals (computationally expensive for long signals).|
 
+
 ## Known issues
+
 - `heartpy` detection will fail for mitdb:105:V1, mitdb:115:V1, mitdb:200:V1, and mitdb:201:V1. It raises a `BadSignalWarning`, which is caught in `utils.evaluate_single`.
 - For signal lengths starting somewhere between 600 and 900 minutes, the `heartpy` detector takes at least several hours for ltdb:15814:ECG2.
-- For signal lengths starting somewhere between 300 and 600 minutes, `wfdb-xqrs` takes at least 20 times longer for ltdb:14134:ECG2 and ltdb:14184:ECG2 than for the other ltdb records.
+- For signal lengths starting somewhere between 300 and 600 minutes, `wfdb-xqrs` takes at least 20 times longer for ltdb:14134:ECG2 and ltdb:14184:ECG2 than for the other records.
```

### Comparing `sleepecg-0.5.7/examples/benchmark/benchmark_detectors.py` & `sleepecg-0.5.8/examples/benchmark/benchmark_detectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     cfg = yaml.safe_load(config_file)
 
 try:
     cfg = cfg[benchmark]
 except KeyError:
     raise ValueError(f"Invalid benchmark: {benchmark!r}, available: {list(cfg)}.") from None
 
-
 if cfg.get("suppress_warnings", False):
     warnings.filterwarnings("ignore")
 
 outfile_dir = Path(cfg.get("outfile_dir", "."))
 outfile_dir.mkdir(parents=True, exist_ok=True)
 
 db_slug = cfg["db_slug"]
@@ -66,24 +65,20 @@
     "TP",
     "FP",
     "FN",
 ]
 if cfg.get("calc_rri_similarity", False):
     fieldnames += ["pearsonr", "spearmanr", "rmse"]
 
-# Trigger imports and jit compilation to make runtime benchmarks representative
+# trigger imports and jit compilation to make runtime benchmarks representative
 for detector in cfg["detectors"]:
     detector_dispatch(records[0].ecg[: 10 * records[0].fs], records[0].fs, detector)
 
-
 with open(csv_filepath, "w", newline="") as csv_file:
-    writer = csv.DictWriter(
-        csv_file,
-        fieldnames=fieldnames,
-    )
+    writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
     writer.writeheader()
     for signal_len in cfg["signal_lengths"]:
         print(f"==== Signal length: {signal_len} minutes ====")
         for detector in cfg["detectors"]:
             detector_results = []
             for record in tqdm(records, desc=detector, leave=False, disable=True):
                 if len(record.ecg) < signal_len * record.fs * 60:
```

### Comparing `sleepecg-0.5.7/examples/benchmark/config.yml` & `sleepecg-0.5.8/examples/benchmark/config.yml`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/examples/benchmark/plot_benchmark_results.py` & `sleepecg-0.5.8/examples/benchmark/plot_benchmark_results.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/examples/benchmark/utils.py` & `sleepecg-0.5.8/examples/benchmark/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # License: BSD (3-clause)
 
 """Utilities for runtime and detection quality benchmarks."""
 
 from __future__ import annotations
 
 import time
-from typing import Any, Iterator
+from collections.abc import Iterator
+from typing import Any
 
 import numpy as np
-
 import sleepecg
 from sleepecg.io.ecg_readers import ECGRecord
 
 
 class HeartpyWarning(Warning):
     """Warning for all Heartpy-related warnings."""
 
@@ -167,17 +167,15 @@
         )
 
         if calc_rri_similarity:
             pearsonr, spearmanr, rmse = sleepecg.rri_similarity(detection, annotation)
 
     except HeartpyWarning:
         runtime = np.nan
-        TP = []
-        FP = []
-        FN = annotation
+        TP, FP, FN = [], [], annotation
 
         if calc_rri_similarity:
             pearsonr = np.nan
             spearmanr = np.nan
             rmse = np.nan
 
     result = {
@@ -189,15 +187,9 @@
         "max_distance": max_distance,
         "runtime": runtime,
         "TP": len(TP),
         "FP": len(FP),
         "FN": len(FN),
     }
     if calc_rri_similarity:
-        result.update(
-            {
-                "pearsonr": pearsonr,
-                "spearmanr": spearmanr,
-                "rmse": rmse,
-            }
-        )
+        result.update({"pearsonr": pearsonr, "spearmanr": spearmanr, "rmse": rmse})
     return result
```

### Comparing `sleepecg-0.5.7/examples/classifiers/wrn_gru_mesa_weighted.py` & `sleepecg-0.5.8/examples/classifiers/wrn_gru_mesa.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,121 @@
-# %%
-from tensorflow.keras import layers, models
-from tqdm import tqdm
+import warnings
 
 from sleepecg import (
     evaluate,
     extract_features,
     load_classifier,
     prepare_data_keras,
     print_class_balance,
     read_mesa,
     read_shhs,
     save_classifier,
     set_nsrr_token,
 )
+from tensorflow.keras import layers, models
+from tqdm import tqdm
 
-# %% Read data and extract features
 set_nsrr_token("your-token-here")
-records = list(read_mesa())
 
-feature_extraction_params = {
-    "lookback": 120,
-    "lookforward": 150,
-    "feature_selection": [
-        "hrv-time",
-        "hrv-frequency",
-        "recording_start_time",
-        "age",
-        "gender",
-    ],
-    "min_rri": 0.3,
-    "max_rri": 2,
-    "max_nans": 0.5,
-}
-
-features_train, stages_train, feature_ids = extract_features(
-    tqdm(records),
-    **feature_extraction_params,
-    n_jobs=-2,
-)
-
-# %% Merge sleep stages, pad and mask data as preparation for keras NN
-stages_mode = "wake-rem-nrem"
-
-features_train_pad, stages_train_pad, sample_weight = prepare_data_keras(
-    features_train,
-    stages_train,
-    stages_mode,
-)
-print_class_balance(stages_train_pad, stages_mode)
-
-# %% Define and train model
-model = models.Sequential(
-    [
-        layers.Input((None, features_train_pad.shape[2])),
-        layers.Masking(-1),
-        layers.BatchNormalization(),
-        layers.Dense(64),
-        layers.ReLU(),
-        layers.Bidirectional(layers.GRU(8, return_sequences=True)),
-        layers.Bidirectional(layers.GRU(8, return_sequences=True)),
-        layers.Dense(stages_train_pad.shape[-1], activation="softmax"),
-    ]
-)
-
-model.compile(
-    optimizer="rmsprop",
-    loss="categorical_crossentropy",
-    metrics=["accuracy"],
-)
-model.build()
-model.summary()
-
-# %% Train model
-model.fit(
-    features_train_pad,
-    stages_train_pad,
-    epochs=25,
-    sample_weight=sample_weight,
-)
-
-# %% Store classifier
-save_classifier(
-    name="wrn-gru-mesa-weighted",
-    model=model,
-    stages_mode=stages_mode,
-    feature_extraction_params=feature_extraction_params,
-    mask_value=-1,
-    classifiers_dir="./classifiers",
-)
+TRAIN = True  # set to False to skip training and load classifier from disk
 
-# %% Load classifier from disk for validation
-clf = load_classifier("wrn-gru-mesa-weighted", "./classifiers")
+# silence warnings (which might pop up during feature extraction)
+warnings.filterwarnings(
+    "ignore", category=RuntimeWarning, message="HR analysis window too short"
+)
+
+if TRAIN:
+    print("‣  Starting training...")
+    print("‣‣ Extracting features...")
+    records = list(read_mesa(offline=False))
+
+    feature_extraction_params = {
+        "lookback": 120,
+        "lookforward": 150,
+        "feature_selection": [
+            "hrv-time",
+            "hrv-frequency",
+            "recording_start_time",
+            "age",
+            "gender",
+        ],
+        "min_rri": 0.3,
+        "max_rri": 2,
+        "max_nans": 0.5,
+    }
+
+    features_train, stages_train, feature_ids = extract_features(
+        tqdm(records),
+        **feature_extraction_params,
+        n_jobs=-1,
+    )
+
+    print("‣‣ Preparing data for Keras...")
+    stages_mode = "wake-rem-nrem"
+
+    features_train_pad, stages_train_pad, _ = prepare_data_keras(
+        features_train,
+        stages_train,
+        stages_mode,
+    )
+    print_class_balance(stages_train_pad, stages_mode)
+
+    print("‣‣ Defining model...")
+    model = models.Sequential(
+        [
+            layers.Input((None, features_train_pad.shape[2])),
+            layers.Masking(-1),
+            layers.BatchNormalization(),
+            layers.Dense(64),
+            layers.ReLU(),
+            layers.Bidirectional(layers.GRU(8, return_sequences=True)),
+            layers.Bidirectional(layers.GRU(8, return_sequences=True)),
+            layers.Dense(stages_train_pad.shape[-1], activation="softmax"),
+        ]
+    )
+
+    model.compile(
+        optimizer="rmsprop",
+        loss="categorical_crossentropy",
+        metrics=["accuracy"],
+    )
+    model.build()
+    model.summary()
+
+    print("‣‣ Training model...")
+    model.fit(
+        features_train_pad,
+        stages_train_pad,
+        epochs=25,
+    )
+
+    print("‣‣ Saving classifier...")
+    save_classifier(
+        name="wrn-gru-mesa",
+        model=model,
+        stages_mode=stages_mode,
+        feature_extraction_params=feature_extraction_params,
+        mask_value=-1,
+        classifiers_dir="./classifiers",
+    )
+
+print("‣  Starting testing...")
+print("‣‣ Loading classifier...")
+clf = load_classifier("wrn-gru-mesa", "./classifiers")
 
-# %% Read data and extract features
-shhs = list(read_shhs())
+print("‣‣ Extracting features...")
+shhs = list(read_shhs(offline=False))
 
 features_test, stages_test, feature_ids = extract_features(
     tqdm(shhs),
     **clf.feature_extraction_params,
     n_jobs=-2,
 )
 
-# %% Predict & evaluate
+print("‣‣ Evaluating classifier...")
 features_test_pad, stages_test_pad, _ = prepare_data_keras(
     features_test,
     stages_test,
     clf.stages_mode,
 )
 y_pred = clf.model.predict(features_test_pad)
 evaluate(stages_test_pad, y_pred, clf.stages_mode)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sleepecg-0.5.7/mkdocs.yml` & `sleepecg-0.5.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/pyproject.toml` & `sleepecg-0.5.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
-requires = ["setuptools", "oldest-supported-numpy"]
+requires = ["setuptools", "setuptools-scm", "oldest-supported-numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sleepecg"
 description = "A package for sleep stage classification using ECG data"
 license = {text = "BSD 3-Clause"}
 authors = [
     {name = "Florian Hofer", email = "hofaflo@gmail.com"},
     {name = "Clemens Brunner", email = "clemens.brunner@gmail.com"},
 ]
+readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "License :: OSI Approved :: BSD License",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
@@ -25,50 +29,44 @@
 dependencies = [
     "numpy >= 1.20.0",
     "PyYAML >= 5.4.0",
     "requests >= 2.25.0",
     "scipy >= 1.7.0",
     "tqdm >= 4.60.0",
 ]
-dynamic = ["version", "readme"]
+dynamic = ["version"]
 
 [project.optional-dependencies]
 full = [  # complete package functionality
-    "edfio >= 0.1.1",
+    "edfio >= 0.4.0",
     "joblib >= 1.0.0",
     "matplotlib >= 3.5.0",
-    "numba >= 0.59.0",
-    "tensorflow >= 2.7.0; python_version < '3.12'",
+    "numba >= 0.59.1",
+    "tensorflow >= 2.16.1",
     "wfdb >= 3.4.0",
 ]
 
 dev = [  # everything needed for development
-    "edfio >= 0.1.1",
-    "joblib >= 1.0.0",
-    "matplotlib >= 3.5.0",
-    "mkdocs-material >= 8.4.0",
-    "mkdocstrings-python >= 0.7.1",
+    "sleepecg[doc]",
+    "sleepecg[full]",
     "mypy >= 0.991",
-    "numba >= 0.59.0",
     "pre-commit >= 2.13.0",
     "pytest >= 6.2.0",
-    "ruff >= 0.1.8",
+    "ruff >= 0.4.0",
     "setuptools >= 56.0.0",
-    "tensorflow >= 2.7.0; python_version < '3.12'",
-    "wfdb >= 3.4.0",
 ]
 
 doc = [  # RTD uses this when building the documentation
     "mkdocs-material >= 8.4.0",
     "mkdocstrings-python >= 0.8.2",
 ]
 
 cibw = [  # cibuildwheel uses this for running the test suite
-    "edfio >= 0.1.1",
-    "numba >= 0.59.0",
+    "edfio >= 0.4.0",
+    "numba >= 0.59.1",
     "wfdb >= 3.4.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/cbrnr/sleepecg"
 documentation = "https://sleepecg.readthedocs.io/en/latest/"
 repository = "https://github.com/cbrnr/sleepecg"
@@ -87,16 +85,14 @@
 [tool.cibuildwheel.macos]
 archs = "x86_64 arm64"
 
 [tool.cibuildwheel.windows]
 archs = "AMD64"
 
 [tool.mypy]
-packages = ["sleepecg"]
-exclude = '^sleepecg/test/'
 ignore_missing_imports = true
 disallow_untyped_defs = true
 warn_unreachable = true
 strict_equality = true
 pretty = true
 
 [tool.pytest.ini_options]
@@ -104,28 +100,23 @@
 filterwarnings = [
     "error",
     'ignore:.*datetime.datetime.utcfromtimestamp\(\):DeprecationWarning',
     'ignore:(?s).*Pyarrow:DeprecationWarning',
 ]
 
 [tool.ruff]
-select = ["D", "E", "F", "I", "W"]
 line-length = 92
-ignore = ["D105"]
 exclude = ["setup.py"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint]
+select = ["D", "E", "F", "I", "W", "UP"]
+ignore = ["D105"]
+
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "**/examples/*.py" = ["D100"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.setuptools.dynamic]
 version = {attr = "sleepecg.__version__"}
-readme = {file = "README.md", content-type = "text/markdown"}
-
-[tool.setuptools.packages.find]
-exclude = ["examples"]
-
-[tool.setuptools.package-data]
-"*" = ["*.pyi"]
```

### Comparing `sleepecg-0.5.7/sleepecg/__init__.py` & `sleepecg-0.5.8/src/sleepecg/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 from sleepecg.config import get_config, set_config
 from sleepecg.feature_extraction import extract_features, preprocess_rri
 from sleepecg.heartbeats import compare_heartbeats, detect_heartbeats, rri_similarity
 from sleepecg.io import *  # noqa: F403
 from sleepecg.plot import plot_ecg, plot_hypnogram
 from sleepecg.utils import get_toy_ecg
 
-__version__ = "0.5.7"
+__version__ = "0.5.8"
```

### Comparing `sleepecg-0.5.7/sleepecg/_heartbeat_detection.c` & `sleepecg-0.5.8/src/sleepecg/_heartbeat_detection.c`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/sleepecg/classification.py` & `sleepecg-0.5.8/src/sleepecg/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from __future__ import annotations
 
 import shutil
 from dataclasses import dataclass
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Any, Optional, Protocol
+from typing import Any, Protocol
 from zipfile import ZipFile
 
 import numpy as np
 import yaml
 
 from sleepecg.config import get_config
 from sleepecg.feature_extraction import extract_features
@@ -86,15 +86,15 @@
     # influence the class weights -> slice with [1:]
     class_weight = np.sum(stage_counts[1:]) / stage_counts
     sample_weight = class_weight[stages_padded]
 
     return features_padded, stages_padded_onehot, sample_weight
 
 
-def print_class_balance(stages: np.ndarray, stages_mode: Optional[str] = None) -> None:
+def print_class_balance(stages: np.ndarray, stages_mode: str | None = None) -> None:
     """
     Print the number of samples and percentages of each class in `stages`.
 
     Parameters
     ----------
     stages : np.ndarray
         A 2D array of shape `(n_records, n_samples)` containing integer class labels or a
@@ -127,16 +127,16 @@
 
 
 def save_classifier(
     name: str,
     model: Any,
     stages_mode: str,
     feature_extraction_params: dict[str, Any],
-    mask_value: Optional[int] = None,
-    classifiers_dir: Optional[str | Path] = None,
+    mask_value: int | None = None,
+    classifiers_dir: str | Path | None = None,
 ) -> None:
     """
     Save a trained classifier to disk.
 
     The `model` itself and a `.yml` file containing classifier metadata are stored as
     `<name>.zip` in `classifiers_dir`. Model serialization is performed as suggested by the
     respective package documentation. Currently only Keras models are supported.
@@ -179,27 +179,25 @@
         classifier_info["mask_value"] = mask_value
 
     with TemporaryDirectory() as tmpdir:
         with open(f"{tmpdir}/info.yml", "w") as infofile:
             yaml.dump(classifier_info, infofile)
 
         if model_type == "keras":
-            model.save(f"{tmpdir}/classifier")
+            model.save(f"{tmpdir}/classifier.keras")
         else:
             raise ValueError(f"Saving model of type {type(model)} is not supported")
 
         shutil.make_archive(str(target_file), "zip", tmpdir)
 
 
 class _Model(Protocol):
-    def fit(self, X: np.ndarray, y: np.ndarray) -> None:
-        ...
+    def fit(self, X: np.ndarray, y: np.ndarray) -> None: ...
 
-    def predict(self, X: np.ndarray) -> np.ndarray:
-        ...
+    def predict(self, X: np.ndarray) -> np.ndarray: ...
 
 
 @dataclass
 class SleepClassifier:
     """
     Store a sleep classifier model and metadata.
 
@@ -224,16 +222,16 @@
         `None`.
     """
 
     model: _Model
     stages_mode: str
     feature_extraction_params: dict[str, Any]
     model_type: str
-    mask_value: Optional[int] = None
-    source_file: Optional[Path] = None
+    mask_value: int | None = None
+    source_file: Path | None = None
 
     def __repr__(self) -> str:
         if self.source_file is not None:
             return (
                 f"<SleepClassifier | {self.stages_mode}, {self.model_type}, "
                 f"{self.source_file.name}>"
             )
@@ -247,15 +245,15 @@
             f"    model type: {self.model_type}\n"
             f"    source file: {self.source_file}\n"
         )
 
 
 def load_classifier(
     name: str,
-    classifiers_dir: Optional[str | Path] = None,
+    classifiers_dir: str | Path | None = None,
     silence_tf_messages: bool = True,
 ) -> SleepClassifier:
     """
     Load a `SleepClassifier` from disk.
 
     This functions reads `.zip` files saved by `save_classifier()`. Pass `'SleepECG'` as the
     second argument to load a classifier bundled with SleepECG.
@@ -301,15 +299,15 @@
             environ_orig = os.environ.copy()
             if silence_tf_messages:
                 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 
             from tensorflow import keras
 
             try:
-                classifier = keras.models.load_model(f"{tmpdir}/classifier")
+                classifier = keras.models.load_model(f"{tmpdir}/classifier.keras")
             finally:
                 os.environ.clear()
                 os.environ.update(environ_orig)
 
         else:
             raise ValueError(
                 f"Loading model of type {classifier_info['model_type']} is not supported"
@@ -318,15 +316,15 @@
     return SleepClassifier(
         model=classifier,
         source_file=soure_file,
         **classifier_info,
     )
 
 
-def list_classifiers(classifiers_dir: Optional[str | Path] = None) -> None:
+def list_classifiers(classifiers_dir: str | Path | None = None) -> None:
     """
     List available classifiers.
 
     Parameters
     ----------
     classifiers_dir : str | pathlib.Path, optional
         Directory in which to look for classifiers. If `None` (default), the value is taken
```

### Comparing `sleepecg-0.5.7/sleepecg/config.py` & `sleepecg-0.5.8/src/sleepecg/config.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/sleepecg/data/ecg.npz` & `sleepecg-0.5.8/src/sleepecg/data/ecg.npz`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/sleepecg/feature_extraction.py` & `sleepecg-0.5.8/src/sleepecg/feature_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # License: BSD (3-clause)
 
 """Functions and utilities related to feature extraction."""
 
 from __future__ import annotations
 
 import warnings
-from typing import Iterable, Optional
+from collections.abc import Iterable
 
 import numpy as np
 from numpy.lib.stride_tricks import sliding_window_view
 from scipy.interpolate import interp1d
 from scipy.signal import periodogram
 
 from sleepecg.io.sleep_readers import SleepRecord
@@ -61,14 +61,15 @@
 
 _TIME_DOMAIN_EXPECTED_WARNING_MESSAGES = (
     "All-NaN slice encountered",
     "Degrees of freedom <= 0 for slice",
     "divide by zero encountered in divide",
     "divide by zero encountered in log10",
     "invalid value encountered in sqrt",
+    "invalid value encountered in divide",
     "Mean of empty slice",
 )
 
 
 def _create_ragged_array(data: list[np.ndarray]) -> np.ndarray:
     """
     Convert a list of arrays with different lengths to a numpy array.
@@ -501,16 +502,16 @@
                 f"{min_window_time:.1f}s required, got {window_time}s"
             )
             warnings.warn(msg, category=RuntimeWarning)
 
 
 def preprocess_rri(
     rri: np.ndarray,
-    min_rri: Optional[float] = None,
-    max_rri: Optional[float] = None,
+    min_rri: float | None = None,
+    max_rri: float | None = None,
 ) -> np.ndarray:
     """
     Replace invalid RRI samples with `np.nan`.
 
     Parameters
     ----------
     rri : np.ndarray
@@ -674,18 +675,18 @@
 
 
 def extract_features(
     records: Iterable[SleepRecord],
     lookback: int = 0,
     lookforward: int = 30,
     sleep_stage_duration: int = 30,
-    feature_selection: Optional[list[str]] = None,
+    feature_selection: list[str] | None = None,
     fs_rri_resample: float = 4,
-    min_rri: Optional[float] = None,
-    max_rri: Optional[float] = None,
+    min_rri: float | None = None,
+    max_rri: float | None = None,
     max_nans: float = 0,
     n_jobs: int = 1,
 ) -> tuple[list[np.ndarray], list[np.ndarray | None], list[str]]:
     """
     Calculate features from sleep data (e.g. heart rate).
 
     Time and frequency domain heart rate variability (HRV) features are calculated based on
```

### Comparing `sleepecg-0.5.7/sleepecg/heartbeats.py` & `sleepecg-0.5.8/src/sleepecg/heartbeats.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/sleepecg/io/ecg_readers.py` & `sleepecg-0.5.8/src/sleepecg/io/ecg_readers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 #
 # License: BSD (3-clause)
 
 """Functions for reading datasets containing ECG and beat annotations."""
 
 from __future__ import annotations
 
+from collections.abc import Iterator
 from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterator, Optional
+from typing import TYPE_CHECKING
 
 import numpy as np
 from tqdm import tqdm
 
 if TYPE_CHECKING:
     import matplotlib.pyplot as plt
 
@@ -41,29 +42,29 @@
     id : str, optional
         The record ID, by default `None`.
     """
 
     ecg: np.ndarray
     fs: float
     annotation: np.ndarray
-    lead: Optional[str] = None
-    id: Optional[str] = None
+    lead: str | None = None
+    id: str | None = None
 
     def export(self, filename: str | Path) -> None:
         """
         Export ECG record to CSV.
 
         Parameters
         ----------
         filename : str | pathlib.Path
             File name to write to.
         """
         export_ecg_record(self, filename)
 
-    def plot(self, **kwargs: np.ndarray) -> tuple["plt.Figure", "plt.Axes"]:
+    def plot(self, **kwargs: np.ndarray) -> tuple[plt.Figure, plt.Axes]:
         """
         Plot ECG time series with optional markers.
 
         Parameters
         ----------
         **kwargs : np.ndarray
             Positions of annotations (i.e. heartbeats) in samples. If more than one marker
@@ -103,15 +104,15 @@
         comments="",
     )
 
 
 def read_ltdb(
     records_pattern: str = "*",
     offline: bool = False,
-    data_dir: Optional[str | Path] = None,
+    data_dir: str | Path | None = None,
 ) -> Iterator[ECGRecord]:
     """
     Lazily read records from [LTDB](https://physionet.org/content/ltdb/).
 
     Parameters
     ----------
     records_pattern : str, optional
@@ -134,15 +135,15 @@
         data_dir = get_config("data_dir")
     yield from _read_mitbih("ltdb", records_pattern, offline, data_dir)
 
 
 def read_mitdb(
     records_pattern: str = "*",
     offline: bool = False,
-    data_dir: Optional[str | Path] = None,
+    data_dir: str | Path | None = None,
 ) -> Iterator[ECGRecord]:
     """
     Lazily read records from [MITDB](https://physionet.org/content/mitdb/).
 
     Parameters
     ----------
     records_pattern : str, optional
@@ -231,15 +232,15 @@
                 lead=signal_name,
                 id=record_id,
             )
 
 
 def read_gudb(
     offline: bool = False,
-    data_dir: Optional[str | Path] = None,
+    data_dir: str | Path | None = None,
 ) -> Iterator[ECGRecord]:
     """
     Lazily read records from [GUDB](https://berndporr.github.io/ECG-GUDB/).
 
     Required files are downloaded if not present in `'<data_dir>/gudb'`.
 
     Parameters
```

### Comparing `sleepecg-0.5.7/sleepecg/io/gudb.py` & `sleepecg-0.5.8/src/sleepecg/io/gudb.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # License: BSD (3-clause)
 
 """Utilities for downloading GUDB data."""
 
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Optional
 
 from sleepecg.config import get_config
 from sleepecg.io.utils import _calculate_checksum
 
 _GUDB_MD5 = {
     "subject_00/sitting/ECG.tsv": "06cdda76a17ff6efe4d4b18ccbc66e0f",
     "subject_00/sitting/annotation_cs.tsv": "fd0e6f5796a103637e29c4f9c14d155c",
@@ -366,15 +365,15 @@
     "subject_24/hand_bike/annotation_cables.tsv": "0b138798b9dbe8661fa2727d5f2220e6",
     "subject_24/jogging/ECG.tsv": "6f91604784f258ac6ca8f7f9408a2e03",
     "subject_24/jogging/annotation_cs.tsv": "74226610ebd87d1a13ea015ad4b40d7f",
     "subject_24/jogging/annotation_cables.tsv": "05ce602e00716d40607f6bb5665fc0a4",
 }
 
 
-def _generate_gudb_md5(data_dir: Optional[str | Path] = None) -> dict[str, str]:
+def _generate_gudb_md5(data_dir: str | Path | None = None) -> dict[str, str]:
     """
     Compute checksums for files in GUDB.
 
     This function can be used to compute the checksums from scratch if the data is already
     available locally. The global `_GUDB_MD5` dictionary should be equal to the return value
     of this function, so usually it is not necessary to run this function.
```

### Comparing `sleepecg-0.5.7/sleepecg/io/nsrr.py` & `sleepecg-0.5.8/src/sleepecg/io/nsrr.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/sleepecg/io/physionet.py` & `sleepecg-0.5.8/src/sleepecg/io/physionet.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # License: BSD (3-clause)
 
 """Simple interface for downloading PhysioNet data."""
 
 from __future__ import annotations
 
 import fnmatch
+from collections.abc import Iterable
 from pathlib import Path
-from typing import Iterable
 
 from tqdm import tqdm
 
 from sleepecg.io.utils import _download_file
 
 _PHYSIONET_FILES_URL = "https://physionet.org/files/"
 _CHECKSUM_FILENAME = "SHA256SUMS.txt"
```

### Comparing `sleepecg-0.5.7/sleepecg/io/sleep_readers.py` & `sleepecg-0.5.8/src/sleepecg/io/sleep_readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 """Read datasets containing ECG data and sleep stage annotations."""
 
 from __future__ import annotations
 
 import csv
 import datetime
+from collections.abc import Iterator
 from dataclasses import dataclass
 from enum import IntEnum
 from pathlib import Path
-from typing import Iterator, NamedTuple, Optional
+from typing import NamedTuple
 from xml.etree import ElementTree
 
 import numpy as np
 
 from sleepecg.config import get_config
 from sleepecg.heartbeats import detect_heartbeats
 from sleepecg.io.nsrr import _download_nsrr_file, _get_nsrr_url, _list_nsrr, download_nsrr
@@ -56,17 +57,17 @@
         `None`.
     age : int, optional
         The subject's age in years, by default `None`.
     weight : float, optional
         The subject's weight in kg, by default `None`.
     """
 
-    gender: Optional[int] = None
-    age: Optional[int] = None
-    weight: Optional[float] = None
+    gender: int | None = None
+    age: int | None = None
+    weight: float | None = None
 
 
 @dataclass
 class SleepRecord:
     """
     Store a single sleep record.
 
@@ -83,20 +84,20 @@
         Time at which the recording was started, by default `None`.
     heartbeat_times : np.ndarray, optional
         Times of heartbeats relative to recording start in seconds, by default `None`.
     subject_data : SubjectData, optional
         Dataclass containing subject data (such as gender or age), by default `None`.
     """
 
-    sleep_stages: Optional[np.ndarray] = None
-    sleep_stage_duration: Optional[int] = None
-    id: Optional[str] = None
-    recording_start_time: Optional[datetime.time] = None
-    heartbeat_times: Optional[np.ndarray] = None
-    subject_data: Optional[SubjectData] = None
+    sleep_stages: np.ndarray | None = None
+    sleep_stage_duration: int | None = None
+    id: str | None = None
+    recording_start_time: datetime.time | None = None
+    heartbeat_times: np.ndarray | None = None
+    subject_data: SubjectData | None = None
 
 
 class _ParseNsrrXmlResult(NamedTuple):
     sleep_stages: np.ndarray
     sleep_stage_duration: int
     recording_start_time: datetime.time
 
@@ -163,15 +164,15 @@
 
 
 def read_mesa(
     records_pattern: str = "*",
     heartbeats_source: str = "annotation",
     offline: bool = False,
     keep_edfs: bool = False,
-    data_dir: Optional[str | Path] = None,
+    data_dir: str | Path | None = None,
 ) -> Iterator[SleepRecord]:
     """
     Lazily read records from [MESA](https://sleepdata.org/datasets/mesa).
 
     Each MESA record consists of an `.edf` file containing raw polysomnography data and an
     `.xml` file containing annotated events. Since the entire MESA dataset requires about
     385 GB of disk space, `.edf` files can be deleted after heartbeat times have been
@@ -358,15 +359,15 @@
             subject_data=subject_data[record_id],
         )
 
 
 def read_slpdb(
     records_pattern: str = "*",
     offline: bool = False,
-    data_dir: Optional[str | Path] = None,
+    data_dir: str | Path | None = None,
 ) -> Iterator[SleepRecord]:
     """
     Lazily read records from [SLPDB](https://physionet.org/content/slpdb).
 
     Required files are downloaded from PhysioNet to `<data_dir>/slpdb`.
 
     Parameters
@@ -471,15 +472,15 @@
 
 
 def read_shhs(
     records_pattern: str = "*",
     heartbeats_source: str = "annotation",
     offline: bool = False,
     keep_edfs: bool = False,
-    data_dir: Optional[str | Path] = None,
+    data_dir: str | Path | None = None,
 ) -> Iterator[SleepRecord]:
     """
     Lazily read records from [SHHS](https://sleepdata.org/datasets/shhs).
 
     Each SHHS record consists of an `.edf` file containing raw polysomnography data and an
     `.xml` file containing annotated events. Since the entire SHHS dataset requires about
     356 GB of disk space, `.edf` files can be deleted after heartbeat times have been
```

### Comparing `sleepecg-0.5.7/sleepecg/io/utils.py` & `sleepecg-0.5.8/src/sleepecg/io/utils.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.7/sleepecg/plot.py` & `sleepecg-0.5.8/src/sleepecg/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     Parameters
     ----------
     record : SleepRecord
         A single record (i.e. night).
     stages_pred : np.ndarray
         The predicted stages, either as a 1D array of integers or a 2D array of
-        probabilties.
+        probabilities.
     stages_mode : str
         Identifier of the grouping mode. Can be any of `'wake-sleep'`, `'wake-rem-nrem'`,
         `'wake-rem-light-n3'`, or `'wake-rem-n1-n2-n3'`.
     stages_pred_duration : int, optional
         Duration of the predicted sleep stages in seconds, by default `30`.
     merge_annotations : bool, optional
         If `True`, merge annotations according to `stages_mode`, otherwise plot original
```

### Comparing `sleepecg-0.5.7/sleepecg/test/test_classification.py` & `sleepecg-0.5.8/tests/test_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # License: BSD (3-clause)
 
 """Tests for functions related to classifier training and evaluation."""
 
 import numpy as np
 import pytest
-
 from sleepecg.classification import _merge_sleep_stages
 
 
 @pytest.mark.parametrize(
     ["mode", "output"],
     [
         ("wake-sleep", [0, 1, 1, 1, 1, 2]),
```

### Comparing `sleepecg-0.5.7/sleepecg/test/test_config.py` & `sleepecg-0.5.8/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # © SleepECG developers
 #
 # License: BSD (3-clause)
 
 """Tests for the configuration interface."""
 
 import pytest
-
 import sleepecg.config
 from sleepecg import get_config, set_config
 
 
 @pytest.fixture(autouse=True)
 def temp_test_config(tmp_path):
     """Create, use and delete a temporary user config file for testing."""
```

### Comparing `sleepecg-0.5.7/sleepecg/test/test_feature_extraction.py` & `sleepecg-0.5.8/tests/test_feature_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 """Tests for feature extraction."""
 
 import datetime
 
 import numpy as np
 import pytest
-
 from sleepecg.feature_extraction import (
     _FEATURE_GROUPS,
     _hrv_frequencydomain_features,
     _hrv_timedomain_features,
     _metadata_features,
 )
 from sleepecg.io.sleep_readers import SleepRecord, SubjectData
```

### Comparing `sleepecg-0.5.7/sleepecg/test/test_heartbeat_detection.py` & `sleepecg-0.5.8/tests/test_heartbeat_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """Tests for heartbeat detection."""
 
 import sys
 
 import numpy as np
 import pytest
 from scipy.signal import resample_poly
-
 from sleepecg import compare_heartbeats, detect_heartbeats, get_toy_ecg
 
 pytestmark = pytest.mark.c_extension
 ecg, fs = get_toy_ecg()
 y_true = detect_heartbeats(ecg, fs)  # 478 true peaks
```

### Comparing `sleepecg-0.5.7/sleepecg/test/test_heartbeats.py` & `sleepecg-0.5.8/tests/test_heartbeats.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 """Tests for heartbeat detection and detector evaluation."""
 
 from sys import version_info
 
 import numpy as np
 import pytest
-
 from sleepecg import compare_heartbeats, detect_heartbeats, read_mitdb
 
 
 def test_compare_heartbeats():
     """Test heartbeat comparison results."""
     detection = np.array([20, 33, 43, 53, 73])
     annotation = np.array([20, 34, 58, 75, 99])
```

### Comparing `sleepecg-0.5.7/sleepecg/test/test_sleep_readers.py` & `sleepecg-0.5.8/tests/test_sleep_readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from __future__ import annotations
 
 import datetime
 from pathlib import Path
 
 import numpy as np
 from edfio import Edf, EdfSignal
-
 from sleepecg import SleepStage, get_toy_ecg, read_mesa, read_shhs, read_slpdb
 from sleepecg.io.sleep_readers import Gender
 
 
 def _dummy_nsrr_edf(filename: str, hours: float, ecg_channel: str):
     ecg_5_min, fs = get_toy_ecg()
     seconds = int(hours * 60 * 60)
```

### Comparing `sleepecg-0.5.7/sleepecg/utils.py` & `sleepecg-0.5.8/src/sleepecg/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 #
 # License: BSD (3-clause)
 
 """Utility functions."""
 
 import datetime
 import warnings
+from collections.abc import Iterable
 from pathlib import Path
-from typing import Any, Callable, Iterable, TypeVar
+from typing import Any, Callable, TypeVar
 
 import numpy as np
 
 from sleepecg.io.sleep_readers import SleepStage
 
 # required to propagate the return type annotation through _parallel
 _Returnable = TypeVar("_Returnable")
```

### Comparing `sleepecg-0.5.7/sleepecg.egg-info/PKG-INFO` & `sleepecg-0.5.8/src/sleepecg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: sleepecg
-Version: 0.5.7
+Version: 0.5.8
 Summary: A package for sleep stage classification using ECG data
 Author-email: Florian Hofer <hofaflo@gmail.com>, Clemens Brunner <clemens.brunner@gmail.com>
 License: BSD 3-Clause
 Project-URL: homepage, https://github.com/cbrnr/sleepecg
 Project-URL: documentation, https://sleepecg.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/cbrnr/sleepecg
 Project-URL: changelog, https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md
 Keywords: sleep,ecg,qrs,peak
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
@@ -22,40 +25,34 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: PyYAML>=5.4.0
 Requires-Dist: requests>=2.25.0
 Requires-Dist: scipy>=1.7.0
 Requires-Dist: tqdm>=4.60.0
 Provides-Extra: full
-Requires-Dist: edfio>=0.1.1; extra == "full"
+Requires-Dist: edfio>=0.4.0; extra == "full"
 Requires-Dist: joblib>=1.0.0; extra == "full"
 Requires-Dist: matplotlib>=3.5.0; extra == "full"
-Requires-Dist: numba>=0.59.0; extra == "full"
-Requires-Dist: tensorflow>=2.7.0; python_version < "3.12" and extra == "full"
+Requires-Dist: numba>=0.59.1; extra == "full"
+Requires-Dist: tensorflow>=2.16.1; extra == "full"
 Requires-Dist: wfdb>=3.4.0; extra == "full"
 Provides-Extra: dev
-Requires-Dist: edfio>=0.1.1; extra == "dev"
-Requires-Dist: joblib>=1.0.0; extra == "dev"
-Requires-Dist: matplotlib>=3.5.0; extra == "dev"
-Requires-Dist: mkdocs-material>=8.4.0; extra == "dev"
-Requires-Dist: mkdocstrings-python>=0.7.1; extra == "dev"
+Requires-Dist: sleepecg[doc]; extra == "dev"
+Requires-Dist: sleepecg[full]; extra == "dev"
 Requires-Dist: mypy>=0.991; extra == "dev"
-Requires-Dist: numba>=0.59.0; extra == "dev"
 Requires-Dist: pre-commit>=2.13.0; extra == "dev"
 Requires-Dist: pytest>=6.2.0; extra == "dev"
-Requires-Dist: ruff>=0.1.8; extra == "dev"
+Requires-Dist: ruff>=0.4.0; extra == "dev"
 Requires-Dist: setuptools>=56.0.0; extra == "dev"
-Requires-Dist: tensorflow>=2.7.0; python_version < "3.12" and extra == "dev"
-Requires-Dist: wfdb>=3.4.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: mkdocs-material>=8.4.0; extra == "doc"
 Requires-Dist: mkdocstrings-python>=0.8.2; extra == "doc"
 Provides-Extra: cibw
-Requires-Dist: edfio>=0.1.1; extra == "cibw"
-Requires-Dist: numba>=0.59.0; extra == "cibw"
+Requires-Dist: edfio>=0.4.0; extra == "cibw"
+Requires-Dist: numba>=0.59.1; extra == "cibw"
 Requires-Dist: wfdb>=3.4.0; extra == "cibw"
 
 ![Python](https://img.shields.io/pypi/pyversions/sleepecg.svg?logo=python&logoColor=white)
 [![PyPI](https://img.shields.io/pypi/v/sleepecg)](https://pypi.org/project/sleepecg/)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/sleepecg.svg?label=conda-forge)](https://anaconda.org/conda-forge/sleepecg)
 [![Docs](https://readthedocs.org/projects/sleepecg/badge/?version=latest)](https://sleepecg.readthedocs.io/en/stable/index.html)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05411/status.svg)](https://doi.org/10.21105/joss.05411)
@@ -116,25 +113,25 @@
 
 
 ### Dependencies
 
 SleepECG requires Python ≥ 3.9 and the following packages:
 
 - [numpy](https://numpy.org/) ≥ 1.20.0
+- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
 - [requests](https://requests.readthedocs.io/en/latest/) ≥ 2.25.0
 - [scipy](https://scipy.org/) ≥ 1.7.0
 - [tqdm](https://tqdm.github.io/) ≥ 4.60.0
-- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
 
 Optional dependencies provide additional features:
 
-- [edfio](https://github.com/the-siesta-group/edfio/) ≥ 0.1.1 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
+- [edfio](https://github.com/the-siesta-group/edfio/) ≥ 0.4.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
 - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
 - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
-- [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-- [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
+- [numba](https://numba.pydata.org/) ≥ 0.59.1 (JIT-compiled heartbeat detector)
+- [tensorflow](https://www.tensorflow.org/) ≥ 2.16.1 (sleep stage classification with Keras models)
 - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
 
 
 ### Contributing
 
 The [contributing guide](https://github.com/cbrnr/sleepecg/blob/main/CONTRIBUTING.md) contains detailed instructions on how to contribute to SleepECG.
```

### Comparing `sleepecg-0.5.7/sleepecg.egg-info/SOURCES.txt` & `sleepecg-0.5.8/src/sleepecg.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
-MANIFEST.in
 README.md
 mkdocs.yml
 pyproject.toml
 readthedocs.yml
 setup.py
 .github/dependabot.yml
 .github/workflows/release.yml
@@ -46,40 +45,40 @@
 examples/benchmark/config.yml
 examples/benchmark/plot_benchmark_results.py
 examples/benchmark/requirements-benchmark.txt
 examples/benchmark/utils.py
 examples/classifiers/wrn_gru_mesa.py
 examples/classifiers/wrn_gru_mesa_weighted.py
 examples/classifiers/ws_gru_mesa.py
-sleepecg/__init__.py
-sleepecg/_heartbeat_detection.c
-sleepecg/_heartbeat_detection.pyi
-sleepecg/classification.py
-sleepecg/config.py
-sleepecg/config.yml
-sleepecg/feature_extraction.py
-sleepecg/heartbeats.py
-sleepecg/plot.py
-sleepecg/py.typed
-sleepecg/utils.py
-sleepecg.egg-info/PKG-INFO
-sleepecg.egg-info/SOURCES.txt
-sleepecg.egg-info/dependency_links.txt
-sleepecg.egg-info/requires.txt
-sleepecg.egg-info/top_level.txt
-sleepecg/classifiers/wrn-gru-mesa-weighted.zip
-sleepecg/classifiers/wrn-gru-mesa.zip
-sleepecg/classifiers/ws-gru-mesa.zip
-sleepecg/data/ecg.npz
-sleepecg/io/__init__.py
-sleepecg/io/ecg_readers.py
-sleepecg/io/gudb.py
-sleepecg/io/nsrr.py
-sleepecg/io/physionet.py
-sleepecg/io/sleep_readers.py
-sleepecg/io/utils.py
-sleepecg/test/test_classification.py
-sleepecg/test/test_config.py
-sleepecg/test/test_feature_extraction.py
-sleepecg/test/test_heartbeat_detection.py
-sleepecg/test/test_heartbeats.py
-sleepecg/test/test_sleep_readers.py
+src/sleepecg/__init__.py
+src/sleepecg/_heartbeat_detection.c
+src/sleepecg/_heartbeat_detection.pyi
+src/sleepecg/classification.py
+src/sleepecg/config.py
+src/sleepecg/config.yml
+src/sleepecg/feature_extraction.py
+src/sleepecg/heartbeats.py
+src/sleepecg/plot.py
+src/sleepecg/py.typed
+src/sleepecg/utils.py
+src/sleepecg.egg-info/PKG-INFO
+src/sleepecg.egg-info/SOURCES.txt
+src/sleepecg.egg-info/dependency_links.txt
+src/sleepecg.egg-info/requires.txt
+src/sleepecg.egg-info/top_level.txt
+src/sleepecg/classifiers/wrn-gru-mesa-weighted.zip
+src/sleepecg/classifiers/wrn-gru-mesa.zip
+src/sleepecg/classifiers/ws-gru-mesa.zip
+src/sleepecg/data/ecg.npz
+src/sleepecg/io/__init__.py
+src/sleepecg/io/ecg_readers.py
+src/sleepecg/io/gudb.py
+src/sleepecg/io/nsrr.py
+src/sleepecg/io/physionet.py
+src/sleepecg/io/sleep_readers.py
+src/sleepecg/io/utils.py
+tests/test_classification.py
+tests/test_config.py
+tests/test_feature_extraction.py
+tests/test_heartbeat_detection.py
+tests/test_heartbeats.py
+tests/test_sleep_readers.py
```

