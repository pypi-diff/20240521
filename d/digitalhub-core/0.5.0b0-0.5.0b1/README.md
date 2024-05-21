# Comparing `tmp/digitalhub_core-0.5.0b0.tar.gz` & `tmp/digitalhub_core-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_core-0.5.0b0.tar", last modified: Mon May 20 12:48:09 2024, max compression
+gzip compressed data, was "digitalhub_core-0.5.0b1.tar", last modified: Tue May 21 15:53:29 2024, max compression
```

## Comparing `digitalhub_core-0.5.0b0.tar` & `digitalhub_core-0.5.0b1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.5.0b0/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.190919 digitalhub_core-0.5.0b0/digitalhub_core/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.190919 digitalhub_core-0.5.0b0/digitalhub_core/client/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.190919 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/dhcore.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16292 2024-05-13 12:38:37.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/local.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.190919 digitalhub_core-0.5.0b0/digitalhub_core/context/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/context/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.5.0b0/digitalhub_core/context/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/context/context.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.194919 digitalhub_core-0.5.0b0/digitalhub_core/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.194919 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.194919 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1435 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1748 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.194919 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6641 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14010 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.198919 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6298 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16737 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.198919 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8705 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    22032 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      927 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.198919 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4897 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14326 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3532 2024-05-09 11:08:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2620 2024-05-13 12:22:42.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.198919 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6160 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8742 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5550 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10643 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6358 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16023 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/registry/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/registry/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/registry/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/registry/registry.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3714 2024-05-06 11:10:35.000000 digitalhub_core-0.5.0b0/digitalhub_core/registry/utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/runtimes/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1005 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b0/digitalhub_core/runtimes/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/stores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-04-19 08:14:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-04-19 08:14:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-04-19 08:14:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-04-19 08:14:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/digitalhub_core/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/api.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/env_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/exceptions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/file_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/generic_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/git_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/io_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/logger.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/uri_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3901 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-05-20 07:16:51.000000 digitalhub_core-0.5.0b0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.509397 digitalhub_core-0.5.0b1/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.5.0b1/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14995 2024-05-21 15:53:29.509397 digitalhub_core-0.5.0b1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.485396 digitalhub_core-0.5.0b1/digitalhub_core/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.485396 digitalhub_core-0.5.0b1/digitalhub_core/client/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.489396 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/dhcore.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16292 2024-05-13 12:38:37.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/local.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.489396 digitalhub_core-0.5.0b1/digitalhub_core/context/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/context/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.5.0b1/digitalhub_core/context/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/context/context.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.489396 digitalhub_core-0.5.0b1/digitalhub_core/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.493396 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.493396 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1435 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1748 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.493396 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6641 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14010 2024-05-21 13:14:46.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.497396 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6298 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16737 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.497396 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8705 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    22032 2024-05-21 13:14:46.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      927 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.497396 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4897 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14326 2024-05-21 13:14:46.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3532 2024-05-09 11:08:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2620 2024-05-13 12:22:42.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.501397 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6160 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8742 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.501397 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5550 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10643 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.501397 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6358 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16023 2024-05-21 13:14:46.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.501397 digitalhub_core-0.5.0b1/digitalhub_core/registry/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/registry/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/registry/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/registry/registry.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3714 2024-05-06 11:10:35.000000 digitalhub_core-0.5.0b1/digitalhub_core/registry/utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/runtimes/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1005 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/runtimes/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core/stores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3635 2024-05-21 14:15:02.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3623 2024-05-21 14:15:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4548 2024-05-21 14:15:53.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7995 2024-05-21 14:16:16.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     9035 2024-05-21 15:25:40.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/api.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/env_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/exceptions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/file_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/generic_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/git_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/io_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/logger.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/uri_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14995 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3901 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1687 2024-05-21 15:31:37.000000 digitalhub_core-0.5.0b1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-21 15:53:29.509397 digitalhub_core-0.5.0b1/setup.cfg
```

### Comparing `digitalhub_core-0.5.0b0/LICENSE.txt` & `digitalhub_core-0.5.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/PKG-INFO` & `digitalhub_core-0.5.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.5.0b0
+Version: 0.5.0b1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,17 +225,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: boto3
-Requires-Dist: aiobotocore
 Requires-Dist: pydantic>=1.10.8,~=1.10
-Requires-Dist: pandas<2.2,>=1.2
 Requires-Dist: sqlalchemy~=1.4
 Requires-Dist: psycopg2-binary~=2.8
 Requires-Dist: pyarrow<15,>=10.0
 Requires-Dist: requests~=2.31
 Requires-Dist: PyYAML~=5.1
 Requires-Dist: GitPython>=3
 Provides-Extra: dev
```

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/__init__.py` & `digitalhub_core-0.5.0b1/digitalhub_core/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/client/builder.py` & `digitalhub_core-0.5.0b1/digitalhub_core/client/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/client/objects/base.py` & `digitalhub_core-0.5.0b1/digitalhub_core/client/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/client/objects/dhcore.py` & `digitalhub_core-0.5.0b1/digitalhub_core/client/objects/dhcore.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/client/objects/local.py` & `digitalhub_core-0.5.0b1/digitalhub_core/client/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/context/builder.py` & `digitalhub_core-0.5.0b1/digitalhub_core/context/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/context/context.py` & `digitalhub_core-0.5.0b1/digitalhub_core/context/context.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/base.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/entity.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/metadata.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/spec.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/status.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/metadata.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/spec.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/status.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/crud.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/entity.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/spec.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/crud.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/entity.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/spec.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/crud.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/entity.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/spec.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/registries.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/crud.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/entity.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/spec.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/status.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/crud.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/entity.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/spec.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/crud.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/entity.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/models.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/crud.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/entity.py` & `digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/registry/models.py` & `digitalhub_core-0.5.0b1/digitalhub_core/registry/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/registry/registry.py` & `digitalhub_core-0.5.0b1/digitalhub_core/registry/registry.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/registry/utils.py` & `digitalhub_core-0.5.0b1/digitalhub_core/registry/utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/runtimes/base.py` & `digitalhub_core-0.5.0b1/digitalhub_core/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/runtimes/builder.py` & `digitalhub_core-0.5.0b1/digitalhub_core/runtimes/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/stores/builder.py` & `digitalhub_core-0.5.0b1/digitalhub_core/stores/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/base.py` & `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/remote.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,202 +1,175 @@
 """
-Store module.
+Remote store module.
 """
 from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
+import typing
 from pathlib import Path
-from tempfile import mkdtemp
-from typing import Literal
 
-import pandas as pd
-from digitalhub_core.utils.exceptions import StoreError
-from digitalhub_core.utils.uri_utils import map_uri_scheme
-from pydantic import BaseModel
+import requests
+from digitalhub_core.stores.objects.base import Store, StoreConfig
 
 
-class Store(metaclass=ABCMeta):
+class RemoteStoreConfig(StoreConfig):
     """
-    Store abstract class.
+    Remote store configuration class.
     """
 
-    def __init__(self, name: str, store_type: str) -> None:
+
+class RemoteStore(Store):
+    """
+    HTTP store class. It implements the Store interface and provides methods to fetch
+    artifacts from remote HTTP based storage.
+    """
+
+    def __init__(self, name: str, store_type: str, config: RemoteStoreConfig) -> None:
         """
         Constructor.
 
         Parameters
         ----------
-        name : str
-            Store name.
-        store_type : str
-            Store type. Used to choose the right store implementation.
-        uri : str
-            Store URI.
+        config : RemoteStoreConfig
+            Remote store configuration.
 
-        Returns
-        -------
-        None
+        See Also
+        --------
+        Store.__init__
         """
-        self.name = name
-        self.type = store_type
-
-        # Private attributes
-        self._registry: dict[str, str] = {}
+        super().__init__(name, store_type)
+        self.config = config
 
     ############################
     # IO methods
     ############################
 
-    @abstractmethod
     def download(self, src: str, dst: str | None = None) -> str:
         """
-        Method to download artifact from storage.
-        """
+        Method to download an artifact from backend.
 
-    @abstractmethod
-    def fetch_artifact(self, src: str, dst: str | None = None) -> str:
-        """
-        Method to fetch artifact from storage.
-        """
-
-    @abstractmethod
-    def upload(self, src: str, dst: str | None = None) -> str:
-        """
-        Method to upload artifact to storage.
-        """
-
-    @abstractmethod
-    def persist_artifact(self, src: str, dst: str | None = None) -> str:
-        """
-        Method to persist artifact in storage.
-        """
+        Parameters
+        ----------
+        src : str
+            The source location of the artifact.
+        dst : str
+            The destination of the artifact.
 
-    @abstractmethod
-    def write_df(self, df: pd.DataFrame, dst: str | None = None, **kwargs) -> str:
-        """
-        Write pandas DataFrame as parquet or csv.
+        Returns
+        -------
+        str
+            The path of the downloaded artifact.
         """
+        return self._registry.get(src, self.fetch_artifact(src, dst))
 
-    @staticmethod
-    def read_df(path: str, extension: str, **kwargs) -> pd.DataFrame:
+    def fetch_artifact(self, src: str, dst: str | None = None) -> str:
         """
-        Read DataFrame from path.
+        Method to fetch an artifact from the remote storage and to register
+        it on the paths registry.
+        If the destination is not provided, a temporary folder will be created.
 
         Parameters
         ----------
-        path : str
-            Path to read DataFrame from.
-        extension : str
-            Extension of the file.
-        **kwargs
-            Keyword arguments.
+        src : str
+            The source location of the artifact.
+        dst : str
+            The destination of the artifact.
 
         Returns
         -------
-        pd.DataFrame
-            Pandas DataFrame.
+        str
+            Returns the path of the artifact.
+        """
+        dst = dst if dst is not None else self._build_temp("remote")
+        if not dst.endswith(".csv") and not dst.endswith(".parquet"):
+            dst = str(Path(dst) / "temp.file")
+        return self._download_file(src, dst)
+
+    def upload(self, src: str, dst: str | None = None) -> str:
+        """
+        Method to upload an artifact to the backend. Please note that this method is not implemented
+        since the remote store is not meant to upload artifacts.
 
         Raises
         ------
-        ValueError
-            If format is not supported.
+        NotImplementedError
+            This method is not implemented.
         """
-        if extension == "csv":
-            return pd.read_csv(path, **kwargs)
-        if extension == "parquet":
-            return pd.read_parquet(path, **kwargs)
-        raise ValueError(f"Format {extension} not supported.")
-
-    ############################
-    # Helpers methods
-    ############################
+        raise NotImplementedError("Remote store does not support upload.")
 
-    def _check_local_dst(self, dst: str) -> None:
+    def persist_artifact(self, src: str, dst: str | None = None) -> str:
         """
-        Check if the local destination directory exists. Create in case it does not.
-
-        Parameters
-        ----------
-        dst : str
-            The destination directory.
-
-        Returns
-        -------
-        None
+        Method to persist an artifact. Note that this method is not implemented
+        since the remote store is not meant to write artifacts.
 
         Raises
         ------
-        StoreError
-            If the destination is not a local path.
+        NotImplementedError
+            This method is not implemented.
         """
-        if map_uri_scheme(dst) != "local":
-            raise StoreError(f"Destination '{dst}' is not a local path.")
-        self._build_path(dst)
+        raise NotImplementedError("Remote store does not support persist_artifact.")
+
+    ############################
+    # Private helper methods
+    ############################
 
     @staticmethod
-    def _build_path(path: str) -> None:
+    def _check_head(src) -> None:
         """
-        Get path from store path and path.
+        Check if the source exists.
 
         Parameters
         ----------
-        path : str
-            The path to build.
+        src : str
+            The source location.
 
         Returns
         -------
         None
+
+        Raises
+        ------
+        HTTPError
+            If an error occurs while checking the source.
         """
-        pth = Path(path)
-        if pth.suffix != "":
-            pth = pth.parent
-        pth.mkdir(parents=True, exist_ok=True)
+        r = requests.head(src, timeout=60)
+        r.raise_for_status()
 
-    def _build_temp(self, src: str) -> str:
+    def _download_file(self, url: str, dst: str) -> str:
         """
-        Build a temporary path.
+        Method to download a file from a given url.
 
         Parameters
         ----------
-        src : str
-            Source filename.
+        url : str
+            The url of the file to download.
+        dst : str
+            The destination of the file.
 
         Returns
         -------
         str
-            Temporary path.
+            The path of the downloaded file.
         """
-        tmpdir = mkdtemp()
-        dst = str(Path(tmpdir) / Path(src).name)
-        self._registry[src] = dst
+        self._check_head(url)
+        self._check_local_dst(dst)
+        with requests.get(url, stream=True, timeout=60) as r:
+            r.raise_for_status()
+            with open(dst, "wb") as f:
+                for chunk in r.iter_content(chunk_size=8192):
+                    f.write(chunk)
         return dst
 
+    ############################
+    # Store interface methods
+    ############################
+
     @staticmethod
-    @abstractmethod
     def is_local() -> bool:
         """
-        Method to check if store is local.
-        """
-
-
-class StoreConfig(BaseModel):
-    """
-    Store configuration base class.
-    """
-
+        Check if the store is local.
 
-class StoreParameters(BaseModel):
-    """
-    Store configuration class.
-    """
-
-    name: str
-    """Store id."""
-
-    type: Literal["local", "s3", "remote", "sql"]
-    """Store type to instantiate."""
-
-    config: StoreConfig = None
-    """Configuration for the store."""
-
-    is_default: bool = False
-    """Flag to determine if the store is the default one."""
+        Returns
+        -------
+        bool
+            False
+        """
+        return False
```

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/local.py` & `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/local.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 import shutil
 import typing
 from pathlib import Path
 
 from digitalhub_core.stores.objects.base import Store, StoreConfig
 
-if typing.TYPE_CHECKING:
-    import pandas as pd
 
 
 class LocalStoreConfig(StoreConfig):
     """
     Local store configuration class.
     """
 
@@ -120,40 +118,14 @@
             Returns the URI of the artifact.
         """
         if dst is None:
             dst = str(Path(self.config.path) / Path(src).name)
         self._check_local_dst(dst)
         return shutil.copy(src, dst)
 
-    def write_df(self, df: pd.DataFrame, dst: str | None = None, **kwargs) -> str:
-        """
-        Method to write a dataframe to a file. Kwargs are passed to df.to_parquet().
-        If destination is not provided, the dataframe is written to the default
-        store path with name data.parquet.
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            The dataframe to write.
-        dst : str
-            The destination of the dataframe.
-        **kwargs
-            Keyword arguments.
-
-        Returns
-        -------
-        str
-            Path of written dataframe.
-        """
-        if dst is None or not dst.endswith(".parquet"):
-            dst = str(Path(self.config.path) / "data.parquet")
-        self._check_local_dst(dst)
-        df.to_parquet(dst, index=False, **kwargs)
-        return dst
-
     ############################
     # Store interface methods
     ############################
 
     @staticmethod
     def is_local() -> bool:
         """
```

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/s3.py` & `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/s3.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 
 import boto3
 import botocore.client  # pylint: disable=unused-import
 from botocore.exceptions import ClientError
 from digitalhub_core.stores.objects.base import Store, StoreConfig
 from digitalhub_core.utils.exceptions import StoreError
 
-if typing.TYPE_CHECKING:
-    import pandas as pd
-
 
 # Type aliases
 S3Client = Type["botocore.client.S3"]
 
 
 class S3StoreConfig(StoreConfig):
     """
@@ -124,39 +121,14 @@
         -------
         str
             Returns the URI of the artifact on S3 based storage.
         """
         key = self._get_key(dst) if dst is not None else self._get_key(src)
         return self._upload_file(src, key)
 
-    def write_df(self, df: pd.DataFrame, dst: str | None = None, **kwargs) -> str:
-        """
-        Write a dataframe to S3 based storage. Kwargs are passed to df.to_parquet().
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            The dataframe.
-        dst : str
-            The destination path on S3 based storage.
-        **kwargs
-            Keyword arguments.
-
-        Returns
-        -------
-        str
-            The path S3 path where the dataframe was saved.
-        """
-        if dst is None or not dst.endswith(".parquet"):
-            raise StoreError("Destination must be a parquet file!")
-        fileobj = BytesIO()
-        df.to_parquet(fileobj, index=False, **kwargs)
-        key = self._get_key(dst)
-        return self._upload_fileobj(fileobj, key)
-
     ############################
     # Private helper methods
     ############################
 
     def _get_bucket(self) -> str:
         """
         Get the name of the S3 bucket from the URI.
```

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/sql.py` & `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/sql.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 SQLStore module.
 """
 from __future__ import annotations
 
 from pathlib import Path
+from typing import Any
 
-import pandas as pd
+import pyarrow as pa
+import pyarrow.parquet as pq
 from digitalhub_core.stores.objects.base import Store, StoreConfig
 from digitalhub_core.utils.exceptions import StoreError
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, Table, MetaData
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import SQLAlchemyError
+from sqlalchemy.engine.row import LegacyRow
 
 
 class SQLStoreConfig(StoreConfig):
     """
     SQL store configuration class.
     """
 
@@ -113,40 +116,14 @@
         Raises
         ------
         NotImplementedError
             This method is not implemented.
         """
         raise NotImplementedError("SQL store does not support persist_artifact.")
 
-    def write_df(self, df: pd.DataFrame, dst: str | None = None, **kwargs) -> str:
-        """
-        Write a dataframe to a database. Kwargs are passed to df.to_sql().
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            The dataframe.
-        dst : str
-            The destination table on database.
-        **kwargs
-            Keyword arguments.
-
-        Returns
-        -------
-        str
-            The SQL uri where the dataframe was saved.
-        """
-        if dst is None:
-            schema = str(self.config.pg_schema)
-            table = "table"
-        else:
-            schema = self._get_schema(dst)
-            table = self._get_table_name(dst)
-        return self._upload_table(df, schema, table, **kwargs)
-
     ############################
     # Private helper methods
     ############################
 
     def _get_connection_string(self) -> str:
         """
         Get the connection string.
@@ -157,41 +134,53 @@
             The connection string.
         """
         return (
             f"postgresql+psycopg2://{self.config.user}:{self.config.password}@"
             f"{self.config.host}:{self.config.port}/{self.config.database}"
         )
 
-    def _get_engine(self) -> Engine:
+    def _get_engine(self, schema: str | None = None) -> Engine:
         """
         Create engine from connection string.
 
+        Parameters
+        ----------
+        schema : str
+            The schema.
+
         Returns
         -------
         Engine
             An SQLAlchemy engine.
         """
         connection_string = self._get_connection_string()
         if not isinstance(connection_string, str):
             raise StoreError("Connection string must be a string.")
         try:
+            if schema is not None:
+                return create_engine(connection_string, connect_args={"options": f"-csearch_path={schema}"})
             return create_engine(connection_string)
         except Exception as ex:
             raise StoreError(f"Something wrong with connection string. Arguments: {str(ex.args)}")
 
-    def _check_factory(self) -> Engine:
+    def _check_factory(self, schema: str | None = None) -> Engine:
         """
         Check if the database is accessible and return the engine.
 
+        Parameters
+        ----------
+        schema : str
+            The schema.
+
         Returns
         -------
         Engine
             The database engine.
         """
-        engine = self._get_engine()
+        engine = self._get_engine(schema)
         self._check_access_to_storage(engine)
         return engine
 
     @staticmethod
     def _parse_path(path: str) -> dict:
         """
         Parse the path and return the components.
@@ -290,44 +279,58 @@
             The destination path.
 
         Returns
         -------
         str
             The destination path.
         """
-        engine = self._check_factory()
+        engine = self._check_factory(schema=schema)
         self._check_local_dst(dst)
-        pd.read_sql_table(table, engine, schema=schema).to_parquet(dst, index=False)
+
+        # Read the table from the database
+        sa_table = Table(table, MetaData(), autoload_with=engine)
+        query = sa_table.select()
+        with engine.begin() as conn:
+            result: list[LegacyRow] = conn.execute(query).fetchall()
+
+        # Parse the result
+        data = self._parse_result(result)
+
+        # Convert the result to a pyarrow table and
+        # write the pyarrow table to a Parquet file
+        arrow_table = pa.Table.from_pydict(data)
+        pq.write_table(arrow_table, dst)
+
         engine.dispose()
+
         return dst
 
-    def _upload_table(self, df: pd.DataFrame, schema: str, table: str, **kwargs) -> str:
+    @staticmethod
+    def _parse_result(result: list[LegacyRow]) -> dict:
         """
-        Upload a table to SQL based storage.
+        Convert a list of list of tuples to a dict.
 
         Parameters
         ----------
-        df : pd.DataFrame
-            The dataframe.
-        schema : str
-            Destination schema.
-        table : str
-            Destination table.
-        **kwargs
-            Keyword arguments.
+        result : list[LegacyRow]
+            The data to convert.
 
         Returns
         -------
-        str
-            The SQL URI where the dataframe was saved.
+        dict
+            The converted data.
         """
-        engine = self._check_factory()
-        df.to_sql(table, engine, schema=schema, index=False, **kwargs)
-        engine.dispose()
-        return f"sql://{engine.url.database}/{schema}/{table}"
+        data_list = [row.items() for row in result]
+        data = {}
+        for row in data_list:
+            for column_name, value in row:
+                if column_name not in data:
+                    data[column_name] = []
+                data[column_name].append(value)
+        return data
 
     ############################
     # Store interface methods
     ############################
 
     @staticmethod
     def is_local() -> bool:
```

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/utils/api.py` & `digitalhub_core-0.5.0b1/digitalhub_core/utils/api.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/utils/env_utils.py` & `digitalhub_core-0.5.0b1/digitalhub_core/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/utils/file_utils.py` & `digitalhub_core-0.5.0b1/digitalhub_core/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/utils/generic_utils.py` & `digitalhub_core-0.5.0b1/digitalhub_core/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/utils/git_utils.py` & `digitalhub_core-0.5.0b1/digitalhub_core/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/utils/io_utils.py` & `digitalhub_core-0.5.0b1/digitalhub_core/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core/utils/uri_utils.py` & `digitalhub_core-0.5.0b1/digitalhub_core/utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core.egg-info/PKG-INFO` & `digitalhub_core-0.5.0b1/digitalhub_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.5.0b0
+Version: 0.5.0b1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,17 +225,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: boto3
-Requires-Dist: aiobotocore
 Requires-Dist: pydantic>=1.10.8,~=1.10
-Requires-Dist: pandas<2.2,>=1.2
 Requires-Dist: sqlalchemy~=1.4
 Requires-Dist: psycopg2-binary~=2.8
 Requires-Dist: pyarrow<15,>=10.0
 Requires-Dist: requests~=2.31
 Requires-Dist: PyYAML~=5.1
 Requires-Dist: GitPython>=3
 Provides-Extra: dev
```

### Comparing `digitalhub_core-0.5.0b0/digitalhub_core.egg-info/SOURCES.txt` & `digitalhub_core-0.5.0b1/digitalhub_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b0/pyproject.toml` & `digitalhub_core-0.5.0b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-core"
-version = "0.5.0b0"
+version = "0.5.0b1"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -17,17 +17,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["data", "dataops", "kubernetes"]
 requires-python = ">=3.9"
 dependencies = [
     "boto3",
-    "aiobotocore",
     "pydantic~=1.10, >=1.10.8",
-    "pandas>=1.2, <2.2",
     "sqlalchemy~=1.4",
     "psycopg2-binary~=2.8",
     "pyarrow>=10.0, <15",
     "requests~=2.31",
     "PyYAML~=5.1",
     "GitPython>=3",
 ]
@@ -61,15 +59,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
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

