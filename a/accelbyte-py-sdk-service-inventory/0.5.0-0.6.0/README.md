# Comparing `tmp/accelbyte_py_sdk_service_inventory-0.5.0.tar.gz` & `tmp/accelbyte_py_sdk_service_inventory-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_service_inventory-0.5.0.tar", last modified: Tue May  7 06:28:17 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_inventory-0.6.0.tar", last modified: Tue May 21 03:47:31 2024, max compression
```

## Comparing `accelbyte_py_sdk_service_inventory-0.5.0.tar` & `accelbyte_py_sdk_service_inventory-0.6.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.389219 accelbyte_py_sdk_service_inventory-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:28:17.389219 accelbyte_py_sdk_service_inventory-0.5.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.377220 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.377220 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.377220 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/
--rw-rw-r--   0 root         (0) root         (0)     4833 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/
--rw-rw-r--   0 root         (0) root         (0)     4392 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8049 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     5708 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py
--rw-rw-r--   0 root         (0) root         (0)     6566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5781 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py
--rw-rw-r--   0 root         (0) root         (0)     5104 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     5967 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_integration_configuration_req.py
--rw-rw-r--   0 root         (0) root         (0)     8033 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py
--rw-rw-r--   0 root         (0) root         (0)     4996 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py
--rw-rw-r--   0 root         (0) root         (0)    11998 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py
--rw-rw-r--   0 root         (0) root         (0)     3774 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py
--rw-rw-r--   0 root         (0) root         (0)     5155 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4683 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py
--rw-rw-r--   0 root         (0) root         (0)     6082 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py
--rw-rw-r--   0 root         (0) root         (0)     3844 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py
--rw-rw-r--   0 root         (0) root         (0)     4591 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     9060 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_integration_configuration_resp.py
--rw-rw-r--   0 root         (0) root         (0)     3910 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_config.py
--rw-rw-r--   0 root         (0) root         (0)     7908 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py
--rw-rw-r--   0 root         (0) root         (0)    11465 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py
--rw-rw-r--   0 root         (0) root         (0)    10855 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py
--rw-rw-r--   0 root         (0) root         (0)    14498 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5422 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_integration_configurations_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5384 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5037 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5113 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4964 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4887 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py
--rw-rw-r--   0 root         (0) root         (0)     8219 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_operation.py
--rw-rw-r--   0 root         (0) root         (0)     5424 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_paging.py
--rw-rw-r--   0 root         (0) root         (0)     8658 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     9837 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_req.py
--rw-rw-r--   0 root         (0) root         (0)     4655 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     5208 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py
--rw-rw-r--   0 root         (0) root         (0)    11261 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py
--rw-rw-r--   0 root         (0) root         (0)    10367 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py
--rw-rw-r--   0 root         (0) root         (0)     5021 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py
--rw-rw-r--   0 root         (0) root         (0)     5091 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5967 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_integration_configuration_req.py
--rw-rw-r--   0 root         (0) root         (0)     3946 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py
--rw-rw-r--   0 root         (0) root         (0)     8612 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py
--rw-rw-r--   0 root         (0) root         (0)     6193 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py
--rw-rw-r--   0 root         (0) root         (0)     6400 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4446 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_status_integration_configuration_req.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/
--rw-rw-r--   0 root         (0) root         (0)      437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/
--rw-rw-r--   0 root         (0) root         (0)      544 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9263 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/
--rw-rw-r--   0 root         (0) root         (0)      907 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8368 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_create_integratio_c6b1bd.py
--rw-rw-r--   0 root         (0) root         (0)     9942 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_list_integration__420e8d.py
--rw-rw-r--   0 root         (0) root         (0)    10071 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_integratio_fe692f.py
--rw-rw-r--   0 root         (0) root         (0)    10290 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_status_int_703321.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/
--rw-rw-r--   0 root         (0) root         (0)      876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7952 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     7615 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py
--rw-rw-r--   0 root         (0) root         (0)    12436 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py
--rw-rw-r--   0 root         (0) root         (0)     8825 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_purchasable.py
--rw-rw-r--   0 root         (0) root         (0)     8996 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_update_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     8671 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/
--rw-rw-r--   0 root         (0) root         (0)      966 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8313 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py
--rw-rw-r--   0 root         (0) root         (0)     8205 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py
--rw-rw-r--   0 root         (0) root         (0)     8298 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py
--rw-rw-r--   0 root         (0) root         (0)    11039 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py
--rw-rw-r--   0 root         (0) root         (0)     9828 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_update_inventory__e10746.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.381219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/
--rw-rw-r--   0 root         (0) root         (0)      723 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8041 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_create_item_type.py
--rw-rw-r--   0 root         (0) root         (0)     7425 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_delete_item_type.py
--rw-rw-r--   0 root         (0) root         (0)     9774 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_list_item_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/
--rw-rw-r--   0 root         (0) root         (0)     1010 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9804 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py
--rw-rw-r--   0 root         (0) root         (0)     9822 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py
--rw-rw-r--   0 root         (0) root         (0)     9566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py
--rw-rw-r--   0 root         (0) root         (0)     9416 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py
--rw-rw-r--   0 root         (0) root         (0)    13325 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py
--rw-rw-r--   0 root         (0) root         (0)     8703 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py
--rw-rw-r--   0 root         (0) root         (0)     9725 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     7889 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_sync_user_entitlements.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/
--rw-rw-r--   0 root         (0) root         (0)      679 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7894 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py
--rw-rw-r--   0 root         (0) root         (0)     7177 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py
--rw-rw-r--   0 root         (0) root         (0)    10416 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/
--rw-rw-r--   0 root         (0) root         (0)      621 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11160 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/
--rw-rw-r--   0 root         (0) root         (0)      659 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10878 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/public_list_inventory_c_d1722b.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/
--rw-rw-r--   0 root         (0) root         (0)      615 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9623 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/public_list_item_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/
--rw-rw-r--   0 root         (0) root         (0)      878 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8881 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_remove_my_items.py
--rw-rw-r--   0 root         (0) root         (0)     8771 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_update_my_items.py
--rw-rw-r--   0 root         (0) root         (0)     8584 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_consume_my_item.py
--rw-rw-r--   0 root         (0) root         (0)     9212 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py
--rw-rw-r--   0 root         (0) root         (0)    13165 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py
--rw-rw-r--   0 root         (0) root         (0)     8439 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/
--rw-rw-r--   0 root         (0) root         (0)      593 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9525 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     5492 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6055 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py
--rw-rw-r--   0 root         (0) root         (0)    17453 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_integration_configurations.py
--rw-rw-r--   0 root         (0) root         (0)    22341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py
--rw-rw-r--   0 root         (0) root         (0)    19912 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py
--rw-rw-r--   0 root         (0) root         (0)    11247 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py
--rw-rw-r--   0 root         (0) root         (0)    31125 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py
--rw-rw-r--   0 root         (0) root         (0)    11013 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py
--rw-rw-r--   0 root         (0) root         (0)     4934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py
--rw-rw-r--   0 root         (0) root         (0)     4985 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py
--rw-rw-r--   0 root         (0) root         (0)     4468 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_item_types.py
--rw-rw-r--   0 root         (0) root         (0)    20466 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_items.py
--rw-rw-r--   0 root         (0) root         (0)     4333 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:17.385219 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8940 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:28:17.000000 accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_inventory-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:28:17.389219 accelbyte_py_sdk_service_inventory-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.865686 accelbyte_py_sdk_service_inventory-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-21 03:47:31.865686 accelbyte_py_sdk_service_inventory-0.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      876 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.853686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.853686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.853686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/
+-rw-rw-r--   0 root         (0) root         (0)     4833 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.857686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/
+-rw-rw-r--   0 root         (0) root         (0)     4392 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8049 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5708 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py
+-rw-rw-r--   0 root         (0) root         (0)     6566 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5781 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5104 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5967 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_integration_configuration_req.py
+-rw-rw-r--   0 root         (0) root         (0)     8033 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4996 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py
+-rw-rw-r--   0 root         (0) root         (0)    11998 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py
+-rw-rw-r--   0 root         (0) root         (0)     3774 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5155 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4683 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py
+-rw-rw-r--   0 root         (0) root         (0)     6082 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     3844 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4591 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9060 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_integration_configuration_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     3910 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7908 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py
+-rw-rw-r--   0 root         (0) root         (0)    11465 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py
+-rw-rw-r--   0 root         (0) root         (0)    10855 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py
+-rw-rw-r--   0 root         (0) root         (0)    14498 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5422 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_integration_configurations_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5384 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5037 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5113 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4964 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4887 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py
+-rw-rw-r--   0 root         (0) root         (0)     7114 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     8219 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_operation.py
+-rw-rw-r--   0 root         (0) root         (0)     5424 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_paging.py
+-rw-rw-r--   0 root         (0) root         (0)     9357 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)    10532 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4655 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5208 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py
+-rw-rw-r--   0 root         (0) root         (0)    11261 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)    10367 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5021 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5091 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5967 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_integration_configuration_req.py
+-rw-rw-r--   0 root         (0) root         (0)     3946 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py
+-rw-rw-r--   0 root         (0) root         (0)     8612 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py
+-rw-rw-r--   0 root         (0) root         (0)     6193 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py
+-rw-rw-r--   0 root         (0) root         (0)     6400 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4446 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_status_integration_configuration_req.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.857686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.857686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/
+-rw-rw-r--   0 root         (0) root         (0)      544 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9263 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.857686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/
+-rw-rw-r--   0 root         (0) root         (0)      907 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8368 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_create_integratio_c6b1bd.py
+-rw-rw-r--   0 root         (0) root         (0)     9942 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_list_integration__420e8d.py
+-rw-rw-r--   0 root         (0) root         (0)    10071 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_integratio_fe692f.py
+-rw-rw-r--   0 root         (0) root         (0)    10290 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_status_int_703321.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/
+-rw-rw-r--   0 root         (0) root         (0)      876 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7952 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     7615 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)    12436 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py
+-rw-rw-r--   0 root         (0) root         (0)     8825 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_purchasable.py
+-rw-rw-r--   0 root         (0) root         (0)     8996 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_update_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     8671 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/
+-rw-rw-r--   0 root         (0) root         (0)      966 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8313 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py
+-rw-rw-r--   0 root         (0) root         (0)     8205 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py
+-rw-rw-r--   0 root         (0) root         (0)     8298 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py
+-rw-rw-r--   0 root         (0) root         (0)    11039 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py
+-rw-rw-r--   0 root         (0) root         (0)     9828 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_update_inventory__e10746.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/
+-rw-rw-r--   0 root         (0) root         (0)      723 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8041 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_create_item_type.py
+-rw-rw-r--   0 root         (0) root         (0)     7425 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_delete_item_type.py
+-rw-rw-r--   0 root         (0) root         (0)     9774 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_list_item_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/
+-rw-rw-r--   0 root         (0) root         (0)     1010 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9804 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9822 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9566 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9416 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py
+-rw-rw-r--   0 root         (0) root         (0)    13325 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8703 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9725 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     7889 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_sync_user_entitlements.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/
+-rw-rw-r--   0 root         (0) root         (0)      679 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7894 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     7177 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py
+-rw-rw-r--   0 root         (0) root         (0)    10416 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/
+-rw-rw-r--   0 root         (0) root         (0)      621 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11160 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/
+-rw-rw-r--   0 root         (0) root         (0)      659 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10878 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/public_list_inventory_c_d1722b.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9623 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/public_list_item_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/
+-rw-rw-r--   0 root         (0) root         (0)      878 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8881 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_remove_my_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8771 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_update_my_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8584 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_consume_my_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9212 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py
+-rw-rw-r--   0 root         (0) root         (0)    13165 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8439 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.861686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_tags/
+-rw-rw-r--   0 root         (0) root         (0)      593 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9525 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.865686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     5492 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6055 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    17453 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_integration_configurations.py
+-rw-rw-r--   0 root         (0) root         (0)    22341 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py
+-rw-rw-r--   0 root         (0) root         (0)    19912 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py
+-rw-rw-r--   0 root         (0) root         (0)    11247 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py
+-rw-rw-r--   0 root         (0) root         (0)    31125 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py
+-rw-rw-r--   0 root         (0) root         (0)    11013 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py
+-rw-rw-r--   0 root         (0) root         (0)     4934 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py
+-rw-rw-r--   0 root         (0) root         (0)     4985 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py
+-rw-rw-r--   0 root         (0) root         (0)     4468 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_item_types.py
+-rw-rw-r--   0 root         (0) root         (0)    20466 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_items.py
+-rw-rw-r--   0 root         (0) root         (0)     4333 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:47:31.865686 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk_service_inventory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-21 03:47:31.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk_service_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-21 03:47:31.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk_service_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:47:31.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk_service_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 03:47:31.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk_service_inventory.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 03:47:31.000000 accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk_service_inventory.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_inventory-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:47:31.865686 accelbyte_py_sdk_service_inventory-0.6.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/PKG-INFO` & `accelbyte_py_sdk_service_inventory-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-inventory
-Version: 0.5.0
+Version: 0.6.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Inventory Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Inventory Service
-* Version: 0.1.3
+* Version: 0.1.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/README.md` & `accelbyte_py_sdk_service_inventory-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Inventory Service
-* Version: 0.1.3
+* Version: 0.1.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # admin_chaining_operations
 from .wrappers import admin_create_chaining_operations
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .apimodels_admin_update_item_req import ApimodelsAdminUpdateItemReq
 from .apimodels_chaining_operation_req import ApimodelsChainingOperationReq
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_admin_update_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_chaining_operation_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_consume_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_integration_configuration_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_integration_configuration_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_configuration_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_inventory_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_item_type_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_create_tag_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_delete_inventory_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_integration_configuration_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_integration_configuration_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_config.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_configuration_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_inventory_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_item_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_integration_configurations_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_integration_configurations_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_configurations_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_inventory_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_item_types_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_list_tags_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_move_items_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_operation.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_operation.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_paging.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_paging.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_item_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_item_req.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,25 +42,28 @@
 
         item_id: (itemId) REQUIRED str
 
         item_type: (itemType) REQUIRED str
 
         sku: (sku) REQUIRED str
 
+        stackable: (stackable) REQUIRED bool
+
         use_count: (useCount) OPTIONAL int
     """
 
     # region fields
 
     bundled_qty: int  # REQUIRED
     entitlement_type: str  # REQUIRED
     inventory_config: ApimodelsInventoryConfig  # REQUIRED
     item_id: str  # REQUIRED
     item_type: str  # REQUIRED
     sku: str  # REQUIRED
+    stackable: bool  # REQUIRED
     use_count: int  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_bundled_qty(self, value: int) -> ApimodelsPurchaseValidationItemReq:
@@ -85,14 +88,18 @@
         self.item_type = value
         return self
 
     def with_sku(self, value: str) -> ApimodelsPurchaseValidationItemReq:
         self.sku = value
         return self
 
+    def with_stackable(self, value: bool) -> ApimodelsPurchaseValidationItemReq:
+        self.stackable = value
+        return self
+
     def with_use_count(self, value: int) -> ApimodelsPurchaseValidationItemReq:
         self.use_count = value
         return self
 
     # endregion with_x methods
 
     # region to methods
@@ -121,14 +128,18 @@
             result["itemType"] = str(self.item_type)
         elif include_empty:
             result["itemType"] = ""
         if hasattr(self, "sku"):
             result["sku"] = str(self.sku)
         elif include_empty:
             result["sku"] = ""
+        if hasattr(self, "stackable"):
+            result["stackable"] = bool(self.stackable)
+        elif include_empty:
+            result["stackable"] = False
         if hasattr(self, "use_count"):
             result["useCount"] = int(self.use_count)
         elif include_empty:
             result["useCount"] = 0
         return result
 
     # endregion to methods
@@ -140,24 +151,26 @@
         cls,
         bundled_qty: int,
         entitlement_type: str,
         inventory_config: ApimodelsInventoryConfig,
         item_id: str,
         item_type: str,
         sku: str,
+        stackable: bool,
         use_count: Optional[int] = None,
         **kwargs,
     ) -> ApimodelsPurchaseValidationItemReq:
         instance = cls()
         instance.bundled_qty = bundled_qty
         instance.entitlement_type = entitlement_type
         instance.inventory_config = inventory_config
         instance.item_id = item_id
         instance.item_type = item_type
         instance.sku = sku
+        instance.stackable = stackable
         if use_count is not None:
             instance.use_count = use_count
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
@@ -187,14 +200,18 @@
             instance.item_type = str(dict_["itemType"])
         elif include_empty:
             instance.item_type = ""
         if "sku" in dict_ and dict_["sku"] is not None:
             instance.sku = str(dict_["sku"])
         elif include_empty:
             instance.sku = ""
+        if "stackable" in dict_ and dict_["stackable"] is not None:
+            instance.stackable = bool(dict_["stackable"])
+        elif include_empty:
+            instance.stackable = False
         if "useCount" in dict_ and dict_["useCount"] is not None:
             instance.use_count = int(dict_["useCount"])
         elif include_empty:
             instance.use_count = 0
         return instance
 
     @classmethod
@@ -240,23 +257,25 @@
         return {
             "bundledQty": "bundled_qty",
             "entitlementType": "entitlement_type",
             "inventoryConfig": "inventory_config",
             "itemId": "item_id",
             "itemType": "item_type",
             "sku": "sku",
+            "stackable": "stackable",
             "useCount": "use_count",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "bundledQty": True,
             "entitlementType": True,
             "inventoryConfig": True,
             "itemId": True,
             "itemType": True,
             "sku": True,
+            "stackable": True,
             "useCount": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_purchase_validation_req.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
         item_type: (itemType) REQUIRED str
 
         quantity: (quantity) REQUIRED int
 
         sku: (sku) REQUIRED str
 
+        stackable: (stackable) REQUIRED bool
+
         entitlement_type: (entitlementType) OPTIONAL str
 
         inventory_config: (inventoryConfig) OPTIONAL ApimodelsInventoryConfig
 
         items: (items) OPTIONAL List[ApimodelsPurchaseValidationItemReq]
 
         use_count: (useCount) OPTIONAL int
@@ -56,14 +58,15 @@
 
     # region fields
 
     item_id: str  # REQUIRED
     item_type: str  # REQUIRED
     quantity: int  # REQUIRED
     sku: str  # REQUIRED
+    stackable: bool  # REQUIRED
     entitlement_type: str  # OPTIONAL
     inventory_config: ApimodelsInventoryConfig  # OPTIONAL
     items: List[ApimodelsPurchaseValidationItemReq]  # OPTIONAL
     use_count: int  # OPTIONAL
 
     # endregion fields
 
@@ -81,14 +84,18 @@
         self.quantity = value
         return self
 
     def with_sku(self, value: str) -> ApimodelsPurchaseValidationReq:
         self.sku = value
         return self
 
+    def with_stackable(self, value: bool) -> ApimodelsPurchaseValidationReq:
+        self.stackable = value
+        return self
+
     def with_entitlement_type(self, value: str) -> ApimodelsPurchaseValidationReq:
         self.entitlement_type = value
         return self
 
     def with_inventory_config(
         self, value: ApimodelsInventoryConfig
     ) -> ApimodelsPurchaseValidationReq:
@@ -123,14 +130,18 @@
             result["quantity"] = int(self.quantity)
         elif include_empty:
             result["quantity"] = 0
         if hasattr(self, "sku"):
             result["sku"] = str(self.sku)
         elif include_empty:
             result["sku"] = ""
+        if hasattr(self, "stackable"):
+            result["stackable"] = bool(self.stackable)
+        elif include_empty:
+            result["stackable"] = False
         if hasattr(self, "entitlement_type"):
             result["entitlementType"] = str(self.entitlement_type)
         elif include_empty:
             result["entitlementType"] = ""
         if hasattr(self, "inventory_config"):
             result["inventoryConfig"] = self.inventory_config.to_dict(
                 include_empty=include_empty
@@ -156,25 +167,27 @@
     @classmethod
     def create(
         cls,
         item_id: str,
         item_type: str,
         quantity: int,
         sku: str,
+        stackable: bool,
         entitlement_type: Optional[str] = None,
         inventory_config: Optional[ApimodelsInventoryConfig] = None,
         items: Optional[List[ApimodelsPurchaseValidationItemReq]] = None,
         use_count: Optional[int] = None,
         **kwargs,
     ) -> ApimodelsPurchaseValidationReq:
         instance = cls()
         instance.item_id = item_id
         instance.item_type = item_type
         instance.quantity = quantity
         instance.sku = sku
+        instance.stackable = stackable
         if entitlement_type is not None:
             instance.entitlement_type = entitlement_type
         if inventory_config is not None:
             instance.inventory_config = inventory_config
         if items is not None:
             instance.items = items
         if use_count is not None:
@@ -200,14 +213,18 @@
             instance.quantity = int(dict_["quantity"])
         elif include_empty:
             instance.quantity = 0
         if "sku" in dict_ and dict_["sku"] is not None:
             instance.sku = str(dict_["sku"])
         elif include_empty:
             instance.sku = ""
+        if "stackable" in dict_ and dict_["stackable"] is not None:
+            instance.stackable = bool(dict_["stackable"])
+        elif include_empty:
+            instance.stackable = False
         if "entitlementType" in dict_ and dict_["entitlementType"] is not None:
             instance.entitlement_type = str(dict_["entitlementType"])
         elif include_empty:
             instance.entitlement_type = ""
         if "inventoryConfig" in dict_ and dict_["inventoryConfig"] is not None:
             instance.inventory_config = ApimodelsInventoryConfig.create_from_dict(
                 dict_["inventoryConfig"], include_empty=include_empty
@@ -270,27 +287,29 @@
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "itemId": "item_id",
             "itemType": "item_type",
             "quantity": "quantity",
             "sku": "sku",
+            "stackable": "stackable",
             "entitlementType": "entitlement_type",
             "inventoryConfig": "inventory_config",
             "items": "items",
             "useCount": "use_count",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "itemId": True,
             "itemType": True,
             "quantity": True,
             "sku": True,
+            "stackable": True,
             "entitlementType": False,
             "inventoryConfig": False,
             "items": False,
             "useCount": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_inventory_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_remove_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_save_item_to_inventory_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_trade_item_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_integration_configuration_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_integration_configuration_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_inventory_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_item_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_status_integration_configuration_req.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/models/apimodels_update_status_integration_configuration_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_chaining_o_8801c9 import AdminCreateChainingOperations
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_chaining_operations/admin_create_chaining_o_8801c9.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_integratio_c6b1bd import AdminCreateIntegrationConfiguration
 from .admin_list_integration__420e8d import AdminListIntegrationConfigurations
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_create_integratio_c6b1bd.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_create_integratio_c6b1bd.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_list_integration__420e8d.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_list_integration__420e8d.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_integratio_fe692f.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_integratio_fe692f.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_status_int_703321.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_integration_configurations/admin_update_status_int_703321.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_inventory import AdminCreateInventory
 from .admin_get_inventory import AdminGetInventory
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_create_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_get_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_list_inventories.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_purchasable.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_purchasable.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_update_inventory.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/admin_update_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventories/delete_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_inventory__71b514 import AdminCreateInventoryConfiguration
 from .admin_delete_inventory__38371e import AdminDeleteInventoryConfiguration
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_create_inventory__71b514.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_delete_inventory__38371e.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_get_inventory_con_709281.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_list_inventory_co_67d862.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_update_inventory__e10746.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_inventory_configurations/admin_update_inventory__e10746.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_item_type import AdminCreateItemType
 from .admin_delete_item_type import AdminDeleteItemType
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_create_item_type.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_create_item_type.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_delete_item_type.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_delete_item_type.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_list_item_types.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_item_types/admin_list_item_types.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_bulk_remove_items import AdminBulkRemoveItems
 from .admin_bulk_update_my_items import AdminBulkUpdateMyItems
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_remove_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_bulk_update_my_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_consume_user_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_get_inventory_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_list_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_save_item_to_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_sync_user_entitlements.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_items/admin_sync_user_entitlements.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_tag import AdminCreateTag
 from .admin_delete_tag import AdminDeleteTag
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_create_tag.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_delete_tag.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/admin_tags/admin_list_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_inventories import PublicListInventories
 from .public_list_inventories import (
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventories/public_list_inventories.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_inventory_c_d1722b import PublicListInventoryConfigurations
 from .public_list_inventory_c_d1722b import (
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/public_list_inventory_c_d1722b.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_inventory_configurations/public_list_inventory_c_d1722b.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_item_types import PublicListItemTypes
 from .public_list_item_types import (
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/public_list_item_types.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_item_types/public_list_item_types.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_bulk_remove_my_items import PublicBulkRemoveMyItems
 from .public_bulk_update_my_items import PublicBulkUpdateMyItems
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_remove_my_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_remove_my_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_update_my_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_bulk_update_my_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_consume_my_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_consume_my_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_get_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_list_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_items/public_move_my_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_tags/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_tags import PublicListTags
 from .public_list_tags import (
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/operations/public_tags/public_list_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/__init__.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Inventory Service."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._admin_chaining_operations import admin_create_chaining_operations
 from ._admin_chaining_operations import admin_create_chaining_operations_async
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_chaining_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_integration_configurations.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_integration_configurations.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventories.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_inventory_configurations.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_item_types.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_admin_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventories.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_inventory_configurations.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_item_types.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_item_types.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_items.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk/api/inventory/wrappers/_public_tags.py` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk/api/inventory/wrappers/_public_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk_service_inventory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-inventory
-Version: 0.5.0
+Version: 0.6.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Inventory Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Inventory Service
-* Version: 0.1.3
+* Version: 0.1.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_inventory-0.5.0/accelbyte_py_sdk_service_inventory.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_inventory-0.6.0/accelbyte_py_sdk_service_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

