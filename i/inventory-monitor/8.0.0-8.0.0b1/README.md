# Comparing `tmp/inventory-monitor-8.0.0.tar.gz` & `tmp/inventory-monitor-8.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventory-monitor-8.0.0.tar", last modified: Tue May 21 09:39:34 2024, max compression
+gzip compressed data, was "inventory-monitor-8.0.0b1.tar", last modified: Wed May 15 10:21:42 2024, max compression
```

## Comparing `inventory-monitor-8.0.0.tar` & `inventory-monitor-8.0.0b1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.108183 inventory-monitor-8.0.0/
--rw-r--r--   0 root         (0) root         (0)       66 2022-08-17 08:16:04.000000 inventory-monitor-8.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      573 2024-05-21 09:39:34.108183 inventory-monitor-8.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2022-11-11 11:56:29.000000 inventory-monitor-8.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.100183 inventory-monitor-8.0.0/inventory_monitor/
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.104183 inventory-monitor-8.0.0/inventory_monitor/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 10:45:32.000000 inventory-monitor-8.0.0/inventory_monitor/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7075 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/api/serializers.py
--rw-r--r--   0 root         (0) root         (0)      496 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/api/urls.py
--rw-r--r--   0 root         (0) root         (0)     1630 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/api/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.104183 inventory-monitor-8.0.0/inventory_monitor/filtersets/
--rw-r--r--   0 root         (0) root         (0)      319 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/filtersets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7346 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/filtersets/component.py
--rw-r--r--   0 root         (0) root         (0)     5525 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/filtersets/component_service.py
--rw-r--r--   0 root         (0) root         (0)     6369 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/filtersets/contract.py
--rw-r--r--   0 root         (0) root         (0)     2290 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/filtersets/contractor.py
--rw-r--r--   0 root         (0) root         (0)     4622 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/filtersets/invoice.py
--rw-r--r--   0 root         (0) root         (0)     5305 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/filtersets/probe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.104183 inventory-monitor-8.0.0/inventory_monitor/forms/
--rw-r--r--   0 root         (0) root         (0)      289 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/forms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6698 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/forms/component.py
--rw-r--r--   0 root         (0) root         (0)     4418 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/forms/component_service.py
--rw-r--r--   0 root         (0) root         (0)     4684 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/forms/contract.py
--rw-r--r--   0 root         (0) root         (0)      766 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/forms/contractor.py
--rw-r--r--   0 root         (0) root         (0)     2876 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/forms/invoice.py
--rw-r--r--   0 root         (0) root         (0)     3479 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/forms/probe.py
--rw-r--r--   0 root         (0) root         (0)      463 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/graphql.py
--rw-r--r--   0 root         (0) root         (0)     1811 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.104183 inventory-monitor-8.0.0/inventory_monitor/migrations/
--rw-r--r--   0 root         (0) root         (0)     2329 2022-09-01 10:14:20.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     3198 2022-11-02 08:30:17.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0002_contractor_contract.py
--rw-r--r--   0 root         (0) root         (0)     1811 2022-11-11 11:48:13.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
--rw-r--r--   0 root         (0) root         (0)      342 2022-11-11 11:48:53.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0004_delete_invmonfileattachment.py
--rw-r--r--   0 root         (0) root         (0)     1840 2022-11-22 11:20:11.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0005_invoice.py
--rw-r--r--   0 root         (0) root         (0)      409 2022-12-01 11:16:30.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0006_invoice_project.py
--rw-r--r--   0 root         (0) root         (0)     5622 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0008_componentservice_comments.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0009_alter_component_items.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-03-27 12:15:02.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-03-27 12:09:05.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-03 15:32:31.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0012_probe_creation_time.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 12:29:41.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/0013_alter_probe_creation_time.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-22 08:26:09.000000 inventory-monitor-8.0.0/inventory_monitor/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.104183 inventory-monitor-8.0.0/inventory_monitor/models/
--rw-r--r--   0 root         (0) root         (0)      296 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2950 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/models/component.py
--rw-r--r--   0 root         (0) root         (0)     1850 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/models/component_service.py
--rw-r--r--   0 root         (0) root         (0)     3444 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/models/contract.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/models/contractor.py
--rw-r--r--   0 root         (0) root         (0)     1907 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/models/invoice.py
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/models/probe.py
--rw-r--r--   0 root         (0) root         (0)     1187 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/navigation.py
--rw-r--r--   0 root         (0) root         (0)     1453 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.104183 inventory-monitor-8.0.0/inventory_monitor/tables/
--rw-r--r--   0 root         (0) root         (0)      296 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/tables/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1434 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/tables/component.py
--rw-r--r--   0 root         (0) root         (0)      857 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/tables/component_service.py
--rw-r--r--   0 root         (0) root         (0)     1132 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/tables/contract.py
--rw-r--r--   0 root         (0) root         (0)      487 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/tables/contractor.py
--rw-r--r--   0 root         (0) root         (0)      864 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/tables/invoice.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/tables/probe.py
--rw-r--r--   0 root         (0) root         (0)     2049 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/template_content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.100183 inventory-monitor-8.0.0/inventory_monitor/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.108183 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-15 12:39:23.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-03-27 12:07:28.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/component.html
--rw-r--r--   0 root         (0) root         (0)     2988 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/componentservice.html
--rw-r--r--   0 root         (0) root         (0)     6537 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/contract.html
--rw-r--r--   0 root         (0) root         (0)     2109 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/contractor.html
--rw-r--r--   0 root         (0) root         (0)     1558 2023-04-13 10:27:02.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html
--rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 13:55:51.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/import_component_button.html
--rw-r--r--   0 root         (0) root         (0)     2238 2022-11-23 07:44:17.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
--rw-r--r--   0 root         (0) root         (0)     2301 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/invoice.html
--rw-r--r--   0 root         (0) root         (0)     5690 2023-04-04 12:47:57.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/probe.html
--rw-r--r--   0 root         (0) root         (0)     3146 2023-06-06 11:41:23.000000 inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/probe_diff.html
--rw-r--r--   0 root         (0) root         (0)     4203 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/urls.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.108183 inventory-monitor-8.0.0/inventory_monitor/views/
--rw-r--r--   0 root         (0) root         (0)      290 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/views/component.py
--rw-r--r--   0 root         (0) root         (0)     2052 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/views/component_service.py
--rw-r--r--   0 root         (0) root         (0)     7164 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/views/contract.py
--rw-r--r--   0 root         (0) root         (0)     2582 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/views/contractor.py
--rw-r--r--   0 root         (0) root         (0)     1862 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/views/invoice.py
--rw-r--r--   0 root         (0) root         (0)     2096 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/inventory_monitor/views/probe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:39:34.100183 inventory-monitor-8.0.0/inventory_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      573 2024-05-21 09:39:34.000000 inventory-monitor-8.0.0/inventory_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3548 2024-05-21 09:39:34.000000 inventory-monitor-8.0.0/inventory_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:39:34.000000 inventory-monitor-8.0.0/inventory_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:55:56.000000 inventory-monitor-8.0.0/inventory_monitor.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-21 09:39:34.000000 inventory-monitor-8.0.0/inventory_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 09:39:34.108183 inventory-monitor-8.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1217 2024-05-21 09:39:12.000000 inventory-monitor-8.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-17 08:16:04.000000 inventory-monitor-8.0.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2022-11-11 11:56:29.000000 inventory-monitor-8.0.0b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor/
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 10:45:32.000000 inventory-monitor-8.0.0b1/inventory_monitor/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7075 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/api/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      496 2024-05-15 08:27:14.000000 inventory-monitor-8.0.0b1/inventory_monitor/api/urls.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/api/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-15 08:24:02.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7346 2024-05-15 08:24:36.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/component.py
+-rw-r--r--   0 root         (0) root         (0)     5525 2024-05-15 08:24:24.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2024-05-15 08:24:38.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/contract.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2024-05-15 08:24:40.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/contractor.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2024-05-15 08:24:43.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     5305 2024-05-15 08:24:46.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/probe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor/forms/
+-rw-r--r--   0 root         (0) root         (0)      289 2024-05-15 08:23:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6698 2024-05-15 10:03:15.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/component.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2024-05-15 10:03:19.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2024-05-15 10:03:13.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/contract.py
+-rw-r--r--   0 root         (0) root         (0)      766 2024-05-15 10:00:52.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/contractor.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-05-15 10:03:10.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2024-05-15 10:03:03.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/probe.py
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/graphql.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.687589 inventory-monitor-8.0.0b1/inventory_monitor/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2329 2022-09-01 10:14:20.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2022-11-02 08:30:17.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0002_contractor_contract.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2022-11-11 11:48:13.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
+-rw-r--r--   0 root         (0) root         (0)      342 2022-11-11 11:48:53.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0004_delete_invmonfileattachment.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2022-11-22 11:20:11.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0005_invoice.py
+-rw-r--r--   0 root         (0) root         (0)      409 2022-12-01 11:16:30.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0006_invoice_project.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0008_componentservice_comments.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0009_alter_component_items.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-03-27 12:15:02.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-03-27 12:09:05.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0011_alter_component_options_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-03 15:32:31.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0012_probe_creation_time.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 12:29:41.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0013_alter_probe_creation_time.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-22 08:26:09.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.687589 inventory-monitor-8.0.0b1/inventory_monitor/models/
+-rw-r--r--   0 root         (0) root         (0)      296 2024-05-15 08:20:10.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/component.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-05-15 08:12:07.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/contract.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/contractor.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/probe.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/navigation.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.687589 inventory-monitor-8.0.0b1/inventory_monitor/tables/
+-rw-r--r--   0 root         (0) root         (0)      296 2024-05-15 08:23:40.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/component.py
+-rw-r--r--   0 root         (0) root         (0)      857 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/contract.py
+-rw-r--r--   0 root         (0) root         (0)      487 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/contractor.py
+-rw-r--r--   0 root         (0) root         (0)      864 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/invoice.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/probe.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/template_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.679589 inventory-monitor-8.0.0b1/inventory_monitor/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-15 12:39:23.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-03-27 12:07:28.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/component.html
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/componentservice.html
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/contract.html
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/contractor.html
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-04-13 10:27:02.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/device_probes_include.html
+-rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 13:55:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/import_component_button.html
+-rw-r--r--   0 root         (0) root         (0)     2238 2022-11-23 07:44:17.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/invoice.html
+-rw-r--r--   0 root         (0) root         (0)     5690 2023-04-04 12:47:57.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/probe.html
+-rw-r--r--   0 root         (0) root         (0)     3146 2023-06-06 11:41:23.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/probe_diff.html
+-rw-r--r--   0 root         (0) root         (0)     4203 2024-05-15 08:22:10.000000 inventory-monitor-8.0.0b1/inventory_monitor/urls.py
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/inventory_monitor/views/
+-rw-r--r--   0 root         (0) root         (0)      290 2024-05-15 08:23:28.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/component.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/contract.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/contractor.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/probe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-15 10:21:42.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3548 2024-05-15 10:21:42.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:21:42.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:55:56.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-15 10:21:42.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/setup.py
```

### Comparing `inventory-monitor-8.0.0/PKG-INFO` & `inventory-monitor-8.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventory-monitor
-Version: 8.0.0
+Version: 8.0.0b1
 Summary: Asset Management with semi-auto discovery processes
 Home-page: https://gitlab.cesnet.cz/701/done/inventory-monitor-plugin
 Author: Jan Krupa
 License: UNKNOWN
 Keywords: netbox,netbox-plugin
 Platform: UNKNOWN
 Classifier: Framework :: Django
```

### Comparing `inventory-monitor-8.0.0/inventory_monitor/api/serializers.py` & `inventory-monitor-8.0.0b1/inventory_monitor/api/serializers.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/api/views.py` & `inventory-monitor-8.0.0b1/inventory_monitor/api/views.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/filtersets/component.py` & `inventory-monitor-8.0.0b1/inventory_monitor/filtersets/component.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/filtersets/component_service.py` & `inventory-monitor-8.0.0b1/inventory_monitor/filtersets/component_service.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/filtersets/contract.py` & `inventory-monitor-8.0.0b1/inventory_monitor/filtersets/contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/filtersets/contractor.py` & `inventory-monitor-8.0.0b1/inventory_monitor/filtersets/contractor.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/filtersets/invoice.py` & `inventory-monitor-8.0.0b1/inventory_monitor/filtersets/invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/filtersets/probe.py` & `inventory-monitor-8.0.0b1/inventory_monitor/filtersets/probe.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/forms/component.py` & `inventory-monitor-8.0.0b1/inventory_monitor/forms/component.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/forms/component_service.py` & `inventory-monitor-8.0.0b1/inventory_monitor/forms/component_service.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/forms/contract.py` & `inventory-monitor-8.0.0b1/inventory_monitor/forms/contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/forms/contractor.py` & `inventory-monitor-8.0.0b1/inventory_monitor/forms/contractor.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/forms/invoice.py` & `inventory-monitor-8.0.0b1/inventory_monitor/forms/invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/forms/probe.py` & `inventory-monitor-8.0.0b1/inventory_monitor/forms/probe.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/helpers.py` & `inventory-monitor-8.0.0b1/inventory_monitor/helpers.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/migrations/0001_initial.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/migrations/0002_contractor_contract.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0002_contractor_contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/migrations/0005_invoice.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0005_invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0011_alter_component_options_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/models/component.py` & `inventory-monitor-8.0.0b1/inventory_monitor/models/component.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/models/component_service.py` & `inventory-monitor-8.0.0b1/inventory_monitor/models/component_service.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/models/contract.py` & `inventory-monitor-8.0.0b1/inventory_monitor/models/contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/models/contractor.py` & `inventory-monitor-8.0.0b1/inventory_monitor/models/contractor.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/models/invoice.py` & `inventory-monitor-8.0.0b1/inventory_monitor/models/invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/models/probe.py` & `inventory-monitor-8.0.0b1/inventory_monitor/models/probe.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/navigation.py` & `inventory-monitor-8.0.0b1/inventory_monitor/navigation.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/search.py` & `inventory-monitor-8.0.0b1/inventory_monitor/search.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/tables/component.py` & `inventory-monitor-8.0.0b1/inventory_monitor/tables/component.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/tables/component_service.py` & `inventory-monitor-8.0.0b1/inventory_monitor/tables/component_service.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/tables/contract.py` & `inventory-monitor-8.0.0b1/inventory_monitor/tables/contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/tables/invoice.py` & `inventory-monitor-8.0.0b1/inventory_monitor/tables/invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/tables/probe.py` & `inventory-monitor-8.0.0b1/inventory_monitor/tables/probe.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/template_content.py` & `inventory-monitor-8.0.0b1/inventory_monitor/template_content.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/component.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/component.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/componentservice.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/componentservice.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/contract.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/contract.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/contractor.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/contractor.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/device_probes_include.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/invoice.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/invoice.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/probe.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/probe.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/templates/inventory_monitor/probe_diff.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/probe_diff.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/urls.py` & `inventory-monitor-8.0.0b1/inventory_monitor/urls.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/views/component.py` & `inventory-monitor-8.0.0b1/inventory_monitor/views/component.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/views/component_service.py` & `inventory-monitor-8.0.0b1/inventory_monitor/views/component_service.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/views/contract.py` & `inventory-monitor-8.0.0b1/inventory_monitor/views/contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/views/contractor.py` & `inventory-monitor-8.0.0b1/inventory_monitor/views/contractor.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/views/invoice.py` & `inventory-monitor-8.0.0b1/inventory_monitor/views/invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor/views/probe.py` & `inventory-monitor-8.0.0b1/inventory_monitor/views/probe.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/inventory_monitor.egg-info/PKG-INFO` & `inventory-monitor-8.0.0b1/inventory_monitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventory-monitor
-Version: 8.0.0
+Version: 8.0.0b1
 Summary: Asset Management with semi-auto discovery processes
 Home-page: https://gitlab.cesnet.cz/701/done/inventory-monitor-plugin
 Author: Jan Krupa
 License: UNKNOWN
 Keywords: netbox,netbox-plugin
 Platform: UNKNOWN
 Classifier: Framework :: Django
```

### Comparing `inventory-monitor-8.0.0/inventory_monitor.egg-info/SOURCES.txt` & `inventory-monitor-8.0.0b1/inventory_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventory-monitor-8.0.0/setup.py` & `inventory-monitor-8.0.0b1/setup.py`

 * *Files identical despite different names*

