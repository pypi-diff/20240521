# Comparing `tmp/odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.tar.gz` & `tmp/odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.tar", last modified: Tue May 21 08:56:36 2024, max compression
+gzip compressed data, was "odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1.tar", last modified: Fri Nov 10 13:30:36 2023, max compression
```

## Comparing `odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.tar` & `odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1.tar`

### file list

```diff
@@ -1,29 +1,11 @@
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.315971 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      507 2024-05-21 08:56:36.315971 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/PKG-INFO
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.311970 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.311970 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.311970 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/
--rwxrwxr-x   0 jrobles   (1001) jrobles   (1001)       68 2023-12-19 17:24:31.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/__init__.py
--rwxrwxr-x   0 jrobles   (1001) jrobles   (1001)      690 2024-05-21 08:47:10.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/__manifest__.py
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.311970 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/models/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       76 2023-12-19 17:24:31.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/models/__init__.py
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      754 2023-12-19 17:24:31.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/models/models_sm_company.py
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      879 2023-12-19 17:24:31.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/models/models_sm_res_config_settings.py
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.311970 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/services/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       34 2023-12-19 17:24:31.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/services/__init__.py
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     7592 2024-05-21 08:45:37.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/services/cs_invoice_services.py
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     1777 2024-02-01 15:41:51.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/services/schemas.py
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.311970 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/tests/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       38 2024-03-07 10:39:57.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/tests/__init__.py
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     3675 2024-03-07 10:39:57.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/tests/test_cs_invoice_services.py
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.311970 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/views/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      960 2023-12-19 17:24:31.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo/addons/sm_partago_invoicing_rest_api/views/views_res_config_settings.xml
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-21 08:56:36.311970 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      507 2024-05-21 08:56:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/PKG-INFO
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     1140 2024-05-21 08:56:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        1 2024-05-21 08:56:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        1 2024-01-29 11:32:43.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/not-zip-safe
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       93 2024-05-21 08:56:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/requires.txt
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        5 2024-05-21 08:56:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/top_level.txt
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       38 2024-05-21 08:56:36.315971 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/setup.cfg
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      100 2023-12-19 17:24:31.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8/setup.py
+drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-11-10 13:30:36.946740 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/
+-rw-r--r--   0 carla     (1000) carla     (1000)      512 2023-11-10 13:30:36.946740 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/PKG-INFO
+drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-11-10 13:30:36.946740 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/
+-rw-r--r--   0 carla     (1000) carla     (1000)      512 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 carla     (1000) carla     (1000)      402 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 carla     (1000) carla     (1000)        1 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 carla     (1000) carla     (1000)        1 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/not-zip-safe
+-rw-r--r--   0 carla     (1000) carla     (1000)       93 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/requires.txt
+-rw-r--r--   0 carla     (1000) carla     (1000)        5 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/top_level.txt
+-rw-r--r--   0 carla     (1000) carla     (1000)       38 2023-11-10 13:30:36.946740 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/setup.cfg
+-rw-r--r--   0 carla     (1000) carla     (1000)      100 2023-11-10 13:29:57.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/setup.py
```

