# Comparing `tmp/openedx_learning-0.9.3.tar.gz` & `tmp/openedx_learning-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx_learning-0.9.3.tar", last modified: Wed May  8 19:16:13 2024, max compression
+gzip compressed data, was "openedx_learning-0.9.4.tar", last modified: Fri May 17 19:23:46 2024, max compression
```

## Comparing `openedx_learning-0.9.3.tar` & `openedx_learning-0.9.4.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.936154 openedx_learning-0.9.3/openedx_learning/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.936154 openedx_learning-0.9.3/openedx_learning/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.936154 openedx_learning-0.9.3/openedx_learning/contrib/media_server/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/media_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/media_server/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/media_server/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/media_server/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.936154 openedx_learning-0.9.3/openedx_learning/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/components/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/migrations/0002_alter_componentversioncontent_key.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/contents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/contents/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/publishing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/0002_alter_learningpackage_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/model_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    20321 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_learning/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/collations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_learning/rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_learning/rest_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/v1/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_tagging/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_tagging/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_tagging/core/tagging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.948154 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/import_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/template.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0001_squashed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0006_alter_objecttag_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0006_auto_20230802_1631.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0007_tag_import_task_log_null_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0008_taxonomy_description_not_null.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0009_alter_objecttag_object_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0010_cleanups.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0011_remove_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0012_language_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0013_tag_parent_blank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0014_minor_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0015_taxonomy_export_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0016_object_tag_export_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0017_alter_tagimporttask_status.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39335 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/system_defined.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/paginators.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    35581 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/views_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2930 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.141722 openedx_learning-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-17 19:23:46.141722 openedx_learning-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.125722 openedx_learning-0.9.4/openedx_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.125722 openedx_learning-0.9.4/openedx_learning/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.125722 openedx_learning-0.9.4/openedx_learning/contrib/media_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/contrib/media_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/contrib/media_server/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/contrib/media_server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/contrib/media_server/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.125722 openedx_learning-0.9.4/openedx_learning/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.129721 openedx_learning-0.9.4/openedx_learning/core/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/components/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/components/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/components/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.129721 openedx_learning-0.9.4/openedx_learning/core/components/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/components/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/components/migrations/0002_alter_componentversioncontent_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/components/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/components/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.129721 openedx_learning-0.9.4/openedx_learning/core/contents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/contents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/contents/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/contents/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/contents/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.129721 openedx_learning-0.9.4/openedx_learning/core/contents/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/contents/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/contents/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/contents/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.129721 openedx_learning-0.9.4/openedx_learning/core/publishing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.129721 openedx_learning-0.9.4/openedx_learning/core/publishing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/migrations/0002_alter_learningpackage_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/model_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20321 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/core/publishing/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.133722 openedx_learning-0.9.4/openedx_learning/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/lib/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/lib/collations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/lib/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/lib/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/lib/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.133722 openedx_learning-0.9.4/openedx_learning/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/rest_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/rest_api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.133722 openedx_learning-0.9.4/openedx_learning/rest_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/rest_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/rest_api/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_learning/rest_api/v1/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.141722 openedx_learning-0.9.4/openedx_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-17 19:23:46.000000 openedx_learning-0.9.4/openedx_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-17 19:23:46.000000 openedx_learning-0.9.4/openedx_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:23:46.000000 openedx_learning-0.9.4/openedx_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:23:46.000000 openedx_learning-0.9.4/openedx_learning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 19:23:46.000000 openedx_learning-0.9.4/openedx_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 19:23:46.000000 openedx_learning-0.9.4/openedx_learning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.133722 openedx_learning-0.9.4/openedx_tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.133722 openedx_learning-0.9.4/openedx_tagging/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.133722 openedx_learning-0.9.4/openedx_tagging/core/tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.137722 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/import_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/template.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.141722 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0001_squashed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0006_alter_objecttag_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0006_auto_20230802_1631.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0007_tag_import_task_log_null_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0008_taxonomy_description_not_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0009_alter_objecttag_object_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0010_cleanups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0011_remove_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0012_language_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0013_tag_parent_blank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0014_minor_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0015_taxonomy_export_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0016_object_tag_export_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0017_alter_tagimporttask_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.141722 openedx_learning-0.9.4/openedx_tagging/core/tagging/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39335 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/models/import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/models/system_defined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.141722 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.141722 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35581 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/views_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/core/tagging/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/openedx_tagging/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:23:46.141722 openedx_learning-0.9.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-17 19:23:46.145722 openedx_learning-0.9.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2930 2024-05-17 19:23:43.000000 openedx_learning-0.9.4/setup.py
```

### Comparing `openedx_learning-0.9.3/CHANGELOG.rst` & `openedx_learning-0.9.4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/LICENSE.txt` & `openedx_learning-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/PKG-INFO` & `openedx_learning-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-learning
-Version: 0.9.3
+Version: 0.9.4
 Summary: An experiment.
 Home-page: https://github.com/openedx/openedx-learning
 Author: David Ormsbee
 Author-email: dave@tcril.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -15,20 +15,20 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE.txt
-Requires-Dist: djangorestframework<4.0
-Requires-Dist: Django<5.0
 Requires-Dist: edx-drf-extensions
-Requires-Dist: attrs
-Requires-Dist: celery
 Requires-Dist: rules<4.0
+Requires-Dist: celery
+Requires-Dist: Django<5.0
+Requires-Dist: attrs
+Requires-Dist: djangorestframework<4.0
 
 openedx-learning
 =============================
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
```

### Comparing `openedx_learning-0.9.3/README.rst` & `openedx_learning-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/contrib/media_server/apps.py` & `openedx_learning-0.9.4/openedx_learning/contrib/media_server/apps.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/contrib/media_server/views.py` & `openedx_learning-0.9.4/openedx_learning/contrib/media_server/views.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/components/admin.py` & `openedx_learning-0.9.4/openedx_learning/core/components/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/components/api.py` & `openedx_learning-0.9.4/openedx_learning/core/components/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/components/apps.py` & `openedx_learning-0.9.4/openedx_learning/core/components/apps.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/components/migrations/0001_initial.py` & `openedx_learning-0.9.4/openedx_learning/core/components/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/components/migrations/0002_alter_componentversioncontent_key.py` & `openedx_learning-0.9.4/openedx_learning/core/components/migrations/0002_alter_componentversioncontent_key.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/components/models.py` & `openedx_learning-0.9.4/openedx_learning/core/components/models.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/contents/admin.py` & `openedx_learning-0.9.4/openedx_learning/core/contents/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/contents/api.py` & `openedx_learning-0.9.4/openedx_learning/core/contents/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/contents/migrations/0001_initial.py` & `openedx_learning-0.9.4/openedx_learning/core/contents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/contents/models.py` & `openedx_learning-0.9.4/openedx_learning/core/contents/models.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/publishing/admin.py` & `openedx_learning-0.9.4/openedx_learning/core/publishing/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/publishing/api.py` & `openedx_learning-0.9.4/openedx_learning/core/publishing/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/0001_initial.py` & `openedx_learning-0.9.4/openedx_learning/core/publishing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/0002_alter_learningpackage_key_and_more.py` & `openedx_learning-0.9.4/openedx_learning/core/publishing/migrations/0002_alter_learningpackage_key_and_more.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/publishing/model_mixins.py` & `openedx_learning-0.9.4/openedx_learning/core/publishing/model_mixins.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/core/publishing/models.py` & `openedx_learning-0.9.4/openedx_learning/core/publishing/models.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/lib/admin_utils.py` & `openedx_learning-0.9.4/openedx_learning/lib/admin_utils.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/lib/cache.py` & `openedx_learning-0.9.4/openedx_learning/lib/cache.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/lib/collations.py` & `openedx_learning-0.9.4/openedx_learning/lib/collations.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/lib/fields.py` & `openedx_learning-0.9.4/openedx_learning/lib/fields.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/lib/managers.py` & `openedx_learning-0.9.4/openedx_learning/lib/managers.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/lib/test_utils.py` & `openedx_learning-0.9.4/openedx_learning/lib/test_utils.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning/rest_api/v1/components.py` & `openedx_learning-0.9.4/openedx_learning/rest_api/v1/components.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_learning.egg-info/PKG-INFO` & `openedx_learning-0.9.4/openedx_learning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-learning
-Version: 0.9.3
+Version: 0.9.4
 Summary: An experiment.
 Home-page: https://github.com/openedx/openedx-learning
 Author: David Ormsbee
 Author-email: dave@tcril.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -15,20 +15,20 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE.txt
-Requires-Dist: djangorestframework<4.0
-Requires-Dist: Django<5.0
 Requires-Dist: edx-drf-extensions
-Requires-Dist: attrs
-Requires-Dist: celery
 Requires-Dist: rules<4.0
+Requires-Dist: celery
+Requires-Dist: Django<5.0
+Requires-Dist: attrs
+Requires-Dist: djangorestframework<4.0
 
 openedx-learning
 =============================
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
```

### Comparing `openedx_learning-0.9.3/openedx_learning.egg-info/SOURCES.txt` & `openedx_learning-0.9.4/openedx_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/admin.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/api.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/data.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/data.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/actions.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,24 +240,21 @@
 
         return errors
 
     def execute(self) -> None:
         """
         Creates a Tag
         """
-        parent = None
-        if self.tag.parent_id:
-            parent = self.taxonomy.tag_set.get(external_id=self.tag.parent_id)
-        taxonomy_tag = Tag(
+        Tag.objects.create(
             taxonomy=self.taxonomy,
-            parent=parent,
+            parent=self.taxonomy.tag_set.get(external_id=self.tag.parent_id)
+            if self.tag.parent_id is not None else None,
             value=self.tag.value,
             external_id=self.tag.id,
         )
-        taxonomy_tag.save()
 
 
 class UpdateParentTag(ImportAction):
     """
     Action for update the parent of a Tag
 
     Action created if there is a change on the parent
@@ -405,16 +402,15 @@
         return []
 
     def execute(self) -> None:
         """
         Delete a tag
         """
         try:
-            taxonomy_tag = self._get_tag()
-            taxonomy_tag.delete()
+            self._get_tag().delete()
         except Tag.DoesNotExist:
             pass  # The tag may be already cascade deleted if the parent tag was deleted
 
 
 class WithoutChanges(ImportAction):
     """
     Action when there is no change on the Tag
```

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/api.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 - Function to force clean the status of an import task, or a way to avoid
   a lock: a task not in SUCCESS or ERROR due to something unexpected
   (ex. server crash)
 - Join/reduce actions on TagImportPlan. See `generate_actions()`
 """
 from __future__ import annotations
 
+import time
 from typing import BinaryIO
 
 from django.utils.translation import gettext as _
 
 from ..models import TagImportTask, TagImportTaskState, Taxonomy
 from .import_plan import TagImportPlan, TagImportTask
 from .parsers import ParserFormat, get_parser
@@ -73,14 +74,15 @@
     Set `replace` to True to delete all not readed Tag of the given taxonomy.
     Ex. Given a taxonomy with `tag_1`, `tag_2` and `tag_3`. If there is only `tag_1`
     in the file (regardless of action), then `tag_2` and `tag_3` will be deleted
     if `replace=True`
 
     Set `plan_only` to True to only generate the actions and not execute them.
     """
+    global_start_time = time.time()
     _import_validations(taxonomy)
 
     # Checks that exists only one task import in progress at a time per taxonomy
     if not _check_unique_import_task(taxonomy):
         raise ValueError(
             _(
                 "There is an import task running. "
@@ -88,41 +90,69 @@
             )
         )
 
     # Creating import task
     task = TagImportTask.create(taxonomy)
 
     try:
+        # Start of parsing
+
         # Get the parser and parse the file
+        start_time = time.time()
         task.log_parser_start()
         parser = get_parser(parser_format)
         tags, errors = parser.parse_import(file)
 
         # Check if there are errors in the parse
         if errors:
             task.handle_parser_errors(errors)
             return False, task, None
 
-        task.log_parser_end()
+        end_time = time.time()
+        elapsed_time = end_time - start_time
+        elapsed_time = round(elapsed_time, 5)
+        task.log_parser_end(elapsed_time)
+
+        # End of parsing
+
+        # Start of generate actions
+
+        start_time = time.time()
 
-        # Generate actions
         task.log_start_planning()
         tag_import_plan = TagImportPlan(taxonomy)
         tag_import_plan.generate_actions(tags, replace)
-        task.log_plan(tag_import_plan)
+
+        end_time = time.time()
+        elapsed_time = end_time - start_time
+        elapsed_time = round(elapsed_time, 5)
+        task.log_plan(tag_import_plan, elapsed_time)
+
+        # End of generate actions
 
         if tag_import_plan.errors:
             task.handle_plan_errors()
             return False, task, tag_import_plan
 
         if not plan_only:
+            # Start of execute
+            start_time = time.time()
             task.log_start_execute()
             tag_import_plan.execute(task)
+            end_time = time.time()
+            elapsed_time = end_time - start_time
+            elapsed_time = round(elapsed_time, 5)
+            task.log_end_execute(elapsed_time)
+            # End of execute
+
+        global_end_time = time.time()
+        global_elapsed_time = global_end_time - global_start_time
+        global_elapsed_time = round(global_elapsed_time, 5)
 
-        task.end_success()
+        task.end_success(global_elapsed_time)
 
         return True, task, tag_import_plan
     except Exception as exception:
         # Log any exception
         task.log_exception(exception)
         return False, task, None
```

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/exceptions.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/import_plan.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/import_plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,12 +203,16 @@
         Executes each action
 
         If task is set, creates logs for each action
         """
         if self.errors:
             return
         for action in self.actions:
+            # Avoid to save each log because it is slow and costs a lot in memory
+            # It is necessary to save at the end.
             if task:
-                task.add_log(f"#{action.index}: {str(action)} [Started]")
+                task.add_log(f"#{action.index}: {str(action)} [Started]", save=False)
             action.execute()
             if task:
-                task.add_log("Success")
+                task.add_log("Success", save=False)
+        if task:
+            task.save()
```

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/parsers.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/parsers.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/tasks.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/tasks.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/template.csv` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/template.csv`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/template.json` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/import_export/template.json`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0001_initial.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0001_squashed.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0001_squashed.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0006_auto_20230802_1631.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0006_auto_20230802_1631.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0008_taxonomy_description_not_null.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0008_taxonomy_description_not_null.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0009_alter_objecttag_object_id.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0009_alter_objecttag_object_id.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0010_cleanups.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0010_cleanups.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0011_remove_required.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0011_remove_required.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0012_language_taxonomy.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0012_language_taxonomy.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0013_tag_parent_blank.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0013_tag_parent_blank.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0014_minor_fixes.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0014_minor_fixes.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0015_taxonomy_export_id.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0015_taxonomy_export_id.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0016_object_tag_export_id.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0016_object_tag_export_id.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0017_alter_tagimporttask_status.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/migrations/0017_alter_tagimporttask_status.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/models/base.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/models/base.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/models/import_export.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/models/import_export.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,19 +86,19 @@
 
     def log_parser_start(self):
         """
         Logs the parser start event.
         """
         self.add_log(_("Starting to load data from file"))
 
-    def log_parser_end(self):
+    def log_parser_end(self, elapsed_time):
         """
         Logs the parser finished event.
         """
-        self.add_log(_("Load data finished"))
+        self.add_log(_("Load data finished. Time elapsed: ") + str(elapsed_time) + _(" seconds"))
 
     def handle_parser_errors(self, errors):
         """
         Handles parser errors by logging them and moving the task status to ERROR.
         """
         for error in errors:
             self.add_log(f"{str(error)}", save=False)
@@ -109,19 +109,19 @@
         """
         Starts task planning with a log message, and moves the task status to PLANNING.
         """
         self.add_log(_("Starting plan actions"), save=False)
         self.status = TagImportTaskState.PLANNING.value
         self.save()
 
-    def log_plan(self, plan):
+    def log_plan(self, plan, elapsed_time):
         """
         Logs the task plan.
         """
-        self.add_log(_("Plan finished"))
+        self.add_log(_("Plan finished. Time elapsed: ") + str(elapsed_time) + _(" seconds"))
         plan_str = plan.plan()
         self.log += f"\n{plan_str}\n"
         self.save()
 
     def handle_plan_errors(self):
         """
         Handles plan errors by moving the task status to ERROR.
@@ -134,14 +134,17 @@
         """
         Starts task execution with a log message, and moves the task status to EXECUTING.
         """
         self.add_log(_("Starting execute actions"), save=False)
         self.status = TagImportTaskState.EXECUTING.value
         self.save()
 
-    def end_success(self):
+    def log_end_execute(self, elapsed_time):
+        self.add_log(_("Execute actions finished. Time elapsed: ") + str(elapsed_time) + _(" seconds"))
+
+    def end_success(self, elapsed_time):
         """
         Completes task execution with a log message, and moves the task status to SUCCESS.
         """
-        self.add_log(_("Execution finished"), save=False)
+        self.add_log(_("Execution finished. Total time elapsed: ") + str(elapsed_time) + _("seconds"), save=False)
         self.status = TagImportTaskState.SUCCESS.value
         self.save()
```

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/models/system_defined.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/models/system_defined.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/models/utils.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/models/utils.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/paginators.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/paginators.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/utils.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/utils.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/permissions.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/serializers.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/urls.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/views.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/views.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/views_import.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/rest_api/v1/views_import.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/openedx_tagging/core/tagging/rules.py` & `openedx_learning-0.9.4/openedx_tagging/core/tagging/rules.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.3/setup.py` & `openedx_learning-0.9.4/setup.py`

 * *Files identical despite different names*

