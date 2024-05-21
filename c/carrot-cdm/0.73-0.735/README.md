# Comparing `tmp/carrot-cdm-0.73.tar.gz` & `tmp/carrot-cdm-0.735.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carrot-cdm-0.73.tar", last modified: Tue May 14 13:19:21 2024, max compression
+gzip compressed data, was "carrot-cdm-0.735.tar", last modified: Tue May 21 13:30:23 2024, max compression
```

## Comparing `carrot-cdm-0.73.tar` & `carrot-cdm-0.735.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.977548 carrot-cdm-0.73/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 13:19:20.000000 carrot-cdm-0.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 13:19:21.977548 carrot-cdm-0.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 13:19:20.000000 carrot-cdm-0.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.969548 carrot-cdm-0.73/carrot/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 13:19:21.000000 carrot-cdm-0.73/carrot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.969548 carrot-cdm-0.73/carrot/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/analyses/example_serology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.969548 carrot-cdm-0.73/carrot/cdm/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.969548 carrot-cdm-0.73/carrot/cdm/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33952 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.969548 carrot-cdm-0.73/carrot/cdm/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.969548 carrot-cdm-0.73/carrot/cdm/objects/versions/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.973548 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/death.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/specimen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cdm/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.973548 carrot-cdm-0.73/carrot/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.973548 carrot-cdm-0.73/carrot/cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    41561 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)    23111 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7841 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/pseudonymise.py
--rw-r--r--   0 runner    (1001) docker     (127)    47910 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/cli/subcommands/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.973548 carrot-cdm-0.73/carrot/io/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/io/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.973548 carrot-cdm-0.73/carrot/io/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/io/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/io/plugins/bclink.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/io/plugins/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/io/plugins/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.977548 carrot-cdm-0.73/carrot/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/bash_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/bclink_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.977548 carrot-cdm-0.73/carrot/tools/extract/
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/extract/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/mappingrules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/omopcdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-14 13:19:20.000000 carrot-cdm-0.73/carrot/tools/rules_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:19:21.977548 carrot-cdm-0.73/carrot_cdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 13:19:21.000000 carrot-cdm-0.73/carrot_cdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-14 13:19:21.000000 carrot-cdm-0.73/carrot_cdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:19:21.000000 carrot-cdm-0.73/carrot_cdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 13:19:21.000000 carrot-cdm-0.73/carrot_cdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 13:19:21.000000 carrot-cdm-0.73/carrot_cdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 13:19:21.000000 carrot-cdm-0.73/carrot_cdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:19:21.977548 carrot-cdm-0.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-14 13:19:20.000000 carrot-cdm-0.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.847089 carrot-cdm-0.735/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 13:30:22.000000 carrot-cdm-0.735/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-21 13:30:23.843089 carrot-cdm-0.735/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 13:30:22.000000 carrot-cdm-0.735/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.839089 carrot-cdm-0.735/carrot/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.839089 carrot-cdm-0.735/carrot/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/analyses/example_serology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.839089 carrot-cdm-0.735/carrot/cdm/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.839089 carrot-cdm-0.735/carrot/cdm/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33952 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.839089 carrot-cdm-0.735/carrot/cdm/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.839089 carrot-cdm-0.735/carrot/cdm/objects/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.839089 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/death.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/specimen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cdm/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.839089 carrot-cdm-0.735/carrot/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.843089 carrot-cdm-0.735/carrot/cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41561 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23111 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7841 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/pseudonymise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48434 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/cli/subcommands/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.843089 carrot-cdm-0.735/carrot/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/io/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.843089 carrot-cdm-0.735/carrot/io/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/io/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/io/plugins/bclink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/io/plugins/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/io/plugins/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.843089 carrot-cdm-0.735/carrot/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/bash_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/bclink_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.843089 carrot-cdm-0.735/carrot/tools/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/extract/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/mappingrules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/omopcdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-21 13:30:22.000000 carrot-cdm-0.735/carrot/tools/rules_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:30:23.843089 carrot-cdm-0.735/carrot_cdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-21 13:30:23.000000 carrot-cdm-0.735/carrot_cdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-21 13:30:23.000000 carrot-cdm-0.735/carrot_cdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:30:23.000000 carrot-cdm-0.735/carrot_cdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 13:30:23.000000 carrot-cdm-0.735/carrot_cdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-21 13:30:23.000000 carrot-cdm-0.735/carrot_cdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 13:30:23.000000 carrot-cdm-0.735/carrot_cdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:30:23.847089 carrot-cdm-0.735/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-21 13:30:22.000000 carrot-cdm-0.735/setup.py
```

### Comparing `carrot-cdm-0.73/LICENSE` & `carrot-cdm-0.735/LICENSE`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/PKG-INFO` & `carrot-cdm-0.735/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrot-cdm
-Version: 0.73
+Version: 0.735
 Summary: Python package for performing mapping of ETL to CDM 
 Home-page: https://github.com/HDRUK/CaRROT-CDM
 Author: CO-CONNECT Collaboration
 Author-email: pdappleby@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `carrot-cdm-0.73/carrot/analyses/example_serology.py` & `carrot-cdm-0.735/carrot/analyses/example_serology.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/__init__.py` & `carrot-cdm-0.735/carrot/cdm/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/decorators.py` & `carrot-cdm-0.735/carrot/cdm/decorators.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/model.py` & `carrot-cdm-0.735/carrot/cdm/model.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/__init__.py` & `carrot-cdm-0.735/carrot/cdm/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/common.py` & `carrot-cdm-0.735/carrot/cdm/objects/common.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/death.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/death.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/measurement.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/measurement.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/observation.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/observation.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/person.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/person.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/specimen.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/specimen.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py` & `carrot-cdm-0.735/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cdm/operations.py` & `carrot-cdm-0.735/carrot/cdm/operations.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/cli.py` & `carrot-cdm-0.735/carrot/cli/cli.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/airflow.py` & `carrot-cdm-0.735/carrot/cli/subcommands/airflow.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/display.py` & `carrot-cdm-0.735/carrot/cli/subcommands/display.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/etl.py` & `carrot-cdm-0.735/carrot/cli/subcommands/etl.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/generate.py` & `carrot-cdm-0.735/carrot/cli/subcommands/generate.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/get.py` & `carrot-cdm-0.735/carrot/cli/subcommands/get.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/info.py` & `carrot-cdm-0.735/carrot/cli/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/pseudonymise.py` & `carrot-cdm-0.735/carrot/cli/subcommands/pseudonymise.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/run.py` & `carrot-cdm-0.735/carrot/cli/subcommands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -785,14 +785,20 @@
                                     key = srcfilename + "~all~" + tgtfile + "~" + outrecord[1] +"~"
                                     metrics.increment_key_count(key, "output_count")
                                     key = srcfilename + "~" + datacol +"~" + tgtfile + "~" + outrecord[1] + "~" + outrecord[2]
                                     metrics.increment_key_count(key, "output_count")
                                 else:
                                     key = srcfilename + "~" + datacol +"~" + tgtfile + "~" + outrecord[2] + "~"
                                     metrics.increment_key_count(key, "output_count")
+                                    key = srcfilename + "~all~" + tgtfile + "~" + outrecord[2] + "~"
+                                    metrics.increment_key_count(key, "output_count")
+                                    key = "all~all~" + tgtfile + "~" + outrecord[2] + "~"
+                                    metrics.increment_key_count(key, "output_count")
+                                    key = "all~all~all~" + outrecord[2] + "~"
+                                    metrics.increment_key_count(key, "output_count")
                                 fhd[tgtfile].write("\t".join(outrecord) + "\n")
                             else:
                                 key = srcfilename + "~all~" + tgtfile + "~all~"
                                 metrics.increment_key_count(key, "invalid_person_ids")
                                 rejidcounts[srcfilename] += 1
 
         fh.close()
```

### Comparing `carrot-cdm-0.73/carrot/cli/subcommands/search.py` & `carrot-cdm-0.735/carrot/cli/subcommands/search.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/io/common.py` & `carrot-cdm-0.735/carrot/io/common.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/io/plugins/bclink.py` & `carrot-cdm-0.735/carrot/io/plugins/bclink.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/io/plugins/local.py` & `carrot-cdm-0.735/carrot/io/plugins/local.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/io/plugins/sql.py` & `carrot-cdm-0.735/carrot/io/plugins/sql.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/__init__.py` & `carrot-cdm-0.735/carrot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/bash_helpers.py` & `carrot-cdm-0.735/carrot/tools/bash_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/bclink_helpers.py` & `carrot-cdm-0.735/carrot/tools/bclink_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/dag.py` & `carrot-cdm-0.735/carrot/tools/dag.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/extract/__init__.py` & `carrot-cdm-0.735/carrot/tools/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/extract/templates.py` & `carrot-cdm-0.735/carrot/tools/extract/templates.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/file_helpers.py` & `carrot-cdm-0.735/carrot/tools/file_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/logger.py` & `carrot-cdm-0.735/carrot/tools/logger.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/mappingrules.py` & `carrot-cdm-0.735/carrot/tools/mappingrules.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/metrics.py` & `carrot-cdm-0.735/carrot/tools/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,16 @@
             if "invalid_date_fields" in dvalue:
                 invalid_date_fields = str(dvalue["invalid_date_fields"])
 
             output_count = "0"
             if "output_count" in dvalue:
                 output_count = str(dvalue["output_count"])
 
-            if (int(output_count) >= self.log_threshold) or (tablename == "person"):
+            #if (int(output_count) >= self.log_threshold) or (tablename == "person"):
+            if (int(output_count) >= self.log_threshold):
               summary_str += self.dataset_name + "\t" + source + "\t" + fieldname + "\t" + tablename + "\t" + concept_id + "\t" + additional +"\t" + input_count + "\t" + invalid_person_ids + "\t" + invalid_date_fields + "\t" + invalid_source_fields + "\t" + output_count + "\n"
 
         return summary_str
 
     def add_log_data(self, msg):
         self.log_data += msg + "\n"
```

### Comparing `carrot-cdm-0.73/carrot/tools/omopcdm.py` & `carrot-cdm-0.735/carrot/tools/omopcdm.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/profiling.py` & `carrot-cdm-0.735/carrot/tools/profiling.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot/tools/rules_helpers.py` & `carrot-cdm-0.735/carrot/tools/rules_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/carrot_cdm.egg-info/PKG-INFO` & `carrot-cdm-0.735/carrot_cdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrot-cdm
-Version: 0.73
+Version: 0.735
 Summary: Python package for performing mapping of ETL to CDM 
 Home-page: https://github.com/HDRUK/CaRROT-CDM
 Author: CO-CONNECT Collaboration
 Author-email: pdappleby@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `carrot-cdm-0.73/carrot_cdm.egg-info/SOURCES.txt` & `carrot-cdm-0.735/carrot_cdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.73/setup.py` & `carrot-cdm-0.735/setup.py`

 * *Files identical despite different names*

