# Comparing `tmp/ob-metaflow-stubs-3.5.tar.gz` & `tmp/ob-metaflow-stubs-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-stubs-3.5.tar", last modified: Fri May 17 23:07:06 2024, max compression
+gzip compressed data, was "ob-metaflow-stubs-3.6.tar", last modified: Tue May 21 17:36:52 2024, max compression
```

## Comparing `ob-metaflow-stubs-3.5.tar` & `ob-metaflow-stubs-3.6.tar`

### file list

```diff
@@ -1,168 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 23:06:40.000000 ob-metaflow-stubs-3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-17 23:06:40.000000 ob-metaflow-stubs-3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.573435 ob-metaflow-stubs-3.5/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.573435 ob-metaflow-stubs-3.5/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.573435 ob-metaflow-stubs-3.5/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.573435 ob-metaflow-stubs-3.5/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.581435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.581435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_credential.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.581435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/logs_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/perimeters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/procpoll.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/metaflow-stubs/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/profilers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/tagging_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 23:07:06.000000 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-17 23:07:06.000000 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:07:06.000000 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 23:07:06.000000 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 23:06:40.000000 ob-metaflow-stubs-3.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 23:06:40.000000 ob-metaflow-stubs-3.5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 17:36:32.000000 ob-metaflow-stubs-3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-21 17:36:32.000000 ob-metaflow-stubs-3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 17:36:49.000000 ob-metaflow-stubs-3.6/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.242765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.242765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.242765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.242765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29098 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/logs_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/perimeters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/procpoll.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/metaflow-stubs/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/profilers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:49.000000 ob-metaflow-stubs-3.6/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/pylint_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/tagging_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/tuple_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-21 17:36:52.000000 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-21 17:36:52.000000 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:36:52.000000 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 17:36:52.000000 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 17:36:32.000000 ob-metaflow-stubs-3.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-21 17:36:32.000000 ob-metaflow-stubs-3.6/version.py
```

### Comparing `ob-metaflow-stubs-3.5/PKG-INFO` & `ob-metaflow-stubs-3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.5
+Version: 3.6
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.406286                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.007848                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import metaflow.datastore.inputs
-    import metaflow.plugins.datatools.s3.s3
-    import metaflow.events
+    import metaflow.metaflow_current
+    import metaflow.parameters
     import datetime
+    import metaflow.events
+    import metaflow.datastore.inputs
+    import typing
     import metaflow._vendor.click.types
     import metaflow.client.core
     import io
-    import metaflow.parameters
-    import metaflow.metaflow_current
+    import metaflow.plugins.datatools.s3.s3
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -917,14 +917,98 @@
     log_options: List[str], optional, default None
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
         Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
+@typing.overload
+def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
+    
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
+    
+    Parameters
+    ----------
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
+    """
+    ...
+
+@typing.overload
+def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+    """
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
+    
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
+    
+    Parameters
+    ----------
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
+    """
+    ...
+
+@typing.overload
+def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies environment variables to be set prior to the execution of a step.
+    
+    Parameters
+    ----------
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
+@typing.overload
+def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+    """
+    Specifies environment variables to be set prior to the execution of a step.
+    
+    Parameters
+    ----------
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
 def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on Kubernetes.
     
     Parameters
     ----------
     cpu : int, default 1
@@ -977,14 +1061,47 @@
         Shared memory size (in MiB) required for this step
     port: int, optional
         Port number to specify in the Kubernetes job object
     """
     ...
 
 @typing.overload
+def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
+    
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
+    
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
 def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the Conda environment for the step.
     
     Information in this decorator will augment any
     attributes set in the `@conda_base` flow-level decorator. Hence,
     you can use `@conda_base` to set packages required by all
@@ -1034,171 +1151,14 @@
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
-    
-    Parameters
-    ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
-    """
-    ...
-
-@typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
-    """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
-    
-    Parameters
-    ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
-    """
-    ...
-
-@typing.overload
-def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
-    
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
-    
-    Parameters
-    ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
-    """
-    ...
-
-@typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
-    """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
-    
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
-    
-    Parameters
-    ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
-    """
-    ...
-
-@typing.overload
-def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
-    """
-    ...
-
-@typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
-    """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
-    """
-    ...
-
-@typing.overload
 def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the resources needed when executing this step.
     
     Use `@resources` to specify the resource requirements
     independently of the specific compute layer (`@batch`, `@kubernetes`).
     
@@ -1268,208 +1228,216 @@
     shared_memory : int, optional, default None
         The value for the size (in MiB) of the /dev/shm volume for this step.
         This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    Creates a human-readable report, a Metaflow Card, after this step completes.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Note that you may add multiple `@card` decorators in a step with different parameters.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
     """
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    Creates a human-readable report, a Metaflow Card, after this step completes.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Note that you may add multiple `@card` decorators in a step with different parameters.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
     """
     ...
 
 @typing.overload
-def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Specifies that the step will success under all circumstances.
+    
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
     Parameters
     ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 @typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
     """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Specifies that the step will success under all circumstances.
+    
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
     Parameters
     ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 @typing.overload
-def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies a timeout for your step.
+    
+    This decorator is useful if this step may hang indefinitely.
+    
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies a timeout for your step.
+    
+    This decorator is useful if this step may hang indefinitely.
+    
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies the PyPI packages for all steps of the flow.
+    Specifies the times when the flow should be run when running on a
+    production scheduler.
     
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    hourly : bool, default False
+        Run the workflow hourly.
+    daily : bool, default True
+        Run the workflow daily.
+    weekly : bool, default False
+        Run the workflow weekly.
+    cron : str, optional, default None
+        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
+        specified by this expression.
+    timezone : str, optional, default None
+        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
+        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
     """
     ...
 
 @typing.overload
-def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
-    """
-    Specifies the PyPI packages for all steps of the flow.
-    
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
+def schedule(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
     ...
 
-def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def schedule(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None):
     """
-    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
-    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    Specifies the times when the flow should be run when running on a
+    production scheduler.
     
     Parameters
     ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    external_dag_id : str
-        The dag_id that contains the task you want to wait for.
-    external_task_ids : List[str]
-        The list of task_ids that you want to wait for.
-        If None (default value) the sensor waits for the DAG. (Default: None)
-    allowed_states : List[str]
-        Iterable of allowed states, (Default: ['success'])
-    failed_states : List[str]
-        Iterable of failed or dis-allowed states. (Default: None)
-    execution_delta : datetime.timedelta
-        time difference with the previous execution to look at,
-        the default is the same logical date as the current task or DAG. (Default: None)
-    check_existence: bool
-        Set to True to check if the external task exists or check if
-        the DAG to wait for exists. (Default: True)
+    hourly : bool, default False
+        Run the workflow hourly.
+    daily : bool, default True
+        Run the workflow daily.
+    weekly : bool, default False
+        Run the workflow weekly.
+    cron : str, optional, default None
+        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
+        specified by this expression.
+    timezone : str, optional, default None
+        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
+        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
     """
     ...
 
 def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
     before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
@@ -1508,109 +1476,14 @@
         a reference to the s3 connection on Airflow. (Default: None)
     verify : bool
         Whether or not to verify SSL certificates for S3 connection. (Default: None)
     """
     ...
 
 @typing.overload
-def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the event(s) that this flow depends on.
-    
-    ```
-    @trigger(event='foo')
-    ```
-    or
-    ```
-    @trigger(events=['foo', 'bar'])
-    ```
-    
-    Additionally, you can specify the parameter mappings
-    to map event payload to Metaflow parameters for the flow.
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
-    ```
-    or
-    ```
-    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
-                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
-    ```
-    
-    'parameters' can also be a list of strings and tuples like so:
-    ```
-    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
-    ```
-    This is equivalent to:
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
-    ```
-    
-    Parameters
-    ----------
-    event : Union[str, Dict[str, Any]], optional, default None
-        Event dependency for this flow.
-    events : List[Union[str, Dict[str, Any]]], default []
-        Events dependency for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
-@typing.overload
-def trigger(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def trigger(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}):
-    """
-    Specifies the event(s) that this flow depends on.
-    
-    ```
-    @trigger(event='foo')
-    ```
-    or
-    ```
-    @trigger(events=['foo', 'bar'])
-    ```
-    
-    Additionally, you can specify the parameter mappings
-    to map event payload to Metaflow parameters for the flow.
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
-    ```
-    or
-    ```
-    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
-                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
-    ```
-    
-    'parameters' can also be a list of strings and tuples like so:
-    ```
-    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
-    ```
-    This is equivalent to:
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
-    ```
-    
-    Parameters
-    ----------
-    event : Union[str, Dict[str, Any]], optional, default None
-        Event dependency for this flow.
-    events : List[Union[str, Dict[str, Any]]], default []
-        Events dependency for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
-@typing.overload
 def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the Conda environment for all steps of the flow.
     
     Use `@conda_base` to set common libraries required by all
     steps and use `@conda` to specify step-specific additions.
     
@@ -1651,14 +1524,56 @@
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables Conda.
     """
     ...
 
+def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
+    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    external_dag_id : str
+        The dag_id that contains the task you want to wait for.
+    external_task_ids : List[str]
+        The list of task_ids that you want to wait for.
+        If None (default value) the sensor waits for the DAG. (Default: None)
+    allowed_states : List[str]
+        Iterable of allowed states, (Default: ['success'])
+    failed_states : List[str]
+        Iterable of failed or dis-allowed states. (Default: None)
+    execution_delta : datetime.timedelta
+        time difference with the previous execution to look at,
+        the default is the same logical date as the current task or DAG. (Default: None)
+    check_existence: bool
+        Set to True to check if the external task exists or check if
+        the DAG to wait for exists. (Default: True)
+    """
+    ...
+
 def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies what flows belong to the same project.
     
     A project-specific namespace is created for all flows that
     use the same `@project(name)`.
     
@@ -1670,59 +1585,49 @@
         contain only lowercase alphanumeric characters and underscores.
     
     
     """
     ...
 
 @typing.overload
-def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies the times when the flow should be run when running on a
-    production scheduler.
+    Specifies the PyPI packages for all steps of the flow.
     
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    hourly : bool, default False
-        Run the workflow hourly.
-    daily : bool, default True
-        Run the workflow daily.
-    weekly : bool, default False
-        Run the workflow weekly.
-    cron : str, optional, default None
-        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
-        specified by this expression.
-    timezone : str, optional, default None
-        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
-        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
+    packages : Dict[str, str], default: {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def schedule(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
     ...
 
-def schedule(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None):
+def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies the times when the flow should be run when running on a
-    production scheduler.
+    Specifies the PyPI packages for all steps of the flow.
     
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    hourly : bool, default False
-        Run the workflow hourly.
-    daily : bool, default True
-        Run the workflow daily.
-    weekly : bool, default False
-        Run the workflow weekly.
-    cron : str, optional, default None
-        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
-        specified by this expression.
-    timezone : str, optional, default None
-        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
-        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
+    packages : Dict[str, str], default: {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
 def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the flow(s) that this flow depends on.
@@ -1821,14 +1726,109 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
+@typing.overload
+def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the event(s) that this flow depends on.
+    
+    ```
+    @trigger(event='foo')
+    ```
+    or
+    ```
+    @trigger(events=['foo', 'bar'])
+    ```
+    
+    Additionally, you can specify the parameter mappings
+    to map event payload to Metaflow parameters for the flow.
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
+    ```
+    or
+    ```
+    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
+                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
+    ```
+    
+    'parameters' can also be a list of strings and tuples like so:
+    ```
+    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
+    ```
+    This is equivalent to:
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
+    ```
+    
+    Parameters
+    ----------
+    event : Union[str, Dict[str, Any]], optional, default None
+        Event dependency for this flow.
+    events : List[Union[str, Dict[str, Any]]], default []
+        Events dependency for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
+@typing.overload
+def trigger(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def trigger(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}):
+    """
+    Specifies the event(s) that this flow depends on.
+    
+    ```
+    @trigger(event='foo')
+    ```
+    or
+    ```
+    @trigger(events=['foo', 'bar'])
+    ```
+    
+    Additionally, you can specify the parameter mappings
+    to map event payload to Metaflow parameters for the flow.
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
+    ```
+    or
+    ```
+    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
+                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
+    ```
+    
+    'parameters' can also be a list of strings and tuples like so:
+    ```
+    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
+    ```
+    This is equivalent to:
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
+    ```
+    
+    Parameters
+    ----------
+    event : Union[str, Dict[str, Any]], optional, default None
+        Event dependency for this flow.
+    events : List[Union[str, Dict[str, Any]]], default []
+        Events dependency for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
     pass None to this call.
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/cards.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.426484                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.028185                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.components
     import typing
     import metaflow.plugins.cards.card_client
     import metaflow
-    import metaflow.plugins.cards.card_modules.basic
-    import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.card
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/cli.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.431329                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.033630                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/client/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.428982                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.030601                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
+    import typing
     import metaflow.client.core
+    import metaflow.events
     import datetime
-    import typing
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/client/core.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.415443                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.016999                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
     import tarfile
-    import metaflow.exception
+    import metaflow.metaflow_current
+    import datetime
+    import typing
     import metaflow
     import metaflow.events
-    import datetime
     import metaflow.client.core
-    import metaflow.metaflow_current
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/client/filecache.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/client/filecache.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.432173                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.034470                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.datastore.content_addressed_store
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/clone_util.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/clone_util.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.429538                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.031199                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/events.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/events.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.417317                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.019115                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.events
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/exception.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/exception.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.408075                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.009652                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/flowspec.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/flowspec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.416745                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.018350                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
+    import metaflow.parameters
     import metaflow.datastore.inputs
-    import metaflow.exception
+    import typing
     import metaflow.unbounded_foreach
-    import metaflow.parameters
+    import metaflow.exception
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/includefile.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/includefile.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.424730                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.026439                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.parameters
     import typing
-    import metaflow.plugins.datatools.s3.s3
     import metaflow._vendor.click.types
     import io
-    import metaflow.parameters
+    import metaflow.plugins.datatools.s3.s3
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/metadata/metadata.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/metadata/metadata.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.450367                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.051902                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metadata.metadata
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/metadata/util.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/metadata/util.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.492339                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.094351                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def copy_tree(src, dst, update = False):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/metaflow_config.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/metaflow_config.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.409083                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.010618                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
@@ -128,14 +128,16 @@
 
 DEFAULT_CONTAINER_REGISTRY: None
 
 INCLUDE_FOREACH_STACK: bool
 
 MAXIMUM_FOREACH_VALUE_CHARS: int
 
+DEFAULT_RUNTIME_LIMIT: int
+
 UI_URL: None
 
 CONTACT_INFO: dict
 
 ECS_S3_ACCESS_IAM_ROLE: None
 
 ECS_FARGATE_EXECUTION_ROLE: None
@@ -182,28 +184,32 @@
 
 KUBERNETES_IMAGE_PULL_POLICY: None
 
 KUBERNETES_CONTAINER_REGISTRY: None
 
 KUBERNETES_FETCH_EC2_METADATA: bool
 
-KUBERNETES_PORT: None
-
 KUBERNETES_SHARED_MEMORY: None
 
+KUBERNETES_PORT: None
+
 KUBERNETES_CPU: None
 
 KUBERNETES_MEMORY: None
 
 KUBERNETES_DISK: None
 
 ARGO_WORKFLOWS_KUBERNETES_SECRETS: str
 
 ARGO_WORKFLOWS_ENV_VARS_TO_SKIP: str
 
+KUBERNETES_JOBSET_GROUP: str
+
+KUBERNETES_JOBSET_VERSION: str
+
 ARGO_EVENTS_SERVICE_ACCOUNT: None
 
 ARGO_EVENTS_EVENT_BUS: str
 
 ARGO_EVENTS_EVENT_SOURCE: None
 
 ARGO_EVENTS_EVENT: None
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/metaflow_current.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/metaflow_current.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.494647                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.096690                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
+    import metaflow.plugins.cards.component_serializer
     import typing
     import metaflow
     import metaflow.events
-    import metaflow.plugins.cards.component_serializer
-    import metaflow.metaflow_current
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
     @staticmethod
@@ -238,27 +238,14 @@
         Returns
         -------
         CardComponentCollector
             The or one of the cards attached to this step.
         """
         ...
     @property
-    def trigger(self) -> "metaflow.events.Trigger":
-        """
-        (only in the presence of the @trigger, or @trigger_on_finish decorators)
-        
-        Returns `Trigger` if the current run is triggered by an event
-        
-        Returns
-        -------
-        Trigger
-            `Trigger` if triggered by an event
-        """
-        ...
-    @property
     def project_name(self) -> str:
         """
         (only in the presence of the @project decorator)
         
         The name of the project assigned to this flow, i.e. `X` in `@project(name=X)`.
         
         Returns
@@ -317,11 +304,24 @@
         
         Returns
         -------
         bool
             True if the flow is deployed with `--production`.
         """
         ...
+    @property
+    def trigger(self) -> "metaflow.events.Trigger":
+        """
+        (only in the presence of the @trigger_on_finish, or @trigger decorators)
+        
+        Returns `Trigger` if the current run is triggered by an event
+        
+        Returns
+        -------
+        Trigger
+            `Trigger` if triggered by an event
+        """
+        ...
     ...
 
 current: Current
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/mflog/mflog.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/mflog/mflog.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.450679                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.052216                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import datetime
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/multicore_utils.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/multicore_utils.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.409498                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.011139                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/parameters.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/parameters.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.410594                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.012207                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
     import metaflow.parameters
-    import metaflow.exception
     import metaflow._vendor.click.types
+    import metaflow.exception
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
 
 class ParameterFieldTypeMismatch(metaflow.exception.MetaflowException, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.418834                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.020602                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.unbounded_foreach
@@ -48,18 +48,18 @@
 
 AWS_CLIENT_PROVIDERS_DESC: list
 
 SENSOR_FLOW_DECORATORS: list
 
 SECRETS_PROVIDERS_DESC: list
 
-AZURE_CLIENT_PROVIDERS_DESC: list
-
 GCP_CLIENT_PROVIDERS_DESC: list
 
+AZURE_CLIENT_PROVIDERS_DESC: list
+
 def get_plugin_cli():
     ...
 
 STEP_DECORATORS: list
 
 FLOW_DECORATORS: list
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.454060                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.058065                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.metaflow_current
     import metaflow._vendor.click.types
+    import metaflow.metaflow_current
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -94,15 +94,19 @@
     ...
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, shared_memory = None, port = None):
+    def create_jobset(self, job_spec = None, run_id = None, step_name = None, task_id = None, namespace = None, env = None, num_parallel = None, port = None, annotations = None, labels = None):
+        ...
+    def create_job_object(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None, port = None, name_pattern = None, num_parallel = None):
+        ...
+    def create_k8sjob(self, job):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 def get_run_time_limit_for_task(step_decos):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.455472                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.058997                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.452012                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.056147                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.451642                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.055778                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/exception.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.452232                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.080765                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,15 +13,16 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
-    def __init__(self, msg):
-        ...
+class MetaflowAzureAuthenticationError(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class MetaflowAzureResourceError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowAzurePackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.452451                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.056605                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.482092                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.084171                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.482473                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.084546                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.decorators
+    import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.exception
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.482812                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.084883                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.decorators
+    import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.exception
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_client.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.471450                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.067987                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_events.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.470142                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.066635                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.475477                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.071971                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import metaflow.parameters
-    import metaflow.metaflow_current
     import metaflow._vendor.click.types
+    import metaflow.metaflow_current
+    import metaflow.parameters
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.476966                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.073540                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
-    import metaflow.parameters
+    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.parameters
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.470895                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.067427                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
     import metaflow.decorators
+    import metaflow.events
     import metaflow
     import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/aws_client.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.429283                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.030905                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/aws_utils.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.456054                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.059575                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.490116                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.087596                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.491394                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.088957                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.489097                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.086597                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.490817                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.088299                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.491786                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.083033                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.secrets
     import abc
+    import metaflow.plugins.secrets
     import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-AWS_SECRETS_MANAGER_DEFAULT_REGION: None
-
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
         ...
     ...
 
-class MetaflowAWSSecretsManagerBadResponse(metaflow.exception.MetaflowException, metaclass=type):
+def get_credentials(scopes, *args, **kwargs):
     ...
 
-class MetaflowAWSSecretsManagerDuplicateKey(metaflow.exception.MetaflowException, metaclass=type):
+GCP_SECRET_MANAGER_PREFIX: None
+
+class MetaflowGcpSecretsManagerBadResponse(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class MetaflowAWSSecretsManagerJSONParseError(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowGcpSecretsManagerDuplicateKey(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class MetaflowAWSSecretsManagerNotJSONObject(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowGcpSecretsManagerJSONParseError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class AwsSecretsManagerSecretsProvider(metaflow.plugins.secrets.SecretsProvider, metaclass=abc.ABCMeta):
+class MetaflowGcpSecretsManagerNotJSONObject(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class GcpSecretManagerSecretsProvider(metaflow.plugins.secrets.SecretsProvider, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None):
         """
-        Reads a secret from AWS Secrets Manager and returns it as a dictionary of environment variables.
-        
-        The secret payload from AWS is EITHER a string OR a binary blob.
+        Reads a secret from GCP Secrets Manager and returns it as a dictionary of environment variables.
         
         If the secret contains a string payload ("SecretString"):
-        - if the `parse_secret_string_as_json` option is True (default):
-            {SecretString} will be parsed as a JSON. If successfully parsed, AND the JSON contains a
+        - if the `json` option is True:
+            Secret will be parsed as a JSON. If successfully parsed, AND the JSON contains a
             top-level object, each entry K/V in the object will also be converted to an entry in the result. V will
             always be casted to a string (if not already a string).
-        - If `parse_secret_string_as_json` option is False:
-            {SecretString} will be returned as a single entry in the result, with the key being the secret_id.
+        - If `json` option is False (default):
+            Will be returned as a single entry in the result, with the key being the last part after / in secret_id.
         
-        Otherwise, the secret contains a binary blob payload ("SecretBinary"). In this case
-        - The result dic contains '{SecretName}': '{SecretBinary}', where {SecretBinary} is a base64-encoded string
+        On GCP Secrets Manager, the secret payload is a binary blob. However, by default we interpret it as UTF8 encoded
+        string. To disable this, set the `binary` option to True, the binary will be base64 encoded in the result.
         
         All keys in the result are sanitized to be more valid environment variable names. This is done on a best effort
         basis. Further validation is expected to be done by the invoking @secrets decorator itself.
         
-        :param secret_id: ARN or friendly name of the secret
+        :param secret_id: GCP Secrets Manager secret ID
         :param options: unused
-        :param role: AWS IAM Role ARN to assume before reading the secret
         :return: dict of environment variables. All keys and values are strings.
         """
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.483597                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.089179                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 SFN_DYNAMO_DB_TABLE: None
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.484424                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.089995                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class EventBridgeClient(object, metaclass=type):
     def __init__(self, name):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.484156                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.037911                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class EnvironmentDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.486752                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.092175                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.487959                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.093376                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
-    import metaflow.parameters
+    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.parameters
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.484731                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.090297                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 AWS_SANDBOX_ENABLED: bool
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.483986                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.089563                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_credential.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_credential.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.478498                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.080547                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class AzureDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.479877                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.081912                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.secrets
     import abc
+    import metaflow.plugins.secrets
     import metaflow.exception
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_utils.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.479111                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.081158                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.479450                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.081477                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/includefile_support.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.445315                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.046914                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.469694                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.080287                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import metaflow.exception
+    import metaflow.parameters
     import datetime
+    import typing
     import metaflow.client.core
-    import metaflow.parameters
+    import metaflow.exception
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
         """
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_client.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.446900                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.048440                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.plugins.cards.card_client
     import metaflow
     import metaflow.exception
-    import metaflow.plugins.cards.card_client
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_creator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.465629                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.031886                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
+    import metaflow.exception
 
-current: metaflow.metaflow_current.Current
-
-ASYNC_TIMEOUT: int
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
 
-class CardProcessManager(object, metaclass=type):
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class CardCreator(object, metaclass=type):
-    def __init__(self, top_level_options):
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
+        ...
+    def has_pylint(self):
         ...
-    def create(self, card_uuid = None, user_set_card_id = None, runtime_card = False, decorator_attributes = None, card_options = None, logger = None, mode = "render", final = False, sync = False):
+    def run(self, logger = None, warnings = False, pylint_config = []):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_datastore.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.467172                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.077595                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.466447                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.076862                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.463562                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.074010                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.441045                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.042607                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
-    import metaflow
     import metaflow.plugins.cards.card_modules.card
+    import metaflow
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.447294                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.048834                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.483134                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.095556                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
-def main(template, data = None, **kwargs):
-    ...
-
-def cli_main():
-    """
-    Render mustache templates using json files
-    """
-    ...
-
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
     Render a mustache template.
     
     Renders a mustache template with a data scope and partial capability.
     Given the file structure...
     ╷
@@ -69,10 +60,18 @@
     
     Returns:
     
     A string containing the rendered template.
     """
     ...
 
-class ChevronError(SyntaxError, metaclass=type):
+version: str
+
+def main(template, data = None, **kwargs):
+    ...
+
+def cli_main():
+    """
+    Render mustache templates using json files
+    """
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.493476                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.085214                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
+def main(template, data = None, **kwargs):
+    ...
+
+def cli_main():
+    """
+    Render mustache templates using json files
+    """
+    ...
+
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
     Render a mustache template.
     
     Renders a mustache template with a data scope and partial capability.
     Given the file structure...
     ╷
@@ -60,18 +69,10 @@
     
     Returns:
     
     A string containing the rendered template.
     """
     ...
 
-version: str
-
-def main(template, data = None, **kwargs):
-    ...
-
-def cli_main():
-    """
-    Render mustache templates using json files
-    """
+class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.493096                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.095167                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.492728                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.094751                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.449158                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.050594                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.plugins.cards.card_modules.components
     import typing
     import metaflow.plugins.cards.card_modules.basic
-    import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.card
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.481344                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.083432                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.481528                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.083624                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.442223                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.043855                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow
     import metaflow.plugins.cards.card_modules.card
+    import metaflow
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_resolver.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.467650                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.078080                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/component_serializer.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.465382                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.075898                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.components
-    import metaflow.exception
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.exception
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
     def component_id(self, value):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/exception.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.464122                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.074559                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/catch_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.435882                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.038931                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.435119                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.037478                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import io
-    import metaflow.exception
     import metaflow.plugins.datatools.s3.s3
+    import metaflow.exception
 
 def read_in_chunks(dst, src, src_sz, max_chunk_size):
     ...
 
 class MetaflowLocalNotFound(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/local.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.444844                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.046456                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.460482                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.061783                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import io
     import metaflow.plugins.datatools.s3.s3
+    import metaflow.exception
 
 class RangeInfo(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, total_size: int, request_offset: int = 0, request_length: int = -1):
         """
         Create new instance of RangeInfo(total_size, request_offset, request_length)
         """
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.422024                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.023682                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
+    import metaflow.metaflow_current
     import metaflow.datastore.inputs
-    import metaflow.exception
-    import metaflow.plugins.datatools.s3.s3
+    import typing
     import io
-    import metaflow.metaflow_current
+    import metaflow.plugins.datatools.s3.s3
+    import metaflow.exception
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
@@ -246,14 +246,17 @@
 
 S3_TRANSIENT_RETRY_COUNT: int
 
 S3_SERVER_SIDE_ENCRYPTION: None
 
 TEMPDIR: str
 
+def namedtuple_with_defaults(typename, field_descr, defaults = ()):
+    ...
+
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.492112                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.094112                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.444331                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.045949                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/debug_logger.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.438347                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.040680                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.event_logger
+    import metaflow.monitor
 
-class DebugEventLogger(metaflow.event_logger.NullEventLogger, metaclass=type):
+class DebugMonitor(metaflow.monitor.NullMonitor, metaclass=type):
     @classmethod
     def get_worker(cls):
         ...
     ...
 
-class DebugEventLoggerSidecar(object, metaclass=type):
+class DebugMonitorSidecar(object, metaclass=type):
     def __init__(self):
         ...
     def process_message(self, msg):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/debug_monitor.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.438574                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.008439                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.monitor
+    import metaflow.exception
 
-class DebugMonitor(metaflow.monitor.NullMonitor, metaclass=type):
-    @classmethod
-    def get_worker(cls):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
+    def __str__(self):
+        ...
+    ...
+
+CLIENT_REFRESH_INTERVAL_SECONDS: int
+
+class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class DebugMonitorSidecar(object, metaclass=type):
+class KubernetesClient(object, metaclass=type):
     def __init__(self):
         ...
-    def process_message(self, msg):
+    def get(self):
+        ...
+    def job(self, **kwargs):
+        ...
+    def jobset(self, **kwargs):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/environment_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.436844                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.037755                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class EnvironmentDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
+
+MAX_ATTEMPTS: int
+
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+        ...
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/events_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.437161                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.039292                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
     import metaflow.metaflow_current
 
-current: metaflow.metaflow_current.Current
-
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
-        ...
-    ...
+current: metaflow.metaflow_current.Current
 
-class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
+VALID_NAME_RE: str
+
+VALID_NAME_LEN: int
+
+class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     def get_top_level_options(self):
         ...
     ...
 
+def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
+    ...
+
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.477348                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.054819                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.parallel_decorator
     import metaflow.decorators
+    import metaflow.plugins.parallel_decorator
     import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.480991                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.093774                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.secrets
     import abc
+    import metaflow.plugins.secrets
     import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
+AWS_SECRETS_MANAGER_DEFAULT_REGION: None
+
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
         ...
     ...
 
-def get_credentials(scopes, *args, **kwargs):
+class MetaflowAWSSecretsManagerBadResponse(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-GCP_SECRET_MANAGER_PREFIX: None
-
-class MetaflowGcpSecretsManagerBadResponse(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowAWSSecretsManagerDuplicateKey(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class MetaflowGcpSecretsManagerDuplicateKey(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowAWSSecretsManagerJSONParseError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class MetaflowGcpSecretsManagerJSONParseError(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowAWSSecretsManagerNotJSONObject(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class MetaflowGcpSecretsManagerNotJSONObject(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class GcpSecretManagerSecretsProvider(metaflow.plugins.secrets.SecretsProvider, metaclass=abc.ABCMeta):
+class AwsSecretsManagerSecretsProvider(metaflow.plugins.secrets.SecretsProvider, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None):
         """
-        Reads a secret from GCP Secrets Manager and returns it as a dictionary of environment variables.
+        Reads a secret from AWS Secrets Manager and returns it as a dictionary of environment variables.
+        
+        The secret payload from AWS is EITHER a string OR a binary blob.
         
         If the secret contains a string payload ("SecretString"):
-        - if the `json` option is True:
-            Secret will be parsed as a JSON. If successfully parsed, AND the JSON contains a
+        - if the `parse_secret_string_as_json` option is True (default):
+            {SecretString} will be parsed as a JSON. If successfully parsed, AND the JSON contains a
             top-level object, each entry K/V in the object will also be converted to an entry in the result. V will
             always be casted to a string (if not already a string).
-        - If `json` option is False (default):
-            Will be returned as a single entry in the result, with the key being the last part after / in secret_id.
+        - If `parse_secret_string_as_json` option is False:
+            {SecretString} will be returned as a single entry in the result, with the key being the secret_id.
         
-        On GCP Secrets Manager, the secret payload is a binary blob. However, by default we interpret it as UTF8 encoded
-        string. To disable this, set the `binary` option to True, the binary will be base64 encoded in the result.
+        Otherwise, the secret contains a binary blob payload ("SecretBinary"). In this case
+        - The result dic contains '{SecretName}': '{SecretBinary}', where {SecretBinary} is a base64-encoded string
         
         All keys in the result are sanitized to be more valid environment variable names. This is done on a best effort
         basis. Further validation is expected to be done by the invoking @secrets decorator itself.
         
-        :param secret_id: GCP Secrets Manager secret ID
+        :param secret_id: ARN or friendly name of the secret
         :param options: unused
+        :param role: AWS IAM Role ARN to assume before reading the secret
         :return: dict of environment variables. All keys and values are strings.
         """
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_exceptions.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.480288                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.082331                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.480570                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.082614                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.445848                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.047395                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.461401                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.062766                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -108,15 +108,19 @@
     ...
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, shared_memory = None, port = None):
+    def create_jobset(self, job_spec = None, run_id = None, step_name = None, task_id = None, namespace = None, env = None, num_parallel = None, port = None, annotations = None, labels = None):
+        ...
+    def create_job_object(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None, port = None, name_pattern = None, num_parallel = None):
+        ...
+    def create_k8sjob(self, job):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 def validate_kube_labels(labels: typing.Optional[typing.Dict[str, typing.Optional[str]]]) -> bool:
     """
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.463091                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.065458                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
-    import metaflow.exception
     import metaflow._vendor.click.types
+    import metaflow.exception
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
     def __repr__(self):
@@ -25,37 +25,48 @@
 
 class CommandException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 def sync_local_metadata_from_datastore(metadata_local_dir, task_ds):
     ...
 
+UBF_CONTROL: str
+
+UBF_TASK: str
+
 DATASTORE_LOCAL_DIR: str
 
 KUBERNETES_LABELS: str
 
 TASK_LOG_SOURCE: str
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, shared_memory = None, port = None):
+    def create_jobset(self, job_spec = None, run_id = None, step_name = None, task_id = None, namespace = None, env = None, num_parallel = None, port = None, annotations = None, labels = None):
+        ...
+    def create_job_object(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None, port = None, name_pattern = None, num_parallel = None):
+        ...
+    def create_k8sjob(self, job):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 class KubernetesKilledException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 def parse_kube_keyvalue_list(items: typing.List[str], requires_both: bool = True):
     ...
 
+class KubernetesException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
 class KubernetesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
     def package_init(self, flow, step_name, environment):
         ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.406863                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.039609                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
+    import metaflow.decorators
+    import metaflow.metaflow_current
+
+current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-CLIENT_REFRESH_INTERVAL_SECONDS: int
-
-class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
+class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
+        ...
     ...
 
-class KubernetesClient(object, metaclass=type):
-    def __init__(self):
-        ...
-    def get(self):
-        ...
-    def job(self, **kwargs):
+class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
-    def jobset(self, **kwargs):
+    def get_top_level_options(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.462311                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.064598                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -61,32 +61,30 @@
 
 KUBERNETES_PERSISTENT_VOLUME_CLAIMS: str
 
 KUBERNETES_TOLERATIONS: str
 
 KUBERNETES_SERVICE_ACCOUNT: None
 
-KUBERNETES_PORT: None
-
 KUBERNETES_SHARED_MEMORY: None
 
+KUBERNETES_PORT: None
+
 KUBERNETES_CPU: None
 
 KUBERNETES_MEMORY: None
 
 KUBERNETES_DISK: None
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
     ...
 
-UBF_CONTROL: str
-
 def get_docker_registry(image_uri):
     """
     Explanation:
         (.+?(?:[:.].+?)\/)? - [GROUP 0] REGISTRY
             .+?                  - A registry must start with at least one character
             (?:[:.].+?)\/       - A registry must have ":" or "." and end with "/"
             ?                    - Make a registry optional
@@ -142,14 +140,33 @@
 
 class KubernetesException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 def parse_kube_keyvalue_list(items: typing.List[str], requires_both: bool = True):
     ...
 
+UBF_CONTROL: str
+
+class TaskIdConstructor(object, metaclass=type):
+    @classmethod
+    def jobset_worker_id(cls, control_task_id: str):
+        ...
+    @classmethod
+    def join_step_task_ids(cls, num_parallel):
+        """
+        Called within the step decorator to set the `flow._control_mapper_tasks`.
+        Setting these allows the flow to know which tasks are needed in the join step.
+        We set this in the `task_pre_step` method of the decorator.
+        """
+        ...
+    @classmethod
+    def argo(cls):
+        ...
+    ...
+
 MAX_MEMORY_PER_TASK: None
 
 MAX_CPU_PER_TASK: None
 
 class KubernetesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/logs_cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/logs_cli.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.442639                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.044277                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow._vendor.click.core
     import metaflow.plugins.logs_cli
+    import metaflow._vendor.click.core
     import metaflow.exception
 
 LOGGER_TIMESTAMP: str
 
 class CommandException(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/parallel_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.432988                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.035528                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/perimeters.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/perimeters.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.407159                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.008737                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/project_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.437478                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.056372                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.metaflow_current
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-current: metaflow.metaflow_current.Current
-
-VALID_NAME_RE: str
-
-VALID_NAME_LEN: int
-
-class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
-        ...
-    def get_top_level_options(self):
+class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
+    def __init__(self, msg):
         ...
     ...
 
-def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
+class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.433428                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.053306                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAGIC_FILE: str
+def conda_platform():
+    ...
+
+def wheel_tags(wheel):
+    ...
+
+def pip_tags(python_version, mamba_platform):
+    ...
+
+def parse_filename_from_url(url):
+    ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.456935                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.053014                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.458135                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.054062                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/pypi_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.456403                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.052481                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.458525                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.054451                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.pypi.conda_environment
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/resources_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.433559                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.035958                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/retry_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.436472                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.040076                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAX_ATTEMPTS: int
-
-class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+class StorageExecutor(object, metaclass=type):
+    def __init__(self, use_processes = False):
+        ...
+    def warm_up(self):
         ...
-    def step_task_retry_count(self):
+    def submit(self, *args, **kwargs):
         ...
     ...
 
+def handle_executor_exceptions(func):
+    """
+    Decorator for handling errors that come from an Executor. This decorator should
+    only be used on functions where executor errors are possible. I.e. the function
+    uses StorageExecutor.
+    """
+    ...
+
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.436685                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.038211                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.478286                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.066265                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.secrets
     import abc
+    import metaflow.plugins.secrets
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.478049                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.066027                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/storage_executor.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.437970                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.036324                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.decorators
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class StorageExecutor(object, metaclass=type):
-    def __init__(self, use_processes = False):
+UBF_CONTROL: str
+
+DEFAULT_RUNTIME_LIMIT: int
+
+class TimeoutException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class TimeoutDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def __init__(self, *args, **kwargs):
+        ...
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
-    def warm_up(self):
+    def task_pre_step(self, step_name, task_datastore, metadata, run_id, task_id, flow, graph, retry_count, max_user_code_retries, ubf_context, inputs):
         ...
-    def submit(self, *args, **kwargs):
+    def task_post_step(self, step_name, flow, graph, retry_count, max_user_code_retries):
         ...
     ...
 
-def handle_executor_exceptions(func):
-    """
-    Decorator for handling errors that come from an Executor. This decorator should
-    only be used on functions where executor errors are possible. I.e. the function
-    uses StorageExecutor.
-    """
+def get_run_time_limit_for_task(step_decos):
     ...
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/tag_cli.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.443780                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.045410                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.events
+    import metaflow.metaflow_current
     import datetime
+    import metaflow.events
     import metaflow.client.core
-    import metaflow.metaflow_current
+    import metaflow.exception
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.432659                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.034949                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/procpoll.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/procpoll.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.429992                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.031599                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.procpoll
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/profilers/__init__.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/profilers/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.407392                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.008967                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class gpu_profile(object, metaclass=type):
     def __init__(self, include_artifacts = True, artifact_prefix = "gpu_profile_", interval = 1):
```

### Comparing `ob-metaflow-stubs-3.5/metaflow-stubs/tagging_util.pyi` & `ob-metaflow-stubs-3.6/metaflow-stubs/tagging_util.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.3+ob(v1)                                                   #
-# Generated on 2024-05-17T23:07:04.410906                                        #
+# MF version: 2.11.16.1+ob(v1)                                                   #
+# Generated on 2024-05-21T17:36:50.012512                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/PKG-INFO` & `ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.5
+Version: 3.6
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/SOURCES.txt` & `ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 metaflow-stubs/metaflow_current.pyi
 metaflow-stubs/multicore_utils.pyi
 metaflow-stubs/parameters.pyi
 metaflow-stubs/procpoll.pyi
 metaflow-stubs/py.typed
 metaflow-stubs/pylint_wrapper.pyi
 metaflow-stubs/tagging_util.pyi
+metaflow-stubs/tuple_util.pyi
 metaflow-stubs/client/__init__.pyi
 metaflow-stubs/client/core.pyi
 metaflow-stubs/client/filecache.pyi
 metaflow-stubs/metadata/metadata.pyi
 metaflow-stubs/metadata/util.pyi
 metaflow-stubs/mflog/mflog.pyi
 metaflow-stubs/plugins/__init__.pyi
@@ -120,14 +121,15 @@
 metaflow-stubs/plugins/gcp/gs_utils.pyi
 metaflow-stubs/plugins/gcp/includefile_support.pyi
 metaflow-stubs/plugins/kubernetes/__init__.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi
 metaflow-stubs/plugins/pypi/__init__.pyi
 metaflow-stubs/plugins/pypi/conda_decorator.pyi
 metaflow-stubs/plugins/pypi/conda_environment.pyi
 metaflow-stubs/plugins/pypi/pypi_decorator.pyi
 metaflow-stubs/plugins/pypi/pypi_environment.pyi
 metaflow-stubs/plugins/pypi/utils.pyi
 metaflow-stubs/plugins/secrets/__init__.pyi
```

### Comparing `ob-metaflow-stubs-3.5/setup.py` & `ob-metaflow-stubs-3.6/setup.py`

 * *Files identical despite different names*

