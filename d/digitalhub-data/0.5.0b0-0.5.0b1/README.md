# Comparing `tmp/digitalhub_data-0.5.0b0.tar.gz` & `tmp/digitalhub_data-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_data-0.5.0b0.tar", last modified: Mon May 20 12:48:40 2024, max compression
+gzip compressed data, was "digitalhub_data-0.5.0b1.tar", last modified: Tue May 21 15:54:06 2024, max compression
```

## Comparing `digitalhub_data-0.5.0b0.tar` & `digitalhub_data-0.5.0b1.tar`

### file list

```diff
@@ -1,44 +1,62 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.010801 digitalhub_data-0.5.0b0/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-20 12:48:40.010801 digitalhub_data-0.5.0b0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.006801 digitalhub_data-0.5.0b0/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-20 09:51:09.000000 digitalhub_data-0.5.0b0/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.006801 digitalhub_data-0.5.0b0/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.006801 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-20 09:51:09.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6484 2024-05-20 09:51:09.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.006801 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6975 2024-05-20 09:51:09.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2994 2024-05-06 09:59:04.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      415 2024-05-06 11:22:14.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.006801 digitalhub_data-0.5.0b0/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-20 09:51:09.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6000 2024-05-20 09:51:09.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      773 2024-05-06 11:19:40.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.010801 digitalhub_data-0.5.0b0/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.5.0b0/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.010801 digitalhub_data-0.5.0b0/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.5.0b0/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.5.0b0/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:40.010801 digitalhub_data-0.5.0b0/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-20 12:48:39.000000 digitalhub_data-0.5.0b0/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1346 2024-05-20 12:48:40.000000 digitalhub_data-0.5.0b0/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-20 12:48:39.000000 digitalhub_data-0.5.0b0/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-20 12:48:39.000000 digitalhub_data-0.5.0b0/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-20 12:48:39.000000 digitalhub_data-0.5.0b0/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-05-20 07:16:51.000000 digitalhub_data-0.5.0b0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-20 12:48:40.010801 digitalhub_data-0.5.0b0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.150311 digitalhub_data-0.5.0b1/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.150311 digitalhub_data-0.5.0b1/digitalhub_data/datastores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:15.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3283 2024-05-21 13:54:52.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.154312 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:57.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3442 2024-05-21 14:03:19.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1507 2024-05-21 13:34:40.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      826 2024-05-21 13:34:45.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1353 2024-05-21 13:34:51.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2016 2024-05-21 13:34:58.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.154312 digitalhub_data-0.5.0b1/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.154312 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6484 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6975 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2972 2024-05-21 13:35:17.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      415 2024-05-06 11:22:14.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6000 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      773 2024-05-06 11:19:40.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/readers/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:54:41.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1148 2024-05-21 12:30:09.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 10:51:19.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      667 2024-05-21 13:09:30.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1902 2024-05-21 13:14:39.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/pandas.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      278 2024-05-21 12:28:44.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/registry.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.5.0b1/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.5.0b1/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1918 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       52 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1130 2024-05-21 15:33:27.000000 digitalhub_data-0.5.0b1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/setup.cfg
```

### Comparing `digitalhub_data-0.5.0b0/PKG-INFO` & `digitalhub_data-0.5.0b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.5.0b0
+Version: 0.5.0b1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-core~=0.5
+Requires-Dist: digitalhub-core==0.5.0b1
+Provides-Extra: pandas
+Requires-Dist: pandas<2.2,>=1.2; extra == "pandas"
 
 # Digitalhub-data Library
 
 The Digitalhub-data SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-data layer is the second layer of the Digitalhub Data platform, focused on operations on data.
 It contains the data entities and objects (Dataitems) and the methods to manage them.
```

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/builder.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/crud.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from __future__ import annotations
 
 import shutil
 import typing
 from pathlib import Path
+from typing import Any
 
-from digitalhub_core.stores.builder import get_default_store, get_store
+from digitalhub_data.datastores.builder import get_default_datastore, get_datastore
 from digitalhub_data.entities.dataitems.entity._base import Dataitem
 
-if typing.TYPE_CHECKING:
-    import pandas as pd
-
 
 class DataitemTable(Dataitem):
 
     """
     Table dataitem.
     """
 
-    def as_df(self, file_format: str | None = None, **kwargs) -> pd.DataFrame:
+    def as_df(self, file_format: str | None = None, **kwargs) -> Any:
         """
         Read dataitem as a pandas DataFrame. If the dataitem is not local, it will be downloaded
         to a temporary folder and deleted after the method is executed. If no file_format is passed,
         the function will try to infer it from the dataitem.spec.path attribute.
         The path of the dataitem is specified in the spec attribute, and must be a store aware path.
         If the dataitem is stored on s3 bucket, the path must be s3://<bucket>/<path_to_dataitem>.
         If the dataitem is stored on database (Postgres is the only one supported), the path must
@@ -32,61 +30,61 @@
         file_format : str
             Format of the file. (Supported csv and parquet).
         **kwargs
             Keyword arguments.
 
         Returns
         -------
-        pd.DataFrame
-            Pandas DataFrame.
+        Any
+            DataFrame.
         """
-        store = get_store(self.spec.path)
+        datastore = get_datastore(self.spec.path)
         tmp_path = False
 
         # Download dataitem if not local
         if not self._check_local(self.spec.path):
-            path = store.download(self.spec.path)
+            path = datastore.download(self.spec.path)
             tmp_path = True
         else:
             path = self.spec.path
 
         # Check file format and get dataitem as DataFrame
         extension = self._get_extension(self.spec.path, file_format)
-        df = store.read_df(path, extension, **kwargs)
+        df = datastore.read_df(path, extension, **kwargs)
 
         # Delete tmp folder
         if tmp_path:
             pth = Path(path)
             if pth.is_file():
                 pth = pth.parent
             shutil.rmtree(pth)
 
         return df
 
-    def write_df(self, target_path: str | None = None, df: pd.DataFrame | None = None, **kwargs) -> str:
+    def write_df(self, target_path: str | None = None, df: Any | None = None, **kwargs) -> str:
         """
         Write pandas DataFrame as parquet.
         If no target_path is passed, the dataitem will be written into the default store.
         If no DataFrame is passed, the dataitem will be written into the target_path.
 
         Parameters
         ----------
         target_path : str
             Path to write the dataframe to
-        df : pd.DataFrame
+        df : Any
             DataFrame to write.
         **kwargs
             Keyword arguments.
 
         Returns
         -------
         str
             Path to the written dataframe.
         """
         if target_path is None:
             target_path = f"{self.project}/{self.ENTITY_TYPE}/{self.kind}/{self.name}.parquet"
-            store = get_default_store()
+            datastore = get_default_datastore()
         else:
-            store = get_store(target_path)
+            datastore = get_datastore(target_path)
         if df is None:
             df = self.as_df()
-        return store.write_df(df, target_path, **kwargs)
+        return datastore.write_df(df, target_path, **kwargs)
```

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/models.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/spec.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/dataitems/status.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/projects/crud.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/projects/entity.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/projects/spec.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/entities/registries.py` & `digitalhub_data-0.5.0b1/digitalhub_data/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data/utils/data_utils.py` & `digitalhub_data-0.5.0b1/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data.egg-info/PKG-INFO` & `digitalhub_data-0.5.0b1/digitalhub_data.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.5.0b0
+Version: 0.5.0b1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-core~=0.5
+Requires-Dist: digitalhub-core==0.5.0b1
+Provides-Extra: pandas
+Requires-Dist: pandas<2.2,>=1.2; extra == "pandas"
 
 # Digitalhub-data Library
 
 The Digitalhub-data SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-data layer is the second layer of the Digitalhub Data platform, focused on operations on data.
 It contains the data entities and objects (Dataitems) and the methods to manage them.
```

### Comparing `digitalhub_data-0.5.0b0/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub_data-0.5.0b1/digitalhub_data.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 pyproject.toml
 digitalhub_data/__init__.py
 digitalhub_data.egg-info/PKG-INFO
 digitalhub_data.egg-info/SOURCES.txt
 digitalhub_data.egg-info/dependency_links.txt
 digitalhub_data.egg-info/requires.txt
 digitalhub_data.egg-info/top_level.txt
+digitalhub_data/datastores/__init__.py
+digitalhub_data/datastores/builder.py
+digitalhub_data/datastores/objects/__init__.py
+digitalhub_data/datastores/objects/base.py
+digitalhub_data/datastores/objects/local.py
+digitalhub_data/datastores/objects/remote.py
+digitalhub_data/datastores/objects/s3.py
+digitalhub_data/datastores/objects/sql.py
 digitalhub_data/entities/__init__.py
 digitalhub_data/entities/entity_types.py
 digitalhub_data/entities/registries.py
 digitalhub_data/entities/dataitems/__init__.py
 digitalhub_data/entities/dataitems/builder.py
 digitalhub_data/entities/dataitems/crud.py
 digitalhub_data/entities/dataitems/metadata.py
@@ -25,9 +33,15 @@
 digitalhub_data/entities/projects/crud.py
 digitalhub_data/entities/projects/entity.py
 digitalhub_data/entities/projects/spec.py
 digitalhub_data/entities/runs/__init__.py
 digitalhub_data/entities/runs/models.py
 digitalhub_data/entities/runs/spec.py
 digitalhub_data/entities/runs/status.py
+digitalhub_data/readers/__init__.py
+digitalhub_data/readers/builder.py
+digitalhub_data/readers/registry.py
+digitalhub_data/readers/objects/__init__.py
+digitalhub_data/readers/objects/base.py
+digitalhub_data/readers/objects/pandas.py
 digitalhub_data/utils/__init__.py
 digitalhub_data/utils/data_utils.py
```

### Comparing `digitalhub_data-0.5.0b0/pyproject.toml` & `digitalhub_data-0.5.0b1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
-version = "0.5.0b0"
+version = "0.5.0b1"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -16,22 +16,26 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["data", "dataops", "kubernetes"]
 requires-python = ">=3.9"
 dependencies = [
-    "digitalhub-core~=0.5",
+    "digitalhub-core==0.5.0b1",
+]
+[project.optional-dependencies]
+pandas = [
+    "pandas>=1.2, <2.2",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.5.0b0"
+current_version = "0.5.0b1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

