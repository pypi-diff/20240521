# Comparing `tmp/lamindb_setup-0.72.1.tar.gz` & `tmp/lamindb_setup-0.72.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.72.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.72.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.72.1.tar` & `lamindb_setup-0.72.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     8499 2024-05-10 21:24:49.730141 lamindb_setup-0.72.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-05-10 21:24:49.730245 lamindb_setup-0.72.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-05-10 21:24:49.730323 lamindb_setup-0.72.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-05-10 21:24:49.730400 lamindb_setup-0.72.1/.gitignore
--rw-r--r--   0        0        0     1474 2024-05-10 21:24:49.730816 lamindb_setup-0.72.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-05-10 21:24:49.730899 lamindb_setup-0.72.1/LICENSE
--rw-r--r--   0        0        0      265 2024-05-10 21:24:49.730963 lamindb_setup-0.72.1/README.md
--rw-r--r--   0        0        0   101877 2024-05-19 21:07:06.511965 lamindb_setup-0.72.1/docs/changelog.md
--rw-r--r--   0        0        0     2574 2024-05-10 21:24:49.732231 lamindb_setup-0.72.1/docs/hub-cloud/01-init-local-instance.ipynb
--rw-r--r--   0        0        0     3948 2024-05-10 21:24:49.732413 lamindb_setup-0.72.1/docs/hub-cloud/02-connect-local-instance.ipynb
--rw-r--r--   0        0        0    10851 2024-05-10 21:27:09.131102 lamindb_setup-0.72.1/docs/hub-cloud/03-add-managed-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-05-10 21:24:49.732848 lamindb_setup-0.72.1/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3202 2024-05-19 16:54:54.607860 lamindb_setup-0.72.1/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3886 2024-05-10 21:24:49.733461 lamindb_setup-0.72.1/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     5454 2024-05-10 21:24:49.733811 lamindb_setup-0.72.1/docs/hub-cloud/07-keep-artifacts-local.ipynb
--rw-r--r--   0        0        0     3160 2024-05-10 21:24:49.734110 lamindb_setup-0.72.1/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      177 2024-05-10 21:24:49.734470 lamindb_setup-0.72.1/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-05-10 21:24:49.735076 lamindb_setup-0.72.1/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-05-10 21:24:49.735685 lamindb_setup-0.72.1/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-05-10 21:24:49.736223 lamindb_setup-0.72.1/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2712 2024-05-10 21:24:49.736468 lamindb_setup-0.72.1/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-05-10 21:24:49.736795 lamindb_setup-0.72.1/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-05-10 21:24:49.737035 lamindb_setup-0.72.1/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-05-10 21:24:49.737170 lamindb_setup-0.72.1/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6182 2024-05-10 21:24:49.737508 lamindb_setup-0.72.1/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      177 2024-05-10 21:24:49.737594 lamindb_setup-0.72.1/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-05-10 21:24:49.737664 lamindb_setup-0.72.1/docs/index.md
--rw-r--r--   0        0        0      513 2024-05-10 21:24:49.737976 lamindb_setup-0.72.1/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-05-10 21:24:49.738046 lamindb_setup-0.72.1/docs/reference.md
--rw-r--r--   0        0        0     1542 2024-05-19 21:06:50.944181 lamindb_setup-0.72.1/lamindb_setup/__init__.py
--rw-r--r--   0        0        0      846 2024-05-10 21:24:49.738940 lamindb_setup-0.72.1/lamindb_setup/_cache.py
--rw-r--r--   0        0        0      129 2024-05-10 21:24:49.739174 lamindb_setup-0.72.1/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2613 2024-05-10 21:24:49.739337 lamindb_setup-0.72.1/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1186 2024-05-10 21:24:49.739588 lamindb_setup-0.72.1/lamindb_setup/_close.py
--rw-r--r--   0        0        0    12728 2024-05-10 21:27:09.131888 lamindb_setup-0.72.1/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     5524 2024-05-19 16:54:54.608343 lamindb_setup-0.72.1/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1534 2024-05-10 21:24:49.740572 lamindb_setup-0.72.1/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2120 2024-05-10 21:24:49.740766 lamindb_setup-0.72.1/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1874 2024-05-10 21:24:49.741154 lamindb_setup-0.72.1/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11897 2024-05-10 21:27:09.133186 lamindb_setup-0.72.1/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8815 2024-05-10 21:24:49.741821 lamindb_setup-0.72.1/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      940 2024-05-10 21:24:49.742316 lamindb_setup-0.72.1/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      679 2024-05-10 21:24:49.742498 lamindb_setup-0.72.1/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1419 2024-05-10 21:27:09.133733 lamindb_setup-0.72.1/lamindb_setup/_set_managed_storage.py
--rw-r--r--   0        0        0     3670 2024-05-10 21:24:49.743106 lamindb_setup-0.72.1/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1568 2024-05-10 21:24:49.743380 lamindb_setup-0.72.1/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      416 2024-05-10 21:24:49.743642 lamindb_setup-0.72.1/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     4972 2024-05-19 18:41:24.261429 lamindb_setup-0.72.1/lamindb_setup/core/_aws_credentials.py
--rw-r--r--   0        0        0     1799 2024-05-10 21:24:49.743767 lamindb_setup-0.72.1/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2520 2024-05-10 21:24:49.743894 lamindb_setup-0.72.1/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      276 2024-05-10 21:24:49.744017 lamindb_setup-0.72.1/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5504 2024-05-10 21:24:49.744168 lamindb_setup-0.72.1/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    16352 2024-05-19 18:41:24.261649 lamindb_setup-0.72.1/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4859 2024-05-10 21:24:49.745092 lamindb_setup-0.72.1/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1875 2024-05-10 21:24:49.745226 lamindb_setup-0.72.1/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3141 2024-05-10 21:24:49.745514 lamindb_setup-0.72.1/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    16612 2024-05-16 15:52:55.373201 lamindb_setup-0.72.1/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3922 2024-05-10 21:24:49.746016 lamindb_setup-0.72.1/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2704 2024-05-10 21:24:49.746338 lamindb_setup-0.72.1/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    13236 2024-05-19 16:54:54.609402 lamindb_setup-0.72.1/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     2084 2024-05-10 21:24:49.747202 lamindb_setup-0.72.1/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1344 2024-05-10 21:24:49.747359 lamindb_setup-0.72.1/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     3002 2024-05-10 21:24:49.747517 lamindb_setup-0.72.1/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6893 2024-05-10 21:24:49.747774 lamindb_setup-0.72.1/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3542 2024-05-16 15:52:55.373912 lamindb_setup-0.72.1/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      305 2024-05-10 21:24:49.748488 lamindb_setup-0.72.1/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2269 2024-05-16 15:52:55.374538 lamindb_setup-0.72.1/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      532 2024-05-10 21:24:49.749051 lamindb_setup-0.72.1/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    26339 2024-05-19 16:54:54.609931 lamindb_setup-0.72.1/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     3325 2024-05-10 21:24:49.749714 lamindb_setup-0.72.1/noxfile.py
--rw-r--r--   0        0        0     4138 2024-05-10 21:24:49.750224 lamindb_setup-0.72.1/pyproject.toml
--rw-r--r--   0        0        0     5387 2024-05-10 21:24:49.750488 lamindb_setup-0.72.1/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      270 2024-05-10 21:24:49.751063 lamindb_setup-0.72.1/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     5716 2024-05-10 21:24:49.751513 lamindb_setup-0.72.1/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      538 2024-05-10 21:24:49.751867 lamindb_setup-0.72.1/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      504 2024-05-10 21:24:49.752008 lamindb_setup-0.72.1/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      482 2024-05-10 21:24:49.752363 lamindb_setup-0.72.1/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      595 2024-05-10 21:24:49.752562 lamindb_setup-0.72.1/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11234 2024-05-10 21:24:49.752730 lamindb_setup-0.72.1/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      772 2024-05-10 21:27:09.135946 lamindb_setup-0.72.1/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      401 2024-05-10 21:24:49.753243 lamindb_setup-0.72.1/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      193 2024-05-10 21:24:49.753482 lamindb_setup-0.72.1/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1469 2024-05-10 21:24:49.753625 lamindb_setup-0.72.1/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0     1109 2024-05-10 21:24:49.754187 lamindb_setup-0.72.1/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1642 2024-05-10 21:24:49.754795 lamindb_setup-0.72.1/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     2023 2024-05-10 21:24:49.755035 lamindb_setup-0.72.1/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      891 2024-05-10 21:24:49.755350 lamindb_setup-0.72.1/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      878 2024-05-10 21:24:49.755587 lamindb_setup-0.72.1/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1058 2024-05-10 21:24:49.755741 lamindb_setup-0.72.1/tests/storage/test_to_url.py
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.72.1/PKG-INFO
+-rw-r--r--   0        0        0     8499 2024-05-10 21:24:49.730141 lamindb_setup-0.72.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-05-10 21:24:49.730245 lamindb_setup-0.72.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-05-10 21:24:49.730323 lamindb_setup-0.72.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-05-10 21:24:49.730400 lamindb_setup-0.72.2/.gitignore
+-rw-r--r--   0        0        0     1474 2024-05-10 21:24:49.730816 lamindb_setup-0.72.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-05-10 21:24:49.730899 lamindb_setup-0.72.2/LICENSE
+-rw-r--r--   0        0        0      265 2024-05-10 21:24:49.730963 lamindb_setup-0.72.2/README.md
+-rw-r--r--   0        0        0   102229 2024-05-21 16:43:05.022906 lamindb_setup-0.72.2/docs/changelog.md
+-rw-r--r--   0        0        0     2574 2024-05-10 21:24:49.732231 lamindb_setup-0.72.2/docs/hub-cloud/01-init-local-instance.ipynb
+-rw-r--r--   0        0        0     3948 2024-05-10 21:24:49.732413 lamindb_setup-0.72.2/docs/hub-cloud/02-connect-local-instance.ipynb
+-rw-r--r--   0        0        0    10851 2024-05-10 21:27:09.131102 lamindb_setup-0.72.2/docs/hub-cloud/03-add-managed-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-05-10 21:24:49.732848 lamindb_setup-0.72.2/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3202 2024-05-19 16:54:54.607860 lamindb_setup-0.72.2/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3886 2024-05-10 21:24:49.733461 lamindb_setup-0.72.2/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     5454 2024-05-10 21:24:49.733811 lamindb_setup-0.72.2/docs/hub-cloud/07-keep-artifacts-local.ipynb
+-rw-r--r--   0        0        0     3160 2024-05-10 21:24:49.734110 lamindb_setup-0.72.2/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      177 2024-05-10 21:24:49.734470 lamindb_setup-0.72.2/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-05-10 21:24:49.735076 lamindb_setup-0.72.2/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-05-10 21:24:49.735685 lamindb_setup-0.72.2/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-05-10 21:24:49.736223 lamindb_setup-0.72.2/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2712 2024-05-10 21:24:49.736468 lamindb_setup-0.72.2/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-05-10 21:24:49.736795 lamindb_setup-0.72.2/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-05-10 21:24:49.737035 lamindb_setup-0.72.2/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-05-10 21:24:49.737170 lamindb_setup-0.72.2/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6182 2024-05-10 21:24:49.737508 lamindb_setup-0.72.2/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      177 2024-05-10 21:24:49.737594 lamindb_setup-0.72.2/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-05-10 21:24:49.737664 lamindb_setup-0.72.2/docs/index.md
+-rw-r--r--   0        0        0      513 2024-05-10 21:24:49.737976 lamindb_setup-0.72.2/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-05-10 21:24:49.738046 lamindb_setup-0.72.2/docs/reference.md
+-rw-r--r--   0        0        0     1542 2024-05-21 16:42:57.044808 lamindb_setup-0.72.2/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0      846 2024-05-10 21:24:49.738940 lamindb_setup-0.72.2/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0      129 2024-05-10 21:24:49.739174 lamindb_setup-0.72.2/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2613 2024-05-10 21:24:49.739337 lamindb_setup-0.72.2/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1186 2024-05-10 21:24:49.739588 lamindb_setup-0.72.2/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    12728 2024-05-10 21:27:09.131888 lamindb_setup-0.72.2/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     5524 2024-05-19 16:54:54.608343 lamindb_setup-0.72.2/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1534 2024-05-10 21:24:49.740572 lamindb_setup-0.72.2/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2120 2024-05-10 21:24:49.740766 lamindb_setup-0.72.2/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1874 2024-05-10 21:24:49.741154 lamindb_setup-0.72.2/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11897 2024-05-10 21:27:09.133186 lamindb_setup-0.72.2/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8815 2024-05-10 21:24:49.741821 lamindb_setup-0.72.2/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      940 2024-05-10 21:24:49.742316 lamindb_setup-0.72.2/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      679 2024-05-10 21:24:49.742498 lamindb_setup-0.72.2/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1419 2024-05-10 21:27:09.133733 lamindb_setup-0.72.2/lamindb_setup/_set_managed_storage.py
+-rw-r--r--   0        0        0     3670 2024-05-10 21:24:49.743106 lamindb_setup-0.72.2/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1568 2024-05-10 21:24:49.743380 lamindb_setup-0.72.2/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      416 2024-05-10 21:24:49.743642 lamindb_setup-0.72.2/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     5293 2024-05-20 12:51:17.170079 lamindb_setup-0.72.2/lamindb_setup/core/_aws_credentials.py
+-rw-r--r--   0        0        0     1799 2024-05-10 21:24:49.743767 lamindb_setup-0.72.2/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2520 2024-05-10 21:24:49.743894 lamindb_setup-0.72.2/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      276 2024-05-10 21:24:49.744017 lamindb_setup-0.72.2/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5504 2024-05-10 21:24:49.744168 lamindb_setup-0.72.2/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    16352 2024-05-19 18:41:24.261649 lamindb_setup-0.72.2/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4859 2024-05-10 21:24:49.745092 lamindb_setup-0.72.2/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1875 2024-05-10 21:24:49.745226 lamindb_setup-0.72.2/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3141 2024-05-10 21:24:49.745514 lamindb_setup-0.72.2/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    16949 2024-05-20 14:46:17.603753 lamindb_setup-0.72.2/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3922 2024-05-10 21:24:49.746016 lamindb_setup-0.72.2/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2704 2024-05-10 21:24:49.746338 lamindb_setup-0.72.2/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    13236 2024-05-19 16:54:54.609402 lamindb_setup-0.72.2/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     2084 2024-05-10 21:24:49.747202 lamindb_setup-0.72.2/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1344 2024-05-10 21:24:49.747359 lamindb_setup-0.72.2/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     3002 2024-05-10 21:24:49.747517 lamindb_setup-0.72.2/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6893 2024-05-10 21:24:49.747774 lamindb_setup-0.72.2/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3542 2024-05-16 15:52:55.373912 lamindb_setup-0.72.2/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      305 2024-05-10 21:24:49.748488 lamindb_setup-0.72.2/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2269 2024-05-16 15:52:55.374538 lamindb_setup-0.72.2/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      532 2024-05-10 21:24:49.749051 lamindb_setup-0.72.2/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    26339 2024-05-19 16:54:54.609931 lamindb_setup-0.72.2/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     3325 2024-05-10 21:24:49.749714 lamindb_setup-0.72.2/noxfile.py
+-rw-r--r--   0        0        0     4138 2024-05-10 21:24:49.750224 lamindb_setup-0.72.2/pyproject.toml
+-rw-r--r--   0        0        0     5387 2024-05-10 21:24:49.750488 lamindb_setup-0.72.2/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      270 2024-05-10 21:24:49.751063 lamindb_setup-0.72.2/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     5716 2024-05-10 21:24:49.751513 lamindb_setup-0.72.2/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      538 2024-05-10 21:24:49.751867 lamindb_setup-0.72.2/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      504 2024-05-10 21:24:49.752008 lamindb_setup-0.72.2/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      482 2024-05-10 21:24:49.752363 lamindb_setup-0.72.2/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      595 2024-05-10 21:24:49.752562 lamindb_setup-0.72.2/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11234 2024-05-10 21:24:49.752730 lamindb_setup-0.72.2/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      772 2024-05-10 21:27:09.135946 lamindb_setup-0.72.2/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      401 2024-05-10 21:24:49.753243 lamindb_setup-0.72.2/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      193 2024-05-10 21:24:49.753482 lamindb_setup-0.72.2/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1469 2024-05-10 21:24:49.753625 lamindb_setup-0.72.2/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0     1109 2024-05-10 21:24:49.754187 lamindb_setup-0.72.2/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1642 2024-05-10 21:24:49.754795 lamindb_setup-0.72.2/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     2023 2024-05-10 21:24:49.755035 lamindb_setup-0.72.2/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      891 2024-05-10 21:24:49.755350 lamindb_setup-0.72.2/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      878 2024-05-10 21:24:49.755587 lamindb_setup-0.72.2/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1058 2024-05-10 21:24:49.755741 lamindb_setup-0.72.2/tests/storage/test_to_url.py
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.72.2/PKG-INFO
```

### Comparing `lamindb_setup-0.72.1/.github/workflows/build.yml` & `lamindb_setup-0.72.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/.github/workflows/latest-changes.yml` & `lamindb_setup-0.72.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/.gitignore` & `lamindb_setup-0.72.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/.pre-commit-config.yaml` & `lamindb_setup-0.72.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/LICENSE` & `lamindb_setup-0.72.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/changelog.md` & `lamindb_setup-0.72.2/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Deal with migration errors when keep-artifacts-local is true | [767](https://github.com/laminlabs/lamindb-setup/pull/767) | [falexwolf](https://github.com/falexwolf) | 2024-05-20 | 0.72.2
 ♻️ Do not error if empty dict in `access_aws` | [764](https://github.com/laminlabs/lamindb-setup/pull/764) | [falexwolf](https://github.com/falexwolf) | 2024-05-19 | 0.72.1
+🐛 Keep training slash in aws cache keys | [766](https://github.com/laminlabs/lamindb-setup/pull/766) | [Koncopd](https://github.com/Koncopd) | 2024-05-19 |
 🐛 Check empty after storage record root init in delete | [763](https://github.com/laminlabs/lamindb-setup/pull/763) | [Koncopd](https://github.com/Koncopd) | 2024-05-18 |
 ✨ Call `access_aws` for all paths and cache | [762](https://github.com/laminlabs/lamindb-setup/pull/762) | [Koncopd](https://github.com/Koncopd) | 2024-05-18 | 0.72.0
 ⚡️ Speed-up file hash | [761](https://github.com/laminlabs/lamindb-setup/pull/761) | [Koncopd](https://github.com/Koncopd) | 2024-05-11 | 0.71.4
 ♻️ Account for public storage locations | [758](https://github.com/laminlabs/lamindb-setup/pull/758) | [falexwolf](https://github.com/falexwolf) | 2024-05-10 |
 ♻️ Make init_instance_hub idempotent | [757](https://github.com/laminlabs/lamindb-setup/pull/757) | [falexwolf](https://github.com/falexwolf) | 2024-05-09 |
 ♻️ Refactor delete & connect | [756](https://github.com/laminlabs/lamindb-setup/pull/756) | [falexwolf](https://github.com/falexwolf) | 2024-05-09 |
 🔥 Remove laminapp-admin logic | [755](https://github.com/laminlabs/lamindb-setup/pull/755) | [falexwolf](https://github.com/falexwolf) | 2024-05-08 |
```

### Comparing `lamindb_setup-0.72.1/docs/hub-cloud/01-init-local-instance.ipynb` & `lamindb_setup-0.72.2/docs/hub-cloud/01-init-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-cloud/02-connect-local-instance.ipynb` & `lamindb_setup-0.72.2/docs/hub-cloud/02-connect-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-cloud/03-add-managed-storage.ipynb` & `lamindb_setup-0.72.2/docs/hub-cloud/03-add-managed-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.72.2/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.72.2/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.72.2/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-cloud/07-keep-artifacts-local.ipynb` & `lamindb_setup-0.72.2/docs/hub-cloud/07-keep-artifacts-local.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.72.2/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.72.2/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.72.2/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.72.2/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.72.2/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.72.2/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.72.2/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.72.2/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.72.2/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/docs/notebooks.md` & `lamindb_setup-0.72.2/docs/notebooks.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/__init__.py` & `lamindb_setup-0.72.2/lamindb_setup/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.72.1"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.72.2"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._check_setup import _check_instance_setup
 from ._close import close
```

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_cache.py` & `lamindb_setup-0.72.2/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_check_setup.py` & `lamindb_setup-0.72.2/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_close.py` & `lamindb_setup-0.72.2/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.72.2/lamindb_setup/_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_delete.py` & `lamindb_setup-0.72.2/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_django.py` & `lamindb_setup-0.72.2/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_exportdb.py` & `lamindb_setup-0.72.2/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_importdb.py` & `lamindb_setup-0.72.2/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_init_instance.py` & `lamindb_setup-0.72.2/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_migrate.py` & `lamindb_setup-0.72.2/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_register_instance.py` & `lamindb_setup-0.72.2/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_schema.py` & `lamindb_setup-0.72.2/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_set_managed_storage.py` & `lamindb_setup-0.72.2/lamindb_setup/_set_managed_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_setup_user.py` & `lamindb_setup-0.72.2/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.72.2/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_aws_credentials.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_aws_credentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     hosted_buckets_list = [f"s3://lamin-{region}" for region in HOSTED_REGIONS]
     hosted_buckets_list.append("s3://scverse-spatial-eu-central-1")
     HOSTED_BUCKETS = tuple(hosted_buckets_list)
 else:
     HOSTED_BUCKETS = ("s3://lamin-hosted-test",)  # type: ignore
 
 
+def _keep_trailing_slash(path_str: str):
+    return path_str if path_str[-1] == "/" else path_str + "/"
+
+
 AWS_CREDENTIALS_EXPIRATION = 11 * 60 * 60  # refresh credentials after 11 hours
 
 
 class AWSCredentialsManager:
     def __init__(self):
         self._credentials_cache = {}
 
@@ -77,15 +81,18 @@
             cache_regions = path._kwargs["cache_regions"]
         else:
             cache_regions = True
 
         return S3Path(path, cache_regions=cache_regions, **connection_options)
 
     def enrich_path(self, path: S3Path, access_token: str | None = None) -> S3Path:
-        path_str = path.as_posix().rstrip("/")
+        # trailing slash is needed to avoid returning incorrect results
+        # with .startswith
+        # for example s3://lamindata-eu should not receive cache for s3://lamindata
+        path_str = _keep_trailing_slash(path.as_posix())
         root = self._find_root(path_str)
 
         if root is not None:
             set_cache = False
             credentials = self._get_cached_credentials(root)
 
             if access_token is not None:
@@ -123,15 +130,15 @@
                     # do not write the first level for the known hosted buckets
                     if path_str.startswith(HOSTED_BUCKETS):
                         root = "/".join(path.path.rstrip("/").split("/")[:2])
                     else:
                         # write the bucket for everything else
                         root = path._url.netloc
                     root = "s3://" + root
-                self._set_cached_credentials(root, credentials)
+                self._set_cached_credentials(_keep_trailing_slash(root), credentials)
 
         return self._path_inject_options(path, credentials)
 
 
 _aws_credentials_manager: AWSCredentialsManager | None = None
```

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_hub_core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_settings.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_settings_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import os
 import shutil
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal
 
+from django.db.utils import ProgrammingError
 from lamin_utils import logger
 
 from ._hub_client import call_with_fallback
 from ._hub_crud import select_account_handle_name_by_lnid
 from ._hub_utils import LaminDsn, LaminDsnModel
 from ._settings_save import save_instance_settings
 from ._settings_storage import StorageSettings, init_storage, mark_storage_root
@@ -102,16 +103,23 @@
     ) -> StorageSettings | None:
         from lnschema_core.models import Storage
 
         if local_root is not None:
             local_records = Storage.objects.filter(root=local_root)
         else:
             local_records = Storage.objects.filter(type="local")
+        all_local_records = local_records.all()
+        try:
+            # trigger an error in case of a migration issue
+            all_local_records.first()
+        except ProgrammingError:
+            logger.error("not able to load Storage registry: please migrate")
+            return None
         found = False
-        for record in local_records.all():
+        for record in all_local_records:
             root_path = Path(record.root)
             if root_path.exists():
                 marker_path = root_path / ".lamindb/_is_initialized"
                 if marker_path.exists():
                     uid = marker_path.read_text()
                     if uid == record.uid:
                         found = True
```

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_settings_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.72.2/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.72.2/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/django.py` & `lamindb_setup-0.72.2/lamindb_setup/core/django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/hashing.py` & `lamindb_setup-0.72.2/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/types.py` & `lamindb_setup-0.72.2/lamindb_setup/core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/lamindb_setup/core/upath.py` & `lamindb_setup-0.72.2/lamindb_setup/core/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/noxfile.py` & `lamindb_setup-0.72.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/pyproject.toml` & `lamindb_setup-0.72.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.72.2/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.72.2/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/hub-cloud/test_login.py` & `lamindb_setup-0.72.2/tests/hub-cloud/test_login.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/hub-local/conftest.py` & `lamindb_setup-0.72.2/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/hub-local/test_all.py` & `lamindb_setup-0.72.2/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/hub-prod/conftest.py` & `lamindb_setup-0.72.2/tests/hub-prod/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.72.2/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/hub-prod/test_upath.py` & `lamindb_setup-0.72.2/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/storage/test_hashing.py` & `lamindb_setup-0.72.2/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/storage/test_storage_access.py` & `lamindb_setup-0.72.2/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/storage/test_storage_basis.py` & `lamindb_setup-0.72.2/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/storage/test_storage_stats.py` & `lamindb_setup-0.72.2/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/tests/storage/test_to_url.py` & `lamindb_setup-0.72.2/tests/storage/test_to_url.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.1/PKG-INFO` & `lamindb_setup-0.72.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.72.1
+Version: 0.72.2
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

