# Comparing `tmp/google-pso-data-validator-4.5.0.tar.gz` & `tmp/google_pso_data_validator-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-pso-data-validator-4.5.0.tar", last modified: Mon Mar 18 19:56:25 2024, max compression
+gzip compressed data, was "google_pso_data_validator-5.0.0.tar", last modified: Tue May 21 18:11:53 2024, max compression
```

## Comparing `google-pso-data-validator-4.5.0.tar` & `google_pso_data_validator-5.0.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.761662 google-pso-data-validator-4.5.0/
--rw-r--r--   0 root         (0) root         (0)    11358 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    45816 2024-03-18 19:56:25.761662 google-pso-data-validator-4.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    44079 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.745660 google-pso-data-validator-4.5.0/data_validation/
--rw-r--r--   0 root         (0) root         (0)      715 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26378 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/app.py
--rw-r--r--   0 root         (0) root         (0)    48514 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/cli_tools.py
--rw-r--r--   0 root         (0) root         (0)      881 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/client_info.py
--rw-r--r--   0 root         (0) root         (0)     9690 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/clients.py
--rw-r--r--   0 root         (0) root         (0)    14254 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/combiner.py
--rw-r--r--   0 root         (0) root         (0)    40169 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/config_manager.py
--rw-r--r--   0 root         (0) root         (0)     5233 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/consts.py
--rw-r--r--   0 root         (0) root         (0)    14680 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/data_validation.py
--rw-r--r--   0 root         (0) root         (0)      687 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1269 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/jellyfish_distance.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/metadata.py
--rw-r--r--   0 root         (0) root         (0)    16257 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/partition_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.745660 google-pso-data-validator-4.5.0/data_validation/query_builder/
--rw-r--r--   0 root         (0) root         (0)      575 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/query_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2583 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/query_builder/partition_row_builder.py
--rw-r--r--   0 root         (0) root         (0)    19239 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/query_builder/query_builder.py
--rw-r--r--   0 root         (0) root         (0)     3697 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/query_builder/random_row_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.749661 google-pso-data-validator-4.5.0/data_validation/result_handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/result_handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3970 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/result_handlers/bigquery.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/result_handlers/text.py
--rw-r--r--   0 root         (0) root         (0)    14320 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/schema_validation.py
--rw-r--r--   0 root         (0) root         (0)     1773 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/secret_manager.py
--rw-r--r--   0 root         (0) root         (0)    10173 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/state_manager.py
--rw-r--r--   0 root         (0) root         (0)    16109 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/data_validation/validation_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.757661 google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45816 2024-03-18 19:56:25.000000 google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3149 2024-03-18 19:56:25.000000 google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 19:56:25.000000 google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-18 19:56:25.000000 google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      586 2024-03-18 19:56:25.000000 google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-18 19:56:25.000000 google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-03-18 19:56:25.761662 google-pso-data-validator-4.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2877 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.737660 google-pso-data-validator-4.5.0/third_party/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.741660 google-pso-data-validator-4.5.0/third_party/ibis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.749661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_addon/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_addon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_addon/api.py
--rw-r--r--   0 root         (0) root         (0)    20102 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_addon/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.749661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/
--rw-r--r--   0 root         (0) root         (0)     6916 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1378 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/api.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/client.py
--rw-r--r--   0 root         (0) root         (0)     2748 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/compiler.py
--rw-r--r--   0 root         (0) root         (0)     1517 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     2300 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.749661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/tests/
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4999 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1292 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.753661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/
--rw-r--r--   0 root         (0) root         (0)     2649 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1264 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/api.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/compiler.py
--rw-r--r--   0 root         (0) root         (0)     1492 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/datatypes.py
--rw-r--r--   0 root         (0) root         (0)    15919 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.753661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_impala/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_impala/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7187 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_impala/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.753661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mssql/
--rw-r--r--   0 root         (0) root         (0)     2987 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mssql/api.py
--rw-r--r--   0 root         (0) root         (0)     1315 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mssql/datatypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.753661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.753661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mysql/base_sql_compiler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mysql/base_sql_compiler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4596 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_mysql/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.757661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/
--rw-r--r--   0 root         (0) root         (0)     3043 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1228 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/api.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/compiler.py
--rw-r--r--   0 root         (0) root         (0)     6593 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/datatypes.py
--rw-r--r--   0 root         (0) root         (0)    14411 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.757661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_postgres/
--rw-r--r--   0 root         (0) root         (0)      101 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4126 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_postgres/client.py
--rw-r--r--   0 root         (0) root         (0)      839 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_postgres/datatypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.757661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_redshift/
--rw-r--r--   0 root         (0) root         (0)     4053 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_redshift/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1170 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_redshift/api.py
--rw-r--r--   0 root         (0) root         (0)     1543 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_redshift/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.757661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_snowflake/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_snowflake/api.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_snowflake/datatypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 19:56:25.757661 google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/
--rw-r--r--   0 root         (0) root         (0)     9164 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1210 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/api.py
--rw-r--r--   0 root         (0) root         (0)     1810 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/compiler.py
--rw-r--r--   0 root         (0) root         (0)     7034 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     8568 2024-03-18 19:55:09.000000 google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.669832 google_pso_data_validator-5.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11358 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    44174 2024-05-21 18:11:53.669832 google_pso_data_validator-5.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    42437 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.645830 google_pso_data_validator-5.0.0/data_validation/
+-rw-r--r--   0 root         (0) root         (0)      715 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26743 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/app.py
+-rw-r--r--   0 root         (0) root         (0)    48321 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/cli_tools.py
+-rw-r--r--   0 root         (0) root         (0)      881 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/client_info.py
+-rw-r--r--   0 root         (0) root         (0)     9690 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/clients.py
+-rw-r--r--   0 root         (0) root         (0)    14254 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/combiner.py
+-rw-r--r--   0 root         (0) root         (0)    40557 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/config_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/consts.py
+-rw-r--r--   0 root         (0) root         (0)    15266 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)      687 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/gcs_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/jellyfish_distance.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    16257 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/partition_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.649831 google_pso_data_validator-5.0.0/data_validation/query_builder/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/query_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/query_builder/partition_row_builder.py
+-rw-r--r--   0 root         (0) root         (0)    19435 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/query_builder/query_builder.py
+-rw-r--r--   0 root         (0) root         (0)     3697 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/query_builder/random_row_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.649831 google_pso_data_validator-5.0.0/data_validation/result_handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/result_handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/result_handlers/bigquery.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/result_handlers/text.py
+-rw-r--r--   0 root         (0) root         (0)    14320 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/schema_validation.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/secret_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/state_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16109 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/data_validation/validation_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.669832 google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    44174 2024-05-21 18:11:53.000000 google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3179 2024-05-21 18:11:53.000000 google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:11:53.000000 google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-21 18:11:53.000000 google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2024-05-21 18:11:53.000000 google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-21 18:11:53.000000 google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-21 18:11:53.669832 google_pso_data_validator-5.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.633829 google_pso_data_validator-5.0.0/third_party/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.637830 google_pso_data_validator-5.0.0/third_party/ibis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.653831 google_pso_data_validator-5.0.0/third_party/ibis/ibis_addon/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_addon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_addon/api.py
+-rw-r--r--   0 root         (0) root         (0)    24099 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_addon/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.653831 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/
+-rw-r--r--   0 root         (0) root         (0)     6916 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/api.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/client.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.657831 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.657831 google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/
+-rw-r--r--   0 root         (0) root         (0)     2649 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/api.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)    15987 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.657831 google_pso_data_validator-5.0.0/third_party/ibis/ibis_impala/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_impala/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_impala/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.657831 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mssql/
+-rw-r--r--   0 root         (0) root         (0)     2987 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mssql/api.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mssql/datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.661832 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.661832 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_mysql/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.661832 google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/
+-rw-r--r--   0 root         (0) root         (0)     3043 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/api.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     6593 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)    14411 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.665832 google_pso_data_validator-5.0.0/third_party/ibis/ibis_postgres/
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_postgres/client.py
+-rw-r--r--   0 root         (0) root         (0)      839 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_postgres/datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.665832 google_pso_data_validator-5.0.0/third_party/ibis/ibis_redshift/
+-rw-r--r--   0 root         (0) root         (0)     4053 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_redshift/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_redshift/api.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_redshift/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.665832 google_pso_data_validator-5.0.0/third_party/ibis/ibis_snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_snowflake/api.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_snowflake/datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:11:53.669832 google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/
+-rw-r--r--   0 root         (0) root         (0)     9164 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/api.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     9817 2024-05-21 18:10:11.000000 google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/registry.py
```

### Comparing `google-pso-data-validator-4.5.0/LICENSE` & `google_pso_data_validator-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/PKG-INFO` & `google_pso_data_validator-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-pso-data-validator
-Version: 4.5.0
+Version: 5.0.0
 Summary: A package to enable easy data validation
 Home-page: https://github.com/pypa/sampleproject
 Author: Dylan Hercher
 Author-email: dhercher@google.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -168,15 +168,15 @@
   [--cast-to-bigint or -ctb]
                         If flag is present, cast all int32 columns to int64 before aggregation
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--threshold or -th THRESHOLD]
                         Float value. Maximum pct_difference allowed for validation to be considered a success. Defaults to 0.0
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
@@ -238,15 +238,15 @@
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -318,15 +318,15 @@
                         e.g.: 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
                         Defaults  to table.
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail).
@@ -365,23 +365,23 @@
                         File containing the target sql commands
   [--count COLUMNS]     Comma separated list of columns for count or * for all columns
   [--sum COLUMNS]       Comma separated list of columns for sum or * for all numeric
   [--min COLUMNS]       Comma separated list of columns for min or * for all numeric
   [--max COLUMNS]       Comma separated list of columns for max or * for all numeric
   [--avg COLUMNS]       Comma separated list of columns for avg or * for all numeric
   [--std COLUMNS]       Comma separated list of columns for stddev_samp or * for all numeric
-  [--exclude-columns or -ec]   
+  [--exclude-columns or -ec]
                         Flag to indicate the list of columns provided should be excluded and not included.
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -435,15 +435,15 @@
                        Common column between source and target tables for join
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -479,32 +479,31 @@
 }
 ```
 
 ### Running DVT with YAML Configuration Files
 
 Running DVT with YAML configuration files is the recommended approach if:
 * you want to customize the configuration for any given validation OR
-* you want to run DVT at scale (i.e. row validations across many partitions)
+* you want to run DVT at scale (i.e. run multiple validations sequentially or in parallel)
 
-We recommend generating YAML configs with the `--config-file <file-name>` flag when running a validation command. The validation 
-config file is saved to the GCS path specified by the `PSO_DV_CONFIG_HOME` env variable if that has been set;
-otherwise, it is saved to wherever the tool is run.
+We recommend generating YAML configs with the `--config-file <file-name>` flag when running a validation command, which supports
+GCS and local paths.
 
 You can use the `data-validation configs` command to run and view YAMLs.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) configs run
   [--config-file or -c CONFIG_FILE]
                         Path to YAML config file to run. Supports local and GCS paths.
   [--config-dir or -cdir CONFIG_DIR]
                         Directory path containing YAML configs to be run sequentially. Supports local and GCS paths.
   [--dry-run or -dr]    If this flag is present, prints the source and target SQL generated in lieu of running the validation.
   [--kube-completions or -kc]
                         Flag to indicate usage in Kubernetes index completion mode.
-                        See *Scaling DVT to run 10's to 1000's of validations concurrently* section
+                        See *Scaling DVT* section
 ```
 
 ```
 data-validation configs list
   [--config-dir or -cdir CONFIG_DIR]
                         GCS or local directory from which to list validation YAML configs. Defaults to current local directory.
 ```
@@ -514,27 +513,25 @@
   [--config-file or -c CONFIG_FILE] GCS or local path of validation YAML to print.
 ```
 
 View the complete YAML file for a Grouped Column validation on the
 [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-config-grouped-column-validation) page.
 
 
-#### Scaling DVT to run 10's to 1000's of validations concurrently
+### Scaling DVT
 
-As described above, you can run multiple validation configs sequentially with the `--config-dir` flag. To optimize the validation speed for large tables, you can run DVT concurrently using GKE Jobs ([Google Kubernetes Jobs](https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview#batch_jobs)) or [Cloud Run Jobs](https://cloud.google.com/run/docs/create-jobs). If you are not familiar with Kubernetes or Cloud Run Jobs, see [Scaling DVT with Kubernetes](docs/internal/kubernetes_jobs.md) for a detailed overview.
+You can scale DVT for large table validations by running the tool in a distributed manner. To optimize the validation speed for large tables, you can use GKE Jobs ([Google Kubernetes Jobs](https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview#batch_jobs)) or [Cloud Run Jobs](https://cloud.google.com/run/docs/create-jobs). If you are not familiar with Kubernetes or Cloud Run Jobs, see [Scaling DVT with Distributed Jobs](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/internal/distributed_jobs.md) for a detailed overview.
 
-In order to validate partitions concurrently, both the `--kube-completions` and `--config-dir` flags are required. The `--kube-completions` flag specifies that the validation is being run in indexed completion mode in Kubernetes or as multiple independent tasks in Cloud Run. The `--config-dir` flag will specify the directory with the YAML files to be executed in parallel. If you used `generate-table-partitions` to generate the YAMLs, this would be the directory where the partition files numbered `0000.yaml` to `<partition_num - 1>.yaml` are stored i.e (`my_config_dir/source_schema.source_table/`)
 
-In order to run DVT in a container, you have to build a Docker image - [see instructions here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/tree/develop/samples/docker#readme). You will also need to set the `PSO_DV_CONFIG_HOME` environment variable to point to a GCS prefix where the connection configuration files are stored. In Cloud Run you can use the option `--set-env-vars` or `--update-env-vars` to pass [the environment variable](https://cloud.google.com/run/docs/configuring/services/environment-variables#setting). We recommend that you use the `bq-result-handler` to save your validation results to BigQuery. 
+We recommend first generating table partitions with the `generate-table-partitions` command for your large tables. Then, use Cloud Run or GKE to distribute validating each chunk in parallel. See the [Cloud Run Jobs Quickstart sample](https://github.com/GoogleCloudPlatform/professional-services-data-validator/tree/develop/samples/cloud_run_jobs) to get started. 
 
-The Cloud Run and Kubernetes pods must run in a network with access to the database servers. Every Cloud Run job is associated with a [service account](https://cloud.google.com/run/docs/securing/service-identity). You need to ensure that this service account has access to Google Cloud Storage (to read connection configuration and YAML files) and BigQuery (to publish results). If you are using Kubernetes, you will need to use a service account with the same privileges as mentioned for Cloud Run. In Kubernetes, you will need to set up [workload identity](https://cloud.google.com/kubernetes-engine/docs/how-to/workload-identity) so the DVT container can impersonate the service account.
+When running DVT in a distributed fashion, both the `--kube-completions` and `--config-dir` flags are required. The `--kube-completions` flag specifies that the validation is being run in indexed completion mode in Kubernetes or as multiple independent tasks in Cloud Run. If the `-kc` option is used and you are not running in indexed mode, you will receive a warning and the container will process all the validations sequentially. If the `-kc` option is used and a config directory is not provided (i.e. a `--config-file` is provided instead), a warning is issued.
 
-In Cloud Run, the [job](https://cloud.google.com/run/docs/create-jobs) must be run as multiple, independent tasks with the task count set to the number of partitions generated. In Kubernetes, set the number of completions to the number of partitions generated - see [Kubernetes Parallel Jobs](https://kubernetes.io/docs/concepts/workloads/controllers/job/#parallel-jobs). The option `--kube-completions or -kc` tells DVT that many DVT containers are running in a Kubernetes cluster. Each DVT container only validates the specific partition YAML (based on the index assigned by Kubernetes control plane). If the `-kc` option is used and you are not running in indexed mode, you will receive a warning and the container will process all the validations sequentially. If the `-kc` option is used and a config directory is not provided (a `--config-file` is provided instead), a warning is issued.
+The `--config-dir` flag will specify the directory with the YAML files to be executed in parallel. If you used `generate-table-partitions` to generate the YAMLs, this would be the directory where the partition files numbered `0000.yaml` to `<partition_num - 1>.yaml` are stored i.e (`gs://my_config_dir/source_schema.source_table/`). When creating your Cloud Run Job, set the number of tasks equal to the number of table partitions so the task index matches the YAML file to be validated. When executed, each Cloud Run task will validate a partition in parallel.
 
-By default, each partition validation is retried up to 3 times if there is an error. In Kubernetes and Cloud Run, you can set the parallelism to the number you want. Keep in mind that if you are validating 1000's of partitions in parallel, you may find that setting the parallelism too high (say 100) may result in timeouts and slow down the validation.   
 
 ### Validation Reports
 
 The result handlers tell DVT where to store the results of
 each validation. The tool can write the results of a validation run to Google
 BigQuery or print to stdout (default). View the schema of the results
 table [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/terraform/results_schema.json).
@@ -631,15 +628,16 @@
 If you are aggregating columns with large values, you can CAST() before aggregation
 with calculated fields as shown in [this example](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-with-calc-fields-cast-to-numeric-before-aggregation).
 
 ### Filters
 
 Filters let you apply a WHERE statement to your validation query (ie. `SELECT *
 FROM table WHERE created_at > 30 days ago AND region_id = 71;`). The filter is
-written in the syntax of the given source.
+written in the syntax of the given source and must reference columns in the
+underlying table, not projected DVT expressions.
 
 Note that you are writing the query to execute, which does not have to match
 between source and target as long as the results can be expected to align. If
 the target filter is omitted, the source filter will run on both the source and
 target tables.
 
 ### Primary Keys
```

### Comparing `google-pso-data-validator-4.5.0/README.md` & `google_pso_data_validator-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
   [--cast-to-bigint or -ctb]
                         If flag is present, cast all int32 columns to int64 before aggregation
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--threshold or -th THRESHOLD]
                         Float value. Maximum pct_difference allowed for validation to be considered a success. Defaults to 0.0
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
@@ -190,15 +190,15 @@
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -270,15 +270,15 @@
                         e.g.: 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
                         Defaults  to table.
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail).
@@ -317,23 +317,23 @@
                         File containing the target sql commands
   [--count COLUMNS]     Comma separated list of columns for count or * for all columns
   [--sum COLUMNS]       Comma separated list of columns for sum or * for all numeric
   [--min COLUMNS]       Comma separated list of columns for min or * for all numeric
   [--max COLUMNS]       Comma separated list of columns for max or * for all numeric
   [--avg COLUMNS]       Comma separated list of columns for avg or * for all numeric
   [--std COLUMNS]       Comma separated list of columns for stddev_samp or * for all numeric
-  [--exclude-columns or -ec]   
+  [--exclude-columns or -ec]
                         Flag to indicate the list of columns provided should be excluded and not included.
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -387,15 +387,15 @@
                        Common column between source and target tables for join
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -431,32 +431,31 @@
 }
 ```
 
 ### Running DVT with YAML Configuration Files
 
 Running DVT with YAML configuration files is the recommended approach if:
 * you want to customize the configuration for any given validation OR
-* you want to run DVT at scale (i.e. row validations across many partitions)
+* you want to run DVT at scale (i.e. run multiple validations sequentially or in parallel)
 
-We recommend generating YAML configs with the `--config-file <file-name>` flag when running a validation command. The validation 
-config file is saved to the GCS path specified by the `PSO_DV_CONFIG_HOME` env variable if that has been set;
-otherwise, it is saved to wherever the tool is run.
+We recommend generating YAML configs with the `--config-file <file-name>` flag when running a validation command, which supports
+GCS and local paths.
 
 You can use the `data-validation configs` command to run and view YAMLs.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) configs run
   [--config-file or -c CONFIG_FILE]
                         Path to YAML config file to run. Supports local and GCS paths.
   [--config-dir or -cdir CONFIG_DIR]
                         Directory path containing YAML configs to be run sequentially. Supports local and GCS paths.
   [--dry-run or -dr]    If this flag is present, prints the source and target SQL generated in lieu of running the validation.
   [--kube-completions or -kc]
                         Flag to indicate usage in Kubernetes index completion mode.
-                        See *Scaling DVT to run 10's to 1000's of validations concurrently* section
+                        See *Scaling DVT* section
 ```
 
 ```
 data-validation configs list
   [--config-dir or -cdir CONFIG_DIR]
                         GCS or local directory from which to list validation YAML configs. Defaults to current local directory.
 ```
@@ -466,27 +465,25 @@
   [--config-file or -c CONFIG_FILE] GCS or local path of validation YAML to print.
 ```
 
 View the complete YAML file for a Grouped Column validation on the
 [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-config-grouped-column-validation) page.
 
 
-#### Scaling DVT to run 10's to 1000's of validations concurrently
+### Scaling DVT
 
-As described above, you can run multiple validation configs sequentially with the `--config-dir` flag. To optimize the validation speed for large tables, you can run DVT concurrently using GKE Jobs ([Google Kubernetes Jobs](https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview#batch_jobs)) or [Cloud Run Jobs](https://cloud.google.com/run/docs/create-jobs). If you are not familiar with Kubernetes or Cloud Run Jobs, see [Scaling DVT with Kubernetes](docs/internal/kubernetes_jobs.md) for a detailed overview.
+You can scale DVT for large table validations by running the tool in a distributed manner. To optimize the validation speed for large tables, you can use GKE Jobs ([Google Kubernetes Jobs](https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview#batch_jobs)) or [Cloud Run Jobs](https://cloud.google.com/run/docs/create-jobs). If you are not familiar with Kubernetes or Cloud Run Jobs, see [Scaling DVT with Distributed Jobs](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/internal/distributed_jobs.md) for a detailed overview.
 
-In order to validate partitions concurrently, both the `--kube-completions` and `--config-dir` flags are required. The `--kube-completions` flag specifies that the validation is being run in indexed completion mode in Kubernetes or as multiple independent tasks in Cloud Run. The `--config-dir` flag will specify the directory with the YAML files to be executed in parallel. If you used `generate-table-partitions` to generate the YAMLs, this would be the directory where the partition files numbered `0000.yaml` to `<partition_num - 1>.yaml` are stored i.e (`my_config_dir/source_schema.source_table/`)
 
-In order to run DVT in a container, you have to build a Docker image - [see instructions here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/tree/develop/samples/docker#readme). You will also need to set the `PSO_DV_CONFIG_HOME` environment variable to point to a GCS prefix where the connection configuration files are stored. In Cloud Run you can use the option `--set-env-vars` or `--update-env-vars` to pass [the environment variable](https://cloud.google.com/run/docs/configuring/services/environment-variables#setting). We recommend that you use the `bq-result-handler` to save your validation results to BigQuery. 
+We recommend first generating table partitions with the `generate-table-partitions` command for your large tables. Then, use Cloud Run or GKE to distribute validating each chunk in parallel. See the [Cloud Run Jobs Quickstart sample](https://github.com/GoogleCloudPlatform/professional-services-data-validator/tree/develop/samples/cloud_run_jobs) to get started. 
 
-The Cloud Run and Kubernetes pods must run in a network with access to the database servers. Every Cloud Run job is associated with a [service account](https://cloud.google.com/run/docs/securing/service-identity). You need to ensure that this service account has access to Google Cloud Storage (to read connection configuration and YAML files) and BigQuery (to publish results). If you are using Kubernetes, you will need to use a service account with the same privileges as mentioned for Cloud Run. In Kubernetes, you will need to set up [workload identity](https://cloud.google.com/kubernetes-engine/docs/how-to/workload-identity) so the DVT container can impersonate the service account.
+When running DVT in a distributed fashion, both the `--kube-completions` and `--config-dir` flags are required. The `--kube-completions` flag specifies that the validation is being run in indexed completion mode in Kubernetes or as multiple independent tasks in Cloud Run. If the `-kc` option is used and you are not running in indexed mode, you will receive a warning and the container will process all the validations sequentially. If the `-kc` option is used and a config directory is not provided (i.e. a `--config-file` is provided instead), a warning is issued.
 
-In Cloud Run, the [job](https://cloud.google.com/run/docs/create-jobs) must be run as multiple, independent tasks with the task count set to the number of partitions generated. In Kubernetes, set the number of completions to the number of partitions generated - see [Kubernetes Parallel Jobs](https://kubernetes.io/docs/concepts/workloads/controllers/job/#parallel-jobs). The option `--kube-completions or -kc` tells DVT that many DVT containers are running in a Kubernetes cluster. Each DVT container only validates the specific partition YAML (based on the index assigned by Kubernetes control plane). If the `-kc` option is used and you are not running in indexed mode, you will receive a warning and the container will process all the validations sequentially. If the `-kc` option is used and a config directory is not provided (a `--config-file` is provided instead), a warning is issued.
+The `--config-dir` flag will specify the directory with the YAML files to be executed in parallel. If you used `generate-table-partitions` to generate the YAMLs, this would be the directory where the partition files numbered `0000.yaml` to `<partition_num - 1>.yaml` are stored i.e (`gs://my_config_dir/source_schema.source_table/`). When creating your Cloud Run Job, set the number of tasks equal to the number of table partitions so the task index matches the YAML file to be validated. When executed, each Cloud Run task will validate a partition in parallel.
 
-By default, each partition validation is retried up to 3 times if there is an error. In Kubernetes and Cloud Run, you can set the parallelism to the number you want. Keep in mind that if you are validating 1000's of partitions in parallel, you may find that setting the parallelism too high (say 100) may result in timeouts and slow down the validation.   
 
 ### Validation Reports
 
 The result handlers tell DVT where to store the results of
 each validation. The tool can write the results of a validation run to Google
 BigQuery or print to stdout (default). View the schema of the results
 table [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/terraform/results_schema.json).
@@ -583,15 +580,16 @@
 If you are aggregating columns with large values, you can CAST() before aggregation
 with calculated fields as shown in [this example](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-with-calc-fields-cast-to-numeric-before-aggregation).
 
 ### Filters
 
 Filters let you apply a WHERE statement to your validation query (ie. `SELECT *
 FROM table WHERE created_at > 30 days ago AND region_id = 71;`). The filter is
-written in the syntax of the given source.
+written in the syntax of the given source and must reference columns in the
+underlying table, not projected DVT expressions.
 
 Note that you are writing the query to execute, which does not have to match
 between source and target as long as the results can be expected to align. If
 the target filter is omitted, the source filter will run on both the source and
 target tables.
 
 ### Primary Keys
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/__init__.py` & `google_pso_data_validator-5.0.0/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/__main__.py` & `google_pso_data_validator-5.0.0/data_validation/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,29 @@
 }
 
 
 def _get_arg_config_file(args):
     """Return String YAML config file path."""
     if not args.config_file:
         raise ValueError("YAML Config File was not supplied.")
-
+    elif not args.config_file.endswith(".yaml"):
+        raise ValueError(
+            f"Invalid YAML config name: {args.config_file}. Provide YAML file extension."
+        )
     return args.config_file
 
 
 def _get_arg_config_file_json(args):
     """Return String JSON config file path."""
     if not args.config_file_json:
         raise ValueError("JSON Config File was not supplied.")
-
+    elif not args.config_file_json.endswith(".json"):
+        raise ValueError(
+            f"Invalid JSON config name: {args.config_file_json}. Provide JSON file extension."
+        )
     return args.config_file_json
 
 
 def get_aggregate_config(args, config_manager: ConfigManager):
     """Return list of formatted aggregation objects.
 
     Args:
@@ -346,38 +352,38 @@
                 f"{args.config_dir}{job_index:04d}.yaml"
                 if args.config_dir.endswith("/")
                 else f"{args.config_dir}/{job_index:04d}.yaml"
             )
             setattr(args, "config_dir", None)
             setattr(args, "config_file", config_file_path)
             config_managers = build_config_managers_from_yaml(args, config_file_path)
+            run_validations(args, config_managers)
         else:
             if args.kube_completions:
                 logging.warning(
                     "--kube-completions or -kc specified, however not running in Kubernetes Job completion, check your command line."
                 )
-            mgr = state_manager.StateManager(file_system_root_path=args.config_dir)
-            config_file_names = mgr.list_validations_in_dir(args.config_dir)
+            config_file_names = cli_tools.list_validations(config_dir=args.config_dir)
             config_managers = []
             for file in config_file_names:
-                config_managers.extend(build_config_managers_from_yaml(args, file))
+                config_managers = build_config_managers_from_yaml(args, file)
+                run_validations(args, config_managers)
     else:
         if args.kube_completions:
             logging.warning(
                 "--kube-completions or -kc specified, which requires a config directory, however a specific config file is provided."
             )
         config_file_path = _get_arg_config_file(args)
         config_managers = build_config_managers_from_yaml(args, config_file_path)
-
-    run_validations(args, config_managers)
+        run_validations(args, config_managers)
 
 
 def build_config_managers_from_yaml(args, config_file_path):
     """Returns List[ConfigManager] instances ready to be executed."""
-    if "config_dir" in args and args.config_dir:
+    if args.config_dir:
         yaml_configs = cli_tools.get_validation(config_file_path, args.config_dir)
     else:
         yaml_configs = cli_tools.get_validation(config_file_path)
 
     mgr = state_manager.StateManager()
     source_conn = mgr.get_connection_config(yaml_configs[consts.YAML_SOURCE])
     target_conn = mgr.get_connection_config(yaml_configs[consts.YAML_TARGET])
@@ -612,15 +618,15 @@
     """Build a JSON config file from the supplied configs.
 
     Args:
         config_managers (list[ConfigManager]): List of config manager instances.
     """
     json_config = convert_config_to_json(config_managers)
     config_file_path = _get_arg_config_file_json(args)
-    cli_tools.store_validation_json(config_file_path, json_config)
+    cli_tools.store_validation(config_file_path, json_config)
 
 
 def partition_and_store_config_files(args: Namespace) -> None:
     """Build multiple YAML Config files using user specified partition logic
 
     Args:
         args (Namespace): User specified Arguments
@@ -669,15 +675,15 @@
 
 def run_validation_configs(args):
     """Run commands related to validation config YAMLs."""
     if args.validation_config_cmd == "run":
         config_runner(args)
     elif args.validation_config_cmd == "list":
         config_dir = args.config_dir or "./"
-        cli_tools.list_validations(config_dir=config_dir)
+        cli_tools.print_validations_in_dir(config_dir=config_dir)
     elif args.validation_config_cmd == "get":
         # Get and print yaml file config.
         yaml = cli_tools.get_validation(_get_arg_config_file(args))
         dump(yaml, sys.stdout)
     else:
         raise ValueError(f"Configs argument '{args.validate_cmd}' is not supported")
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/app.py` & `google_pso_data_validator-5.0.0/data_validation/app.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/cli_tools.py` & `google_pso_data_validator-5.0.0/data_validation/cli_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,18 +45,20 @@
 
 import argparse
 import csv
 import json
 import logging
 import sys
 import uuid
+import os
 from argparse import Namespace
 from typing import Dict, List
+from yaml import Dumper, Loader, dump, load
 
-from data_validation import clients, consts, state_manager
+from data_validation import clients, consts, state_manager, gcs_helper
 
 CONNECTION_SOURCE_FIELDS = {
     "BigQuery": [
         ["project_id", "GCP Project to use for BigQuery"],
         ["google_service_account_key_path", "(Optional) GCP SA Key Path"],
     ],
     "Teradata": [
@@ -1077,55 +1079,54 @@
 
 def get_connection(connection_name):
     """Return dict connection details for a specific connection."""
     mgr = state_manager.StateManager()
     return mgr.get_connection_config(connection_name)
 
 
-def store_validation(validation_file_name, yaml_config):
-    """Store the validation YAML config under the given name."""
-    mgr = state_manager.StateManager()
-    mgr.create_validation_yaml(validation_file_name, yaml_config)
+def store_validation(validation_file_name, config, include_log=True):
+    """Store the validation config under the given name."""
+    validation_path = gcs_helper.get_validation_path(validation_file_name)
+
+    if validation_file_name.endswith(".yaml"):
+        config_str = dump(config, Dumper=Dumper)
+    elif validation_file_name.endswith("json"):
+        config_str = json.dumps(config)
+    else:
+        raise ValueError(f"Invalid validation file name: {validation_file_name}")
 
+    gcs_helper.write_file(validation_path, config_str, include_log=include_log)
 
-def store_validation_json(validation_file_name, json_config):
-    """Store the validation JSON config under the given name."""
-    mgr = state_manager.StateManager()
-    mgr.create_validation_json(validation_file_name, json_config)
 
+def get_validation(name: str, config_dir: str = None):
+    """Return validation YAML config."""
+    if config_dir:
+        validation_path = os.path.join(config_dir, name)
+    else:
+        validation_path = gcs_helper.get_validation_path(name)
 
-def store_partition(target_file_path, yaml_config, target_folder_path=None):
-    """Store the partition YAML config under the given name."""
-    mgr = state_manager.StateManager(target_folder_path)
-    mgr.create_partition_yaml(target_file_path, yaml_config)
+    validation_bytes = gcs_helper.read_file(validation_path)
+    return load(validation_bytes, Loader=Loader)
 
 
-def get_validation(validation_name, config_dir=None):
-    """Return validation YAML for a specific connection."""
-    if config_dir:
-        mgr = state_manager.StateManager(file_system_root_path=config_dir)
-        return mgr.get_validation_config(validation_name, config_dir)
+def list_validations(config_dir="./"):
+    """List all saved validation YAMLs in a directory."""
+    logging.info(f"Looking for validations in path {config_dir}")
+    if gcs_helper._is_gcs_path(config_dir):
+        if not config_dir.endswith("/"):
+            config_dir += "/"
+        files = gcs_helper.list_gcs_directory(config_dir)
     else:
-        if validation_name.startswith("gs://"):
-            obj_depth = len(validation_name.split("/"))
-            gcs_prefix = "/".join(validation_name.split("/")[: obj_depth - 1])
-            mgr = state_manager.StateManager(file_system_root_path=gcs_prefix)
-            return mgr.get_validation_config(
-                validation_name.split("/")[obj_depth - 1], gcs_prefix
-            )
-        else:
-            mgr = state_manager.StateManager()
-            return mgr.get_validation_config(validation_name)
+        files = os.listdir(config_dir)
 
+    return [file_name for file_name in files if file_name.endswith(".yaml")]
 
-def list_validations(config_dir="./"):
-    """List all saved validation YAMLs."""
-    mgr = state_manager.StateManager(file_system_root_path=config_dir)
-    validations = mgr.list_validations_in_dir(config_dir=config_dir)
 
+def print_validations_in_dir(config_dir="./"):
+    validations = list_validations(config_dir=config_dir)
     logging.info("Validation YAMLs found:")
     for validation_name in validations:
         logging.info(validation_name)
 
 
 def get_labels(arg_labels):
     """Return list of tuples representing key-value label pairs."""
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/client_info.py` & `google_pso_data_validator-5.0.0/data_validation/client_info.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/clients.py` & `google_pso_data_validator-5.0.0/data_validation/clients.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/combiner.py` & `google_pso_data_validator-5.0.0/data_validation/combiner.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/config_manager.py` & `google_pso_data_validator-5.0.0/data_validation/config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import logging
-from typing import Optional, Union, TYPE_CHECKING
-import yaml
+from typing import TYPE_CHECKING, Optional, Union
 
 import google.oauth2.service_account
-
 import ibis.expr.datatypes as dt
+import yaml
 
-from data_validation import clients, consts, state_manager
+from data_validation import clients, consts, gcs_helper, state_manager
 from data_validation.result_handlers.bigquery import BigQueryResultHandler
 from data_validation.result_handlers.text import TextResultHandler
 from data_validation.validation_builder import ValidationBuilder
 
-
 if TYPE_CHECKING:
     import ibis.expr.types.TableExpr
 
 
 class ConfigManager(object):
     _config: dict = None
     _source_conn = None
@@ -318,17 +316,16 @@
     ):
         """Append datatype allow_list to existing config."""
         full_allow_list = []
         if allow_list:
             allow_list = allow_list.replace(" ", "")
             full_allow_list.append(allow_list)
         if allow_list_file:
-            mgr = state_manager.StateManager(file_system_root_path=allow_list_file)
             try:
-                allow_list_yaml = mgr.read_file(allow_list_file)
+                allow_list_yaml = gcs_helper.read_file(allow_list_file)
             except FileNotFoundError as e:
                 raise ValueError(
                     "Cannot locate --allow-list-file: {allow_list_file}"
                 ) from e
             allow_list_dict = yaml.safe_load(allow_list_yaml)
             full_allow_list.append(
                 ",".join([f"{_[0]}:{_[1]}" for _ in allow_list_dict.items()])
@@ -539,15 +536,15 @@
                 casefold_source_columns[column.casefold()]
             ].type()
             target_ibis_type = target_table[
                 casefold_target_columns[column.casefold()]
             ].type()
             cast_type = (
                 "string"
-                if self._decimal_column_too_big_for_pandas(
+                if self._key_column_needs_casting_to_string(
                     source_ibis_type, target_ibis_type
                 )
                 else None
             )
 
             column_config = {
                 consts.CONFIG_SOURCE_COLUMN: casefold_source_columns[column.casefold()],
@@ -691,14 +688,27 @@
                 and (
                     target_column_ibis_type.precision is None
                     or target_column_ibis_type.precision > 18
                 )
             )
         )
 
+    def _key_column_needs_casting_to_string(
+        self,
+        source_column_ibis_type: dt.DataType,
+        target_column_ibis_type: dt.DataType,
+    ) -> bool:
+        return bool(
+            self._decimal_column_too_big_for_pandas(
+                source_column_ibis_type, target_column_ibis_type
+            )
+            or isinstance(source_column_ibis_type, dt.Binary)
+            or isinstance(target_column_ibis_type, dt.Binary)
+        )
+
     def build_config_column_aggregates(
         self, agg_type, arg_value, exclude_cols, supported_types, cast_to_bigint=False
     ):
         """Return list of aggregate objects of given agg_type."""
 
         def require_pre_agg_calc_field(
             column_type: str, agg_type: str, cast_to_bigint: bool
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/consts.py` & `google_pso_data_validator-5.0.0/data_validation/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     ROW_VALIDATION,
     SCHEMA_VALIDATION,
     CUSTOM_QUERY,
 ]
 
 # State Manager Fields
 DEFAULT_ENV_DIRECTORY = "~/.config/google-pso-data-validator/"
-ENV_DIRECTORY_VAR = "PSO_DV_CONFIG_HOME"
+ENV_DIRECTORY_VAR = "PSO_DV_CONN_HOME"
 
 # Yaml File Config Fields
 YAML_RESULT_HANDLER = "result_handler"
 YAML_SOURCE = "source"
 YAML_TARGET = "target"
 YAML_VALIDATIONS = "validations"
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/data_validation.py` & `google_pso_data_validator-5.0.0/data_validation/data_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,18 +102,23 @@
 
     def _add_random_row_filter(self):
         """Add random row filters to the validation builder."""
         if not self.config_manager.primary_keys:
             raise ValueError("Primary Keys are required for Random Row Filters")
 
         # Filter for only first primary key (multi-pk filter not supported)
-        primary_key_info = self.config_manager.primary_keys[0]
+        source_pk_column = self.config_manager.primary_keys[0][
+            consts.CONFIG_SOURCE_COLUMN
+        ]
+        target_pk_column = self.config_manager.primary_keys[0][
+            consts.CONFIG_TARGET_COLUMN
+        ]
 
         randomRowBuilder = RandomRowBuilder(
-            [primary_key_info[consts.CONFIG_SOURCE_COLUMN]],
+            [source_pk_column],
             self.config_manager.random_row_batch_size(),
         )
 
         if (self.config_manager.validation_type == consts.CUSTOM_QUERY) and (
             self.config_manager.custom_query_type == consts.ROW_VALIDATION.lower()
         ):
             query = randomRowBuilder.compile_custom_query(
@@ -124,32 +129,41 @@
             query = randomRowBuilder.compile(
                 self.config_manager.source_client,
                 self.config_manager.source_schema,
                 self.config_manager.source_table,
                 self.validation_builder.source_builder,
             )
 
+        # Check if source table's primary key is BINARY, if so then
+        # force cast the id columns to STRING (HEX).
+        binary_conversion_required = False
+        if query[source_pk_column].type().is_binary():
+            binary_conversion_required = True
+            query = query.mutate(
+                **{source_pk_column: query[source_pk_column].cast("string")}
+            )
+
         random_rows = self.config_manager.source_client.execute(query)
         if len(random_rows) == 0:
             return
+
+        random_values = list(random_rows[source_pk_column])
+        if binary_conversion_required:
+            # For binary ids we have a list of hex strings for our IN list.
+            # Each of these needs to be cast back to binary.
+            random_values = [ibis.literal(_).cast("binary") for _ in random_values]
+
         filter_field = {
             consts.CONFIG_TYPE: consts.FILTER_TYPE_ISIN,
-            consts.CONFIG_FILTER_SOURCE_COLUMN: primary_key_info[
-                consts.CONFIG_FIELD_ALIAS
-            ],
-            consts.CONFIG_FILTER_SOURCE_VALUE: random_rows[
-                primary_key_info[consts.CONFIG_SOURCE_COLUMN]
-            ],
-            consts.CONFIG_FILTER_TARGET_COLUMN: primary_key_info[
-                consts.CONFIG_FIELD_ALIAS
-            ],
-            consts.CONFIG_FILTER_TARGET_VALUE: random_rows[
-                primary_key_info[consts.CONFIG_SOURCE_COLUMN]
-            ],
+            consts.CONFIG_FILTER_SOURCE_COLUMN: source_pk_column,
+            consts.CONFIG_FILTER_SOURCE_VALUE: random_values,
+            consts.CONFIG_FILTER_TARGET_COLUMN: target_pk_column,
+            consts.CONFIG_FILTER_TARGET_VALUE: random_values,
         }
+
         self.validation_builder.add_filter(filter_field)
 
     def query_too_large(self, rows_df, grouped_fields):
         """Return bool to dictate if another level of recursion
         would create a too large result set.
 
         Rules to define too large are:
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/exceptions.py` & `google_pso_data_validator-5.0.0/data_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/jellyfish_distance.py` & `google_pso_data_validator-5.0.0/data_validation/jellyfish_distance.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/metadata.py` & `google_pso_data_validator-5.0.0/data_validation/metadata.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/partition_builder.py` & `google_pso_data_validator-5.0.0/data_validation/partition_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,14 +357,14 @@
         for table in yaml_configs_list:
             target_folder_name = table["target_folder_name"]
             target_folder_path = os.path.join(self.config_dir, target_folder_name)
             for partition in table["partitions"]:
                 yaml_config = partition["yaml_config"]
                 target_file_name = partition["target_file_name"]
                 target_file_path = os.path.join(target_folder_path, target_file_name)
-                cli_tools.store_partition(
-                    target_file_path, yaml_config, target_folder_path
+                cli_tools.store_validation(
+                    target_file_path, yaml_config, include_log=False
                 )
 
         logging.info(
             f"Success! Table partition configs written to directory: {self.config_dir}"
         )
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/query_builder/__init__.py` & `google_pso_data_validator-5.0.0/data_validation/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/query_builder/partition_row_builder.py` & `google_pso_data_validator-5.0.0/data_validation/query_builder/partition_row_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/query_builder/query_builder.py` & `google_pso_data_validator-5.0.0/data_validation/query_builder/query_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -496,33 +496,40 @@
         """Return an Ibis query object
 
         Args:
             table (IbisTable): The Ibis Table expression.
         """
 
         # Build Query Expressions
+        compiled_filters = self.compile_filter_fields(table)
+        filtered_table = table.filter(compiled_filters) if compiled_filters else table
+
         if self.calculated_fields:
             depth_limit = max(
                 field.config.get(consts.CONFIG_DEPTH, 0)
                 for field in self.calculated_fields
             )
             for n in range(0, (depth_limit + 1)):
-                table = table.mutate(self.compile_calculated_fields(table, n))
+                filtered_table = filtered_table.mutate(
+                    self.compile_calculated_fields(filtered_table, n)
+                )
 
         if (
             validation_type == consts.ROW_VALIDATION
             or validation_type == consts.CUSTOM_QUERY
         ):
             if self.comparison_fields:
-                table = table.projection(self.compile_comparison_fields(table))
+                filtered_table = filtered_table.projection(
+                    self.compile_comparison_fields(filtered_table)
+                )
         else:
             if self.comparison_fields:
-                table = table.mutate(self.compile_comparison_fields(table))
-        compiled_filters = self.compile_filter_fields(table)
-        filtered_table = table.filter(compiled_filters) if compiled_filters else table
+                filtered_table = filtered_table.mutate(
+                    self.compile_comparison_fields(filtered_table)
+                )
         compiled_groups = self.compile_group_fields(filtered_table)
         grouped_table = (
             filtered_table.group_by(compiled_groups)
             if compiled_groups
             else filtered_table
         )
         if self.aggregate_fields:
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/query_builder/random_row_builder.py` & `google_pso_data_validator-5.0.0/data_validation/query_builder/random_row_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/result_handlers/bigquery.py` & `google_pso_data_validator-5.0.0/data_validation/result_handlers/bigquery.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/result_handlers/text.py` & `google_pso_data_validator-5.0.0/data_validation/result_handlers/text.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/schema_validation.py` & `google_pso_data_validator-5.0.0/data_validation/schema_validation.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/data_validation/secret_manager.py` & `google_pso_data_validator-5.0.0/data_validation/secret_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright 2021 Google LLC
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
```

### Comparing `google-pso-data-validator-4.5.0/data_validation/validation_builder.py` & `google_pso_data_validator-5.0.0/data_validation/validation_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/PKG-INFO` & `google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-pso-data-validator
-Version: 4.5.0
+Version: 5.0.0
 Summary: A package to enable easy data validation
 Home-page: https://github.com/pypa/sampleproject
 Author: Dylan Hercher
 Author-email: dhercher@google.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -168,15 +168,15 @@
   [--cast-to-bigint or -ctb]
                         If flag is present, cast all int32 columns to int64 before aggregation
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--threshold or -th THRESHOLD]
                         Float value. Maximum pct_difference allowed for validation to be considered a success. Defaults to 0.0
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
@@ -238,15 +238,15 @@
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -318,15 +318,15 @@
                         e.g.: 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
                         Defaults  to table.
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail).
@@ -365,23 +365,23 @@
                         File containing the target sql commands
   [--count COLUMNS]     Comma separated list of columns for count or * for all columns
   [--sum COLUMNS]       Comma separated list of columns for sum or * for all numeric
   [--min COLUMNS]       Comma separated list of columns for min or * for all numeric
   [--max COLUMNS]       Comma separated list of columns for max or * for all numeric
   [--avg COLUMNS]       Comma separated list of columns for avg or * for all numeric
   [--std COLUMNS]       Comma separated list of columns for stddev_samp or * for all numeric
-  [--exclude-columns or -ec]   
+  [--exclude-columns or -ec]
                         Flag to indicate the list of columns provided should be excluded and not included.
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -435,15 +435,15 @@
                        Common column between source and target tables for join
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
-                        YAML Config File Path to be used for storing validations and other features.
+                        YAML Config File Path to be used for storing validations and other features. Supports GCS and local paths.
                         See: *Running DVT with YAML Configuration Files* section
   [--config-file-json or -cj CONFIG_FILE_JSON]
                         JSON Config File Path to be used for storing validations only for application purposes.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt FORMAT]
                         Format for stdout output. Supported formats are (text, csv, json, table). Defaults to table.
@@ -479,32 +479,31 @@
 }
 ```
 
 ### Running DVT with YAML Configuration Files
 
 Running DVT with YAML configuration files is the recommended approach if:
 * you want to customize the configuration for any given validation OR
-* you want to run DVT at scale (i.e. row validations across many partitions)
+* you want to run DVT at scale (i.e. run multiple validations sequentially or in parallel)
 
-We recommend generating YAML configs with the `--config-file <file-name>` flag when running a validation command. The validation 
-config file is saved to the GCS path specified by the `PSO_DV_CONFIG_HOME` env variable if that has been set;
-otherwise, it is saved to wherever the tool is run.
+We recommend generating YAML configs with the `--config-file <file-name>` flag when running a validation command, which supports
+GCS and local paths.
 
 You can use the `data-validation configs` command to run and view YAMLs.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) configs run
   [--config-file or -c CONFIG_FILE]
                         Path to YAML config file to run. Supports local and GCS paths.
   [--config-dir or -cdir CONFIG_DIR]
                         Directory path containing YAML configs to be run sequentially. Supports local and GCS paths.
   [--dry-run or -dr]    If this flag is present, prints the source and target SQL generated in lieu of running the validation.
   [--kube-completions or -kc]
                         Flag to indicate usage in Kubernetes index completion mode.
-                        See *Scaling DVT to run 10's to 1000's of validations concurrently* section
+                        See *Scaling DVT* section
 ```
 
 ```
 data-validation configs list
   [--config-dir or -cdir CONFIG_DIR]
                         GCS or local directory from which to list validation YAML configs. Defaults to current local directory.
 ```
@@ -514,27 +513,25 @@
   [--config-file or -c CONFIG_FILE] GCS or local path of validation YAML to print.
 ```
 
 View the complete YAML file for a Grouped Column validation on the
 [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-config-grouped-column-validation) page.
 
 
-#### Scaling DVT to run 10's to 1000's of validations concurrently
+### Scaling DVT
 
-As described above, you can run multiple validation configs sequentially with the `--config-dir` flag. To optimize the validation speed for large tables, you can run DVT concurrently using GKE Jobs ([Google Kubernetes Jobs](https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview#batch_jobs)) or [Cloud Run Jobs](https://cloud.google.com/run/docs/create-jobs). If you are not familiar with Kubernetes or Cloud Run Jobs, see [Scaling DVT with Kubernetes](docs/internal/kubernetes_jobs.md) for a detailed overview.
+You can scale DVT for large table validations by running the tool in a distributed manner. To optimize the validation speed for large tables, you can use GKE Jobs ([Google Kubernetes Jobs](https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview#batch_jobs)) or [Cloud Run Jobs](https://cloud.google.com/run/docs/create-jobs). If you are not familiar with Kubernetes or Cloud Run Jobs, see [Scaling DVT with Distributed Jobs](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/internal/distributed_jobs.md) for a detailed overview.
 
-In order to validate partitions concurrently, both the `--kube-completions` and `--config-dir` flags are required. The `--kube-completions` flag specifies that the validation is being run in indexed completion mode in Kubernetes or as multiple independent tasks in Cloud Run. The `--config-dir` flag will specify the directory with the YAML files to be executed in parallel. If you used `generate-table-partitions` to generate the YAMLs, this would be the directory where the partition files numbered `0000.yaml` to `<partition_num - 1>.yaml` are stored i.e (`my_config_dir/source_schema.source_table/`)
 
-In order to run DVT in a container, you have to build a Docker image - [see instructions here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/tree/develop/samples/docker#readme). You will also need to set the `PSO_DV_CONFIG_HOME` environment variable to point to a GCS prefix where the connection configuration files are stored. In Cloud Run you can use the option `--set-env-vars` or `--update-env-vars` to pass [the environment variable](https://cloud.google.com/run/docs/configuring/services/environment-variables#setting). We recommend that you use the `bq-result-handler` to save your validation results to BigQuery. 
+We recommend first generating table partitions with the `generate-table-partitions` command for your large tables. Then, use Cloud Run or GKE to distribute validating each chunk in parallel. See the [Cloud Run Jobs Quickstart sample](https://github.com/GoogleCloudPlatform/professional-services-data-validator/tree/develop/samples/cloud_run_jobs) to get started. 
 
-The Cloud Run and Kubernetes pods must run in a network with access to the database servers. Every Cloud Run job is associated with a [service account](https://cloud.google.com/run/docs/securing/service-identity). You need to ensure that this service account has access to Google Cloud Storage (to read connection configuration and YAML files) and BigQuery (to publish results). If you are using Kubernetes, you will need to use a service account with the same privileges as mentioned for Cloud Run. In Kubernetes, you will need to set up [workload identity](https://cloud.google.com/kubernetes-engine/docs/how-to/workload-identity) so the DVT container can impersonate the service account.
+When running DVT in a distributed fashion, both the `--kube-completions` and `--config-dir` flags are required. The `--kube-completions` flag specifies that the validation is being run in indexed completion mode in Kubernetes or as multiple independent tasks in Cloud Run. If the `-kc` option is used and you are not running in indexed mode, you will receive a warning and the container will process all the validations sequentially. If the `-kc` option is used and a config directory is not provided (i.e. a `--config-file` is provided instead), a warning is issued.
 
-In Cloud Run, the [job](https://cloud.google.com/run/docs/create-jobs) must be run as multiple, independent tasks with the task count set to the number of partitions generated. In Kubernetes, set the number of completions to the number of partitions generated - see [Kubernetes Parallel Jobs](https://kubernetes.io/docs/concepts/workloads/controllers/job/#parallel-jobs). The option `--kube-completions or -kc` tells DVT that many DVT containers are running in a Kubernetes cluster. Each DVT container only validates the specific partition YAML (based on the index assigned by Kubernetes control plane). If the `-kc` option is used and you are not running in indexed mode, you will receive a warning and the container will process all the validations sequentially. If the `-kc` option is used and a config directory is not provided (a `--config-file` is provided instead), a warning is issued.
+The `--config-dir` flag will specify the directory with the YAML files to be executed in parallel. If you used `generate-table-partitions` to generate the YAMLs, this would be the directory where the partition files numbered `0000.yaml` to `<partition_num - 1>.yaml` are stored i.e (`gs://my_config_dir/source_schema.source_table/`). When creating your Cloud Run Job, set the number of tasks equal to the number of table partitions so the task index matches the YAML file to be validated. When executed, each Cloud Run task will validate a partition in parallel.
 
-By default, each partition validation is retried up to 3 times if there is an error. In Kubernetes and Cloud Run, you can set the parallelism to the number you want. Keep in mind that if you are validating 1000's of partitions in parallel, you may find that setting the parallelism too high (say 100) may result in timeouts and slow down the validation.   
 
 ### Validation Reports
 
 The result handlers tell DVT where to store the results of
 each validation. The tool can write the results of a validation run to Google
 BigQuery or print to stdout (default). View the schema of the results
 table [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/terraform/results_schema.json).
@@ -631,15 +628,16 @@
 If you are aggregating columns with large values, you can CAST() before aggregation
 with calculated fields as shown in [this example](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-with-calc-fields-cast-to-numeric-before-aggregation).
 
 ### Filters
 
 Filters let you apply a WHERE statement to your validation query (ie. `SELECT *
 FROM table WHERE created_at > 30 days ago AND region_id = 71;`). The filter is
-written in the syntax of the given source.
+written in the syntax of the given source and must reference columns in the
+underlying table, not projected DVT expressions.
 
 Note that you are writing the query to execute, which does not have to match
 between source and target as long as the results can be expected to align. If
 the target filter is omitted, the source filter will run on both the source and
 target tables.
 
 ### Primary Keys
```

### Comparing `google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/SOURCES.txt` & `google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 data_validation/client_info.py
 data_validation/clients.py
 data_validation/combiner.py
 data_validation/config_manager.py
 data_validation/consts.py
 data_validation/data_validation.py
 data_validation/exceptions.py
+data_validation/gcs_helper.py
 data_validation/jellyfish_distance.py
 data_validation/metadata.py
 data_validation/partition_builder.py
 data_validation/schema_validation.py
 data_validation/secret_manager.py
 data_validation/state_manager.py
 data_validation/validation_builder.py
```

### Comparing `google-pso-data-validator-4.5.0/google_pso_data_validator.egg-info/requires.txt` & `google_pso_data_validator-5.0.0/google_pso_data_validator.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/setup.py` & `google_pso_data_validator-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import os
 
 import setuptools
 
 name = "google-pso-data-validator"
 description = "A package to enable easy data validation"
-version = "4.5.0"
+version = "5.0.0"
 release_status = "Development Status :: 3 - Alpha"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 dependencies = [
     # Dependency corrections from our requirements
```

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_addon/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_addon/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_addon/operations.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_addon/operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,20 +31,26 @@
 import ibis.expr.rules as rlz
 import pandas as pd
 import sqlalchemy as sa
 from ibis.backends.base.sql.alchemy.registry import _cast as sa_fixed_cast
 from ibis.backends.base.sql.alchemy.registry import fixed_arity as sa_fixed_arity
 from ibis.backends.base.sql.alchemy.translator import AlchemyExprTranslator
 from ibis.backends.base.sql.compiler.translator import ExprTranslator
-from ibis.backends.base.sql.registry import fixed_arity
-from ibis.backends.bigquery.client import _DTYPE_TO_IBIS_TYPE as _BQ_DTYPE_TO_IBIS_TYPE
-from ibis.backends.bigquery.client import _LEGACY_TO_STANDARD as _BQ_LEGACY_TO_STANDARD
+from ibis.backends.base.sql.registry import (
+    fixed_arity,
+    type_to_sql_string as base_type_to_sql_string,
+)
+from ibis.backends.bigquery.client import (
+    _DTYPE_TO_IBIS_TYPE as _BQ_DTYPE_TO_IBIS_TYPE,
+    _LEGACY_TO_STANDARD as _BQ_LEGACY_TO_STANDARD,
+)
 from ibis.backends.bigquery.compiler import BigQueryExprTranslator
 from ibis.backends.bigquery.registry import (
     STRFTIME_FORMAT_FUNCTIONS as BQ_STRFTIME_FORMAT_FUNCTIONS,
+    bigquery_cast,
 )
 from ibis.backends.impala.compiler import ImpalaExprTranslator
 from ibis.backends.mssql.compiler import MsSqlExprTranslator
 from ibis.backends.mysql.compiler import MySQLExprTranslator
 from ibis.backends.pandas.dispatch import execute_node
 from ibis.backends.pandas.execution.temporal import execute_epoch_seconds
 from ibis.backends.postgres.compiler import PostgreSQLExprTranslator
@@ -119,14 +125,26 @@
     return BinaryLength(binary_value).to_expr()
 
 
 def compile_to_char(numeric_value, fmt):
     return ToChar(numeric_value, fmt=fmt).to_expr()
 
 
+@bigquery_cast.register(str, dt.Binary, dt.String)
+def bigquery_cast_from_binary_generate(compiled_arg, from_, to):
+    """Cast of binary to string should be hex conversion."""
+    return f"TO_HEX({compiled_arg})"
+
+
+@bigquery_cast.register(str, dt.String, dt.Binary)
+def bigquery_cast_to_binary_generate(compiled_arg, from_, to):
+    """Cast of binary to string should be hex conversion."""
+    return f"FROM_HEX({compiled_arg})"
+
+
 def format_hash_bigquery(translator, op):
     arg = translator.translate(op.arg)
     if op.how == "farm_fingerprint":
         return f"FARM_FINGERPRINT({arg})"
     else:
         raise ValueError(f"unexpected value for 'how': {op.how}")
 
@@ -359,68 +377,144 @@
         fmt = (
             "FM" + ("9" * (precision - arg_dtype.scale)) + "." + ("9" * arg_dtype.scale)
         )
         return sa.func.rtrim(sa.func.to_char(sa_arg, fmt), ".")
     return None
 
 
+def sa_cast_hive(t, op):
+    arg = op.arg
+    typ = op.to
+    arg_dtype = arg.output_dtype
+
+    arg_formatted = t.translate(arg)
+
+    if arg_dtype.is_binary() and typ.is_string():
+        # Binary to string cast is a "to hex" conversion for DVT.
+        return f"lower(hex({arg_formatted}))"
+    elif arg_dtype.is_string() and typ.is_binary():
+        # Binary from string cast is a "from hex" conversion for DVT.
+        return f"unhex({arg_formatted})"
+
+    # Follow the original Ibis code path.
+    # Cannot use sa_fixed_cast() because of ImpalaExprTranslator ancestry.
+    sql_type = base_type_to_sql_string(typ)
+    return "CAST({} AS {})".format(arg_formatted, sql_type)
+
+
 def sa_cast_postgres(t, op):
     custom_cast = sa_cast_decimal_when_scale_padded_fmt_fm(t, op)
     if custom_cast is not None:
         return custom_cast
 
+    arg = op.arg
+    typ = op.to
+    arg_dtype = arg.output_dtype
+
+    sa_arg = t.translate(arg)
+    if arg_dtype.is_binary() and typ.is_string():
+        # Binary to string cast is a "to hex" conversion for DVT.
+        return sa.func.encode(sa_arg, sa.literal("hex"))
+    elif arg_dtype.is_string() and typ.is_binary():
+        # Binary from string cast is a "from hex" conversion for DVT.
+        return sa.func.decode(sa_arg, sa.literal("hex"))
+
     # Follow the original Ibis code path.
     return sa_fixed_cast(t, op)
 
 
 def sa_cast_mssql(t, op):
     arg = op.arg
     typ = op.to
     arg_dtype = arg.output_dtype
 
+    sa_arg = t.translate(arg)
     # Specialize going from a binary float type to a string.
     if (arg_dtype.is_float32() or arg_dtype.is_float64()) and typ.is_string():
-        sa_arg = t.translate(arg)
         # This prevents output in scientific notation, at least for my tests it did.
         return sa.func.format(sa_arg, "G")
+    elif arg_dtype.is_binary() and typ.is_string():
+        # Binary to string cast is a "to hex" conversion for DVT.
+        return sa.func.lower(
+            sa.func.convert(sa.text("VARCHAR(MAX)"), sa_arg, sa.literal(2))
+        )
+    elif arg_dtype.is_string() and typ.is_binary():
+        # Binary from string cast is a "from hex" conversion for DVT.
+        return sa.func.convert(sa.text("VARBINARY(MAX)"), sa_arg, sa.literal(2))
 
     # Follow the original Ibis code path.
     return sa_fixed_cast(t, op)
 
 
 def sa_cast_mysql(t, op):
     # Add cast from numeric to string
     arg = op.arg
     typ = op.to
     arg_dtype = arg.output_dtype
 
+    sa_arg = t.translate(arg)
     # Specialize going from numeric(p,s>0) to string
     if (
         arg_dtype.is_decimal()
         and arg_dtype.scale
         and arg_dtype.scale > 0
         and typ.is_string()
     ):
         # When casting a number to string MySQL includes the full scale, e.g.:
         #   SELECT CAST(CAST(100 AS DECIMAL(5,2)) AS CHAR);
         #     100.00
         # This doesn't match most engines which would return "100".
         # We've used a workaround from StackOverflow:
         #   https://stackoverflow.com/a/20111398
         return sa_fixed_cast(t, op) + sa.literal(0)
+    elif arg_dtype.is_binary() and typ.is_string():
+        # Binary to string cast is a "to hex" conversion for DVT.
+        return sa.func.lower(sa.func.hex(sa_arg))
+    elif arg_dtype.is_string() and typ.is_binary():
+        # Binary from string cast is a "from hex" conversion for DVT.
+        return sa.func.unhex(sa_arg)
+
+    # Follow the original Ibis code path.
+    return sa_fixed_cast(t, op)
+
+
+def sa_cast_oracle(t, op):
+    arg = op.arg
+    typ = op.to
+    arg_dtype = arg.output_dtype
+
+    sa_arg = t.translate(arg)
+    if arg_dtype.is_binary() and typ.is_string():
+        # Binary to string cast is a "to hex" conversion for DVT.
+        return sa.func.lower(sa.func.rawtohex(sa_arg))
+    elif arg_dtype.is_string() and typ.is_binary():
+        # Binary from string cast is a "from hex" conversion for DVT.
+        return sa.func.hextoraw(sa_arg)
 
     # Follow the original Ibis code path.
     return sa_fixed_cast(t, op)
 
 
 def sa_cast_snowflake(t, op):
     custom_cast = sa_cast_decimal_when_scale_padded_fmt_fm(t, op)
     if custom_cast is not None:
         return custom_cast
 
+    arg = op.arg
+    typ = op.to
+    arg_dtype = arg.output_dtype
+
+    sa_arg = t.translate(arg)
+    if arg_dtype.is_binary() and typ.is_string():
+        # Binary to string cast is a "to hex" conversion for DVT.
+        return sa.func.hex_encode(sa_arg, sa.literal(0))
+    elif arg_dtype.is_string() and typ.is_binary():
+        # Binary from string cast is a "from hex" conversion for DVT.
+        return sa.func.hex_decode_binary(sa_arg)
+
     # Follow the original Ibis code path.
     return sa_fixed_cast(t, op)
 
 
 def _sa_string_join(t, op):
     return sa.func.concat(*map(t.translate, op.arg))
 
@@ -472,25 +566,38 @@
         else:
             ibis_type = ibis_type
     if field.mode == "REPEATED":
         ibis_type = dt.Array(ibis_type)
     return ibis_type
 
 
+def string_to_epoch(ts: str):
+    "Function to convert string timestamp to epoch seconds"
+    from dateutil.parser import isoparse
+    from dateutil.tz import UTC
+    from datetime import datetime, timezone
+
+    parsed_ts = isoparse(ts).astimezone(UTC)
+    return (parsed_ts - datetime(1970, 1, 1, tzinfo=timezone.utc)).total_seconds()
+
+
 @execute_node.register(ops.ExtractEpochSeconds, (datetime.datetime, pd.Series))
 def execute_epoch_seconds_new(op, data, **kwargs):
     import numpy as np
 
     convert = getattr(data, "view", data.astype)
-    # Add try/except to handle large timestamps outside of datetime64[ns]as per Issue #1053
     try:
         series = convert(np.int64)
         return (series // 1_000_000_000).astype(np.int32)
-    except:
-        return pd.Series(np.nan)
+    except TypeError:
+        # Catch 'TypeError' for large timestamps beyond max datetime64[ns] as per Issue #1053
+        # Cast to string instead to work around datetime64[ns] limitation
+        series = data.astype("string")
+        epoch_series = series.map(string_to_epoch)
+        return epoch_series
 
 
 execute_epoch_seconds = execute_epoch_seconds_new
 
 BinaryValue.byte_length = compile_binary_length
 
 NumericValue.to_char = compile_to_char
@@ -502,21 +609,23 @@
 BigQueryExprTranslator._registry[BinaryLength] = sa_format_binary_length
 
 AlchemyExprTranslator._registry[RawSQL] = format_raw_sql
 AlchemyExprTranslator._registry[HashBytes] = format_hashbytes_alchemy
 ExprTranslator._registry[RawSQL] = format_raw_sql
 ExprTranslator._registry[HashBytes] = format_hashbytes_base
 
+ImpalaExprTranslator._registry[Cast] = sa_cast_hive
 ImpalaExprTranslator._registry[RawSQL] = format_raw_sql
 ImpalaExprTranslator._registry[HashBytes] = format_hashbytes_hive
 ImpalaExprTranslator._registry[RandomScalar] = fixed_arity("RAND", 0)
 ImpalaExprTranslator._registry[Strftime] = strftime_impala
 ImpalaExprTranslator._registry[BinaryLength] = sa_format_binary_length
 
 if OracleExprTranslator:
+    OracleExprTranslator._registry[Cast] = sa_cast_oracle
     OracleExprTranslator._registry[RawSQL] = sa_format_raw_sql
     OracleExprTranslator._registry[HashBytes] = sa_format_hashbytes_oracle
     OracleExprTranslator._registry[ToChar] = sa_format_to_char
     OracleExprTranslator._registry[BinaryLength] = sa_format_binary_length_oracle
 
 PostgreSQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_postgres
 PostgreSQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
```

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/__init__.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/client.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/compiler.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/datatypes.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/registry.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/registry.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/__init__.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/compiler.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/datatypes.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_db2/registry.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_db2/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
     sa_arg = t.translate(arg)
 
     # specialize going from an integer type to a timestamp
     if arg_dtype.is_integer() and typ.is_timestamp():
         return t.integer_to_timestamp(sa_arg, tz=typ.timezone)
 
     if arg_dtype.is_binary() and typ.is_string():
-        return sa.func.encode(sa_arg, "escape")
+        # Binary to string cast is a "to hex" conversion for DVT.
+        return sa.func.lower(sa.func.hex(sa_arg))
 
     if typ.is_binary():
         #  decode yields a column of memoryview which is annoying to deal with
         # in pandas. CAST(expr AS BYTEA) is correct and returns byte strings.
         return sa.cast(sa_arg, sa.LargeBinary())
 
     if typ.is_json() and not t.native_json_type:
```

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_impala/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_impala/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,16 @@
                 t = t.replace(":int", ":int32")
 
             if "varchar" in t:
                 t = t.replace(":varchar", ":string")
             else:
                 t = t.replace(":char", ":string")
             return t
+        elif "binary" in t:
+            return "binary"
         else:
             raise Exception(t)
 
 
 def get_schema(self, table_name, database=None):
     """
     Return a Schema object for the indicated table and database
```

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_mssql/__init__.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_mssql/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_mssql/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_mssql/datatypes.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_mssql/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_mysql/compiler.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_mysql/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/__init__.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/compiler.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/datatypes.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_oracle/registry.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_oracle/registry.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_postgres/client.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_postgres/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_postgres/datatypes.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_postgres/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_redshift/__init__.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_redshift/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_redshift/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_redshift/compiler.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_redshift/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_snowflake/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_snowflake/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_snowflake/datatypes.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_snowflake/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/__init__.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/api.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/compiler.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/datatypes.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,21 @@
         if return_ibis_type:
             return dt.string(nullable=cls._col_data_nullable(col_data))
 
         print('Unsupported Date Type Seen: "%s"' % col_data["Type"])
         return "VARCHAR"
 
     @classmethod
+    def to_ibis_from_BV(cls, col_data, return_ibis_type=True):
+        if return_ibis_type:
+            return dt.binary(nullable=cls._col_data_nullable(col_data))
+
+        return "VARBYTE"
+
+    @classmethod
     def to_ibis_from_CV(cls, col_data, return_ibis_type=True):
         if return_ibis_type:
             return dt.string(nullable=cls._col_data_nullable(col_data))
 
         return "VARCHAR"
 
     @classmethod
```

### Comparing `google-pso-data-validator-4.5.0/third_party/ibis/ibis_teradata/registry.py` & `google_pso_data_validator-5.0.0/third_party/ibis/ibis_teradata/registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import re
 import string
 import warnings
 from multipledispatch import Dispatcher
 
 import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
-
 from ibis.common.exceptions import UnsupportedOperationError
 from ibis.backends.base.sql.registry import operation_registry, fixed_arity
 from third_party.ibis.ibis_teradata.datatypes import ibis_type_to_teradata_type
 
 _operation_registry = operation_registry.copy()
 
 
@@ -40,14 +39,48 @@
 
 
 @teradata_cast.register(str, dt.Timestamp, dt.Integer)
 def teradata_cast_timestamp_to_integer(compiled_arg, from_, to):
     return "UNIX_MICROS({})".format(compiled_arg)
 
 
+@teradata_cast.register(str, dt.Binary, dt.String)
+def teradata_cast_binary_to_string(compiled_arg, from_, to):
+    return "LOWER(FROM_BYTES({}, 'base16'))".format(compiled_arg)
+
+
+@teradata_cast.register(str, dt.String, dt.Binary)
+def teradata_cast_string_to_binary(compiled_arg, from_, to):
+    return "TO_BYTES({}, 'base16')".format(compiled_arg)
+
+
+@teradata_cast.register(str, dt.Decimal, dt.String)
+def teradata_cast_decimal_to_string(compiled_arg, from_, to):
+    """Specialize cast from decimal to string.
+
+    Teradata has two behaviours we need to avoid:
+    1) SELECT CAST(CAST(7 AS DECIMAL(5,2)) AS VARCHAR(64));
+    7.00
+    2) SELECT CAST(CAST(-0.7 AS DECIMAL(5,2)) AS VARCHAR(64));
+    -.70
+
+    This function uses a format mask to give these results from above examples:
+    1) 7
+    2) -0.7
+    """
+    precision = from_.precision or 38
+    if from_.scale and from_.scale > 0:
+        fmt = "FM" + ("9" * (precision - from_.scale)) + "." + ("9" * from_.scale)
+        return f"RTRIM(TO_CHAR({compiled_arg},'{fmt}'),'.')"
+    elif from_.scale is not None and from_.scale == 0:
+        fmt = "FM" + ("9" * (precision - from_.scale))
+        return f"TO_CHAR({compiled_arg},'{fmt}')"
+    return "TO_CHAR({},'TM9')".format(compiled_arg)
+
+
 @teradata_cast.register(str, dt.DataType, dt.DataType)
 def teradata_cast_generate(compiled_arg, from_, to):
     sql_type = ibis_type_to_teradata_type(to)
     return "CAST({} AS {})".format(compiled_arg, sql_type)
 
 
 def _cast(t, op):
```

