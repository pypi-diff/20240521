# Comparing `tmp/forloop_modules-1.1.3.tar.gz` & `tmp/forloop_modules-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forloop_modules-1.1.3.tar", last modified: Fri May 17 06:51:40 2024, max compression
+gzip compressed data, was "forloop_modules-1.1.4.tar", last modified: Tue May 21 18:31:39 2024, max compression
```

## Comparing `forloop_modules-1.1.3.tar` & `forloop_modules-1.1.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.859665 forloop_modules-1.1.3/
--rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      658 2024-05-17 06:51:40.859665 forloop_modules-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.465051 forloop_modules-1.1.3/forloop_modules/
--rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.489786 forloop_modules-1.1.3/forloop_modules/errors/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/errors/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/errors/errors.py
--rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.1.3/forloop_modules/flog.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.630080 forloop_modules-1.1.3/forloop_modules/function_handlers/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/__init__.py
--rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/api_endpoint_handlers.py
--rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/api_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.684336 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/__init__.py
--rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
--rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
--rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/data_types_validation.py
--rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/docs.py
--rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
--rw-rw-rw-   0        0        0     7933 2024-05-03 13:07:28.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/form_dict_list.py
--rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
--rw-rw-rw-   0        0        0    25173 2024-05-03 13:07:28.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/browser_handlers.py
--rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/cleaning_handlers.py
--rw-rw-rw-   0        0        0    12333 2024-05-16 23:27:10.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/control_flow_handlers.py
--rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/data_handlers.py
--rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/database_handlers.py
--rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/datetime_handlers.py
--rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/file_managment_handlers.py
--rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/integration_handlers.py
--rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/mapping_handlers.py
--rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/model_handlers.py
--rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/orchestration_handlers.py
--rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/rpa_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.710017 forloop_modules-1.1.3/forloop_modules/function_handlers/transformations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/transformations/__init__.py
--rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/transformations/basic_transforms.py
--rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/transformations/imputation.py
--rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/transformations/outliers.py
--rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/variable_handlers.py
--rw-rw-rw-   0        0        0   103383 2024-05-03 13:07:28.000000 forloop_modules-1.1.3/forloop_modules/function_handlers/webscraping_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.752259 forloop_modules-1.1.3/forloop_modules/globals/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/globals/__init__.py
--rw-rw-rw-   0        0        0     5162 2024-05-03 13:07:28.000000 forloop_modules-1.1.3/forloop_modules/globals/active_entity_tracker.py
--rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/globals/database_utilities_handler.py
--rw-rw-rw-   0        0        0     7845 2024-05-10 08:26:16.000000 forloop_modules-1.1.3/forloop_modules/globals/db_connection.py
--rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/globals/dbtables_loader_popups.py
--rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/globals/docs_categories.py
--rw-rw-rw-   0        0        0    18806 2024-05-16 23:27:10.000000 forloop_modules-1.1.3/forloop_modules/globals/local_variable_handler.py
--rw-rw-rw-   0        0        0    33335 2024-05-10 08:26:16.000000 forloop_modules-1.1.3/forloop_modules/globals/scraping_utilities_handler.py
--rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/globals/variable_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.768606 forloop_modules-1.1.3/forloop_modules/integrations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/integrations/__init__.py
--rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/integrations/slack_integration.py
--rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/integrations/testing_check_slack_notifications.py
--rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/node_detail_form.py
--rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/pipeline_function_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.779727 forloop_modules-1.1.3/forloop_modules/queries/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/queries/__init__.py
--rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/queries/context_request_backend_auxiliary_functions.py
--rw-rw-rw-   0        0        0    21803 2024-05-16 23:27:10.000000 forloop_modules-1.1.3/forloop_modules/queries/db_model_templates.py
--rw-rw-rw-   0        0        0    42313 2024-05-16 23:27:10.000000 forloop_modules-1.1.3/forloop_modules/queries/node_context_requests_backend.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.781230 forloop_modules-1.1.3/forloop_modules/redis/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/redis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.782235 forloop_modules-1.1.3/forloop_modules/redis/config/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/redis/config/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-05-17 06:48:31.000000 forloop_modules-1.1.3/forloop_modules/redis/config/config.py
--rw-rw-rw-   0        0        0     6573 2024-05-16 23:27:10.000000 forloop_modules-1.1.3/forloop_modules/redis/redis_connection.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.851229 forloop_modules-1.1.3/forloop_modules/utils/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/utils/__init__.py
--rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.1.3/forloop_modules/utils/definitions.py
--rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/utils/encryption.py
--rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/utils/pandas_operations.py
--rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/utils/pickle_serializer.py
--rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/utils/script_utils.py
--rw-rw-rw-   0        0        0     2021 2024-05-03 13:07:28.000000 forloop_modules-1.1.3/forloop_modules/utils/sse_parser.py
--rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/utils/str_helpers.py
--rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.1.3/forloop_modules/utils/synchronization_flags.py
--rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.1.3/forloop_modules/utils/url_template_builder.py
--rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.1.3/forloop_modules/utils/various.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.484131 forloop_modules-1.1.3/forloop_modules.egg-info/
--rw-rw-rw-   0        0        0      658 2024-05-17 06:51:40.000000 forloop_modules-1.1.3/forloop_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3529 2024-05-17 06:51:40.000000 forloop_modules-1.1.3/forloop_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 06:51:40.000000 forloop_modules-1.1.3/forloop_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-17 06:51:40.000000 forloop_modules-1.1.3/forloop_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 06:51:40.859665 forloop_modules-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-05-17 06:48:38.000000 forloop_modules-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.859665 forloop_modules-1.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.1.3/tests/test_url_template_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.343184 forloop_modules-1.1.4/
+-rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      658 2024-05-21 18:31:39.342184 forloop_modules-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:38.911182 forloop_modules-1.1.4/forloop_modules/
+-rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:38.930212 forloop_modules-1.1.4/forloop_modules/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/errors/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/errors/errors.py
+-rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.1.4/forloop_modules/flog.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.112723 forloop_modules-1.1.4/forloop_modules/function_handlers/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/__init__.py
+-rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/api_endpoint_handlers.py
+-rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/api_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.156725 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/__init__.py
+-rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
+-rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/data_types_validation.py
+-rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/docs.py
+-rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
+-rw-rw-rw-   0        0        0     7933 2024-05-03 13:07:28.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/form_dict_list.py
+-rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
+-rw-rw-rw-   0        0        0    25173 2024-05-03 13:07:28.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/browser_handlers.py
+-rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/cleaning_handlers.py
+-rw-rw-rw-   0        0        0    12333 2024-05-16 23:27:10.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/control_flow_handlers.py
+-rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/data_handlers.py
+-rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/database_handlers.py
+-rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/datetime_handlers.py
+-rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/file_managment_handlers.py
+-rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/integration_handlers.py
+-rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/mapping_handlers.py
+-rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/model_handlers.py
+-rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/orchestration_handlers.py
+-rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/rpa_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.178518 forloop_modules-1.1.4/forloop_modules/function_handlers/transformations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/transformations/__init__.py
+-rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/transformations/basic_transforms.py
+-rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/transformations/imputation.py
+-rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/transformations/outliers.py
+-rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/variable_handlers.py
+-rw-rw-rw-   0        0        0   103383 2024-05-03 13:07:28.000000 forloop_modules-1.1.4/forloop_modules/function_handlers/webscraping_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.229700 forloop_modules-1.1.4/forloop_modules/globals/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/globals/__init__.py
+-rw-rw-rw-   0        0        0     5162 2024-05-03 13:07:28.000000 forloop_modules-1.1.4/forloop_modules/globals/active_entity_tracker.py
+-rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/globals/database_utilities_handler.py
+-rw-rw-rw-   0        0        0     8917 2024-05-21 18:30:50.000000 forloop_modules-1.1.4/forloop_modules/globals/db_connection.py
+-rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/globals/dbtables_loader_popups.py
+-rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/globals/docs_categories.py
+-rw-rw-rw-   0        0        0    18806 2024-05-16 23:27:10.000000 forloop_modules-1.1.4/forloop_modules/globals/local_variable_handler.py
+-rw-rw-rw-   0        0        0    33335 2024-05-10 08:26:16.000000 forloop_modules-1.1.4/forloop_modules/globals/scraping_utilities_handler.py
+-rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/globals/variable_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.243705 forloop_modules-1.1.4/forloop_modules/integrations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/integrations/__init__.py
+-rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/integrations/slack_integration.py
+-rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/integrations/testing_check_slack_notifications.py
+-rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/node_detail_form.py
+-rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/pipeline_function_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.259643 forloop_modules-1.1.4/forloop_modules/queries/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/queries/__init__.py
+-rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/queries/context_request_backend_auxiliary_functions.py
+-rw-rw-rw-   0        0        0    21803 2024-05-16 23:27:10.000000 forloop_modules-1.1.4/forloop_modules/queries/db_model_templates.py
+-rw-rw-rw-   0        0        0    42315 2024-05-21 18:30:50.000000 forloop_modules-1.1.4/forloop_modules/queries/node_context_requests_backend.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.265644 forloop_modules-1.1.4/forloop_modules/redis/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/redis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.269645 forloop_modules-1.1.4/forloop_modules/redis/config/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/redis/config/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-05-17 06:48:31.000000 forloop_modules-1.1.4/forloop_modules/redis/config/config.py
+-rw-rw-rw-   0        0        0     6573 2024-05-16 23:27:10.000000 forloop_modules-1.1.4/forloop_modules/redis/redis_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.335168 forloop_modules-1.1.4/forloop_modules/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/utils/__init__.py
+-rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.1.4/forloop_modules/utils/definitions.py
+-rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/utils/encryption.py
+-rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/utils/pandas_operations.py
+-rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/utils/pickle_serializer.py
+-rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/utils/script_utils.py
+-rw-rw-rw-   0        0        0     2021 2024-05-03 13:07:28.000000 forloop_modules-1.1.4/forloop_modules/utils/sse_parser.py
+-rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/utils/str_helpers.py
+-rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.1.4/forloop_modules/utils/synchronization_flags.py
+-rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.1.4/forloop_modules/utils/url_template_builder.py
+-rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.1.4/forloop_modules/utils/various.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:38.925195 forloop_modules-1.1.4/forloop_modules.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-05-21 18:31:38.000000 forloop_modules-1.1.4/forloop_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3529 2024-05-21 18:31:38.000000 forloop_modules-1.1.4/forloop_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 18:31:38.000000 forloop_modules-1.1.4/forloop_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-21 18:31:38.000000 forloop_modules-1.1.4/forloop_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 18:31:39.343184 forloop_modules-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-21 18:31:02.000000 forloop_modules-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:39.342184 forloop_modules-1.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.1.4/tests/test_url_template_builder.py
```

### Comparing `forloop_modules-1.1.3/LICENSE` & `forloop_modules-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/PKG-INFO` & `forloop_modules-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop_modules
-Version: 1.1.3
+Version: 1.1.4
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.1.3/forloop_modules/errors/errors.py` & `forloop_modules-1.1.4/forloop_modules/errors/errors.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/flog.py` & `forloop_modules-1.1.4/forloop_modules/flog.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/api_endpoint_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/api_endpoint_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/api_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/api_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/data_types_validation.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/data_types_validation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/docs.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/docs.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/form_dict_list.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/form_dict_list.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/browser_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/browser_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/cleaning_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/cleaning_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/control_flow_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/control_flow_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/data_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/data_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/database_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/database_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/datetime_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/datetime_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/file_managment_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/file_managment_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/integration_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/integration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/mapping_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/mapping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/model_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/model_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/orchestration_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/orchestration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/rpa_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/rpa_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/transformations/basic_transforms.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/transformations/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/transformations/imputation.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/transformations/imputation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/transformations/outliers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/transformations/outliers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/variable_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/variable_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/function_handlers/webscraping_handlers.py` & `forloop_modules-1.1.4/forloop_modules/function_handlers/webscraping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/globals/active_entity_tracker.py` & `forloop_modules-1.1.4/forloop_modules/globals/active_entity_tracker.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/globals/database_utilities_handler.py` & `forloop_modules-1.1.4/forloop_modules/globals/database_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/globals/db_connection.py` & `forloop_modules-1.1.4/forloop_modules/globals/db_connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from typing import Literal, Optional, Union
 
+import rsa
 from pydantic import BaseModel
 
 import dbhydra.dbhydra_core as dh
 import forloop_modules.flog as flog
 from forloop_modules.redis.redis_connection import (
     create_redis_key_for_project_db_private_key,
     kv_redis,
 )
 from forloop_modules.utils.encryption import (
     convert_base64_private_key_to_rsa_private_key,
+    convert_rsa_private_to_base64_private_key,
     decrypt_text,
+    encrypt_text,
 )
 
 DbDialect = Literal["MySQL", "SQL Server", "PostgreSQL", "Xlsx structure", "MongoDB", "BigQuery"]
 DBInstance = Union[dh.MysqlDb, dh.SqlServerDb, dh.PostgresDb, dh.XlsxDB, dh.MongoDb, dh.BigQueryDb]
 
 
 class DbDetails(BaseModel):
@@ -145,14 +148,34 @@
         LOCALLY=False,
         DIALECT=db_dict["dialect"],
     )
 
     return db_details
 
 
+def encrypt_db_password(password: str, project_uid: str) -> str:
+    redis_key = create_redis_key_for_project_db_private_key(project_uid=project_uid)
+    private_key_base64 = kv_redis.get(redis_key)
+
+    if private_key_base64 is None:
+        # If no private key for project exists, create a new one and store it into Redis
+        public_key, private_key = rsa.newkeys(512)
+        redis_key = create_redis_key_for_project_db_private_key(project_uid=project_uid)
+        private_key_base64 = convert_rsa_private_to_base64_private_key(private_key=private_key)
+        kv_redis.set(redis_key, private_key_base64)
+    else:
+        # Else decode the private key to bytes and use it to create encryption (public) key
+        private_key = convert_base64_private_key_to_rsa_private_key(
+            private_key_base64=private_key_base64
+        )
+        public_key = rsa.PublicKey(private_key.n, private_key.e)
+
+    return encrypt_text(text=password, public_key=public_key)
+
+
 def decrypt_db_details(database: dict) -> DbDetails:
     """Decrypt the password of the database using the private key stored in Redis."""
     redis_key = create_redis_key_for_project_db_private_key(project_uid=database['project_uid'])
     private_key_base64 = kv_redis.get(redis_key)
 
     if private_key_base64 is not None:
         private_key = convert_base64_private_key_to_rsa_private_key(
```

### Comparing `forloop_modules-1.1.3/forloop_modules/globals/dbtables_loader_popups.py` & `forloop_modules-1.1.4/forloop_modules/globals/dbtables_loader_popups.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/globals/local_variable_handler.py` & `forloop_modules-1.1.4/forloop_modules/globals/local_variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/globals/scraping_utilities_handler.py` & `forloop_modules-1.1.4/forloop_modules/globals/scraping_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/globals/variable_handler.py` & `forloop_modules-1.1.4/forloop_modules/globals/variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/integrations/slack_integration.py` & `forloop_modules-1.1.4/forloop_modules/integrations/slack_integration.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/integrations/testing_check_slack_notifications.py` & `forloop_modules-1.1.4/forloop_modules/integrations/testing_check_slack_notifications.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/node_detail_form.py` & `forloop_modules-1.1.4/forloop_modules/node_detail_form.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/pipeline_function_handlers.py` & `forloop_modules-1.1.4/forloop_modules/pipeline_function_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/queries/context_request_backend_auxiliary_functions.py` & `forloop_modules-1.1.4/forloop_modules/queries/context_request_backend_auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/queries/db_model_templates.py` & `forloop_modules-1.1.4/forloop_modules/queries/db_model_templates.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/queries/node_context_requests_backend.py` & `forloop_modules-1.1.4/forloop_modules/queries/node_context_requests_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1110,15 +1110,15 @@
     return project_databases
 
 # def get_all_databases():
 #     response=requests.get(SERVER+":"+str(PORT)+"/api/v1/databases")
 #     return(response)
 
 # def delete_database_by_uid(database_uid):
-#     response=requests.delete(SERVER+":"+str(PORT)+"/api/v1/database/"+str(database_uid))
+#     response=requests.delete(SERVER+":"+str(PORT)+"/api/v1/databases/"+str(database_uid))
 #     flog.info(f'DELETE Database response: {response.text}')
 #     return(response)
 
 # def new_database(database_name, server, port, database, username, password, dialect, project_uid="0"):
 #     payload = {
 #         "database_name": database_name,
 #         "server": server,
@@ -1145,15 +1145,15 @@
 #         "database": database,
 #         "username": username,
 #         "password": password,
 #         "dialect": dialect,
 #         }
 #     flog.info(f'New Dataset payload: {payload}')
 #
-#     url = f'{SERVER}:{PORT}/api/v1/database/{database_uid}'
+#     url = f'{SERVER}:{PORT}/api/v1/databases/{database_uid}'
 #
 #     response = requests.put(url, json=payload)
 #     flog.info(f'New Database response: {response.text}')
 #
 #     return response
```

### Comparing `forloop_modules-1.1.3/forloop_modules/redis/config/config.py` & `forloop_modules-1.1.4/forloop_modules/redis/config/config.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/redis/redis_connection.py` & `forloop_modules-1.1.4/forloop_modules/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/definitions.py` & `forloop_modules-1.1.4/forloop_modules/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/encryption.py` & `forloop_modules-1.1.4/forloop_modules/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/pandas_operations.py` & `forloop_modules-1.1.4/forloop_modules/utils/pandas_operations.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/pickle_serializer.py` & `forloop_modules-1.1.4/forloop_modules/utils/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/script_utils.py` & `forloop_modules-1.1.4/forloop_modules/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/sse_parser.py` & `forloop_modules-1.1.4/forloop_modules/utils/sse_parser.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/str_helpers.py` & `forloop_modules-1.1.4/forloop_modules/utils/str_helpers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/synchronization_flags.py` & `forloop_modules-1.1.4/forloop_modules/utils/synchronization_flags.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/url_template_builder.py` & `forloop_modules-1.1.4/forloop_modules/utils/url_template_builder.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules/utils/various.py` & `forloop_modules-1.1.4/forloop_modules/utils/various.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/forloop_modules.egg-info/PKG-INFO` & `forloop_modules-1.1.4/forloop_modules.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop-modules
-Version: 1.1.3
+Version: 1.1.4
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.1.3/forloop_modules.egg-info/SOURCES.txt` & `forloop_modules-1.1.4/forloop_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.3/setup.py` & `forloop_modules-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='forloop_modules',
-    version='1.1.3',
+    version='1.1.4',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='This package contains open source modules and integrations within Forloop.ai platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ForloopAI/forloop_modules',
     packages=setuptools.find_packages(),
```

### Comparing `forloop_modules-1.1.3/tests/test_url_template_builder.py` & `forloop_modules-1.1.4/tests/test_url_template_builder.py`

 * *Files identical despite different names*

