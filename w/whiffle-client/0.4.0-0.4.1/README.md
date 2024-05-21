# Comparing `tmp/whiffle_client-0.4.0.tar.gz` & `tmp/whiffle_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiffle_client-0.4.0.tar", last modified: Wed May 15 08:56:35 2024, max compression
+gzip compressed data, was "whiffle_client-0.4.1.tar", last modified: Tue May 21 12:37:55 2024, max compression
```

## Comparing `whiffle_client-0.4.0.tar` & `whiffle_client-0.4.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.938131 whiffle_client-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)    11095 2024-05-15 08:56:35.937131 whiffle_client-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)    10139 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/USER_README.md
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 08:56:35.938131 whiffle_client-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.927131 whiffle_client-0.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.929131 whiffle_client-0.4.0/whiffle_client/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.931131 whiffle_client-0.4.0/whiffle_client/analysis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7628 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/io.py
--rw-rw-rw-   0 root         (0) root         (0)    16433 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     4854 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/scatter.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/skill.py
--rw-rw-rw-   0 root         (0) root         (0)     3231 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3995 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/base_client.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/entrypoints.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.932131 whiffle_client-0.4.0/whiffle_client/loaders/
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/loaders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/loaders/csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.933131 whiffle_client-0.4.0/whiffle_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/resources/example_generic_params.json
--rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/resources/example_yaml_include.yaml
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/resources/example_yaml_include_metmasts.yaml
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.933131 whiffle_client-0.4.0/whiffle_client/snippets/
--rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/snippets/create_mock_powercurve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.933131 whiffle_client-0.4.0/whiffle_client/wind/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.935131 whiffle_client-0.4.0/whiffle_client/wind/components/
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/dates.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/geometries.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/metmast.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/turbine.py
--rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/turbine_model_specs.py
--rw-rw-rw-   0 root         (0) root         (0)     5011 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/wind_simulation_task.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/windfarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.936131 whiffle_client-0.4.0/whiffle_client/wind/mapping/
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/mapping/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/mapping/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4760 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/mapping/turbine_model_specs.py
--rw-rw-rw-   0 root         (0) root         (0)     5983 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/mapping/wind_simulation_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.936131 whiffle_client-0.4.0/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11095 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1652 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.460646 whiffle_client-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)    11095 2024-05-21 12:37:55.459645 whiffle_client-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    10139 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 12:37:55.460646 whiffle_client-0.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.449645 whiffle_client-0.4.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.450645 whiffle_client-0.4.1/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.453645 whiffle_client-0.4.1/whiffle_client/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7628 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    16433 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     4854 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4957 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/skill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3231 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3995 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/base_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/entrypoints.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.453645 whiffle_client-0.4.1/whiffle_client/loaders/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/loaders/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.454645 whiffle_client-0.4.1/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/resources/example_yaml_include.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/resources/example_yaml_include_metmasts.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.454645 whiffle_client-0.4.1/whiffle_client/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/snippets/create_mock_powercurve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.455645 whiffle_client-0.4.1/whiffle_client/wind/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.457646 whiffle_client-0.4.1/whiffle_client/wind/components/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/geometries.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/metmast.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/turbine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/turbine_model_specs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5240 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/wind_simulation_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/windfarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.458645 whiffle_client-0.4.1/whiffle_client/wind/mapping/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/mapping/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/mapping/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4808 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/mapping/turbine_model_specs.py
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/mapping/wind_simulation_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.458645 whiffle_client-0.4.1/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11095 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1652 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.4.0/LICENCE.txt` & `whiffle_client-0.4.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/PKG-INFO` & `whiffle_client-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `whiffle_client-0.4.0/README.md` & `whiffle_client-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/USER_README.md` & `whiffle_client-0.4.1/USER_README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/pyproject.toml` & `whiffle_client-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/tests/test_cli.py` & `whiffle_client-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/tests/test_client.py` & `whiffle_client-0.4.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/analysis/io.py` & `whiffle_client-0.4.1/whiffle_client/analysis/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/analysis/plot.py` & `whiffle_client-0.4.1/whiffle_client/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/analysis/scatter.py` & `whiffle_client-0.4.1/whiffle_client/analysis/scatter.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/analysis/skill.py` & `whiffle_client-0.4.1/whiffle_client/analysis/skill.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/analysis/utils.py` & `whiffle_client-0.4.1/whiffle_client/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/base_client.py` & `whiffle_client-0.4.1/whiffle_client/base_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/client.py` & `whiffle_client-0.4.1/whiffle_client/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/decorators.py` & `whiffle_client-0.4.1/whiffle_client/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,18 @@
     def wrap(func):
         @wraps(func)
         def wrapper(self, *args, **kwargs):
             data = kwargs.get("data", None)
             if isinstance(data, str) or isinstance(data, Path):
                 # Data provided as yaml path
                 data = yaml.load(open(data), Loader=yaml.FullLoader)
-                # TODO: gather from the yaml just the data_type matching the resource_type
-                #       Goal here is to provide
-                data_type = data.pop("type", None)
-                data = class_type(**data)
+                data = class_type.from_dict(data)
             elif isinstance(data, dict):
                 # Data directly provided as dict
-                data = class_type(**data)
+                data = class_type.from_dict(data)
             if data:
                 kwargs["data"] = data._get_api_params()
             else:
                 raise ValueError("Please provide valid data or path to valid data")
             return func(self, *args, **kwargs)
 
         return wrapper
```

### Comparing `whiffle_client-0.4.0/whiffle_client/entrypoints.py` & `whiffle_client-0.4.1/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/io.py` & `whiffle_client-0.4.1/whiffle_client/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/loaders/csv.py` & `whiffle_client-0.4.1/whiffle_client/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.4.1/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/resources/example_yaml_include.yaml` & `whiffle_client-0.4.1/whiffle_client/resources/example_yaml_include.yaml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/snippets/create_mock_powercurve.py` & `whiffle_client-0.4.1/whiffle_client/snippets/create_mock_powercurve.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/wind/client.py` & `whiffle_client-0.4.1/whiffle_client/wind/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/wind/components/__init__.py` & `whiffle_client-0.4.1/whiffle_client/wind/components/__init__.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/wind/components/turbine_model_specs.py` & `whiffle_client-0.4.1/whiffle_client/wind/components/turbine_model_specs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from dataclasses import asdict, dataclass, field
+import inspect
 import json
-
+from dataclasses import asdict, dataclass, field
 
 READ_ONLY_FIELDS = set(["id"])
 
 
 @dataclass
 class TurbineModelSpecs:
     id: int = field(default=None)
@@ -15,14 +15,20 @@
     reference_density: float = field(default=None)
     reference_turbulence_intensity: float = field(default=None)
     reference_windspeed: list[float] = field(default=None)
     thrust_coefficient: list[float] = field(default=None)
     power: list[float] = field(default=None)
     public: bool = field(default_factory=bool)
 
+    @classmethod
+    def from_dict(cls, env):
+        return cls(
+            **{k: v for k, v in env.items() if k in inspect.signature(cls).parameters}
+        )
+
     def _get_api_params(self):
         params = asdict(self)
         _ = [params.pop(key, None) for key in READ_ONLY_FIELDS]
         return params
 
     def __str__(self) -> str:
         return f"{self.__class__}:\n{json.dumps(asdict(self), indent=4)}"
```

### Comparing `whiffle_client-0.4.0/whiffle_client/wind/components/wind_simulation_task.py` & `whiffle_client-0.4.1/whiffle_client/wind/components/wind_simulation_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import datetime
+import inspect
 import json
 from dataclasses import asdict, dataclass, field
 
 import yaml
 from yamlinclude import YamlIncludeConstructor
 
-from whiffle_client.wind.components import Domain, Geometries, Metmast, Windfarm
 from whiffle_client.loaders import csv_loader_constructor
+from whiffle_client.wind.components import Domain, Geometries, Metmast, Windfarm
 from whiffle_client.wind.components.dates import Dates
 
 YamlIncludeConstructor.add_to_loader_class(loader_class=yaml.FullLoader)
 yaml.add_constructor("!include-csv", csv_loader_constructor)
 
 READ_ONLY_FIELDS = set(
     [
@@ -63,14 +64,22 @@
     metmasts: list[Metmast] = field(default_factory=list)
     metmasts_heights: list[float] = field(default_factory=list)
 
     # Output attributes
     wind_resource_grid_heights: list[float] = field(default_factory=list)
     fields_heights: list[float] = field(default_factory=list)
 
+    progress: dict = field(default_factory=dict)
+
+    @classmethod
+    def from_dict(cls, env):
+        return cls(
+            **{k: v for k, v in env.items() if k in inspect.signature(cls).parameters}
+        )
+
     def __post_init__(self):
 
         if isinstance(self.metmasts, list):
             self.metmasts = [
                 Metmast(
                     id=metmast["name"],
                     longitude=metmast["longitude"],
```

### Comparing `whiffle_client-0.4.0/whiffle_client/wind/mapping/base.py` & `whiffle_client-0.4.1/whiffle_client/wind/mapping/base.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.0/whiffle_client/wind/mapping/turbine_model_specs.py` & `whiffle_client-0.4.1/whiffle_client/wind/mapping/turbine_model_specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         -------
         TurbineModelSpecs
             Object instance of the turbine model
         """
         request = self.session.post_request(
             f"{self.session.server_url}{self.URL}", data=data
         )
-        return TurbineModelSpecs(**request.json())
+        return TurbineModelSpecs.from_dict(request.json())
 
     @load_data(TurbineModelSpecs)
     def edit(
         self,
         turbine_model_id: str,
         data: Union[str, dict, Path, TurbineModelSpecs] = None,
     ) -> TurbineModelSpecs:
@@ -56,27 +56,27 @@
         TurbineModelSpecs
             Object instance of the turbine model
         """
         request = self.session.put_request(
             f"{self.session.server_url}{self.URL}/{turbine_model_id}",
             data=data,
         )
-        return TurbineModelSpecs(**request.json())
+        return TurbineModelSpecs.from_dict(request.json())
 
     def get_all(self) -> list[TurbineModelSpecs]:
         """Get a list of all the Turbine Models available to the user
 
         Returns
         -------
         list[TurbineModelSpecs]
             List of TurbineModelSpecs object instances
         """
         request = self.session.get_request(f"{self.session.server_url}{self.URL}")
         return [
-            TurbineModelSpecs(**turbine_model_specs)
+            TurbineModelSpecs.from_dict(turbine_model_specs)
             for turbine_model_specs in request.json()
         ]
 
     def get(
         self,
         turbine_model_id: str = None,
         turbine_model_name: str = None,
@@ -97,25 +97,25 @@
 
         Raises
         ------
         ValueError
             Raises error if either `turbine_model_id` or `turbine_model_name` are not provided
         """
         if turbine_model_id:
-            return TurbineModelSpecs(
-                **self.session.get_request(
+            return TurbineModelSpecs.from_dict(
+                self.session.get_request(
                     f"{self.session.server_url}{self.URL}/{turbine_model_id}"
                 ).json()
             )
         elif turbine_model_name:
             print(
                 "WARN: Accessing turbine model specs by name. Using an `id` is recomended as name does not ensure uniqueness."
             )
             return [
-                TurbineModelSpecs(**specs)
+                TurbineModelSpecs.from_dict(specs)
                 for specs in self.session.get_request(
                     f"{self.session.server_url}{self.URL}?name={turbine_model_name}"
                 ).json()
             ]
         else:
             raise ValueError(
                 "Please provide either valid turbine_model_id or turbine_model_name"
@@ -133,16 +133,16 @@
             Id of the turbine model
 
         Returns
         -------
         TurbineModelSpecs
             TurbineModelSpecs object instance of deleted turbine model
         """
-        return TurbineModelSpecs(
-            **self.session.delete_request(
+        return TurbineModelSpecs.from_dict(
+            self.session.delete_request(
                 f"{self.session.server_url}{self.URL}/{turbine_model_id}"
             ).json()
         )
 
     def download(self):
         """Not implemented"""
         return super().download()
```

### Comparing `whiffle_client-0.4.0/whiffle_client/wind/mapping/wind_simulation_tasks.py` & `whiffle_client-0.4.1/whiffle_client/wind/mapping/wind_simulation_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         -------
         WindSimulationTask
             Object instance of the wind simulation
         """
         wind_simulation_task = self.session.post_request(
             f"{self.session.server_url}{self.URL}", data=data
         )
-        return WindSimulationTask(**wind_simulation_task.json())
+        return WindSimulationTask.from_dict(wind_simulation_task.json())
 
     @load_data(WindSimulationTask)
     def edit(
         self,
         wind_simulation_task_id: str,
         data: Union[str, dict, Path, WindSimulationTask] = None,
     ) -> WindSimulationTask:
@@ -59,15 +59,15 @@
         WindSimulationTask
             Object instance of the wind simulation
         """
         request = self.session.put_request(
             f"{self.session.server_url}{self.URL}/{wind_simulation_task_id}",
             data=data,
         )
-        return WindSimulationTask(**request.json())
+        return WindSimulationTask.from_dict(request.json())
 
     def submit(self, wind_simulation_task_id: str) -> WindSimulationTask:
         """Submit Wind Simulation Task
 
         Parameters
         ----------
         wind_simulation_task_id : str
@@ -77,28 +77,28 @@
         -------
         WindSimulationTask
             Object instance of the wind simulation
         """
         request = self.session.post_request(
             f"{self.session.server_url}{self.URL}/{wind_simulation_task_id}/submit",
         )
-        return WindSimulationTask(**request.json())
+        return WindSimulationTask.from_dict(request.json())
 
     # Wind simulation commands
     def get_all(self) -> list[WindSimulationTask]:
         """Get a list of all the Wind Simulation Tasks available to the user
 
         Returns
         -------
         list[WindSimulationTask]
             List of WindSimulationTasks object instances
         """
         request = self.session.get_request(f"{self.session.server_url}{self.URL}")
         return [
-            WindSimulationTask(**wind_simulation_tasks_params)
+            WindSimulationTask.from_dict(wind_simulation_tasks_params)
             for wind_simulation_tasks_params in request.json()
         ]
 
     def get(self, wind_simulation_task_id: str) -> WindSimulationTask:
         """Get a Wind Simulation Task
 
         Parameters
@@ -107,16 +107,16 @@
             Id of wind simulation
 
         Returns
         -------
         WindSimulationTask
             Requested WindSimulationTask
         """
-        return WindSimulationTask(
-            **self.session.get_request(
+        return WindSimulationTask.from_dict(
+            self.session.get_request(
                 f"{self.session.server_url}{self.URL}/{wind_simulation_task_id}"
             ).json()
         )
 
     def delete(self, wind_simulation_task_id: str):
         """Delete Wind Simulation
```

### Comparing `whiffle_client-0.4.0/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.4.1/whiffle_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `whiffle_client-0.4.0/whiffle_client.egg-info/SOURCES.txt` & `whiffle_client-0.4.1/whiffle_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

