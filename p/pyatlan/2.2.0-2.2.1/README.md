# Comparing `tmp/pyatlan-2.2.0.tar.gz` & `tmp/pyatlan-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-2.2.0.tar", last modified: Wed May 15 12:40:29 2024, max compression
+gzip compressed data, was "pyatlan-2.2.1.tar", last modified: Tue May 21 13:09:02 2024, max compression
```

## Comparing `pyatlan-2.2.0.tar` & `pyatlan-2.2.1.tar`

### file list

```diff
@@ -1,492 +1,503 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.429369 pyatlan-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-15 12:40:23.000000 pyatlan-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 12:40:23.000000 pyatlan-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 12:40:23.000000 pyatlan-2.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-15 12:40:29.429369 pyatlan-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-15 12:40:23.000000 pyatlan-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.353369 pyatlan-2.2.0/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.357369 pyatlan-2.2.0/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.357369 pyatlan-2.2.0/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    77429 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    59409 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/impersonate.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.357369 pyatlan-2.2.0/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/events/atlan_lambda_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.361369 pyatlan-2.2.0/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32321 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/create_typedefs_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.361369 pyatlan-2.2.0/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/enums.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/globals.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/imports.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/init.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/module.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/properties.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/referenceable_attributes.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/referenceable_methods.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/structs.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.365369 pyatlan-2.2.0/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/api_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.405369 pyatlan-2.2.0/pyatlan/model/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_p_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_p_i_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_p_i_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_w_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)   124326 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/auth_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_event_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_event_hub_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/b_i_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/calculation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite3_d_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    51963 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21623 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cube_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cube_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cube_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_studio_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_model_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_dbtable.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/event_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/g_c_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/g_c_s_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/g_c_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/google.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/insight.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/kafka_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_look.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/m_c_incident.py
--rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/m_c_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/materialised_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metabase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metabase_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metabase_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metabase_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_dossier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_fact.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/multi_dimensional_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/no_s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/persona.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/process_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_analysis_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dashboard_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dataset_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/readme_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/redash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/redash_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/redash_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/redash_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/referenceable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/s3_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/saa_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/schema_registry_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_data_element_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_datamodel_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/snowflake_dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/snowflake_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/snowflake_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/snowflake_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/soda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/soda_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/spark_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/table_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_calculated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_datasource_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tag_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_dashlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_liveboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    76441 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.405369 pyatlan-2.2.0/pyatlan/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/fields/atlan_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/fluent_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/fluent_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/keycloak_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.409369 pyatlan-2.2.0/pyatlan/model/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.409369 pyatlan-2.2.0/pyatlan/model/packages/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/base/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/base/miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/base/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/big_query_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/confluent_kafka_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/dbt_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/dynamo_d_b_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/glue_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/postgres_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/powerbi_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/s_q_l_server_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/sigma_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/snowflake_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/snowflake_miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/sql_server_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/tableau_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/multipart_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.409369 pyatlan-2.2.0/pyatlan/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/create_package_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.413369 pyatlan-2.2.0/pyatlan/pkg/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/templates/default_configmap.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/templates/default_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/templates/package_config.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.429369 pyatlan-2.2.0/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16555 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 12:40:23.000000 pyatlan-2.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 12:40:23.000000 pyatlan-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:40:29.429369 pyatlan-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-15 12:40:23.000000 pyatlan-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.413369 pyatlan-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.417369 pyatlan-2.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/adls_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/airflow_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/api_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/custom_package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/data_mesh_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/gcs_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/owner_propagator_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/preset_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/requests_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_sql_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_sso_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.421369 pyatlan-2.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.425369 pyatlan-2.2.0/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_d_l_s_account_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_d_l_s_container_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_d_l_s_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_p_i_path_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_p_i_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/column_process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/data_domain_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/data_product_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/database_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.425369 pyatlan-2.2.0/tests/unit/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/fields/atlan_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/gcs_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/gcs_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/preset_chart_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/preset_dashboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/preset_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/preset_workspace_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.425369 pyatlan-2.2.0/tests/unit/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    68514 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_credential_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21011 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_query_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_sso_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15955 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_workflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.530149 pyatlan-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-21 13:08:58.000000 pyatlan-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 13:08:58.000000 pyatlan-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 13:08:58.000000 pyatlan-2.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-21 13:09:02.530149 pyatlan-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-21 13:08:58.000000 pyatlan-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.442149 pyatlan-2.2.1/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.446149 pyatlan-2.2.1/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.450149 pyatlan-2.2.1/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79101 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59409 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/impersonate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.450149 pyatlan-2.2.1/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/events/atlan_lambda_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.450149 pyatlan-2.2.1/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32321 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/create_typedefs_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.450149 pyatlan-2.2.1/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/enums.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/globals.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/imports.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/init.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/properties.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/referenceable_attributes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/referenceable_methods.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/structs.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.458149 pyatlan-2.2.1/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/api_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.506149 pyatlan-2.2.1/pyatlan/model/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_p_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_p_i_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_p_i_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_w_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/airflow_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/airflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124326 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/auth_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_event_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_event_hub_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/b_i_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/calculation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite3_d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51792 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21623 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cube_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cube_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cube_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_studio_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_model_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_dbtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/event_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/g_c_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/g_c_s_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/g_c_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/kafka_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_look.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/m_c_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/m_c_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/materialised_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metabase_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metabase_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metabase_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_dossier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_fact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/multi_dimensional_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/no_s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11171 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/process_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_analysis_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dashboard_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dataset_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/readme_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/redash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/redash_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/redash_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/redash_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/referenceable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/s3_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/saa_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/schema_registry_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_data_element_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_datamodel_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/snowflake_dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/snowflake_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/snowflake_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/snowflake_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/soda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/soda_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/spark_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/stakeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/stakeholder_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/table_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_calculated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_datasource_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tag_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_dashlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_liveboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77838 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.506149 pyatlan-2.2.1/pyatlan/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/fields/atlan_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/fluent_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/fluent_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/keycloak_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/pyatlan/model/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/pyatlan/model/packages/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/base/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/base/miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/base/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/big_query_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/confluent_kafka_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/dbt_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/dynamo_d_b_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/glue_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/postgres_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/powerbi_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/s_q_l_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/sigma_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/snowflake_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/snowflake_miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/sql_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/tableau_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/multipart_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/pyatlan/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/create_package_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/pyatlan/pkg/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/templates/default_configmap.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/templates/default_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/templates/package_config.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.530149 pyatlan-2.2.1/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-21 13:08:58.000000 pyatlan-2.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 13:08:58.000000 pyatlan-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:09:02.530149 pyatlan-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-21 13:08:58.000000 pyatlan-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.518149 pyatlan-2.2.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/adls_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/airflow_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/api_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/custom_package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/data_mesh_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/gcs_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31905 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/owner_propagator_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/preset_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/requests_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_sql_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_sso_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.522149 pyatlan-2.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26291 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.526149 pyatlan-2.2.1/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_d_l_s_account_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_d_l_s_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_d_l_s_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_p_i_path_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_p_i_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/airflow_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/airflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/column_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/data_domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/data_product_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/database_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.526149 pyatlan-2.2.1/tests/unit/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/fields/atlan_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/gcs_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/gcs_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/preset_chart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/preset_dashboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/preset_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/preset_workspace_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.530149 pyatlan-2.2.1/tests/unit/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69612 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_credential_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21011 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_query_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_sso_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15955 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_workflow_client.py
```

### Comparing `pyatlan-2.2.0/LICENSE` & `pyatlan-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/PKG-INFO` & `pyatlan-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.2.0
+Version: 2.2.1
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyatlan-2.2.0/README.md` & `pyatlan-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-2.2.1/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-2.2.1/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/cache/enum_cache.py` & `pyatlan-2.2.1/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/cache/group_cache.py` & `pyatlan-2.2.1/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/cache/role_cache.py` & `pyatlan-2.2.1/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/cache/user_cache.py` & `pyatlan-2.2.1/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/admin.py` & `pyatlan-2.2.1/pyatlan/client/admin.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/asset.py` & `pyatlan-2.2.1/pyatlan/client/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 from pyatlan.model.assets import (
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
     Connection,
     Database,
+    DataDomain,
+    DataProduct,
     MaterialisedView,
     Persona,
     Purpose,
     Referenceable,
     Schema,
     Table,
     View,
@@ -1527,22 +1529,62 @@
         glossary = self.find_glossary_by_name(name=glossary_name)
         return self.find_term_fast_by_name(
             name=name,
             glossary_qualified_name=glossary.qualified_name,
             attributes=attributes,
         )
 
+    @validate_arguments
+    def find_domain_by_name(
+        self,
+        name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        attributes: Optional[List[StrictStr]] = None,
+    ) -> DataDomain:
+        """
+        Find a data domain by its human-readable name.
+
+        :param name: of the domain
+        :param attributes: (optional) collection of attributes to retrieve for the domain
+        :returns: the domain, if found
+        :raises NotFoundError: if no domain with the provided name exists
+        """
+        attributes = attributes or []
+        query = Term.with_name(name) + Term.with_type_name("DataDomain")
+        return self._search_for_asset_with_name(
+            query=query, name=name, asset_type=DataDomain, attributes=attributes
+        )[0]
+
+    @validate_arguments
+    def find_product_by_name(
+        self,
+        name: constr(strip_whitespace=True, min_length=1, strict=True),  # type: ignore
+        attributes: Optional[List[StrictStr]] = None,
+    ) -> DataProduct:
+        """
+        Find a data product by its human-readable name.
+
+        :param name: of the product
+        :param attributes: (optional) collection of attributes to retrieve for the product
+        :returns: the product, if found
+        :raises NotFoundError: if no product with the provided name exists
+        """
+        attributes = attributes or []
+        query = Term.with_name(name) + Term.with_type_name("DataProduct")
+        return self._search_for_asset_with_name(
+            query=query, name=name, asset_type=DataProduct, attributes=attributes
+        )[0]
+
     # TODO: Try adding @validate_arguments to this method once
     # the issue below is fixed or when we switch to pydantic v2
     # https://github.com/pydantic/pydantic/issues/2901
     def get_hierarchy(
         self,
         glossary: AtlasGlossary,
-        attributes: Optional[List[AtlanField]] = None,
-        related_attributes: Optional[List[AtlanField]] = None,
+        attributes: Optional[List[Union[AtlanField, str]]] = None,
+        related_attributes: Optional[List[Union[AtlanField, str]]] = None,
     ) -> CategoryHierarchy:
         """
         Retrieve category hierarchy in this Glossary, in a traversable form. You can traverse in either depth_first
         or breadth_first order. Both return an ordered list of Glossary objects.
         Note: by default, each category will have a minimal set of information (name, GUID, qualifiedName). If you
         want additional details about each category, specify the attributes you want in the attributes parameter
         of this method.
```

### Comparing `pyatlan-2.2.0/pyatlan/client/atlan.py` & `pyatlan-2.2.1/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/audit.py` & `pyatlan-2.2.1/pyatlan/client/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/common.py` & `pyatlan-2.2.1/pyatlan/client/common.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/constants.py` & `pyatlan-2.2.1/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/credential.py` & `pyatlan-2.2.1/pyatlan/client/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/file.py` & `pyatlan-2.2.1/pyatlan/client/file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/group.py` & `pyatlan-2.2.1/pyatlan/client/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/impersonate.py` & `pyatlan-2.2.1/pyatlan/client/impersonate.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/query.py` & `pyatlan-2.2.1/pyatlan/client/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/role.py` & `pyatlan-2.2.1/pyatlan/client/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/search_log.py` & `pyatlan-2.2.1/pyatlan/client/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/sso.py` & `pyatlan-2.2.1/pyatlan/client/sso.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/task.py` & `pyatlan-2.2.1/pyatlan/client/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/token.py` & `pyatlan-2.2.1/pyatlan/client/token.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/typedef.py` & `pyatlan-2.2.1/pyatlan/client/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/user.py` & `pyatlan-2.2.1/pyatlan/client/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/client/workflow.py` & `pyatlan-2.2.1/pyatlan/client/workflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/errors.py` & `pyatlan-2.2.1/pyatlan/errors.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/events/atlan_event_handler.py` & `pyatlan-2.2.1/pyatlan/events/atlan_event_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-2.2.1/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/class_generator.py` & `pyatlan-2.2.1/pyatlan/generator/class_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/create_typedefs_file.py` & `pyatlan-2.2.1/pyatlan/generator/create_typedefs_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/templates/globals.jinja2` & `pyatlan-2.2.1/pyatlan/generator/templates/globals.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/templates/imports.jinja2` & `pyatlan-2.2.1/pyatlan/generator/templates/imports.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -99,13 +99,12 @@
     PopularityInsights,
     SourceTagAttribute,
     StarredDetails,
 )
 from pyatlan.utils import (
     init_guid,
     next_id,
-    to_camel_case,
     validate_required_fields,
     validate_single_required_field,
     get_parent_qualified_name,
 )
 from pyatlan.model.data_mesh import DataProductsAssetsDSL
```

### Comparing `pyatlan-2.2.0/pyatlan/generator/templates/macros.jinja2` & `pyatlan-2.2.1/pyatlan/generator/templates/macros.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/templates/module.jinja2` & `pyatlan-2.2.1/pyatlan/generator/templates/module.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/templates/properties.jinja2` & `pyatlan-2.2.1/pyatlan/generator/templates/properties.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/templates/referenceable_attributes.jinja2` & `pyatlan-2.2.1/pyatlan/generator/templates/referenceable_attributes.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/templates/referenceable_methods.jinja2` & `pyatlan-2.2.1/pyatlan/generator/templates/referenceable_methods.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/generator/templates/structs.jinja2` & `pyatlan-2.2.1/pyatlan/generator/templates/structs.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/logging.conf` & `pyatlan-2.2.1/pyatlan/logging.conf`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/aggregation.py` & `pyatlan-2.2.1/pyatlan/model/aggregation.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/api_tokens.py` & `pyatlan-2.2.1/pyatlan/model/api_tokens.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/__init__.py` & `pyatlan-2.2.1/pyatlan/model/assets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .referenceable import Referenceable
 from .asset import Asset
 from .data_set import DataSet
 from .tag_attachment import TagAttachment
 from .connection import Connection
 from .process import Process
 from .atlas_glossary_category import AtlasGlossaryCategory
+from .stakeholder_title import StakeholderTitle
 from .badge import Badge
 from .access_control import AccessControl
 from .namespace import Namespace
 from .catalog import Catalog
 from .atlas_glossary import AtlasGlossary
 from .auth_policy import AuthPolicy
 from .process_execution import ProcessExecution
@@ -44,14 +45,15 @@
 from .spark import Spark
 from .tag import Tag
 from .schema_registry import SchemaRegistry
 from .google import Google
 from .azure import Azure
 from .a_w_s import AWS
 from .dbt_column_process import DbtColumnProcess
+from .stakeholder import Stakeholder
 from .airflow_dag import AirflowDag
 from .airflow_task import AirflowTask
 from .s3 import S3
 from .a_d_l_s import ADLS
 from .g_c_s import GCS
 from .monte_carlo import MonteCarlo
 from .metric import Metric
@@ -66,14 +68,15 @@
 from .sisense import Sisense
 from .data_studio import DataStudio
 from .metabase import Metabase
 from .quick_sight import QuickSight
 from .thoughtspot import Thoughtspot
 from .power_b_i import PowerBI
 from .micro_strategy import MicroStrategy
+from .cognos import Cognos
 from .qlik import Qlik
 from .cognite import Cognite
 from .salesforce import Salesforce
 from .readme_template import ReadmeTemplate
 from .readme import Readme
 from .file import File
 from .link import Link
@@ -207,14 +210,22 @@
 from .micro_strategy_metric import MicroStrategyMetric
 from .micro_strategy_cube import MicroStrategyCube
 from .micro_strategy_dossier import MicroStrategyDossier
 from .micro_strategy_fact import MicroStrategyFact
 from .micro_strategy_document import MicroStrategyDocument
 from .micro_strategy_attribute import MicroStrategyAttribute
 from .micro_strategy_visualization import MicroStrategyVisualization
+from .cognos_exploration import CognosExploration
+from .cognos_dashboard import CognosDashboard
+from .cognos_report import CognosReport
+from .cognos_module import CognosModule
+from .cognos_file import CognosFile
+from .cognos_folder import CognosFolder
+from .cognos_package import CognosPackage
+from .cognos_datasource import CognosDatasource
 from .qlik_space import QlikSpace
 from .qlik_app import QlikApp
 from .qlik_chart import QlikChart
 from .qlik_dataset import QlikDataset
 from .qlik_sheet import QlikSheet
 from .cognite_event import CogniteEvent
 from .cognite_asset import CogniteAsset
@@ -250,14 +261,15 @@
 Referenceable.Attributes.update_forward_refs(**localns)
 Asset.Attributes.update_forward_refs(**localns)
 DataSet.Attributes.update_forward_refs(**localns)
 TagAttachment.Attributes.update_forward_refs(**localns)
 Connection.Attributes.update_forward_refs(**localns)
 Process.Attributes.update_forward_refs(**localns)
 AtlasGlossaryCategory.Attributes.update_forward_refs(**localns)
+StakeholderTitle.Attributes.update_forward_refs(**localns)
 Badge.Attributes.update_forward_refs(**localns)
 AccessControl.Attributes.update_forward_refs(**localns)
 Namespace.Attributes.update_forward_refs(**localns)
 Catalog.Attributes.update_forward_refs(**localns)
 AtlasGlossary.Attributes.update_forward_refs(**localns)
 AuthPolicy.Attributes.update_forward_refs(**localns)
 ProcessExecution.Attributes.update_forward_refs(**localns)
@@ -291,14 +303,15 @@
 Spark.Attributes.update_forward_refs(**localns)
 Tag.Attributes.update_forward_refs(**localns)
 SchemaRegistry.Attributes.update_forward_refs(**localns)
 Google.Attributes.update_forward_refs(**localns)
 Azure.Attributes.update_forward_refs(**localns)
 AWS.Attributes.update_forward_refs(**localns)
 DbtColumnProcess.Attributes.update_forward_refs(**localns)
+Stakeholder.Attributes.update_forward_refs(**localns)
 AirflowDag.Attributes.update_forward_refs(**localns)
 AirflowTask.Attributes.update_forward_refs(**localns)
 S3.Attributes.update_forward_refs(**localns)
 ADLS.Attributes.update_forward_refs(**localns)
 GCS.Attributes.update_forward_refs(**localns)
 MonteCarlo.Attributes.update_forward_refs(**localns)
 Metric.Attributes.update_forward_refs(**localns)
@@ -313,14 +326,15 @@
 Sisense.Attributes.update_forward_refs(**localns)
 DataStudio.Attributes.update_forward_refs(**localns)
 Metabase.Attributes.update_forward_refs(**localns)
 QuickSight.Attributes.update_forward_refs(**localns)
 Thoughtspot.Attributes.update_forward_refs(**localns)
 PowerBI.Attributes.update_forward_refs(**localns)
 MicroStrategy.Attributes.update_forward_refs(**localns)
+Cognos.Attributes.update_forward_refs(**localns)
 Qlik.Attributes.update_forward_refs(**localns)
 Cognite.Attributes.update_forward_refs(**localns)
 Salesforce.Attributes.update_forward_refs(**localns)
 ReadmeTemplate.Attributes.update_forward_refs(**localns)
 Readme.Attributes.update_forward_refs(**localns)
 File.Attributes.update_forward_refs(**localns)
 Link.Attributes.update_forward_refs(**localns)
@@ -454,14 +468,22 @@
 MicroStrategyMetric.Attributes.update_forward_refs(**localns)
 MicroStrategyCube.Attributes.update_forward_refs(**localns)
 MicroStrategyDossier.Attributes.update_forward_refs(**localns)
 MicroStrategyFact.Attributes.update_forward_refs(**localns)
 MicroStrategyDocument.Attributes.update_forward_refs(**localns)
 MicroStrategyAttribute.Attributes.update_forward_refs(**localns)
 MicroStrategyVisualization.Attributes.update_forward_refs(**localns)
+CognosExploration.Attributes.update_forward_refs(**localns)
+CognosDashboard.Attributes.update_forward_refs(**localns)
+CognosReport.Attributes.update_forward_refs(**localns)
+CognosModule.Attributes.update_forward_refs(**localns)
+CognosFile.Attributes.update_forward_refs(**localns)
+CognosFolder.Attributes.update_forward_refs(**localns)
+CognosPackage.Attributes.update_forward_refs(**localns)
+CognosDatasource.Attributes.update_forward_refs(**localns)
 QlikSpace.Attributes.update_forward_refs(**localns)
 QlikApp.Attributes.update_forward_refs(**localns)
 QlikChart.Attributes.update_forward_refs(**localns)
 QlikDataset.Attributes.update_forward_refs(**localns)
 QlikSheet.Attributes.update_forward_refs(**localns)
 CogniteEvent.Attributes.update_forward_refs(**localns)
 CogniteAsset.Attributes.update_forward_refs(**localns)
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s.py` & `pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_account.py` & `pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_account.py`

 * *Files 5% similar despite different names*

```diff
@@ -332,30 +332,21 @@
         @init_guid
         def create(
             cls, *, name: str, connection_qualified_name: str
         ) -> ADLSAccount.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name"], [name, connection_qualified_name]
             )
-
-            # Split the connection_qualified_name to extract necessary information
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-
             return ADLSAccount.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
-                connector_name=connector_type.value,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
             )
 
     attributes: ADLSAccount.Attributes = Field(
         default_factory=lambda: ADLSAccount.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_container.py` & `pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,31 +259,23 @@
         def create(
             cls, *, name: str, adls_account_qualified_name: str
         ) -> ADLSContainer.Attributes:
             validate_required_fields(
                 ["name", "adls_account_qualified_name"],
                 [name, adls_account_qualified_name],
             )
-
-            # Split the adls_account_qualified_name to extract necessary information
-            fields = adls_account_qualified_name.split("/")
-            if len(fields) != 4:
-                raise ValueError("Invalid adls_account_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid adls_account_qualified_name") from e
-
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                adls_account_qualified_name, "adls_account_qualified_name", 4
+            )
             return ADLSContainer.Attributes(
                 name=name,
                 adls_account_qualified_name=adls_account_qualified_name,
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connector_name=connector_name,
+                connection_qualified_name=connection_qn,
                 qualified_name=f"{adls_account_qualified_name}/{name}",
-                connector_name=connector_type.value,
                 adls_account=ADLSAccount.ref_by_qualified_name(
                     adls_account_qualified_name
                 ),
             )
 
     attributes: ADLSContainer.Attributes = Field(
         default_factory=lambda: ADLSContainer.Attributes(),
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_object.py` & `pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,34 +517,26 @@
         def create(
             cls, *, name: str, adls_container_qualified_name: str
         ) -> ADLSObject.Attributes:
             validate_required_fields(
                 ["name", "adls_container_qualified_name"],
                 [name, adls_container_qualified_name],
             )
-
-            # Split the qualified_name to extract necessary information
-            fields = adls_container_qualified_name.split("/")
-            if len(fields) != 5:
-                raise ValueError("Invalid qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid qualified_name") from e
             adls_account_qualified_name = get_parent_qualified_name(
                 adls_container_qualified_name
             )
-
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                adls_container_qualified_name, "adls_container_qualified_name", 5
+            )
             return ADLSObject.Attributes(
                 name=name,
                 adls_container_qualified_name=adls_container_qualified_name,
                 qualified_name=f"{adls_container_qualified_name}/{name}",
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
-                connector_name=connector_type.value,
+                connector_name=connector_name,
+                connection_qualified_name=connection_qn,
                 adls_container=ADLSContainer.ref_by_qualified_name(
                     adls_container_qualified_name
                 ),
                 adls_account_qualified_name=adls_account_qualified_name,
             )
 
     attributes: ADLSObject.Attributes = Field(
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/a_p_i.py` & `pyatlan-2.2.1/pyatlan/model/assets/a_p_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/a_p_i_path.py` & `pyatlan-2.2.1/pyatlan/model/assets/a_p_i_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -228,32 +228,24 @@
         def create(
             cls, *, path_raw_uri: str, spec_qualified_name: str
         ) -> APIPath.Attributes:
             validate_required_fields(
                 ["path_raw_uri", "spec_qualified_name"],
                 [path_raw_uri, spec_qualified_name],
             )
-
-            # Split the spec_qualified_name to extract necessary information
-            fields = spec_qualified_name.split("/")
-            if len(fields) != 4:
-                raise ValueError("Invalid spec_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid spec_qualified_name") from e
-
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                spec_qualified_name, "spec_qualified_name", 4
+            )
             return APIPath.Attributes(
                 api_path_raw_u_r_i=path_raw_uri,
                 name=path_raw_uri,
                 api_spec_qualified_name=spec_qualified_name,
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connector_name=connector_name,
+                connection_qualified_name=connection_qn,
                 qualified_name=f"{spec_qualified_name}{path_raw_uri}",
-                connector_name=connector_type.value,
                 api_spec=APISpec.ref_by_qualified_name(spec_qualified_name),
             )
 
     attributes: APIPath.Attributes = Field(
         default_factory=lambda: APIPath.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/a_p_i_spec.py` & `pyatlan-2.2.1/pyatlan/model/assets/a_p_i_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,30 +257,21 @@
         @init_guid
         def create(
             cls, *, name: str, connection_qualified_name: str
         ) -> APISpec.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name"], [name, connection_qualified_name]
             )
-
-            # Split the connection_qualified_name to extract necessary information
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-
             return APISpec.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
-                connector_name=connector_type.value,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
             )
 
     attributes: APISpec.Attributes = Field(
         default_factory=lambda: APISpec.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/a_w_s.py` & `pyatlan-2.2.1/pyatlan/model/assets/a_w_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/access_control.py` & `pyatlan-2.2.1/pyatlan/model/assets/access_control.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/airflow.py` & `pyatlan-2.2.1/pyatlan/model/assets/airflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/airflow_dag.py` & `pyatlan-2.2.1/pyatlan/model/assets/airflow_dag.py`

 * *Files 16% similar despite different names*

```diff
@@ -121,28 +121,21 @@
             *,
             name: str,
             connection_qualified_name: str,
         ) -> AirflowDag.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name"], [name, connection_qualified_name]
             )
-            # Split the connection_qualified_name to extract necessary information
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-
             return AirflowDag.Attributes(
                 name=name,
-                connector_name=connector_type.value,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
             )
 
     attributes: AirflowDag.Attributes = Field(
         default_factory=lambda: AirflowDag.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/airflow_task.py` & `pyatlan-2.2.1/pyatlan/model/assets/airflow_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,29 +369,23 @@
             name: str,
             airflow_dag_qualified_name: str,
         ) -> AirflowTask.Attributes:
             validate_required_fields(
                 ["name", "airflow_dag_qualified_name"],
                 [name, airflow_dag_qualified_name],
             )
-            # Split the airflow_dag_qualified_name to extract necessary information
-            fields = airflow_dag_qualified_name.split("/")
-            if len(fields) != 4:
-                raise ValueError("Invalid airflow_dag_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid airflow_dag_qualified_name") from e
-
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                airflow_dag_qualified_name, "airflow_dag_qualified_name", 4
+            )
             return AirflowTask.Attributes(
                 name=name,
                 airflow_dag_qualified_name=airflow_dag_qualified_name,
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 qualified_name=f"{airflow_dag_qualified_name}/{name}",
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 airflow_dag=AirflowDag.ref_by_qualified_name(
                     airflow_dag_qualified_name
                 ),
             )
 
     attributes: AirflowTask.Attributes = Field(
         default_factory=lambda: AirflowTask.Attributes(),
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/asset.py` & `pyatlan-2.2.1/pyatlan/model/assets/asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary.py` & `pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary_category.py` & `pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary_category.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary_term.py` & `pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/auth_policy.py` & `pyatlan-2.2.1/pyatlan/model/assets/auth_policy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/auth_service.py` & `pyatlan-2.2.1/pyatlan/model/assets/auth_service.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/azure.py` & `pyatlan-2.2.1/pyatlan/model/assets/azure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/azure_event_hub.py` & `pyatlan-2.2.1/pyatlan/model/assets/azure_event_hub.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/azure_event_hub_consumer_group.py` & `pyatlan-2.2.1/pyatlan/model/assets/azure_event_hub_consumer_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus.py` & `pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus_namespace.py` & `pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus_namespace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus_topic.py` & `pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus_topic.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/b_i.py` & `pyatlan-2.2.1/pyatlan/model/assets/b_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/b_i_process.py` & `pyatlan-2.2.1/pyatlan/model/assets/b_i_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/badge.py` & `pyatlan-2.2.1/pyatlan/model/assets/badge.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/calculation_view.py` & `pyatlan-2.2.1/pyatlan/model/assets/calculation_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/catalog.py` & `pyatlan-2.2.1/pyatlan/model/assets/catalog.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cloud.py` & `pyatlan-2.2.1/pyatlan/model/assets/cloud.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cognite.py` & `pyatlan-2.2.1/pyatlan/model/assets/cognite.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cognite3_d_model.py` & `pyatlan-2.2.1/pyatlan/model/assets/cognite3_d_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cognite_asset.py` & `pyatlan-2.2.1/pyatlan/model/assets/cognite_asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cognite_event.py` & `pyatlan-2.2.1/pyatlan/model/assets/cognite_event.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cognite_file.py` & `pyatlan-2.2.1/pyatlan/model/assets/cognite_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cognite_sequence.py` & `pyatlan-2.2.1/pyatlan/model/assets/cognite_sequence.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cognite_time_series.py` & `pyatlan-2.2.1/pyatlan/model/assets/cognite_time_series.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/collection.py` & `pyatlan-2.2.1/pyatlan/model/assets/collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/column.py` & `pyatlan-2.2.1/pyatlan/model/assets/column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1357,31 +1357,28 @@
             cls, *, name: str, parent_qualified_name: str, parent_type: type, order: int
         ) -> Column.Attributes:
             validate_required_fields(
                 ["name", "parent_qualified_name", "parent_type", "order"],
                 [name, parent_qualified_name, parent_type, order],
             )
             fields = parent_qualified_name.split("/")
-            if len(fields) != 6:
-                raise ValueError("Invalid parent_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid parent_qualified_name") from e
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                parent_qualified_name, "parent_qualified_name", 6
+            )
             if order < 0:
                 raise ValueError("Order must be be a positive integer")
             ret_value = Column.Attributes(
                 name=name,
                 qualified_name=f"{parent_qualified_name}/{name}",
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 schema_name=fields[4],
                 schema_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}/{fields[4]}",
                 database_name=fields[3],
                 database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 order=order,
             )
             if parent_type == Table:
                 ret_value.table_qualified_name = parent_qualified_name
                 ret_value.table = Table.ref_by_qualified_name(parent_qualified_name)
                 ret_value.table_name = fields[5]
             elif parent_type == View:
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/column_process.py` & `pyatlan-2.2.1/pyatlan/model/assets/column_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/connection.py` & `pyatlan-2.2.1/pyatlan/model/assets/connection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b.py` & `pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b_collection.py` & `pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b_database.py` & `pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b_database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cube.py` & `pyatlan-2.2.1/pyatlan/model/assets/cube.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cube_dimension.py` & `pyatlan-2.2.1/pyatlan/model/assets/cube_dimension.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cube_field.py` & `pyatlan-2.2.1/pyatlan/model/assets/cube_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/cube_hierarchy.py` & `pyatlan-2.2.1/pyatlan/model/assets/cube_hierarchy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/data_contract.py` & `pyatlan-2.2.1/pyatlan/model/assets/data_contract.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/data_domain.py` & `pyatlan-2.2.1/pyatlan/model/assets/data_domain.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from typing import ClassVar, List, Optional
 from warnings import warn
 
 from pydantic.v1 import Field, StrictStr, validator
 
 from pyatlan.model.fields.atlan_fields import RelationField
-from pyatlan.utils import init_guid, to_camel_case, validate_required_fields
+from pyatlan.utils import init_guid, validate_required_fields
 
 from .asset import SelfAsset
 from .data_mesh import DataMesh
 
 
 class DataDomain(DataMesh):
     """Description"""
@@ -104,25 +104,30 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     DATA_PRODUCTS: ClassVar[RelationField] = RelationField("dataProducts")
     """
     TBC
     """
+    STAKEHOLDERS: ClassVar[RelationField] = RelationField("stakeholders")
+    """
+    TBC
+    """
     PARENT_DOMAIN: ClassVar[RelationField] = RelationField("parentDomain")
     """
     TBC
     """
     SUB_DOMAINS: ClassVar[RelationField] = RelationField("subDomains")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "data_products",
+        "stakeholders",
         "parent_domain",
         "sub_domains",
     ]
 
     @property
     def data_products(self) -> Optional[List[DataProduct]]:
         return None if self.attributes is None else self.attributes.data_products
@@ -130,14 +135,24 @@
     @data_products.setter
     def data_products(self, data_products: Optional[List[DataProduct]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_products = data_products
 
     @property
+    def stakeholders(self) -> Optional[List[Stakeholder]]:
+        return None if self.attributes is None else self.attributes.stakeholders
+
+    @stakeholders.setter
+    def stakeholders(self, stakeholders: Optional[List[Stakeholder]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.stakeholders = stakeholders
+
+    @property
     def parent_domain(self) -> Optional[DataDomain]:
         return None if self.attributes is None else self.attributes.parent_domain
 
     @parent_domain.setter
     def parent_domain(self, parent_domain: Optional[DataDomain]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -153,14 +168,17 @@
             self.attributes = self.Attributes()
         self.attributes.sub_domains = sub_domains
 
     class Attributes(DataMesh.Attributes):
         data_products: Optional[List[DataProduct]] = Field(
             default=None, description=""
         )  # relationship
+        stakeholders: Optional[List[Stakeholder]] = Field(
+            default=None, description=""
+        )  # relationship
         parent_domain: Optional[DataDomain] = Field(
             default=None, description=""
         )  # relationship
         sub_domains: Optional[List[DataDomain]] = Field(
             default=None, description=""
         )  # relationship
 
@@ -170,35 +188,38 @@
             cls,
             *,
             name: StrictStr,
             parent_domain_qualified_name: Optional[StrictStr] = None,
         ) -> DataDomain.Attributes:
             validate_required_fields(["name"], [name])
             parent_domain = None
-            mesh_name = to_camel_case(name)
-            qualified_name = f"default/domain/{mesh_name}"
+            super_domain_qualified_name = None
 
             # In case of sub-domain
             if parent_domain_qualified_name:
                 parent_domain = DataDomain.ref_by_qualified_name(
                     parent_domain_qualified_name
                 )
-                qualified_name = f"{parent_domain_qualified_name}/domain/{mesh_name}"
+                super_domain_qualified_name = DataMesh.get_super_domain_qualified_name(
+                    parent_domain_qualified_name
+                )
 
             return DataDomain.Attributes(
                 name=name,
-                qualified_name=qualified_name,
+                qualified_name=name,
                 parent_domain=parent_domain,
                 parent_domain_qualified_name=parent_domain_qualified_name,
+                super_domain_qualified_name=super_domain_qualified_name,
             )
 
     attributes: DataDomain.Attributes = Field(
         default_factory=lambda: DataDomain.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
         ),
     )
 
 
 from .data_product import DataProduct  # noqa
+from .stakeholder import Stakeholder  # noqa
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/data_mesh.py` & `pyatlan-2.2.1/pyatlan/model/assets/data_mesh.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,34 @@
 
 from .catalog import Catalog
 
 
 class DataMesh(Catalog):
     """Description"""
 
+    @staticmethod
+    def get_super_domain_qualified_name(domain_qualified_name: str):
+        """
+        Retrieve the domain's top-most ancestral domain qualified name.
+
+        :param domain_qualified_name: of the domain, from which to
+        retrieve the top-most ancestral domain qualified name
+        :returns qualified_name: of the top-most ancestral domain, or `None` if it can't be determined
+        """
+        import re
+
+        domain_qn_prefix = re.compile(r"(default/domain/[a-zA-Z0-9-]+/super)/.*")
+        if domain_qualified_name:
+            match = domain_qn_prefix.match(domain_qualified_name)
+            if match and match.group(1):
+                return match.group(1)
+            elif domain_qualified_name.startswith("default/domain/"):
+                return domain_qualified_name
+        return None
+
     type_name: str = Field(default="DataMesh", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataMesh":
             raise ValueError("must be DataMesh")
         return v
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/data_product.py` & `pyatlan-2.2.1/pyatlan/model/assets/data_product.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 
 
 from __future__ import annotations
 
 from datetime import datetime
-from typing import ClassVar, List, Optional
+from typing import ClassVar, List, Optional, Set
 from warnings import warn
 
 from pydantic.v1 import Field, StrictStr, validator
 
 from pyatlan.model.data_mesh import DataProductsAssetsDSL
 from pyatlan.model.enums import (
     DataProductCriticality,
     DataProductSensitivity,
     DataProductStatus,
     DataProductVisibility,
 )
 from pyatlan.model.fields.atlan_fields import KeywordField, NumericField, RelationField
 from pyatlan.model.search import IndexSearchRequest
-from pyatlan.utils import init_guid, to_camel_case, validate_required_fields
+from pyatlan.utils import init_guid, validate_required_fields
 
 from .asset import SelfAsset
 from .data_mesh import DataMesh
 
 
 class DataProduct(DataMesh):
     """Description"""
@@ -186,14 +186,26 @@
     """
     DATA_PRODUCT_SCORE_UPDATED_AT: ClassVar[NumericField] = NumericField(
         "dataProductScoreUpdatedAt", "dataProductScoreUpdatedAt"
     )
     """
     Timestamp when the score of this data product was last updated.
     """
+    DAAP_VISIBILITY_USERS: ClassVar[KeywordField] = KeywordField(
+        "daapVisibilityUsers", "daapVisibilityUsers"
+    )
+    """
+    list of users for product visibility control
+    """
+    DAAP_VISIBILITY_GROUPS: ClassVar[KeywordField] = KeywordField(
+        "daapVisibilityGroups", "daapVisibilityGroups"
+    )
+    """
+    list of groups for product visibility control
+    """
 
     DATA_DOMAIN: ClassVar[RelationField] = RelationField("dataDomain")
     """
     TBC
     """
     OUTPUT_PORTS: ClassVar[RelationField] = RelationField("outputPorts")
     """
@@ -213,14 +225,16 @@
         "daap_sensitivity",
         "data_product_visibility",
         "daap_visibility",
         "data_product_assets_d_s_l",
         "data_product_assets_playbook_filter",
         "data_product_score_value",
         "data_product_score_updated_at",
+        "daap_visibility_users",
+        "daap_visibility_groups",
         "data_domain",
         "output_ports",
         "input_ports",
     ]
 
     @property
     def data_product_status(self) -> Optional[DataProductStatus]:
@@ -377,14 +391,38 @@
         self, data_product_score_updated_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_product_score_updated_at = data_product_score_updated_at
 
     @property
+    def daap_visibility_users(self) -> Optional[Set[str]]:
+        return (
+            None if self.attributes is None else self.attributes.daap_visibility_users
+        )
+
+    @daap_visibility_users.setter
+    def daap_visibility_users(self, daap_visibility_users: Optional[Set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.daap_visibility_users = daap_visibility_users
+
+    @property
+    def daap_visibility_groups(self) -> Optional[Set[str]]:
+        return (
+            None if self.attributes is None else self.attributes.daap_visibility_groups
+        )
+
+    @daap_visibility_groups.setter
+    def daap_visibility_groups(self, daap_visibility_groups: Optional[Set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.daap_visibility_groups = daap_visibility_groups
+
+    @property
     def data_domain(self) -> Optional[DataDomain]:
         return None if self.attributes is None else self.attributes.data_domain
 
     @data_domain.setter
     def data_domain(self, data_domain: Optional[DataDomain]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -437,73 +475,55 @@
         data_product_assets_playbook_filter: Optional[str] = Field(
             default=None, description=""
         )
         data_product_score_value: Optional[float] = Field(default=None, description="")
         data_product_score_updated_at: Optional[datetime] = Field(
             default=None, description=""
         )
+        daap_visibility_users: Optional[Set[str]] = Field(default=None, description="")
+        daap_visibility_groups: Optional[Set[str]] = Field(default=None, description="")
         data_domain: Optional[DataDomain] = Field(
             default=None, description=""
         )  # relationship
         output_ports: Optional[List[Asset]] = Field(
             default=None, description=""
         )  # relationship
         input_ports: Optional[List[Asset]] = Field(
             default=None, description=""
         )  # relationship
 
-        @staticmethod
-        def get_super_domain_qualified_name(domain_qualified_name: str):
-            """
-            Retrieve the domain's top-most ancestral domain qualified name.
-
-            :param domain_qualified_name: of the domain, from which to
-            retrieve the top-most ancestral domain qualified name
-            :returns qualified_name: of the top-most ancestral domain, or `None` if it can't be determined
-            """
-            import re
-
-            domain_qn_prefix = re.compile(r"(default/domain/[a-zA-Z0-9-]+)/.*")
-            if domain_qualified_name:
-                match = domain_qn_prefix.match(domain_qualified_name)
-                if match and match.group(1):
-                    return match.group(1)
-                elif domain_qualified_name.startswith("default/domain/"):
-                    return domain_qualified_name
-            return None
-
         @classmethod
         @init_guid
         def create(
             cls,
             *,
             name: StrictStr,
             domain_qualified_name: StrictStr,
             asset_selection: IndexSearchRequest,
         ) -> DataProduct.Attributes:
             validate_required_fields(
                 ["name", "domain_qualified_name", "asset_selection"],
                 [name, domain_qualified_name, asset_selection],
             )
-            camel_case_name = to_camel_case(name)
             ASSETS_PLAYBOOK_FILTER = (
                 '{"condition":"AND","isGroupLocked":false,"rules":[]}'
             )
             return DataProduct.Attributes(
                 name=name,
                 data_product_assets_d_s_l=DataProductsAssetsDSL(
                     query=asset_selection
                 ).to_string(),
                 data_domain=DataDomain.ref_by_qualified_name(domain_qualified_name),
-                qualified_name=f"{domain_qualified_name}/product/{camel_case_name}",
+                qualified_name=f"{domain_qualified_name}/product/{name}",
                 data_product_assets_playbook_filter=ASSETS_PLAYBOOK_FILTER,
                 parent_domain_qualified_name=domain_qualified_name,
-                super_domain_qualified_name=cls.get_super_domain_qualified_name(
+                super_domain_qualified_name=DataMesh.get_super_domain_qualified_name(
                     domain_qualified_name
                 ),
+                daap_status=DataProductStatus.ACTIVE,
             )
 
     attributes: DataProduct.Attributes = Field(
         default_factory=lambda: DataProduct.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/data_quality.py` & `pyatlan-2.2.1/pyatlan/model/assets/data_quality.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/data_set.py` & `pyatlan-2.2.1/pyatlan/model/assets/data_set.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/data_studio.py` & `pyatlan-2.2.1/pyatlan/model/assets/data_studio.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/data_studio_asset.py` & `pyatlan-2.2.1/pyatlan/model/assets/data_studio_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,30 +342,21 @@
             data_studio_asset_type: GoogleDatastudioAssetType,
             gdsid: str,
         ) -> DataStudioAsset.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name", "data_studio_asset_type"],
                 [name, connection_qualified_name, data_studio_asset_type],
             )
-
-            # Split the connection_qualified_name to extract necessary information
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-
             return DataStudioAsset.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{gdsid}",
                 connection_qualified_name=connection_qualified_name,
-                connector_name=connector_type.value,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
                 data_studio_asset_type=data_studio_asset_type,
             )
 
     attributes: DataStudioAsset.Attributes = Field(
         default_factory=lambda: DataStudioAsset.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/database.py` & `pyatlan-2.2.1/pyatlan/model/assets/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,21 @@
 
     @classmethod
     @init_guid
     def creator(cls, *, name: str, connection_qualified_name: str) -> Database:
         validate_required_fields(
             ["name", "connection_qualified_name"], [name, connection_qualified_name]
         )
-        fields = connection_qualified_name.split("/")
-        if len(fields) != 3:
-            raise ValueError("Invalid connection_qualified_name")
-        try:
-            connector_type = AtlanConnectorType(fields[1])  # type:ignore
-        except ValueError as e:
-            raise ValueError("Invalid connection_qualified_name") from e
         attributes = Database.Attributes(
             name=name,
             connection_qualified_name=connection_qualified_name,
             qualified_name=f"{connection_qualified_name}/{name}",
-            connector_name=connector_type.value,
+            connector_name=AtlanConnectorType.get_connector_name(
+                connection_qualified_name
+            ),
         )
         return cls(attributes=attributes)
 
     @classmethod
     @init_guid
     def create(cls, *, name: str, connection_qualified_name: str) -> Database:
         warn(
@@ -113,26 +108,21 @@
         @init_guid
         def create(
             cls, name: str, connection_qualified_name: str
         ) -> Database.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name"], [name, connection_qualified_name]
             )
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
             return Database.Attributes(
                 name=name,
                 connection_qualified_name=connection_qualified_name,
                 qualified_name=f"{connection_qualified_name}/{name}",
-                connector_name=connector_type.value,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
             )
 
     attributes: Database.Attributes = Field(
         default_factory=lambda: Database.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt_column_process.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt_column_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt_metric.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt_model.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt_model_column.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt_model_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt_process.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt_source.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt_source.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt_tag.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt_tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dbt_test.py` & `pyatlan-2.2.1/pyatlan/model/assets/dbt_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/domo.py` & `pyatlan-2.2.1/pyatlan/model/assets/domo.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/domo_card.py` & `pyatlan-2.2.1/pyatlan/model/assets/domo_card.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/domo_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/domo_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/domo_dataset.py` & `pyatlan-2.2.1/pyatlan/model/assets/domo_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/domo_dataset_column.py` & `pyatlan-2.2.1/pyatlan/model/assets/domo_dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b.py` & `pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py` & `pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py` & `pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_secondary_index.py` & `pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/dynamo_dbtable.py` & `pyatlan-2.2.1/pyatlan/model/assets/dynamo_dbtable.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/event_store.py` & `pyatlan-2.2.1/pyatlan/model/assets/event_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/file.py` & `pyatlan-2.2.1/pyatlan/model/assets/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 from typing import ClassVar, List, Optional
 from warnings import warn
 
 from pydantic.v1 import Field, validator
 
-from pyatlan.model.enums import FileType
+from pyatlan.model.enums import AtlanConnectorType, FileType
 from pyatlan.model.fields.atlan_fields import KeywordField, RelationField
 from pyatlan.utils import init_guid, validate_required_fields
 
 from .resource import Resource
 
 
 class File(Resource):
@@ -130,14 +130,17 @@
                 ["name", "connection_qualified_name", "file_type"],
                 [name, connection_qualified_name, file_type],
             )
             return File.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
                 file_type=file_type,
             )
 
     attributes: File.Attributes = Field(
         default_factory=lambda: File.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/folder.py` & `pyatlan-2.2.1/pyatlan/model/assets/folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/function.py` & `pyatlan-2.2.1/pyatlan/model/assets/function.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/g_c_s.py` & `pyatlan-2.2.1/pyatlan/model/assets/g_c_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/g_c_s_bucket.py` & `pyatlan-2.2.1/pyatlan/model/assets/g_c_s_bucket.py`

 * *Files 7% similar despite different names*

```diff
@@ -255,30 +255,21 @@
         @init_guid
         def create(
             cls, *, name: str, connection_qualified_name: str
         ) -> GCSBucket.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name"], [name, connection_qualified_name]
             )
-
-            # Split the connection_qualified_name to extract necessary information
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-
             return GCSBucket.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
-                connector_name=connector_type.value,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
             )
 
     attributes: GCSBucket.Attributes = Field(
         default_factory=lambda: GCSBucket.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/g_c_s_object.py` & `pyatlan-2.2.1/pyatlan/model/assets/g_c_s_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,31 +417,23 @@
         @init_guid
         def create(
             cls, *, name: str, gcs_bucket_qualified_name: str
         ) -> GCSObject.Attributes:
             validate_required_fields(
                 ["name", "gcs_bucket_qualified_name"], [name, gcs_bucket_qualified_name]
             )
-
-            # Split the gcs_bucket_qualified_name to extract necessary information
-            fields = gcs_bucket_qualified_name.split("/")
-            if len(fields) != 4:
-                raise ValueError("Invalid gcs_bucket_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid gcs_bucket_qualified_name") from e
-
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                gcs_bucket_qualified_name, "gcs_bucket_qualified_name", 4
+            )
             return GCSObject.Attributes(
                 name=name,
                 gcs_bucket_qualified_name=gcs_bucket_qualified_name,
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 qualified_name=f"{gcs_bucket_qualified_name}/{name}",
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 gcs_bucket=GCSBucket.ref_by_qualified_name(gcs_bucket_qualified_name),
             )
 
     attributes: GCSObject.Attributes = Field(
         default_factory=lambda: GCSObject.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/google.py` & `pyatlan-2.2.1/pyatlan/model/assets/google.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/infrastructure.py` & `pyatlan-2.2.1/pyatlan/model/assets/infrastructure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/insight.py` & `pyatlan-2.2.1/pyatlan/model/assets/insight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/kafka.py` & `pyatlan-2.2.1/pyatlan/model/assets/kafka.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/kafka_consumer_group.py` & `pyatlan-2.2.1/pyatlan/model/assets/kafka_consumer_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/kafka_topic.py` & `pyatlan-2.2.1/pyatlan/model/assets/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/link.py` & `pyatlan-2.2.1/pyatlan/model/assets/link.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_explore.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_explore.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_field.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_folder.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_look.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_look.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_model.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_project.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_query.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_tile.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_tile.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/looker_view.py` & `pyatlan-2.2.1/pyatlan/model/assets/looker_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/m_c_incident.py` & `pyatlan-2.2.1/pyatlan/model/assets/m_c_incident.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/m_c_monitor.py` & `pyatlan-2.2.1/pyatlan/model/assets/m_c_monitor.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/materialised_view.py` & `pyatlan-2.2.1/pyatlan/model/assets/materialised_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,29 +312,26 @@
         def create(
             cls, *, name: str, schema_qualified_name: str
         ) -> MaterialisedView.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
             fields = schema_qualified_name.split("/")
-            if len(fields) != 5:
-                raise ValueError("Invalid schema_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid schema_qualified_name") from e
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                schema_qualified_name, "schema_qualified_name", 5
+            )
             return MaterialisedView.Attributes(
                 name=name,
                 database_name=fields[3],
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
                 qualified_name=f"{schema_qualified_name}/{name}",
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
     attributes: MaterialisedView.Attributes = Field(
         default_factory=lambda: MaterialisedView.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/matillion.py` & `pyatlan-2.2.1/pyatlan/model/assets/matillion.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/matillion_component.py` & `pyatlan-2.2.1/pyatlan/model/assets/matillion_component.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/matillion_group.py` & `pyatlan-2.2.1/pyatlan/model/assets/matillion_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/matillion_job.py` & `pyatlan-2.2.1/pyatlan/model/assets/matillion_job.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/matillion_project.py` & `pyatlan-2.2.1/pyatlan/model/assets/matillion_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/metabase.py` & `pyatlan-2.2.1/pyatlan/model/assets/metabase.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/metabase_collection.py` & `pyatlan-2.2.1/pyatlan/model/assets/metabase_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/metabase_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/metabase_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/metabase_question.py` & `pyatlan-2.2.1/pyatlan/model/assets/metabase_question.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/metric.py` & `pyatlan-2.2.1/pyatlan/model/assets/metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_attribute.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_attribute.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_cube.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_cube.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_document.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_document.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_dossier.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_dossier.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_fact.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_fact.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_metric.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_project.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_report.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_visualization.py` & `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_visualization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mode.py` & `pyatlan-2.2.1/pyatlan/model/assets/mode.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mode_chart.py` & `pyatlan-2.2.1/pyatlan/model/assets/mode_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mode_collection.py` & `pyatlan-2.2.1/pyatlan/model/assets/mode_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mode_query.py` & `pyatlan-2.2.1/pyatlan/model/assets/mode_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mode_report.py` & `pyatlan-2.2.1/pyatlan/model/assets/mode_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mode_workspace.py` & `pyatlan-2.2.1/pyatlan/model/assets/mode_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b.py` & `pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b_collection.py` & `pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b_database.py` & `pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b_database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/monte_carlo.py` & `pyatlan-2.2.1/pyatlan/model/assets/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/multi_dimensional_dataset.py` & `pyatlan-2.2.1/pyatlan/model/assets/multi_dimensional_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/namespace.py` & `pyatlan-2.2.1/pyatlan/model/assets/namespace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/no_s_q_l.py` & `pyatlan-2.2.1/pyatlan/model/assets/no_s_q_l.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/object_store.py` & `pyatlan-2.2.1/pyatlan/model/assets/object_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/persona.py` & `pyatlan-2.2.1/pyatlan/model/assets/persona.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_column.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dataflow.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dataflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dataset.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_datasource.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_measure.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_measure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_page.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_page.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_report.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_table.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_tile.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_tile.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_workspace.py` & `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/preset.py` & `pyatlan-2.2.1/pyatlan/model/assets/preset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/preset_chart.py` & `pyatlan-2.2.1/pyatlan/model/assets/preset_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,31 +139,23 @@
         def create(
             cls, *, name: str, preset_dashboard_qualified_name: str
         ) -> PresetChart.Attributes:
             validate_required_fields(
                 ["name", "preset_dashboard_qualified_name"],
                 [name, preset_dashboard_qualified_name],
             )
-
-            # Split the preset_dashboard_qualified_name to extract necessary information
-            fields = preset_dashboard_qualified_name.split("/")
-            if len(fields) != 5:
-                raise ValueError("Invalid preset_dashboard_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid preset_dashboard_qualified_name") from e
-
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                preset_dashboard_qualified_name, "preset_dashboard_qualified_name", 5
+            )
             return PresetChart.Attributes(
                 name=name,
                 preset_dashboard_qualified_name=preset_dashboard_qualified_name,
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 qualified_name=f"{preset_dashboard_qualified_name}/{name}",
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 preset_dashboard=PresetDashboard.ref_by_qualified_name(
                     preset_dashboard_qualified_name
                 ),
             )
 
     attributes: PresetChart.Attributes = Field(
         default_factory=lambda: PresetChart.Attributes(),
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/preset_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/preset_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,31 +300,23 @@
         def create(
             cls, *, name: str, preset_workspace_qualified_name: str
         ) -> PresetDashboard.Attributes:
             validate_required_fields(
                 ["name", "preset_workspace_qualified_name"],
                 [name, preset_workspace_qualified_name],
             )
-
-            # Split the preset_workspace_qualified_name to extract necessary information
-            fields = preset_workspace_qualified_name.split("/")
-            if len(fields) != 4:
-                raise ValueError("Invalid preset_workspace_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid preset_workspace_qualified_name") from e
-
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                preset_workspace_qualified_name, "preset_workspace_qualified_name", 4
+            )
             return PresetDashboard.Attributes(
                 name=name,
                 preset_workspace_qualified_name=preset_workspace_qualified_name,
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 qualified_name=f"{preset_workspace_qualified_name}/{name}",
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 preset_workspace=PresetWorkspace.ref_by_qualified_name(
                     preset_workspace_qualified_name
                 ),
             )
 
     attributes: PresetDashboard.Attributes = Field(
         default_factory=lambda: PresetDashboard.Attributes(),
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/preset_dataset.py` & `pyatlan-2.2.1/pyatlan/model/assets/preset_dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -165,31 +165,23 @@
         def create(
             cls, *, name: str, preset_dashboard_qualified_name: str
         ) -> PresetDataset.Attributes:
             validate_required_fields(
                 ["name", "preset_dashboard_qualified_name"],
                 [name, preset_dashboard_qualified_name],
             )
-
-            # Split the preset_dashboard_qualified_name to extract necessary information
-            fields = preset_dashboard_qualified_name.split("/")
-            if len(fields) != 5:
-                raise ValueError("Invalid preset_dashboard_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid preset_dashboard_qualified_name") from e
-
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                preset_dashboard_qualified_name, "preset_dashboard_qualified_name", 5
+            )
             return PresetDataset.Attributes(
                 name=name,
                 preset_dashboard_qualified_name=preset_dashboard_qualified_name,
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 qualified_name=f"{preset_dashboard_qualified_name}/{name}",
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 preset_dashboard=PresetDashboard.ref_by_qualified_name(
                     preset_dashboard_qualified_name
                 ),
             )
 
     attributes: PresetDataset.Attributes = Field(
         default_factory=lambda: PresetDataset.Attributes(),
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/preset_workspace.py` & `pyatlan-2.2.1/pyatlan/model/assets/preset_workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,30 +316,21 @@
         @init_guid
         def create(
             cls, *, name: str, connection_qualified_name: str
         ) -> PresetWorkspace.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name"], [name, connection_qualified_name]
             )
-
-            # Split the connection_qualified_name to extract necessary information
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-
             return PresetWorkspace.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
-                connector_name=connector_type.value,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
             )
 
     attributes: PresetWorkspace.Attributes = Field(
         default_factory=lambda: PresetWorkspace.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/procedure.py` & `pyatlan-2.2.1/pyatlan/model/assets/procedure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/process.py` & `pyatlan-2.2.1/pyatlan/model/assets/process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/process_execution.py` & `pyatlan-2.2.1/pyatlan/model/assets/process_execution.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/purpose.py` & `pyatlan-2.2.1/pyatlan/model/assets/purpose.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/qlik.py` & `pyatlan-2.2.1/pyatlan/model/assets/qlik.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/qlik_app.py` & `pyatlan-2.2.1/pyatlan/model/assets/qlik_app.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/qlik_chart.py` & `pyatlan-2.2.1/pyatlan/model/assets/qlik_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/qlik_dataset.py` & `pyatlan-2.2.1/pyatlan/model/assets/qlik_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/qlik_sheet.py` & `pyatlan-2.2.1/pyatlan/model/assets/qlik_sheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/qlik_space.py` & `pyatlan-2.2.1/pyatlan/model/assets/qlik_space.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/qlik_stream.py` & `pyatlan-2.2.1/pyatlan/model/assets/qlik_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/query.py` & `pyatlan-2.2.1/pyatlan/model/assets/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/quick_sight.py` & `pyatlan-2.2.1/pyatlan/model/assets/quick_sight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_analysis.py` & `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_analysis.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_analysis_visual.py` & `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_analysis_visual.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dashboard_visual.py` & `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dashboard_visual.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dataset.py` & `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dataset_field.py` & `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dataset_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_folder.py` & `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/readme.py` & `pyatlan-2.2.1/pyatlan/model/assets/readme.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/readme_template.py` & `pyatlan-2.2.1/pyatlan/model/assets/readme_template.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/redash.py` & `pyatlan-2.2.1/pyatlan/model/assets/redash.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/redash_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/redash_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/redash_query.py` & `pyatlan-2.2.1/pyatlan/model/assets/redash_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/redash_visualization.py` & `pyatlan-2.2.1/pyatlan/model/assets/redash_visualization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/referenceable.py` & `pyatlan-2.2.1/pyatlan/model/assets/referenceable.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/resource.py` & `pyatlan-2.2.1/pyatlan/model/assets/resource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/s3.py` & `pyatlan-2.2.1/pyatlan/model/assets/s3.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/s3_bucket.py` & `pyatlan-2.2.1/pyatlan/model/assets/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/s3_object.py` & `pyatlan-2.2.1/pyatlan/model/assets/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/s_q_l.py` & `pyatlan-2.2.1/pyatlan/model/assets/s_q_l.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/saa_s.py` & `pyatlan-2.2.1/pyatlan/model/assets/saa_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/salesforce.py` & `pyatlan-2.2.1/pyatlan/model/assets/salesforce.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/salesforce_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/salesforce_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/salesforce_field.py` & `pyatlan-2.2.1/pyatlan/model/assets/salesforce_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/salesforce_object.py` & `pyatlan-2.2.1/pyatlan/model/assets/salesforce_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/salesforce_organization.py` & `pyatlan-2.2.1/pyatlan/model/assets/salesforce_organization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/salesforce_report.py` & `pyatlan-2.2.1/pyatlan/model/assets/salesforce_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/schema.py` & `pyatlan-2.2.1/pyatlan/model/assets/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,27 +335,24 @@
         ) -> Schema.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(
                 ["database_qualified_name"], [database_qualified_name]
             )
             fields = database_qualified_name.split("/")
-            if len(fields) != 4:
-                raise ValueError("Invalid database_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid database_qualified_name") from e
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                database_qualified_name, "database_qualified_name", 4
+            )
             return Schema.Attributes(
                 name=name,
                 database_name=fields[3],
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 database_qualified_name=database_qualified_name,
                 qualified_name=f"{database_qualified_name}/{name}",
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 database=Database.ref_by_qualified_name(database_qualified_name),
             )
 
     attributes: Schema.Attributes = Field(
         default_factory=lambda: Schema.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/schema_registry.py` & `pyatlan-2.2.1/pyatlan/model/assets/schema_registry.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/schema_registry_subject.py` & `pyatlan-2.2.1/pyatlan/model/assets/schema_registry_subject.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sigma.py` & `pyatlan-2.2.1/pyatlan/model/assets/sigma.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sigma_data_element.py` & `pyatlan-2.2.1/pyatlan/model/assets/sigma_data_element.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sigma_data_element_field.py` & `pyatlan-2.2.1/pyatlan/model/assets/sigma_data_element_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sigma_dataset.py` & `pyatlan-2.2.1/pyatlan/model/assets/sigma_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sigma_dataset_column.py` & `pyatlan-2.2.1/pyatlan/model/assets/sigma_dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sigma_page.py` & `pyatlan-2.2.1/pyatlan/model/assets/sigma_page.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sigma_workbook.py` & `pyatlan-2.2.1/pyatlan/model/assets/sigma_workbook.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sisense.py` & `pyatlan-2.2.1/pyatlan/model/assets/sisense.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sisense_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/sisense_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sisense_datamodel.py` & `pyatlan-2.2.1/pyatlan/model/assets/sisense_datamodel.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sisense_datamodel_table.py` & `pyatlan-2.2.1/pyatlan/model/assets/sisense_datamodel_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sisense_folder.py` & `pyatlan-2.2.1/pyatlan/model/assets/sisense_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/sisense_widget.py` & `pyatlan-2.2.1/pyatlan/model/assets/sisense_widget.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/snowflake_dynamic_table.py` & `pyatlan-2.2.1/pyatlan/model/assets/snowflake_dynamic_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/snowflake_pipe.py` & `pyatlan-2.2.1/pyatlan/model/assets/snowflake_pipe.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/snowflake_stream.py` & `pyatlan-2.2.1/pyatlan/model/assets/snowflake_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/snowflake_tag.py` & `pyatlan-2.2.1/pyatlan/model/assets/snowflake_tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/soda.py` & `pyatlan-2.2.1/pyatlan/model/assets/soda.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/soda_check.py` & `pyatlan-2.2.1/pyatlan/model/assets/soda_check.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/spark.py` & `pyatlan-2.2.1/pyatlan/model/assets/spark.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/spark_job.py` & `pyatlan-2.2.1/pyatlan/model/assets/spark_job.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/table.py` & `pyatlan-2.2.1/pyatlan/model/assets/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,29 +450,26 @@
         @classmethod
         @init_guid
         def create(cls, *, name: str, schema_qualified_name: str) -> Table.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
             fields = schema_qualified_name.split("/")
-            if len(fields) != 5:
-                raise ValueError("Invalid schema_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid schema_qualified_name") from e
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                schema_qualified_name, "schema_qualified_name", 5
+            )
             return Table.Attributes(
                 name=name,
                 database_name=fields[3],
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
                 qualified_name=f"{schema_qualified_name}/{name}",
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
     attributes: Table.Attributes = Field(
         default_factory=lambda: Table.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/table_partition.py` & `pyatlan-2.2.1/pyatlan/model/assets/table_partition.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_calculated_field.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_calculated_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_dashboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_datasource.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_datasource_field.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_datasource_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_flow.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_flow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_metric.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_project.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_site.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_site.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_workbook.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_workbook.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tableau_worksheet.py` & `pyatlan-2.2.1/pyatlan/model/assets/tableau_worksheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tag.py` & `pyatlan-2.2.1/pyatlan/model/assets/tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/tag_attachment.py` & `pyatlan-2.2.1/pyatlan/model/assets/tag_attachment.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot.py` & `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_answer.py` & `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_answer.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_column.py` & `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_dashlet.py` & `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_dashlet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_liveboard.py` & `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_liveboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_table.py` & `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_view.py` & `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_worksheet.py` & `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_worksheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/assets/view.py` & `pyatlan-2.2.1/pyatlan/model/assets/view.py`

 * *Files 5% similar despite different names*

```diff
@@ -262,29 +262,26 @@
         @classmethod
         @init_guid
         def create(cls, *, name: str, schema_qualified_name: str) -> View.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
             fields = schema_qualified_name.split("/")
-            if len(fields) != 5:
-                raise ValueError("Invalid schema_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid schema_qualified_name") from e
+            connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                schema_qualified_name, "schema_qualified_name", 5
+            )
             return View.Attributes(
                 name=name,
                 database_name=fields[3],
-                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                connection_qualified_name=connection_qn,
                 database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
                 qualified_name=f"{schema_qualified_name}/{name}",
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
-                connector_name=connector_type.value,
+                connector_name=connector_name,
                 atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
     attributes: View.Attributes = Field(
         default_factory=lambda: View.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.2.0/pyatlan/model/atlan_image.py` & `pyatlan-2.2.1/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/audit.py` & `pyatlan-2.2.1/pyatlan/model/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/core.py` & `pyatlan-2.2.1/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/credential.py` & `pyatlan-2.2.1/pyatlan/model/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/custom_metadata.py` & `pyatlan-2.2.1/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/data_mesh.py` & `pyatlan-2.2.1/pyatlan/model/data_mesh.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/enums.py` & `pyatlan-2.2.1/pyatlan/model/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,44 @@
         obj._value_ = value
         obj.category = category
         return obj
 
     def to_qualified_name(self):
         return f"default/{self.value}/{int(utils.get_epoch_timestamp())}"
 
+    def get_connector_name(
+        qualified_name: str,
+        attribute_name: str = "connection_qualified_name",
+        qualified_name_len: int = 3,
+    ):
+        """
+        Extracts and returns the connector name from a given qualified name.
+
+        :param qualified_name: qualified name to extract the connector name from.
+        :param attribute_name: name of the attribute. Defaults to `connection_qualified_name`.
+        :param qualified_name_len: expected length of the split qualified name. Defaults to `3`.
+        :raises: `ValueError` if the qualified name is invalid or the connector type is not recognized.
+        :returns: connector name extracted from the qualified name
+        or tuple(connector qualified name, connector name).
+        """
+        err = f"Invalid {attribute_name}"
+        # Split the qualified name
+        # to extract necessary information
+        fields = qualified_name.split("/")
+        if len(fields) != qualified_name_len:
+            raise ValueError(err)
+        try:
+            connector_name = AtlanConnectorType(fields[1]).value  # type:ignore
+            if attribute_name != "connection_qualified_name":
+                connection_qn = f"{fields[0]}/{fields[1]}/{fields[2]}"
+                return connection_qn, connector_name
+            return connector_name
+        except ValueError as e:
+            raise ValueError(err) from e
+
     SNOWFLAKE = ("snowflake", AtlanConnectionCategory.WAREHOUSE)
     TABLEAU = ("tableau", AtlanConnectionCategory.BI)
     REDSHIFT = ("redshift", AtlanConnectionCategory.WAREHOUSE)
     POSTGRES = ("postgres", AtlanConnectionCategory.DATABASE)
     ATHENA = ("athena", AtlanConnectionCategory.QUERY_ENGINE)
     DATABRICKS = ("databricks", AtlanConnectionCategory.LAKE)
     POWERBI = ("powerbi", AtlanConnectionCategory.BI)
```

### Comparing `pyatlan-2.2.0/pyatlan/model/events.py` & `pyatlan-2.2.1/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/fields/atlan_fields.py` & `pyatlan-2.2.1/pyatlan/model/fields/atlan_fields.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/fluent_search.py` & `pyatlan-2.2.1/pyatlan/model/fluent_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/fluent_tasks.py` & `pyatlan-2.2.1/pyatlan/model/fluent_tasks.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/group.py` & `pyatlan-2.2.1/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/keycloak_events.py` & `pyatlan-2.2.1/pyatlan/model/keycloak_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/lineage.py` & `pyatlan-2.2.1/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/__init__.py` & `pyatlan-2.2.1/pyatlan/model/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/base/crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/base/crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/base/miner.py` & `pyatlan-2.2.1/pyatlan/model/packages/base/miner.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/base/package.py` & `pyatlan-2.2.1/pyatlan/model/packages/base/package.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/big_query_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/big_query_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/confluent_kafka_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/confluent_kafka_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/dbt_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/dbt_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/dynamo_d_b_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/dynamo_d_b_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/glue_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/postgres_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/postgres_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/powerbi_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/powerbi_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/s_q_l_server_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/s_q_l_server_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/sigma_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/sigma_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/snowflake_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/snowflake_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/snowflake_miner.py` & `pyatlan-2.2.1/pyatlan/model/packages/snowflake_miner.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/sql_server_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/sql_server_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/packages/tableau_crawler.py` & `pyatlan-2.2.1/pyatlan/model/packages/tableau_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/query.py` & `pyatlan-2.2.1/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/response.py` & `pyatlan-2.2.1/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/role.py` & `pyatlan-2.2.1/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/search.py` & `pyatlan-2.2.1/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/search_log.py` & `pyatlan-2.2.1/pyatlan/model/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/sso.py` & `pyatlan-2.2.1/pyatlan/model/sso.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/structs.py` & `pyatlan-2.2.1/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/task.py` & `pyatlan-2.2.1/pyatlan/model/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/typedef.py` & `pyatlan-2.2.1/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/user.py` & `pyatlan-2.2.1/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/utils.py` & `pyatlan-2.2.1/pyatlan/model/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/model/workflow.py` & `pyatlan-2.2.1/pyatlan/model/workflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/multipart_data_generator.py` & `pyatlan-2.2.1/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/pkg/create_package_files.py` & `pyatlan-2.2.1/pyatlan/pkg/create_package_files.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/pkg/models.py` & `pyatlan-2.2.1/pyatlan/pkg/models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/pkg/templates/default_configmap.jinja2` & `pyatlan-2.2.1/pyatlan/pkg/templates/default_configmap.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/pkg/templates/default_template.jinja2` & `pyatlan-2.2.1/pyatlan/pkg/templates/default_template.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/pkg/templates/package_config.jinja2` & `pyatlan-2.2.1/pyatlan/pkg/templates/package_config.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/pkg/ui.py` & `pyatlan-2.2.1/pyatlan/pkg/ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/pkg/utils.py` & `pyatlan-2.2.1/pyatlan/pkg/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/pkg/widgets.py` & `pyatlan-2.2.1/pyatlan/pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan/utils.py` & `pyatlan-2.2.1/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/pyatlan.egg-info/PKG-INFO` & `pyatlan-2.2.1/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.2.0
+Version: 2.2.1
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyatlan-2.2.0/pyatlan.egg-info/SOURCES.txt` & `pyatlan-2.2.1/pyatlan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -127,14 +127,23 @@
 pyatlan/model/assets/cognite.py
 pyatlan/model/assets/cognite3_d_model.py
 pyatlan/model/assets/cognite_asset.py
 pyatlan/model/assets/cognite_event.py
 pyatlan/model/assets/cognite_file.py
 pyatlan/model/assets/cognite_sequence.py
 pyatlan/model/assets/cognite_time_series.py
+pyatlan/model/assets/cognos.py
+pyatlan/model/assets/cognos_dashboard.py
+pyatlan/model/assets/cognos_datasource.py
+pyatlan/model/assets/cognos_exploration.py
+pyatlan/model/assets/cognos_file.py
+pyatlan/model/assets/cognos_folder.py
+pyatlan/model/assets/cognos_module.py
+pyatlan/model/assets/cognos_package.py
+pyatlan/model/assets/cognos_report.py
 pyatlan/model/assets/collection.py
 pyatlan/model/assets/column.py
 pyatlan/model/assets/column_process.py
 pyatlan/model/assets/connection.py
 pyatlan/model/assets/cosmos_mongo_d_b.py
 pyatlan/model/assets/cosmos_mongo_d_b_collection.py
 pyatlan/model/assets/cosmos_mongo_d_b_database.py
@@ -309,14 +318,16 @@
 pyatlan/model/assets/snowflake_pipe.py
 pyatlan/model/assets/snowflake_stream.py
 pyatlan/model/assets/snowflake_tag.py
 pyatlan/model/assets/soda.py
 pyatlan/model/assets/soda_check.py
 pyatlan/model/assets/spark.py
 pyatlan/model/assets/spark_job.py
+pyatlan/model/assets/stakeholder.py
+pyatlan/model/assets/stakeholder_title.py
 pyatlan/model/assets/table.py
 pyatlan/model/assets/table_partition.py
 pyatlan/model/assets/tableau.py
 pyatlan/model/assets/tableau_calculated_field.py
 pyatlan/model/assets/tableau_dashboard.py
 pyatlan/model/assets/tableau_datasource.py
 pyatlan/model/assets/tableau_datasource_field.py
```

### Comparing `pyatlan-2.2.0/setup.py` & `pyatlan-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/adls_asset_test.py` & `pyatlan-2.2.1/tests/integration/adls_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/admin_test.py` & `pyatlan-2.2.1/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/airflow_asset_test.py` & `pyatlan-2.2.1/tests/integration/airflow_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/api_asset_test.py` & `pyatlan-2.2.1/tests/integration/api_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/atlan_tag_test.py` & `pyatlan-2.2.1/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/client.py` & `pyatlan-2.2.1/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/connection_test.py` & `pyatlan-2.2.1/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/custom_metadata_test.py` & `pyatlan-2.2.1/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/custom_package_test.py` & `pyatlan-2.2.1/tests/integration/custom_package_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/data_mesh_test.py` & `pyatlan-2.2.1/tests/integration/data_mesh_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,54 @@
+import re
 from typing import Generator
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AtlasGlossaryTerm, DataDomain, DataProduct
 from pyatlan.model.core import Announcement
-from pyatlan.model.enums import AnnouncementType, CertificateStatus, EntityStatus
+from pyatlan.model.enums import (
+    AnnouncementType,
+    CertificateStatus,
+    DataProductStatus,
+    EntityStatus,
+)
 from pyatlan.model.fluent_search import CompoundQuery, FluentSearch
 from pyatlan.model.response import AssetMutationResponse
-from pyatlan.utils import to_camel_case
 from tests.integration.client import TestId, delete_asset
 from tests.integration.utils import block
 
 DATA_PRODUCT_ASSETS_PLAYBOOK_FILTER = (
     '{"condition":"AND","isGroupLocked":false,"rules":[]}'
 )
 
 MODULE_NAME = TestId.make_unique("DM")
 
 DATA_DOMAIN_NAME = f"{MODULE_NAME}-data-domain"
-DATA_DOMAIN_MESH_SLUG = to_camel_case(DATA_DOMAIN_NAME)
-DATA_DOMAIN_QUALIFIED_NAME = f"default/domain/{DATA_DOMAIN_MESH_SLUG}"
+DATA_DOMAIN_QUALIFIED_NAME = f"default/domain/{DATA_DOMAIN_NAME}/super"
+DATA_DOMAIN_QN_REGEX = r"default/domain/[a-zA-Z0-9-]+/super"
 DATA_SUB_DOMAIN_NAME = f"{MODULE_NAME}-data-sub-domain"
-DATA_SUB_DOMAIN_MESH_SLUG = to_camel_case(DATA_SUB_DOMAIN_NAME)
 DATA_SUB_DOMAIN_QUALIFIED_NAME = (
-    f"{DATA_DOMAIN_QUALIFIED_NAME}/domain/{DATA_SUB_DOMAIN_MESH_SLUG}"
+    f"{DATA_DOMAIN_QUALIFIED_NAME}/domain/{DATA_SUB_DOMAIN_NAME}"
 )
+DATA_SUB_DOMAIN_QN_REGEX = r"default/domain/[a-zA-Z0-9-]+/super/domain/[a-zA-Z0-9-]+"
 DATA_PRODUCT_NAME = f"{MODULE_NAME}-data-product"
-DATA_PRODUCT_MESH_SLUG = to_camel_case(DATA_PRODUCT_NAME)
 DATA_PRODUCT_QUALIFIED_NAME = (
-    f"{DATA_DOMAIN_QUALIFIED_NAME}/product/{DATA_PRODUCT_MESH_SLUG}"
+    f"{DATA_DOMAIN_QUALIFIED_NAME}/product/{DATA_PRODUCT_NAME}"
 )
+DATA_PRODUCT_QN_REGEX = r"default/domain/[a-zA-Z0-9-]+/super/product/[a-zA-Z0-9-]+"
 
 CERTIFICATE_STATUS = CertificateStatus.VERIFIED
 CERTIFICATE_MESSAGE = "Automated testing of the Python SDK."
 ANNOUNCEMENT_TYPE = AnnouncementType.INFORMATION
 ANNOUNCEMENT_TITLE = "Python SDK testing."
 ANNOUNCEMENT_MESSAGE = "Automated testing of the Python SDK."
 
 response = block(AtlanClient(), AssetMutationResponse())
 
-pytestmark = pytest.mark.skip(
-    "Reset broke data mesh stuff. Some bootstrap policies need to be reset"
-)
-
 
 @pytest.fixture(scope="module")
 def domain(client: AtlanClient) -> Generator[DataDomain, None, None]:
     to_create = DataDomain.create(name=DATA_DOMAIN_NAME)
     response = client.asset.save(to_create)
     result = response.assets_created(asset_type=DataDomain)[0]
     yield result
@@ -55,39 +56,45 @@
 
 
 def test_data_domain(client: AtlanClient, domain: DataDomain):
     assert domain
     assert domain.guid
     assert domain.qualified_name
     assert domain.name == DATA_DOMAIN_NAME
-    assert domain.qualified_name == DATA_DOMAIN_QUALIFIED_NAME
+    assert re.search(DATA_DOMAIN_QN_REGEX, domain.qualified_name)
+    assert domain.parent_domain_qualified_name is None
+    assert domain.super_domain_qualified_name is None
 
 
 @pytest.fixture(scope="module")
 def sub_domain(
     client: AtlanClient,
     domain: DataDomain,
 ) -> Generator[DataDomain, None, None]:
     assert domain.guid
     to_create = DataDomain.create(
         name=DATA_SUB_DOMAIN_NAME,
-        parent_domain_qualified_name=DATA_DOMAIN_QUALIFIED_NAME,
+        parent_domain_qualified_name=domain.qualified_name,
     )
     response = client.asset.save(to_create)
     result = response.assets_created(asset_type=DataDomain)[0]
     yield result
     delete_asset(client, guid=result.guid, asset_type=DataDomain)
 
 
 def test_data_sub_domain(client: AtlanClient, sub_domain: DataDomain):
     assert sub_domain
     assert sub_domain.guid
     assert sub_domain.qualified_name
+    assert sub_domain.parent_domain_qualified_name
+    assert sub_domain.super_domain_qualified_name
     assert sub_domain.name == DATA_SUB_DOMAIN_NAME
-    assert sub_domain.qualified_name == DATA_SUB_DOMAIN_QUALIFIED_NAME
+    assert re.search(DATA_SUB_DOMAIN_QN_REGEX, sub_domain.qualified_name)
+    assert re.search(DATA_DOMAIN_QN_REGEX, sub_domain.parent_domain_qualified_name)
+    assert re.search(DATA_DOMAIN_QN_REGEX, sub_domain.super_domain_qualified_name)
 
 
 def test_update_domain(client: AtlanClient, domain: DataDomain):
     assert domain.qualified_name
     assert domain.name
     updated = client.asset.update_certificate(
         asset_type=DataDomain,
@@ -123,14 +130,25 @@
     assert test_domain.guid == domain.guid
     assert test_domain.qualified_name == domain.qualified_name
     assert test_domain.name == domain.name
     assert test_domain.certificate_status == CERTIFICATE_STATUS
     assert test_domain.certificate_status_message == CERTIFICATE_MESSAGE
 
 
+@pytest.mark.order(after="test_retrieve_domain")
+def test_find_domain_by_name(client: AtlanClient, domain: DataDomain):
+    response = client.asset.find_domain_by_name(
+        name=domain.name, attributes=["certificateStatus"]
+    )
+
+    assert response
+    assert response.guid == domain.guid
+    assert response.certificate_status == CertificateStatus.VERIFIED
+
+
 def test_update_sub_domain(client: AtlanClient, sub_domain: DataDomain):
     assert sub_domain.qualified_name
     assert sub_domain.name
     updated = client.asset.update_certificate(
         asset_type=DataDomain,
         qualified_name=sub_domain.qualified_name,
         name=sub_domain.name,
@@ -164,46 +182,61 @@
     assert test_sub_domain.guid == sub_domain.guid
     assert test_sub_domain.qualified_name == sub_domain.qualified_name
     assert test_sub_domain.name == sub_domain.name
     assert test_sub_domain.certificate_status == CERTIFICATE_STATUS
     assert test_sub_domain.certificate_status_message == CERTIFICATE_MESSAGE
 
 
+@pytest.mark.order(after="test_retrieve_sub_domain")
+def test_find_sub_domain_by_name(client: AtlanClient, sub_domain: DataDomain):
+    response = client.asset.find_domain_by_name(
+        name=sub_domain.name, attributes=["certificateStatus"]
+    )
+
+    assert response
+    assert response.guid == sub_domain.guid
+    assert response.certificate_status == CertificateStatus.VERIFIED
+
+
 @pytest.fixture(scope="module")
 def product(
     client: AtlanClient,
     domain: DataDomain,
 ) -> Generator[DataProduct, None, None]:
     assert domain.guid
     assets = (
         FluentSearch()
         .where(CompoundQuery.active_assets())
         .where(CompoundQuery.asset_type(AtlasGlossaryTerm))
     ).to_request()
     to_create = DataProduct.create(
         name=DATA_PRODUCT_NAME,
         asset_selection=assets,
-        domain_qualified_name=DATA_DOMAIN_QUALIFIED_NAME,
+        domain_qualified_name=domain.qualified_name,
     )
     response = client.asset.save(to_create)
     result = response.assets_created(asset_type=DataProduct)[0]
     yield result
     delete_asset(client, guid=result.guid, asset_type=DataProduct)
 
 
 def test_product(client: AtlanClient, product: DataProduct):
     assert product
     assert product.guid
     assert product.qualified_name
+    assert product.parent_domain_qualified_name
+    assert product.super_domain_qualified_name
     assert product.name == DATA_PRODUCT_NAME
-    assert product.qualified_name == DATA_PRODUCT_QUALIFIED_NAME
     assert (
         product.data_product_assets_playbook_filter
         == DATA_PRODUCT_ASSETS_PLAYBOOK_FILTER
     )
+    assert re.search(DATA_PRODUCT_QN_REGEX, product.qualified_name)
+    assert re.search(DATA_DOMAIN_QN_REGEX, product.parent_domain_qualified_name)
+    assert re.search(DATA_DOMAIN_QN_REGEX, product.super_domain_qualified_name)
 
 
 def test_update_product(client: AtlanClient, product: DataProduct):
     assert product.qualified_name
     assert product.name
     updated = client.asset.update_certificate(
         asset_type=DataProduct,
@@ -242,14 +275,25 @@
     assert test_product.qualified_name == product.qualified_name
     assert test_product.name == product.name
     assert test_product.certificate_status == CERTIFICATE_STATUS
     assert test_product.certificate_status_message == CERTIFICATE_MESSAGE
 
 
 @pytest.mark.order(after="test_retrieve_product")
+def test_find_product_by_name(client: AtlanClient, product: DataProduct):
+    response = client.asset.find_product_by_name(
+        name=product.name, attributes=["daapStatus"]
+    )
+
+    assert response
+    assert response.guid == product.guid
+    assert response.daap_status == DataProductStatus.ACTIVE
+
+
+@pytest.mark.order(after="test_retrieve_product")
 def test_delete_product(client: AtlanClient, product: DataProduct):
     response = client.asset.purge_by_guid(product.guid)
     assert response
     assert not response.assets_created(asset_type=DataProduct)
     assert not response.assets_updated(asset_type=DataProduct)
     deleted = response.assets_deleted(asset_type=DataProduct)
     assert deleted
```

### Comparing `pyatlan-2.2.0/tests/integration/data_studio_asset_test.py` & `pyatlan-2.2.1/tests/integration/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/file_test.py` & `pyatlan-2.2.1/tests/integration/file_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,18 +57,21 @@
     connection: Connection,
     file: File,
 ):
     assert file
     assert file.guid
     assert file.qualified_name
     assert file.name == FILE_NAME
-    assert not file.connector_name
     assert file.connection_qualified_name == connection.qualified_name
     assert file.file_type == FileType.PDF
     assert file.file_path == "https://www.example.com"
+    assert connection.qualified_name
+    assert file.connector_name == AtlanConnectorType.get_connector_name(
+        connection.qualified_name
+    )
 
 
 @pytest.mark.order(after="test_file")
 def test_update_file(
     client: AtlanClient,
     connection: Connection,
     file: File,
```

### Comparing `pyatlan-2.2.0/tests/integration/gcs_asset_test.py` & `pyatlan-2.2.1/tests/integration/gcs_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/glossary_test.py` & `pyatlan-2.2.1/tests/integration/glossary_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import itertools
 import logging
 from time import sleep
-from typing import Generator, List, Optional
+from typing import Generator, List, Optional, Union
 
 import pytest
 from pydantic.v1 import StrictStr
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.errors import InvalidRequestError, NotFoundError
 from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryCategory, AtlasGlossaryTerm
 from pyatlan.model.enums import SaveSemantic
+from pyatlan.model.fields.atlan_fields import AtlanField
 from pyatlan.model.fluent_search import CompoundQuery, FluentSearch
 from pyatlan.model.search import DSL, IndexSearchRequest
 from tests.integration.client import TestId, delete_asset
 
 LOGGER = logging.getLogger(__name__)
 
 MODULE_NAME = TestId.make_unique("GLS")
@@ -650,14 +651,24 @@
         term1.guid
         == client.asset.find_term_by_name(
             name=term1.name, glossary_name=glossary.name
         ).guid
     )
 
 
+@pytest.mark.parametrize(
+    "attributes, related_attributes",
+    [
+        (AtlasGlossaryCategory.TERMS, AtlasGlossaryTerm.NAME),
+        (
+            AtlasGlossaryCategory.TERMS.atlan_field_name,
+            AtlasGlossaryTerm.NAME.atlan_field_name,
+        ),
+    ],
+)
 def test_hierarchy(
     client: AtlanClient,
     hierarchy_glossary: AtlasGlossary,
     top1_category: AtlasGlossaryCategory,
     mid1a_category: AtlasGlossaryCategory,
     leaf1aa_category: AtlasGlossaryCategory,
     leaf1ab_category: AtlasGlossaryCategory,
@@ -665,20 +676,22 @@
     leaf1ba_category: AtlasGlossaryCategory,
     top2_category: AtlasGlossaryCategory,
     mid2a_category: AtlasGlossaryCategory,
     leaf2aa_category: AtlasGlossaryCategory,
     leaf2ab_category: AtlasGlossaryCategory,
     mid2b_category: AtlasGlossaryCategory,
     leaf2ba_category: AtlasGlossaryCategory,
+    attributes: Union[AtlanField, str],
+    related_attributes: Union[AtlanField, str],
 ):
     sleep(10)
     hierarchy = client.asset.get_hierarchy(
         glossary=hierarchy_glossary,
-        attributes=[AtlasGlossaryCategory.TERMS],
-        related_attributes=[AtlasGlossaryTerm.NAME],
+        attributes=[attributes],
+        related_attributes=[related_attributes],
     )
 
     root_categories = hierarchy.root_categories
 
     assert root_categories
     assert len(root_categories) == 2
     assert root_categories[0].name
```

### Comparing `pyatlan-2.2.0/tests/integration/lineage_test.py` & `pyatlan-2.2.1/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/owner_propagator_cfg.py` & `pyatlan-2.2.1/tests/integration/owner_propagator_cfg.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/persona_test.py` & `pyatlan-2.2.1/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/preset_asset_test.py` & `pyatlan-2.2.1/tests/integration/preset_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/purpose_test.py` & `pyatlan-2.2.1/tests/integration/purpose_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     HekaFlow,
     PurposeMetadataAction,
     QueryStatus,
 )
 from pyatlan.model.query import QueryRequest
 from pyatlan.model.typedef import AtlanTagDef
 from tests.integration.client import TestId, delete_asset
+from tests.integration.requests_test import delete_token
 
 MODULE_NAME = TestId.make_unique("Purpose")
 PERSONA_NAME = "Data Assets"
 DB_NAME = "RAW"
 TABLE_NAME = "PACKAGETYPES"
 COLUMN_NAME = "PACKAGETYPENAME"
 SCHEMA_NAME = "WIDEWORLDIMPORTERS_WAREHOUSE"
@@ -63,14 +64,15 @@
         atlan_tag_name=MODULE_NAME,
     )
     client.typedef.purge(MODULE_NAME, typedef_type=AtlanTagDef)
 
 
 @pytest.fixture(scope="module")
 def token(client: AtlanClient) -> Generator[ApiToken, None, None]:
+    token = None
     try:
         token = client.token.create(API_TOKEN_NAME)
         assert token
         assert token.guid
         assert token.display_name
         # After creating the token, assign it to the
         # "Data Assets" persona to grant it query access
@@ -81,15 +83,15 @@
             display_name=token.display_name,
             personas={persona.qualified_name},
         )
         # Note: need to read the token back again to see
         # its associated personas -- will leave that to later...
         yield token
     finally:
-        token.guid and client.token.purge(token.guid)
+        delete_token(client, token)
 
 
 @pytest.fixture(scope="module")
 def query(snowflake_conn) -> QueryRequest:
     # NOTE: This requires pre-existing assets:
     # - Snowflake connection called "development"
     #   with a specific pre-existing table
```

### Comparing `pyatlan-2.2.0/tests/integration/query_parser_test.py` & `pyatlan-2.2.1/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/requests_test.py` & `pyatlan-2.2.1/tests/integration/requests_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generator
+from typing import Generator, Optional
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.api_tokens import ApiToken
 from tests.integration.client import TestId
 
@@ -11,21 +11,43 @@
 
 
 def create_token(client: AtlanClient, name: str) -> ApiToken:
     t = client.token.create(name)
     return t
 
 
+def delete_token(client: AtlanClient, token: Optional[ApiToken] = None):
+    # If there is a partial failure on the server side
+    # and the token is still visible in the Atlan UI,
+    # in that case, the create method may not return a token.
+    # We should retrieve the list of all tokens and delete them here.
+    if not token:
+        tokens = client.token.get().records
+        assert tokens
+        delete_tokens = [
+            token
+            for token in tokens
+            if token.display_name and "psdk_Requests" in token.display_name
+        ]
+        for token in delete_tokens:
+            assert token and token.guid
+            client.token.purge(token.guid)
+        return
+    # In case of no partial failure, directly delete the token
+    token.guid and client.token.purge(token.guid)
+
+
 @pytest.fixture(scope="module")
 def token(client: AtlanClient) -> Generator[ApiToken, None, None]:
+    token = None
     try:
         token = create_token(client, API_TOKEN_NAME)
         yield token
     finally:
-        token.guid and client.token.purge(token.guid)
+        delete_token(client, token)
 
 
 def test_create_token(client: AtlanClient, token: ApiToken):
     assert token
     r = client.token.get_by_name(API_TOKEN_NAME)
     assert r
     assert r.display_name == API_TOKEN_NAME
```

### Comparing `pyatlan-2.2.0/tests/integration/s3_asset_test.py` & `pyatlan-2.2.1/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/test_client.py` & `pyatlan-2.2.1/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/test_file_client.py` & `pyatlan-2.2.1/tests/integration/test_file_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/test_index_search.py` & `pyatlan-2.2.1/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/test_sql_assets.py` & `pyatlan-2.2.1/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/test_sso_client.py` & `pyatlan-2.2.1/tests/integration/test_sso_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/test_task_client.py` & `pyatlan-2.2.1/tests/integration/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/test_workflow_client.py` & `pyatlan-2.2.1/tests/integration/test_workflow_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/integration/utils.py` & `pyatlan-2.2.1/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/conftest.py` & `pyatlan-2.2.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/constants.py` & `pyatlan-2.2.1/tests/unit/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -237,14 +237,42 @@
     ],
     "find_term_by_name": [
         ([[123], "glossary-qn"], "name\n  str type expected"),
         ([None, "glossary-qn"], "none is not an allowed value"),
         (["name", [123]], "glossary_name\n  str type expected"),
         (["name", None], "none is not an allowed value"),
     ],
+    "find_domain_by_name": [
+        (
+            [None, ["attributes"]],
+            "1 validation error for FindDomainByName\nname\n  none is not an allowed value",
+        ),
+        (
+            [" ", ["attributes"]],
+            "1 validation error for FindDomainByName\nname\n  ensure this value has at least 1 characters",
+        ),
+        (
+            ["test-domain", "attributes"],
+            "1 validation error for FindDomainByName\nattributes\n  value is not a valid list",
+        ),
+    ],
+    "find_product_by_name": [
+        (
+            [None, ["attributes"]],
+            "1 validation error for FindProductByName\nname\n  none is not an allowed value",
+        ),
+        (
+            [" ", ["attributes"]],
+            "1 validation error for FindProductByName\nname\n  ensure this value has at least 1 characters",
+        ),
+        (
+            ["test-product", "attributes"],
+            "1 validation error for FindProductByName\nattributes\n  value is not a valid list",
+        ),
+    ],
 }
 
 TEST_ADMIN_CLIENT_METHODS = {
     "get_keycloak_events": [
         (["keycloak-req"], "keycloak_request\n  value is not a valid dict"),
         ([None], "none is not an allowed value"),
     ],
```

### Comparing `pyatlan-2.2.0/tests/unit/model/a_d_l_s_account_test.py` & `pyatlan-2.2.1/tests/unit/model/a_d_l_s_account_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/a_d_l_s_container_test.py` & `pyatlan-2.2.1/tests/unit/model/a_d_l_s_container_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/a_d_l_s_object_test.py` & `pyatlan-2.2.1/tests/unit/model/a_d_l_s_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/a_p_i_path_test.py` & `pyatlan-2.2.1/tests/unit/model/a_p_i_path_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/a_p_i_spec_test.py` & `pyatlan-2.2.1/tests/unit/model/a_p_i_spec_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/airflow_dag.py` & `pyatlan-2.2.1/tests/unit/model/airflow_dag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/airflow_task.py` & `pyatlan-2.2.1/tests/unit/model/airflow_task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/badge_condition_test.py` & `pyatlan-2.2.1/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/badge_test.py` & `pyatlan-2.2.1/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/column_process_test.py` & `pyatlan-2.2.1/tests/unit/model/column_process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/column_test.py` & `pyatlan-2.2.1/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/connection_test.py` & `pyatlan-2.2.1/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/constants.py` & `pyatlan-2.2.1/tests/unit/model/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,21 +78,25 @@
 PRESET_DATASET_NAME = "ps-dataset"
 PRESET_DATASET_QUALIFIED_NAME = (
     f"{PRESET_DASHBOARD_QUALIFIED_NAME}/{PRESET_DATASET_NAME}"
 )
 PERSONA_NAME = "my-persona"
 PURPOSE_NAME = "my-purpose"
 DATA_DOMAIN_NAME = "data-domain"
-DATA_DOMAIN_QUALIFIED_NAME = "default/domain/dataDomain"
+DATA_DOMAIN_QUALIFIED_NAME = f"default/domain/{DATA_DOMAIN_NAME}/super"
 DATA_SUB_DOMAIN_NAME = "data-sub-domain"
-DATA_SUB_DOMAIN_QUALIFIED_NAME = f"{DATA_DOMAIN_QUALIFIED_NAME}/domain/dataSubDomain"
+DATA_SUB_DOMAIN_QUALIFIED_NAME = (
+    f"{DATA_DOMAIN_QUALIFIED_NAME}/domain/{DATA_SUB_DOMAIN_NAME}"
+)
 DATA_PRODUCT_NAME = "data-product"
-DATA_PRODUCT_QUALIFIED_NAME = "default/domain/dataDomain/product/dataProduct"
+DATA_PRODUCT_QUALIFIED_NAME = (
+    f"{DATA_DOMAIN_QUALIFIED_NAME}/product/{DATA_PRODUCT_NAME}"
+)
 DATA_PRODUCT_UNDER_SUB_DOMAIN_QUALIFIED_NAME = (
-    f"{DATA_SUB_DOMAIN_QUALIFIED_NAME}/product/dataProduct"
+    f"{DATA_SUB_DOMAIN_QUALIFIED_NAME}/product/{DATA_PRODUCT_NAME}"
 )
 CP_NAME = "column-process"
 CP_PROCESS_ID = "cp-process-id"
 CP_CONNECTION_QUALIFIED_NAME = "default/vertica/123456789"
 CP_QUALIFIED_NAME_HASH = (
     f"{CP_CONNECTION_QUALIFIED_NAME}/ecb5f77380c04710c979acfb8d3bba2f"
 )
```

### Comparing `pyatlan-2.2.0/tests/unit/model/data_domain_test.py` & `pyatlan-2.2.1/tests/unit/model/data_domain_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 
 from pyatlan.model.assets import DataDomain
 from tests.unit.model.constants import (
     DATA_DOMAIN_NAME,
     DATA_DOMAIN_QUALIFIED_NAME,
     DATA_SUB_DOMAIN_NAME,
-    DATA_SUB_DOMAIN_QUALIFIED_NAME,
 )
 
 
 def _assert_domain(domain: DataDomain) -> None:
     assert domain.name == DATA_DOMAIN_NAME
     assert domain.qualified_name == DATA_DOMAIN_QUALIFIED_NAME
     assert domain.parent_domain_qualified_name is None
@@ -40,15 +39,15 @@
     _assert_domain(test_domain)
 
     test_sub_domain = DataDomain.create(
         name=DATA_SUB_DOMAIN_NAME,
         parent_domain_qualified_name=test_domain.qualified_name,
     )
     assert test_sub_domain.name == DATA_SUB_DOMAIN_NAME
-    assert test_sub_domain.qualified_name == DATA_SUB_DOMAIN_QUALIFIED_NAME
+    assert test_sub_domain.qualified_name == DATA_SUB_DOMAIN_NAME
     assert test_sub_domain.parent_domain_qualified_name == test_domain.qualified_name
 
 
 def test_create_for_modification():
     test_domain = DataDomain.create_for_modification(
         name=DATA_DOMAIN_NAME, qualified_name=DATA_DOMAIN_QUALIFIED_NAME
     )
```

### Comparing `pyatlan-2.2.0/tests/unit/model/data_product_test.py` & `pyatlan-2.2.1/tests/unit/model/data_product_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from json import dumps, load, loads
 from pathlib import Path
 
 import pytest
 
 from pyatlan.model.assets import AtlasGlossary, DataProduct
-from pyatlan.model.enums import CertificateStatus
+from pyatlan.model.enums import CertificateStatus, DataProductStatus
 from pyatlan.model.fluent_search import CompoundQuery, FluentSearch
 from pyatlan.model.search import IndexSearchRequest
 from tests.unit.model.constants import (
     DATA_DOMAIN_QUALIFIED_NAME,
     DATA_PRODUCT_NAME,
     DATA_PRODUCT_QUALIFIED_NAME,
     DATA_PRODUCT_UNDER_SUB_DOMAIN_QUALIFIED_NAME,
@@ -129,14 +129,15 @@
     )
     expected_asset_dsl = dumps(data_product_assets_dsl_json, sort_keys=True)
     assert test_asset_dsl == expected_asset_dsl
     assert test_product.data_product_assets_playbook_filter == ASSETS_PLAYBOOK_FILTER
     _assert_product(
         test_product, qualified_name=DATA_PRODUCT_UNDER_SUB_DOMAIN_QUALIFIED_NAME
     )
+    assert test_product.daap_status == DataProductStatus.ACTIVE
 
 
 def test_create_for_modification():
     test_product = DataProduct.create_for_modification(
         name=DATA_PRODUCT_NAME,
         qualified_name=DATA_PRODUCT_QUALIFIED_NAME,
     )
```

### Comparing `pyatlan-2.2.0/tests/unit/model/data_studio_asset_test.py` & `pyatlan-2.2.1/tests/unit/model/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/database_test.py` & `pyatlan-2.2.1/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/fields/atlan_fields_test.py` & `pyatlan-2.2.1/tests/unit/model/fields/atlan_fields_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/file_test.py` & `pyatlan-2.2.1/tests/unit/model/file_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from pyatlan.model.assets import File
-from pyatlan.model.enums import FileType
+from pyatlan.model.enums import AtlanConnectorType, FileType
 from tests.unit.model.constants import (
     FILE_CONNECTION_QUALIFIED_NAME,
     FILE_NAME,
     FILE_QUALIFIED_NAME,
 )
 
 FILE_TYPE = FileType.PDF
@@ -38,14 +38,17 @@
         name=FILE_NAME,
         connection_qualified_name=FILE_CONNECTION_QUALIFIED_NAME,
         file_type=FILE_TYPE,
     )
     assert attributes.name == FILE_NAME
     assert attributes.connection_qualified_name == FILE_CONNECTION_QUALIFIED_NAME
     assert attributes.qualified_name == FILE_QUALIFIED_NAME
+    assert attributes.connector_name == AtlanConnectorType.get_connector_name(
+        FILE_CONNECTION_QUALIFIED_NAME
+    )
 
 
 @pytest.mark.parametrize(
     "qualified_name, name, message",
     [
         (None, FILE_QUALIFIED_NAME, "qualified_name is required"),
         (FILE_NAME, None, "name is required"),
```

### Comparing `pyatlan-2.2.0/tests/unit/model/gcs_bucket_test.py` & `pyatlan-2.2.1/tests/unit/model/gcs_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/gcs_object_test.py` & `pyatlan-2.2.1/tests/unit/model/gcs_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/glossary_category_test.py` & `pyatlan-2.2.1/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/glossary_term_test.py` & `pyatlan-2.2.1/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/glossary_test.py` & `pyatlan-2.2.1/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/materialised_view_test.py` & `pyatlan-2.2.1/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/preset_chart_test.py` & `pyatlan-2.2.1/tests/unit/model/preset_chart_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/preset_dashboard_test.py` & `pyatlan-2.2.1/tests/unit/model/preset_dashboard_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/preset_dataset_test.py` & `pyatlan-2.2.1/tests/unit/model/preset_dataset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/preset_workspace_test.py` & `pyatlan-2.2.1/tests/unit/model/preset_workspace_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/process_test.py` & `pyatlan-2.2.1/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/readme_test.py` & `pyatlan-2.2.1/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/s3_bucket_test.py` & `pyatlan-2.2.1/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/s3object_test.py` & `pyatlan-2.2.1/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/schema_test.py` & `pyatlan-2.2.1/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/table_test.py` & `pyatlan-2.2.1/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/model/view_test.py` & `pyatlan-2.2.1/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/pkg/conftest.py` & `pyatlan-2.2.1/tests/unit/pkg/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/pkg/test_models.py` & `pyatlan-2.2.1/tests/unit/pkg/test_models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/pkg/test_ui.py` & `pyatlan-2.2.1/tests/unit/pkg/test_ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/pkg/test_utils.py` & `pyatlan-2.2.1/tests/unit/pkg/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/pkg/test_widgets.py` & `pyatlan-2.2.1/tests/unit/pkg/test_widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_atlan_tag_name.py` & `pyatlan-2.2.1/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_client.py` & `pyatlan-2.2.1/tests/unit/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     InvalidRequestError,
     NotFoundError,
 )
 from pyatlan.model.assets import (
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
+    DataDomain,
+    DataProduct,
     Table,
 )
 from pyatlan.model.assets.column import Column
 from pyatlan.model.core import Announcement, BulkRequest
 from pyatlan.model.enums import (
     AnnouncementType,
     CertificateStatus,
@@ -53,14 +55,16 @@
     TEST_TOKEN_CLIENT_METHODS,
     TEST_TYPEDEF_CLIENT_METHODS,
     TEST_USER_CLIENT_METHODS,
 )
 from tests.unit.model.constants import (
     CONNECTION_NAME,
     CONNECTOR_TYPE,
+    DATA_DOMAIN_NAME,
+    DATA_PRODUCT_NAME,
     GLOSSARY_CATEGORY_NAME,
     GLOSSARY_NAME,
     GLOSSARY_QUALIFIED_NAME,
     GLOSSARY_TERM_NAME,
     PERSONA_NAME,
     PURPOSE_NAME,
 )
@@ -1156,14 +1160,46 @@
             name=GLOSSARY_TERM_NAME,
             glossary_qualified_name=GLOSSARY_QUALIFIED_NAME,
             attributes=attributes,
         )
         assert mock_find_term_fast_by_name.return_value == term
 
 
+@patch.object(AssetClient, "_search_for_asset_with_name")
+def test_find_domain_by_name(mock_search_for_asset_with_name):
+    client = AtlanClient()
+    test_domain = DataDomain()
+    test_domain.name = DATA_DOMAIN_NAME
+    mock_search_for_asset_with_name.return_value = [test_domain]
+
+    domain = client.asset.find_domain_by_name(
+        name=DATA_DOMAIN_NAME,
+        attributes=["name"],
+    )
+
+    assert domain and domain == test_domain
+    assert mock_search_for_asset_with_name.call_count == 1
+
+
+@patch.object(AssetClient, "_search_for_asset_with_name")
+def test_find_product_by_name(mock_search_for_asset_with_name):
+    client = AtlanClient()
+    test_product = DataProduct()
+    test_product.name = DATA_PRODUCT_NAME
+    mock_search_for_asset_with_name.return_value = [test_product]
+
+    product = client.asset.find_product_by_name(
+        name=DATA_PRODUCT_NAME,
+        attributes=["name"],
+    )
+
+    assert product and product == test_product
+    assert mock_search_for_asset_with_name.call_count == 1
+
+
 @patch.object(SearchLogClient, "_call_search_api")
 def test_search_log_most_recent_viewers(mock_sl_api_call, sl_most_recent_viewers_json):
     client = AtlanClient()
     mock_sl_api_call.return_value = sl_most_recent_viewers_json
     recent_viewers_aggs = sl_most_recent_viewers_json["aggregations"]
     recent_viewers_aggs_buckets = recent_viewers_aggs[UNIQUE_USERS]["buckets"]
     request = SearchLogRequest.most_recent_viewers(
```

### Comparing `pyatlan-2.2.0/tests/unit/test_core.py` & `pyatlan-2.2.1/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_credential_client.py` & `pyatlan-2.2.1/tests/unit/test_credential_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_custom_metadata.py` & `pyatlan-2.2.1/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_deprecated.py` & `pyatlan-2.2.1/tests/unit/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_events.py` & `pyatlan-2.2.1/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_file_client.py` & `pyatlan-2.2.1/tests/unit/test_file_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_glossary_term.py` & `pyatlan-2.2.1/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_lineage.py` & `pyatlan-2.2.1/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_model.py` & `pyatlan-2.2.1/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_packages.py` & `pyatlan-2.2.1/tests/unit/test_packages.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_query_client.py` & `pyatlan-2.2.1/tests/unit/test_query_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_search_model.py` & `pyatlan-2.2.1/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_sso_client.py` & `pyatlan-2.2.1/tests/unit/test_sso_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_structs.py` & `pyatlan-2.2.1/tests/unit/test_structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_task_client.py` & `pyatlan-2.2.1/tests/unit/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_typedef_model.py` & `pyatlan-2.2.1/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_utils.py` & `pyatlan-2.2.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.0/tests/unit/test_workflow_client.py` & `pyatlan-2.2.1/tests/unit/test_workflow_client.py`

 * *Files identical despite different names*

