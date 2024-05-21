# Comparing `tmp/neuro-sdk-24.2.0.tar.gz` & `tmp/neuro_sdk-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-sdk-24.2.0.tar", last modified: Mon Feb 12 13:15:33 2024, max compression
+gzip compressed data, was "neuro_sdk-24.5.0.tar", last modified: Tue May 21 09:59:49 2024, max compression
```

## Comparing `neuro-sdk-24.2.0.tar` & `neuro_sdk-24.5.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.548762 neuro-sdk-24.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    92728 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-02-12 13:15:33.548762 neuro-sdk-24.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.532762 neuro-sdk-24.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.532762 neuro-sdk-24.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.532762 neuro-sdk-24.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/_templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    24522 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/buckets_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/client_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/config_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/disks_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/functions_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/images_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/jobs_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/jobs_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/parse_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/plugin_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/secrets_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/service_accounts_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/storage_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/storage_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/docs/users_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-02-12 13:15:33.548762 neuro-sdk-24.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.528762 neuro-sdk-24.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.540763 neuro-sdk-24.2.0/src/neuro_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_azure_bucket_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_bucket_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    30600 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    34493 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17452 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_gcs_bucket_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_images.py
--rw-r--r--   0 runner    (1001) docker     (127)    41551 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_rewrite.py
--rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_s3_bucket_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_server_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)    37214 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_url_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/src/neuro_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.548762 neuro-sdk-24.2.0/src/neuro_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-02-12 13:15:33.000000 neuro-sdk-24.2.0/src/neuro_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-12 13:15:33.000000 neuro-sdk-24.2.0/src/neuro_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 13:15:33.000000 neuro-sdk-24.2.0/src/neuro_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 13:15:01.000000 neuro-sdk-24.2.0/src/neuro_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-12 13:15:33.000000 neuro-sdk-24.2.0/src/neuro_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-12 13:15:33.000000 neuro-sdk-24.2.0/src/neuro_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.544762 neuro-sdk-24.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.548762 neuro-sdk-24.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/data/emptyfile.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/data/file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.528762 neuro-sdk-24.2.0/tests/data/nested/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:33.548762 neuro-sdk-24.2.0/tests/data/nested/folder/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/data/nested/folder/file.txt
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_bucket_persistent_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    41447 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21523 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16161 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    63974 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)   110227 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_login_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_public_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)    80423 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_storage_filestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    20708 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_url_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-02-12 13:14:58.000000 neuro-sdk-24.2.0/tests/test_version_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.708868 neuro_sdk-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    92906 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-21 09:59:49.708868 neuro_sdk-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.692868 neuro_sdk-24.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.692868 neuro_sdk-24.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.696868 neuro_sdk-24.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    24522 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/buckets_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/client_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/config_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/disks_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/functions_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/images_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/jobs_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/jobs_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/parse_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/plugin_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/secrets_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/service_accounts_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/storage_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/storage_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/docs/users_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-21 09:59:49.708868 neuro_sdk-24.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.688868 neuro_sdk-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.700868 neuro_sdk-24.5.0/src/neuro_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_azure_bucket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_bucket_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30600 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36879 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_config_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17452 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_gcs_bucket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41769 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_s3_bucket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_server_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37214 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_url_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/src/neuro_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.704867 neuro_sdk-24.5.0/src/neuro_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-21 09:59:49.000000 neuro_sdk-24.5.0/src/neuro_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-21 09:59:49.000000 neuro_sdk-24.5.0/src/neuro_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:59:49.000000 neuro_sdk-24.5.0/src/neuro_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:59:09.000000 neuro_sdk-24.5.0/src/neuro_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-21 09:59:49.000000 neuro_sdk-24.5.0/src/neuro_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 09:59:49.000000 neuro_sdk-24.5.0/src/neuro_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.704867 neuro_sdk-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.704867 neuro_sdk-24.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/data/emptyfile.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/data/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.688868 neuro_sdk-24.5.0/tests/data/nested/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:49.704867 neuro_sdk-24.5.0/tests/data/nested/folder/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/data/nested/folder/file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_bucket_persistent_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45806 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25097 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_config_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16161 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63974 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109308 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19057 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_login_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_public_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80423 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_storage_filestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20708 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_url_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-21 09:59:06.000000 neuro_sdk-24.5.0/tests/test_version_check.py
```

### Comparing `neuro-sdk-24.2.0/CHANGELOG.md` & `neuro_sdk-24.5.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 [comment]: # (Please do not modify this file)
 [comment]: # (Put you comments to changelog.d and it will be moved to changelog in next release)
 
 [comment]: # (Clear the text on make release for canceling the release)
 
 [comment]: # (towncrier release notes start)
 
+Neuro SDK/CLI 24.5.0 (2024-05-21)
+=================================
+
+Features
+--------
+
+- Support AMD, Intel GPUs ([#3007](https://github.com/neuro-inc/neuro-cli/issues/3007))
+
+
 Neuro SDK/CLI 24.2.0 (2024-02-12)
 =================================
 
 No significant changes.
 
 
 Neuro SDK/CLI 24.1.0 (2024-01-02)
```

### Comparing `neuro-sdk-24.2.0/LICENSE` & `neuro_sdk-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/PKG-INFO` & `neuro_sdk-24.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-sdk
-Version: 24.2.0
+Version: 24.5.0
 Summary: Neu.ro SDK
 Home-page: https://github.com/neuro-inc/platform-client-python
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -35,15 +35,15 @@
 Requires-Dist: certifi
 Requires-Dist: toml>=0.10.0
 Requires-Dist: azure-storage-blob!=12.9.0,>=12.8.1
 Requires-Dist: google-auth>=2.0.2
 Requires-Dist: importlib_metadata>=4.11.4; python_version < "3.11"
 Requires-Dist: packaging>=20.4
 Requires-Dist: neuro-admin-client>=23.5.0
-Requires-Dist: neuro-config-client>=23.3.0
+Requires-Dist: neuro-config-client>=24.4.3
 
 [![codecov](https://codecov.io/gh/neuro-inc/platform-client-python/branch/master/graph/badge.svg)](https://codecov.io/gh/neuro-inc/platform-client-python)
 
 # Preface
 
 Welcome to Python Neuro-SDK for https://neu.ro/.
```

### Comparing `neuro-sdk-24.2.0/README.md` & `neuro_sdk-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/Makefile` & `neuro_sdk-24.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/buckets_reference.rst` & `neuro_sdk-24.5.0/docs/buckets_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/client_reference.rst` & `neuro_sdk-24.5.0/docs/client_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/conf.py` & `neuro_sdk-24.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/config_reference.rst` & `neuro_sdk-24.5.0/docs/config_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/disks_reference.rst` & `neuro_sdk-24.5.0/docs/disks_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/functions_reference.rst` & `neuro_sdk-24.5.0/docs/functions_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/images_reference.rst` & `neuro_sdk-24.5.0/docs/images_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/index.rst` & `neuro_sdk-24.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/jobs_reference.rst` & `neuro_sdk-24.5.0/docs/jobs_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/jobs_usage.rst` & `neuro_sdk-24.5.0/docs/jobs_usage.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/make.bat` & `neuro_sdk-24.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/parse_reference.rst` & `neuro_sdk-24.5.0/docs/parse_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/plugin_reference.rst` & `neuro_sdk-24.5.0/docs/plugin_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/secrets_reference.rst` & `neuro_sdk-24.5.0/docs/secrets_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/service_accounts_reference.rst` & `neuro_sdk-24.5.0/docs/service_accounts_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/storage_reference.rst` & `neuro_sdk-24.5.0/docs/storage_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/storage_usage.rst` & `neuro_sdk-24.5.0/docs/storage_usage.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/docs/users_reference.rst` & `neuro_sdk-24.5.0/docs/users_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/setup.cfg` & `neuro_sdk-24.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neuro-sdk
-version = 24.2.0
+version = 24.5.0
 description = Neu.ro SDK
 url = https://github.com/neuro-inc/platform-client-python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Neu.ro Team
 author_email = team@neu.ro
 license = Apache 2
@@ -44,15 +44,15 @@
 	certifi
 	toml>=0.10.0
 	azure-storage-blob>=12.8.1,!=12.9.0
 	google-auth>=2.0.2
 	importlib_metadata>=4.11.4; python_version<"3.11"
 	packaging>=20.4
 	neuro-admin-client>=23.5.0
-	neuro-config-client>=23.3.0
+	neuro-config-client>=24.4.3
 
 [options.packages.find]
 where = src
 
 [flake8]
 exclude = .git,.env,__pycache__,.eggs
 max-line-length = 88
```

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/__init__.py` & `neuro_sdk-24.5.0/src/neuro_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     BlobObject,
     Bucket,
     BucketCredentials,
     BucketEntry,
     PersistentBucketCredentials,
 )
 from ._buckets import Buckets
-from ._client import Client, Preset
+from ._client import Client
 from ._clusters import (
     _AWSCloudProvider,
     _AWSStorage,
     _AWSStorageOptions,
     _AzureCloudProvider,
     _AzureReplicationType,
     _AzureStorage,
@@ -135,28 +135,28 @@
     SecretFile,
     Volume,
     VolumeParseResult,
 )
 from ._parsing_utils import LocalImage, RemoteImage, Tag, TagOption
 from ._plugins import ConfigBuilder, ConfigScope, PluginManager, VersionChecker
 from ._secrets import Secret, Secrets
-from ._server_cfg import Cluster, Project
+from ._server_cfg import Cluster, Preset, Project, ResourcePool
 from ._service_accounts import ServiceAccount, ServiceAccounts
 from ._storage import DiskUsageInfo, FileStatus, FileStatusType, Storage
 from ._tracing import gen_trace_id
 from ._url_utils import CLUSTER_SCHEMES as SCHEMES
 from ._users import Action, Permission, Quota, Share, Users
 from ._utils import (
     ORG_NAME_SENTINEL,
     OrgNameSentinel,
     _ContextManager,
     find_project_root,
 )
 
-__version__ = "24.2.0"
+__version__ = "24.5.0"
 
 
 __all__ = (
     "AbstractDeleteProgress",
     "AbstractDockerImageProgress",
     "AbstractFileProgress",
     "AbstractRecursiveFileProgress",
@@ -221,14 +221,15 @@
     "PersistentBucketCredentials",
     "PluginManager",
     "Preset",
     "Project",
     "Quota",
     "RemoteImage",
     "ResourceNotFound",
+    "ResourcePool",
     "Resources",
     "SCHEMES",
     "Secret",
     "SecretFile",
     "Secrets",
     "ServerNotAvailable",
     "ServiceAccount",
```

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_abc.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_abc.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_admin.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_admin.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_azure_bucket_provider.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_azure_bucket_provider.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_bucket_base.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_bucket_base.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_buckets.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_buckets.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_client.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_client.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_clusters.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_clusters.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_config.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,23 @@
 from yarl import URL
 
 from ._core import _Core
 from ._errors import ConfigError
 from ._login import AuthTokenClient, _AuthConfig, _AuthToken
 from ._plugins import ConfigScope, PluginManager, _ParamType
 from ._rewrite import rewrite_module
-from ._server_cfg import Cluster, Preset, Project, _ServerConfig, get_server_config
+from ._server_cfg import (
+    Cluster,
+    Preset,
+    Project,
+    ResourcePool,
+    TPUResource,
+    _ServerConfig,
+    get_server_config,
+)
 from ._utils import NoPublicConstructor, find_project_root, flat
 
 WIN32 = sys.platform == "win32"
 CMD_RE = re.compile("[A-Za-z][A-Za-z0-9-]*")
 
 MALFORMED_CONFIG_MSG = "Malformed config. Please logout and login again."
 
@@ -97,14 +105,18 @@
             return ret
 
     @property
     def username(self) -> str:
         return self._config_data.auth_token.username
 
     @property
+    def resource_pools(self) -> Mapping[str, ResourcePool]:
+        return MappingProxyType(self._cluster.resource_pools)
+
+    @property
     def presets(self) -> Mapping[str, Preset]:
         return MappingProxyType(self._cluster.presets)
 
     @property
     def clusters(self) -> Mapping[str, Cluster]:
         return MappingProxyType(self._config_data.clusters)
 
@@ -635,36 +647,65 @@
             registry_url=URL(cluster_config["registry_url"]),
             storage_url=URL(cluster_config["storage_url"]),
             users_url=URL(cluster_config["users_url"]),
             monitoring_url=URL(cluster_config["monitoring_url"]),
             secrets_url=URL(cluster_config["secrets_url"]),
             disks_url=URL(cluster_config["disks_url"]),
             buckets_url=URL(cluster_config["buckets_url"]),
+            resource_pools=dict(
+                _deserialize_resource_pool(data)
+                for data in cluster_config.get("resource_pools", [])
+            ),
             presets=dict(
                 _deserialize_resource_preset(data)
                 for data in cluster_config.get("presets", [])
             ),
         )
         ret[cluster.name] = cluster
     return ret
 
 
+def _deserialize_resource_pool(payload: Dict[str, Any]) -> Tuple[str, ResourcePool]:
+    tpu = None
+    if "tpu" in payload:
+        tpu = TPUResource(
+            types=payload["tpu"]["types"],
+            software_versions=payload["tpu"]["software_versions"],
+            ipv4_cidr_block=payload["tpu"]["ipv4_cidr_block"],
+        )
+    resource_pool = ResourcePool(
+        min_size=payload["min_size"],
+        max_size=payload["max_size"],
+        cpu=payload["cpu"],
+        memory=payload["memory"],
+        disk_size=payload["disk_size"],
+        nvidia_gpu=payload.get("nvidia_gpu"),
+        amd_gpu=payload.get("amd_gpu"),
+        intel_gpu=payload.get("intel_gpu"),
+        tpu=tpu,
+        is_preemptible=payload.get("is_preemptible", False),
+    )
+    return (payload["name"], resource_pool)
+
+
 def _deserialize_resource_preset(payload: Dict[str, Any]) -> Tuple[str, Preset]:
     return (
         payload["name"],
         Preset(
             credits_per_hour=Decimal(payload["credits_per_hour"]),
             cpu=payload["cpu"],
             memory=payload["memory"],
-            gpu=payload.get("gpu"),
-            gpu_model=payload.get("gpu_model"),
+            nvidia_gpu=payload.get("nvidia_gpu"),
+            amd_gpu=payload.get("amd_gpu"),
+            intel_gpu=payload.get("intel_gpu"),
             tpu_type=payload.get("tpu_type", None),
             tpu_software_version=payload.get("tpu_software_version", None),
             scheduler_enabled=payload.get("scheduler_enabled", False),
             preemptible_node=payload.get("preemptible_node", False),
+            resource_pool_names=payload.get("resource_pool_names", ()),
         ),
     )
 
 
 def _deserialize_auth_token(payload: Dict[str, Any]) -> _AuthToken:
     auth_payload = payload["auth_token"]
     return _AuthToken(
@@ -774,35 +815,63 @@
             "registry_url": str(cluster.registry_url),
             "storage_url": str(cluster.storage_url),
             "users_url": str(cluster.users_url),
             "monitoring_url": str(cluster.monitoring_url),
             "secrets_url": str(cluster.secrets_url),
             "disks_url": str(cluster.disks_url),
             "buckets_url": str(cluster.buckets_url),
+            "resource_pools": [
+                _serialize_resource_pool(name, resource_pool)
+                for name, resource_pool in cluster.resource_pools.items()
+            ],
             "presets": [
                 _serialize_resource_preset(name, preset)
                 for name, preset in cluster.presets.items()
             ],
         }
         ret.append(cluster_config)
     return json.dumps(ret)
 
 
+def _serialize_resource_pool(name: str, resource_pool: ResourcePool) -> Dict[str, Any]:
+    result = {
+        "name": name,
+        "min_size": resource_pool.min_size,
+        "max_size": resource_pool.max_size,
+        "cpu": resource_pool.cpu,
+        "memory": resource_pool.memory,
+        "disk_size": resource_pool.disk_size,
+        "nvidia_gpu": resource_pool.nvidia_gpu,
+        "amd_gpu": resource_pool.amd_gpu,
+        "intel_gpu": resource_pool.intel_gpu,
+        "is_preemptible": resource_pool.is_preemptible,
+    }
+    if resource_pool.tpu:
+        result["tpu"] = {
+            "types": resource_pool.tpu.types,
+            "software_versions": resource_pool.tpu.software_versions,
+            "ipv4_cidr_block": resource_pool.tpu.ipv4_cidr_block,
+        }
+    return result
+
+
 def _serialize_resource_preset(name: str, preset: Preset) -> Dict[str, Any]:
     return {
         "name": name,
         "credits_per_hour": str(preset.credits_per_hour),
         "cpu": preset.cpu,
         "memory": preset.memory,
-        "gpu": preset.gpu,
-        "gpu_model": preset.gpu_model,
+        "nvidia_gpu": preset.nvidia_gpu,
+        "amd_gpu": preset.amd_gpu,
+        "intel_gpu": preset.intel_gpu,
         "tpu_type": preset.tpu_type,
         "tpu_software_version": preset.tpu_software_version,
         "scheduler_enabled": preset.scheduler_enabled,
         "preemptible_node": preset.preemptible_node,
+        "resource_pool_names": preset.resource_pool_names,
     }
 
 
 def _merge_user_configs(
     older: Mapping[str, Any], newer: Mapping[str, Any]
 ) -> Mapping[str, Any]:
     ret: Dict[str, Any] = {}
```

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_config_factory.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_config_factory.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_core.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_core.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_disks.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_disks.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_errors.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_errors.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_file_filter.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_file_filter.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_file_utils.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_file_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_gcs_bucket_provider.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_gcs_bucket_provider.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_images.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_images.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_jobs.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,17 @@
 
 
 @rewrite_module
 @dataclass(frozen=True)
 class Resources:
     memory: int
     cpu: float
-    gpu: Optional[int] = None
-    gpu_model: Optional[str] = None
+    nvidia_gpu: Optional[int] = None
+    amd_gpu: Optional[int] = None
+    intel_gpu: Optional[int] = None
     shm: bool = True
     tpu_type: Optional[str] = None
     tpu_software_version: Optional[str] = None
 
     @property
     def memory_mb(self) -> int:
         return self.memory // 2**20
@@ -877,17 +878,20 @@
 
 def _resources_to_api(resources: Resources) -> Dict[str, Any]:
     value: Dict[str, Any] = {
         "memory": resources.memory,
         "cpu": resources.cpu,
         "shm": resources.shm,
     }
-    if resources.gpu:
-        value["gpu"] = resources.gpu
-        value["gpu_model"] = resources.gpu_model
+    if resources.nvidia_gpu:
+        value["nvidia_gpu"] = resources.nvidia_gpu
+    if resources.amd_gpu:
+        value["amd_gpu"] = resources.amd_gpu
+    if resources.intel_gpu:
+        value["intel_gpu"] = resources.intel_gpu
     if resources.tpu_type:
         assert resources.tpu_software_version
         value["tpu"] = {
             "type": resources.tpu_type,
             "software_version": resources.tpu_software_version,
         }
     return value
@@ -899,16 +903,17 @@
         tpu = data["tpu"]
         tpu_type = tpu["type"]
         tpu_software_version = tpu["software_version"]
     return Resources(
         memory=data["memory"],
         cpu=data["cpu"],
         shm=data.get("shm", True),
-        gpu=data.get("gpu", None),
-        gpu_model=data.get("gpu_model", None),
+        nvidia_gpu=data.get("nvidia_gpu", None),
+        amd_gpu=data.get("amd_gpu", None),
+        intel_gpu=data.get("intel_gpu", None),
         tpu_type=tpu_type,
         tpu_software_version=tpu_software_version,
     )
 
 
 def _http_port_to_api(port: HTTPPort) -> Dict[str, Any]:
     return {"port": port.port, "requires_auth": port.requires_auth}
```

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_login.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_login.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_parser.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_parser.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_parsing_utils.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_plugins.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_plugins.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_s3_bucket_provider.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_s3_bucket_provider.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_secrets.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_secrets.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_server_cfg.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_server_cfg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from decimal import Decimal
-from typing import Any, Dict, List, Mapping, Optional
+from typing import Any, Dict, List, Mapping, Optional, Sequence
 
 import aiohttp
 from yarl import URL
 
 from ._errors import AuthError
 from ._login import _AuthConfig
 from ._rewrite import rewrite_module
@@ -12,26 +12,50 @@
 
 @rewrite_module
 @dataclass(frozen=True)
 class Preset:
     credits_per_hour: Decimal
     cpu: float
     memory: int
+    nvidia_gpu: Optional[int] = None
+    amd_gpu: Optional[int] = None
+    intel_gpu: Optional[int] = None
     scheduler_enabled: bool = False
     preemptible_node: bool = False
-    gpu: Optional[int] = None
-    gpu_model: Optional[str] = None
     tpu_type: Optional[str] = None
     tpu_software_version: Optional[str] = None
+    resource_pool_names: Sequence[str] = ()
 
     @property
     def memory_mb(self) -> int:
         return self.memory // 2**20
 
 
+@dataclass(frozen=True)
+class TPUResource:
+    ipv4_cidr_block: str
+    types: Sequence[str] = ()
+    software_versions: Sequence[str] = ()
+
+
+@rewrite_module
+@dataclass(frozen=True)
+class ResourcePool:
+    min_size: int
+    max_size: int
+    cpu: float
+    memory: int
+    disk_size: int
+    nvidia_gpu: Optional[int] = None
+    amd_gpu: Optional[int] = None
+    intel_gpu: Optional[int] = None
+    tpu: Optional[TPUResource] = None
+    is_preemptible: bool = False
+
+
 @rewrite_module
 @dataclass(frozen=True)
 class Project:
     @dataclass(frozen=True)
     class Key:
         cluster_name: str
         org_name: Optional[str]
@@ -59,14 +83,15 @@
     registry_url: URL
     storage_url: URL
     users_url: URL
     monitoring_url: URL
     secrets_url: URL
     disks_url: URL
     buckets_url: URL
+    resource_pools: Mapping[str, ResourcePool]
     presets: Mapping[str, Preset]
 
 
 @dataclass(frozen=True)
 class _ServerConfig:
     admin_url: Optional[URL]
     auth_config: _AuthConfig
@@ -88,43 +113,66 @@
     for item in payload.get("projects", []):
         project = _parse_project_config(item)
         ret[project.key] = project
     return ret
 
 
 def _parse_cluster_config(payload: Dict[str, Any]) -> Cluster:
+    resource_pools = {}
+    for data in payload["resource_pool_types"]:
+        tpu = None
+        if "tpu" in data:
+            tpu = TPUResource(
+                types=data["tpu"]["types"],
+                software_versions=data["tpu"]["software_versions"],
+                ipv4_cidr_block=data["tpu"]["ipv4_cidr_block"],
+            )
+        resource_pools[data["name"]] = ResourcePool(
+            min_size=data["min_size"],
+            max_size=data["max_size"],
+            cpu=data["cpu"],
+            memory=data["memory"],
+            disk_size=data["disk_size"],
+            nvidia_gpu=data.get("nvidia_gpu"),
+            amd_gpu=data.get("amd_gpu"),
+            intel_gpu=data.get("intel_gpu"),
+            tpu=tpu,
+            is_preemptible=data.get("is_preemptible", False),
+        )
     presets: Dict[str, Preset] = {}
     for data in payload["resource_presets"]:
         tpu_type = tpu_software_version = None
         if "tpu" in data:
             tpu_payload = data["tpu"]
             tpu_type = tpu_payload["type"]
             tpu_software_version = tpu_payload["software_version"]
         presets[data["name"]] = Preset(
-            # TODO: make credits_per_hour not optional after server updated
-            credits_per_hour=Decimal(data.get("credits_per_hour", "0")),
+            credits_per_hour=Decimal(data["credits_per_hour"]),
             cpu=data["cpu"],
             memory=data["memory"],
-            gpu=data.get("gpu"),
-            gpu_model=data.get("gpu_model"),
+            nvidia_gpu=data.get("nvidia_gpu"),
+            amd_gpu=data.get("amd_gpu"),
+            intel_gpu=data.get("intel_gpu"),
             scheduler_enabled=data.get("scheduler_enabled", False),
             preemptible_node=data.get("preemptible_node", False),
             tpu_type=tpu_type,
             tpu_software_version=tpu_software_version,
+            resource_pool_names=data.get("resource_pool_names", ()),
         )
     cluster_config = Cluster(
         name=payload["name"],
         orgs=payload.get("orgs", [None]),
         registry_url=URL(payload["registry_url"]),
         storage_url=URL(payload["storage_url"]),
         users_url=URL(payload["users_url"]),
         monitoring_url=URL(payload["monitoring_url"]),
         secrets_url=URL(payload["secrets_url"]),
         disks_url=URL(payload["disks_url"]),
         buckets_url=URL(payload["buckets_url"]),
+        resource_pools=resource_pools,
         presets=presets,
     )
     return cluster_config
 
 
 def _parse_clusters(payload: Dict[str, Any]) -> Dict[str, Cluster]:
     ret: Dict[str, Cluster] = {}
```

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_service_accounts.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_service_accounts.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_storage.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_tracing.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_tracing.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_url_utils.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_url_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_users.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_users.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_utils.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk/_version_utils.py` & `neuro_sdk-24.5.0/src/neuro_sdk/_version_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk.egg-info/PKG-INFO` & `neuro_sdk-24.5.0/src/neuro_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-sdk
-Version: 24.2.0
+Version: 24.5.0
 Summary: Neu.ro SDK
 Home-page: https://github.com/neuro-inc/platform-client-python
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -35,15 +35,15 @@
 Requires-Dist: certifi
 Requires-Dist: toml>=0.10.0
 Requires-Dist: azure-storage-blob!=12.9.0,>=12.8.1
 Requires-Dist: google-auth>=2.0.2
 Requires-Dist: importlib_metadata>=4.11.4; python_version < "3.11"
 Requires-Dist: packaging>=20.4
 Requires-Dist: neuro-admin-client>=23.5.0
-Requires-Dist: neuro-config-client>=23.3.0
+Requires-Dist: neuro-config-client>=24.4.3
 
 [![codecov](https://codecov.io/gh/neuro-inc/platform-client-python/branch/master/graph/badge.svg)](https://codecov.io/gh/neuro-inc/platform-client-python)
 
 # Preface
 
 Welcome to Python Neuro-SDK for https://neu.ro/.
```

### Comparing `neuro-sdk-24.2.0/src/neuro_sdk.egg-info/SOURCES.txt` & `neuro_sdk-24.5.0/src/neuro_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/__init__.py` & `neuro_sdk-24.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/data/file.txt` & `neuro_sdk-24.5.0/tests/data/file.txt`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_admin.py` & `neuro_sdk-24.5.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_blob_storage.py` & `neuro_sdk-24.5.0/tests/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_bucket_persistent_credentials.py` & `neuro_sdk-24.5.0/tests/test_bucket_persistent_credentials.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_buckets.py` & `neuro_sdk-24.5.0/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_client.py` & `neuro_sdk-24.5.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_clusters.py` & `neuro_sdk-24.5.0/tests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_config.py` & `neuro_sdk-24.5.0/tests/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Client,
     Cluster,
     ConfigError,
     ConfigScope,
     PluginManager,
     Preset,
     Project,
+    ResourcePool,
 )
 from neuro_sdk._config import (
     _check_sections,
     _merge_user_configs,
     _validate_user_config,
 )
 from neuro_sdk._login import _AuthToken
@@ -174,49 +175,82 @@
             registry_url=URL("https://registry-dev.neu.ro"),
             storage_url=URL("https://storage-dev.neu.ro"),
             users_url=URL("https://users-dev.neu.ro"),
             monitoring_url=URL("https://jobs-dev.neu.ro"),
             secrets_url=URL("https://secrets-dev.neu.ro"),
             disks_url=URL("https://disks-dev.neu.ro"),
             buckets_url=URL("https://buckets-dev.neu.ro"),
+            resource_pools={
+                "cpu": ResourcePool(
+                    min_size=1,
+                    max_size=2,
+                    cpu=7,
+                    memory=14 * 2**30,
+                    disk_size=150 * 2**30,
+                )
+            },
             presets={
                 "cpu-small": Preset(
-                    credits_per_hour=Decimal("10"), cpu=1, memory=2 * 2**30
+                    credits_per_hour=Decimal("10"),
+                    cpu=1,
+                    memory=2 * 2**30,
                 )
             },
         ),
         "another": Cluster(
             name="another",
             orgs=["some-org", None],
             registry_url=URL("https://registry2-dev.neu.ro"),
             storage_url=URL("https://storage2-dev.neu.ro"),
             users_url=URL("https://users2-dev.neu.ro"),
             monitoring_url=URL("https://jobs2-dev.neu.ro"),
             secrets_url=URL("https://secrets2-dev.neu.ro"),
             disks_url=URL("https://disks2-dev.neu.ro"),
             buckets_url=URL("https://buckets2-dev.neu.ro"),
+            resource_pools={
+                "cpu": ResourcePool(
+                    min_size=1,
+                    max_size=2,
+                    cpu=7,
+                    memory=14 * 2**30,
+                    disk_size=150 * 2**30,
+                )
+            },
             presets={
                 "cpu-large": Preset(
-                    credits_per_hour=Decimal("10"), cpu=7, memory=14 * 2**30
+                    credits_per_hour=Decimal("10"),
+                    cpu=7,
+                    memory=14 * 2**30,
                 )
             },
         ),
         "third": Cluster(
             name="third",
             orgs=["some-org", "a-org"],
             registry_url=URL("https://registry3-dev.neu.ro"),
             storage_url=URL("https://storage3-dev.neu.ro"),
             users_url=URL("https://users3-dev.neu.ro"),
             monitoring_url=URL("https://jobs3-dev.neu.ro"),
             secrets_url=URL("https://secrets3-dev.neu.ro"),
             disks_url=URL("https://disks3-dev.neu.ro"),
             buckets_url=URL("https://buckets3-dev.neu.ro"),
+            resource_pools={
+                "cpu": ResourcePool(
+                    min_size=1,
+                    max_size=2,
+                    cpu=7,
+                    memory=14 * 2**30,
+                    disk_size=150 * 2**30,
+                )
+            },
             presets={
                 "cpu-large": Preset(
-                    credits_per_hour=Decimal("10"), cpu=7, memory=14 * 2**30
+                    credits_per_hour=Decimal("10"),
+                    cpu=7,
+                    memory=14 * 2**30,
                 )
             },
         ),
     }
 
 
 async def test_get_cluster_name_from_local(
@@ -241,30 +275,36 @@
         assert client.config.storage_url == URL("https://storage-dev.neu.ro")
         assert client.config.monitoring_url == URL("https://jobs-dev.neu.ro")
         assert client.config.secrets_url == URL("https://secrets-dev.neu.ro")
         assert client.config.disk_api_url == URL("https://disks-dev.neu.ro")
         assert client.config.bucket_api_url == URL("https://buckets-dev.neu.ro")
         assert client.config.presets == {
             "cpu-small": Preset(
-                credits_per_hour=Decimal("10"), cpu=1, memory=2 * 2**30
+                credits_per_hour=Decimal("10"),
+                cpu=1,
+                memory=2 * 2**30,
+                resource_pool_names=[],
             )
         }
 
         local_conf = proj_dir / ".neuro.toml"
         local_conf.write_text(toml.dumps({"job": {"cluster-name": "another"}}))
         assert client.config.cluster_name == "another"
         assert client.config.registry_url == URL("https://registry2-dev.neu.ro")
         assert client.config.storage_url == URL("https://storage2-dev.neu.ro")
         assert client.config.monitoring_url == URL("https://jobs2-dev.neu.ro")
         assert client.config.secrets_url == URL("https://secrets2-dev.neu.ro")
         assert client.config.disk_api_url == URL("https://disks2-dev.neu.ro")
         assert client.config.bucket_api_url == URL("https://buckets2-dev.neu.ro")
         assert client.config.presets == {
             "cpu-large": Preset(
-                credits_per_hour=Decimal("10"), cpu=7, memory=14 * 2**30
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=14 * 2**30,
+                resource_pool_names=[],
             )
         }
 
 
 async def test_get_cluster_name_from_local_invalid_cluster(
     monkeypatch: Any,
     tmp_path: Path,
@@ -317,48 +357,82 @@
     async with make_client(srv.make_url("/")) as client:
         assert client.config.presets == {
             "cpu-large": Preset(
                 credits_per_hour=Decimal("10"),
                 cpu=7,
                 memory=14336 * 2**20,
                 scheduler_enabled=False,
-                gpu=None,
-                gpu_model=None,
-                tpu_type=None,
-                tpu_software_version=None,
+                resource_pool_names=[],
             ),
             "cpu-small": Preset(
                 credits_per_hour=Decimal("10"),
                 cpu=7,
                 memory=2048 * 2**20,
                 scheduler_enabled=False,
-                gpu=None,
-                gpu_model=None,
+                resource_pool_names=[],
+            ),
+            "nvidia-gpu-large": Preset(
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=61440 * 2**20,
+                scheduler_enabled=False,
+                nvidia_gpu=1,
+                tpu_type=None,
+                tpu_software_version=None,
+                resource_pool_names=["nvidia-gpu"],
+            ),
+            "nvidia-gpu-small": Preset(
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=30720 * 2**20,
+                scheduler_enabled=False,
+                nvidia_gpu=1,
+                tpu_type=None,
+                tpu_software_version=None,
+                resource_pool_names=["nvidia-gpu"],
+            ),
+            "amd-gpu-large": Preset(
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=61440 * 2**20,
+                scheduler_enabled=False,
+                amd_gpu=1,
+                tpu_type=None,
+                tpu_software_version=None,
+                resource_pool_names=["amd-gpu"],
+            ),
+            "amd-gpu-small": Preset(
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=30720 * 2**20,
+                scheduler_enabled=False,
+                amd_gpu=1,
                 tpu_type=None,
                 tpu_software_version=None,
+                resource_pool_names=["amd-gpu"],
             ),
-            "gpu-large": Preset(
+            "intel-gpu-large": Preset(
                 credits_per_hour=Decimal("10"),
                 cpu=7,
                 memory=61440 * 2**20,
                 scheduler_enabled=False,
-                gpu=1,
-                gpu_model="nvidia-tesla-v100",
+                intel_gpu=1,
                 tpu_type=None,
                 tpu_software_version=None,
+                resource_pool_names=["intel-gpu"],
             ),
-            "gpu-small": Preset(
+            "intel-gpu-small": Preset(
                 credits_per_hour=Decimal("10"),
                 cpu=7,
                 memory=30720 * 2**20,
                 scheduler_enabled=False,
-                gpu=1,
-                gpu_model="nvidia-tesla-k80",
+                intel_gpu=1,
                 tpu_type=None,
                 tpu_software_version=None,
+                resource_pool_names=["intel-gpu"],
             ),
         }
 
 
 async def test_cluster_name(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
@@ -394,26 +468,28 @@
                 registry_url=URL("https://registry-dev.neu.ro"),
                 storage_url=srv.make_url("/storage"),
                 users_url=srv.make_url("/"),
                 monitoring_url=srv.make_url("/jobs"),
                 secrets_url=srv.make_url("/secrets"),
                 disks_url=srv.make_url("/disk"),
                 buckets_url=srv.make_url("/buckets"),
+                resource_pools=mock.ANY,
                 presets=mock.ANY,
             ),
             "another": Cluster(
                 name="another",
                 orgs=[None, "some_org"],
                 registry_url=srv.make_url("/registry2"),
                 storage_url=srv.make_url("/storage2"),
                 users_url=srv.make_url("/"),
                 monitoring_url=srv.make_url("/jobs2"),
                 secrets_url=srv.make_url("/secrets2"),
                 disks_url=srv.make_url("/disk2"),
                 buckets_url=srv.make_url("/buckets2"),
+                resource_pools=mock.ANY,
                 presets=mock.ANY,
             ),
         }
 
 
 async def test_project_name(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
@@ -486,14 +562,24 @@
                 "registry_url": registry_url,
                 "storage_url": storage_url,
                 "users_url": users_url,
                 "monitoring_url": monitoring_url,
                 "secrets_url": secrets_url,
                 "disks_url": disks_url,
                 "buckets_url": buckets_url,
+                "resource_pool_types": [
+                    {
+                        "name": "cpu",
+                        "min_size": 1,
+                        "max_size": 2,
+                        "cpu": 7,
+                        "memory": 14 * 2**30,
+                        "disk_size": 150 * 2**30,
+                    }
+                ],
                 "resource_presets": [
                     {
                         "name": "cpu-small",
                         "credits_per_hour": "10",
                         "cpu": 2,
                         "memory": 2 * 2**30,
                     }
@@ -526,24 +612,29 @@
                 registry_url=URL(registry_url),
                 storage_url=URL(storage_url),
                 users_url=URL(users_url),
                 monitoring_url=URL(monitoring_url),
                 secrets_url=URL(secrets_url),
                 disks_url=URL(disks_url),
                 buckets_url=URL(buckets_url),
+                resource_pools={
+                    "cpu": ResourcePool(
+                        min_size=1,
+                        max_size=2,
+                        cpu=7,
+                        memory=14 * 2**30,
+                        disk_size=150 * 2**30,
+                    )
+                },
                 presets={
                     "cpu-small": Preset(
                         credits_per_hour=Decimal("10"),
                         cpu=2,
                         memory=2048 * 2**20,
                         scheduler_enabled=False,
-                        gpu=None,
-                        gpu_model=None,
-                        tpu_type=None,
-                        tpu_software_version=None,
                     )
                 },
             )
         }
 
         project = Project(
             name="some-project",
@@ -587,14 +678,24 @@
                 "registry_url": registry_url,
                 "storage_url": storage_url,
                 "users_url": users_url,
                 "monitoring_url": monitoring_url,
                 "secrets_url": secrets_url,
                 "disks_url": disks_url,
                 "buckets_url": buckets_url,
+                "resource_pool_types": [
+                    {
+                        "name": "cpu",
+                        "min_size": 1,
+                        "max_size": 2,
+                        "cpu": 7,
+                        "memory": 14 * 2**30,
+                        "disk_size": 150 * 2**30,
+                    }
+                ],
                 "resource_presets": [
                     {
                         "name": "cpu-small",
                         "credits_per_hour": "10",
                         "cpu": 2,
                         "memory": 2 * 2**30,
                     }
@@ -650,14 +751,24 @@
                 "registry_url": registry_url,
                 "storage_url": storage_url,
                 "users_url": users_url,
                 "monitoring_url": monitoring_url,
                 "secrets_url": secrets_url,
                 "disks_url": disks_url,
                 "buckets_url": buckets_url,
+                "resource_pool_types": [
+                    {
+                        "name": "cpu",
+                        "min_size": 1,
+                        "max_size": 2,
+                        "cpu": 7,
+                        "memory": 14 * 2**30,
+                        "disk_size": 150 * 2**30,
+                    }
+                ],
                 "resource_presets": [
                     {
                         "name": "cpu-small",
                         "credits_per_hour": "10",
                         "cpu": 2,
                         "memory": 2 * 2**30,
                     }
@@ -968,14 +1079,24 @@
                 "registry_url": registry_url,
                 "storage_url": storage_url,
                 "users_url": users_url,
                 "monitoring_url": monitoring_url,
                 "secrets_url": secrets_url,
                 "disks_url": disks_url,
                 "buckets_url": buckets_url,
+                "resource_pool_types": [
+                    {
+                        "name": "cpu",
+                        "min_size": 1,
+                        "max_size": 2,
+                        "cpu": 7,
+                        "memory": 14 * 2**30,
+                        "disk_size": 150 * 2**30,
+                    }
+                ],
                 "resource_presets": [
                     {
                         "name": "cpu-small",
                         "credits_per_hour": "10",
                         "cpu": 2,
                         "memory": 2 * 2**30,
                     }
@@ -1034,14 +1155,24 @@
                 "registry_url": registry_url,
                 "storage_url": storage_url,
                 "users_url": users_url,
                 "monitoring_url": monitoring_url,
                 "secrets_url": secrets_url,
                 "disks_url": disks_url,
                 "buckets_url": buckets_url,
+                "resource_pool_types": [
+                    {
+                        "name": "cpu",
+                        "min_size": 1,
+                        "max_size": 2,
+                        "cpu": 7,
+                        "memory": 14 * 2**30,
+                        "disk_size": 150 * 2**30,
+                    }
+                ],
                 "resource_presets": [
                     {
                         "name": "cpu-small",
                         "credits_per_hour": "10",
                         "cpu": 2,
                         "memory": 2 * 2**30,
                     }
```

### Comparing `neuro-sdk-24.2.0/tests/test_config_factory.py` & `neuro_sdk-24.5.0/tests/test_config_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,42 +116,119 @@
                     "registry_url": "https://registry-dev.test.com",
                     "storage_url": "https://storage-dev.test.com",
                     "users_url": "https://users-dev.test.com",
                     "monitoring_url": "https://monitoring-dev.test.com",
                     "secrets_url": "https://secrets-dev.test.com",
                     "disks_url": "https://disks-dev.test.com",
                     "buckets_url": "https://buckets-dev.test.com",
+                    "resource_pool_types": [
+                        {
+                            "name": "cpu",
+                            "min_size": 1,
+                            "max_size": 2,
+                            "cpu": 7,
+                            "memory": 14 * 2**30,
+                            "disk_size": 150 * 2**30,
+                        },
+                        {
+                            "name": "nvidia-gpu",
+                            "min_size": 0,
+                            "max_size": 1,
+                            "cpu": 7,
+                            "memory": 60 * 2**30,
+                            "disk_size": 150 * 2**30,
+                            "nvidia_gpu": 1,
+                        },
+                        {
+                            "name": "amd-gpu",
+                            "min_size": 0,
+                            "max_size": 1,
+                            "cpu": 7,
+                            "memory": 60 * 2**30,
+                            "disk_size": 150 * 2**30,
+                            "amd_gpu": 1,
+                        },
+                        {
+                            "name": "intel-gpu",
+                            "min_size": 0,
+                            "max_size": 1,
+                            "cpu": 7,
+                            "memory": 60 * 2**30,
+                            "disk_size": 150 * 2**30,
+                            "intel_gpu": 1,
+                        },
+                    ],
                     "resource_presets": [
                         {
-                            "name": "gpu-small",
+                            "name": "nvidia-gpu-small",
+                            "credits_per_hour": "10",
+                            "cpu": 7,
+                            "memory": 30 * 2**30,
+                            "nvidia_gpu": 1,
+                            "resource_pool_names": ["nvidia-gpu"],
+                            "available_resource_pool_names": ["nvidia-gpu"],
+                        },
+                        {
+                            "name": "nvidia-gpu-large",
+                            "credits_per_hour": "10",
+                            "cpu": 7,
+                            "memory": 60 * 2**30,
+                            "nvidia_gpu": 1,
+                            "resource_pool_names": ["nvidia-gpu"],
+                            "available_resource_pool_names": ["nvidia-gpu"],
+                        },
+                        {
+                            "name": "amd-gpu-small",
+                            "credits_per_hour": "10",
+                            "cpu": 7,
+                            "memory": 30 * 2**30,
+                            "amd_gpu": 1,
+                            "resource_pool_names": ["amd-gpu"],
+                            "available_resource_pool_names": ["amd-gpu"],
+                        },
+                        {
+                            "name": "amd-gpu-large",
+                            "credits_per_hour": "10",
+                            "cpu": 7,
+                            "memory": 60 * 2**30,
+                            "amd_gpu": 1,
+                            "resource_pool_names": ["amd-gpu"],
+                            "available_resource_pool_names": ["amd-gpu"],
+                        },
+                        {
+                            "name": "intel-gpu-small",
                             "credits_per_hour": "10",
                             "cpu": 7,
                             "memory": 30 * 2**30,
-                            "gpu": 1,
-                            "gpu_model": "nvidia-tesla-k80",
+                            "intel_gpu": 1,
+                            "resource_pool_names": ["intel-gpu"],
+                            "available_resource_pool_names": ["intel-gpu"],
                         },
                         {
-                            "name": "gpu-large",
+                            "name": "intel-gpu-large",
                             "credits_per_hour": "10",
                             "cpu": 7,
                             "memory": 60 * 2**30,
-                            "gpu": 1,
-                            "gpu_model": "nvidia-tesla-v100",
+                            "intel_gpu": 1,
+                            "resource_pool_names": ["intel-gpu"],
+                            "available_resource_pool_names": ["intel-gpu"],
                         },
                         {
                             "name": "cpu-small",
                             "credits_per_hour": "10",
                             "cpu": 2,
                             "memory": 2 * 2**30,
+                            "available_resource_pool_names": ["cpu"],
                         },
                         {
                             "name": "cpu-large",
                             "credits_per_hour": "10",
                             "cpu": 3,
                             "memory": 14 * 2**30,
+                            "available_resource_pool_names": ["cpu"],
                         },
                     ],
                 }
                 project_config: Dict[str, Any] = {
                     "cluster_name": "default",
                     "org_name": None,
                     "name": "default",
@@ -195,15 +272,15 @@
         return srv
 
     return _factory
 
 
 @pytest.fixture
 async def mock_for_login(
-    mock_for_login_factory: Callable[[MockForLoginControl], Awaitable[_TestServer]]
+    mock_for_login_factory: Callable[[MockForLoginControl], Awaitable[_TestServer]],
 ) -> _TestServer:
     return await mock_for_login_factory(MockForLoginControl())
 
 
 class TestConfigFileInteraction:
     async def test_config_file_absent(self, tmp_home: Path) -> None:
         with pytest.raises(ConfigError, match=r"file.+not exists"):
```

### Comparing `neuro-sdk-24.2.0/tests/test_core.py` & `neuro_sdk-24.5.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_disks.py` & `neuro_sdk-24.5.0/tests/test_disks.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_file_filter.py` & `neuro_sdk-24.5.0/tests/test_file_filter.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_file_utils.py` & `neuro_sdk-24.5.0/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_images.py` & `neuro_sdk-24.5.0/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_jobs.py` & `neuro_sdk-24.5.0/tests/test_jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,17 @@
 
 
 def test_resources_default() -> None:
     resources = Resources(16 * 2**20, 0.5)
     assert resources.memory == 16 * 2**20
     assert resources.memory_mb == 16
     assert resources.cpu == 0.5
-    assert resources.gpu is None
-    assert resources.gpu_model is None
+    assert resources.nvidia_gpu is None
+    assert resources.amd_gpu is None
+    assert resources.intel_gpu is None
     assert resources.shm is True
     assert resources.tpu_type is None
     assert resources.tpu_software_version is None
 
 
 async def test_jobs_monitor(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
@@ -588,16 +589,15 @@
             "image": "submit-image-name",
             "command": "submit-command",
             "http": {"port": 8181},
             "resources": {
                 "memory": 4096 * 2**20,
                 "cpu": 7.0,
                 "shm": True,
-                "gpu": 1,
-                "gpu_model": "test-gpu-model",
+                "nvidia_gpu": 1,
             },
             "volumes": [
                 {
                     "src_storage_uri": "storage://test-user/path_read_only",
                     "dst_path": "/container/read_only",
                     "read_only": True,
                 },
@@ -654,16 +654,15 @@
             "image": "submit-image-name",
             "command": "submit-command",
             "http": {"port": 8181},
             "resources": {
                 "memory": 4096 * 2**20,
                 "cpu": 7.0,
                 "shm": True,
-                "gpu": 1,
-                "gpu_model": "test-gpu-model",
+                "nvidia_gpu": 1,
             },
             "volumes": [
                 {
                     "src_storage_uri": "storage://test-user/path_read_only",
                     "dst_path": "/container/read_only",
                     "read_only": True,
                 },
@@ -718,16 +717,15 @@
             "image": "submit-image-name",
             "command": "submit-command",
             "http": {"port": 8181},
             "resources": {
                 "memory": 4096 * 2**20,
                 "cpu": 7.0,
                 "shm": True,
-                "gpu": 1,
-                "gpu_model": "test-gpu-model",
+                "nvidia_gpu": 1,
             },
             "volumes": [
                 {
                     "src_storage_uri": "storage://test-user/path_read_only",
                     "dst_path": "/container/read_only",
                     "read_only": True,
                 },
@@ -780,16 +778,15 @@
             "image": "submit-image-name",
             "command": "submit-command",
             "http": {"port": 8181},
             "resources": {
                 "memory": 4096 * 2**20,
                 "cpu": 7.0,
                 "shm": True,
-                "gpu": 1,
-                "gpu_model": "test-gpu-model",
+                "nvidia_gpu": 1,
                 "tpu": {"type": "v3-8", "software_version": "1.14"},
             },
             "volumes": [
                 {
                     "src_storage_uri": "storage://test-user/path_read_only",
                     "dst_path": "/container/read_only",
                     "read_only": True,
@@ -860,17 +857,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
 
@@ -953,17 +949,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
         "privileged": True,
     }
@@ -1020,17 +1015,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
         "privileged": True,
         "priority": "high",
@@ -1125,17 +1119,18 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
+                "amd_gpu": 2,
+                "intel_gpu": 3,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
 
@@ -1146,16 +1141,17 @@
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "http": {"port": 8181, "requires_auth": True},
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
+                    "amd_gpu": 2,
+                    "intel_gpu": 3,
                 },
                 "volumes": [
                     {
                         "src_storage_uri": "storage://test-user/path_read_only",
                         "dst_path": "/container/read_only",
                         "read_only": True,
                     },
@@ -1176,15 +1172,22 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(
+            memory=16384 * 2**20,
+            cpu=7,
+            nvidia_gpu=1,
+            amd_gpu=2,
+            intel_gpu=3,
+            shm=True,
+        )
         volumes: List[Volume] = [
             Volume(
                 URL("storage://test-user/path_read_only"), "/container/read_only", True
             ),
             Volume(
                 URL("storage://test-user/path_read_write"),
                 "/container/path_read_write",
@@ -1225,17 +1228,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
 
@@ -1245,16 +1247,15 @@
             "container": {
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
             },
             "scheduler_enabled": False,
             "wait_for_jobs_quota": True,
             "pass_config": False,
             "cluster_name": "default",
             "project_name": "test-project",
@@ -1264,15 +1265,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         container = Container(
             image=RemoteImage.new_external_image(name="submit-image-name"),
             command="submit-command",
             resources=resources,
         )
         ret = await client.jobs.run(
             container=container, scheduler_enabled=False, wait_for_jobs_quota=True
@@ -1305,17 +1306,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
 
@@ -1326,16 +1326,15 @@
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "http": {"port": 8181, "requires_auth": True},
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
                 "volumes": [
                     {
                         "src_storage_uri": "storage://test-user/path_read_only",
                         "dst_path": "/container/read_only",
                         "read_only": True,
                     },
@@ -1358,15 +1357,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         volumes: List[Volume] = [
             Volume(
                 URL("storage://test-user/path_read_only"), "/container/read_only", True
             ),
             Volume(
                 URL("storage://test-user/path_read_write"),
                 "/container/path_read_write",
@@ -1413,17 +1412,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
 
@@ -1434,16 +1432,15 @@
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "http": {"port": 8181, "requires_auth": True},
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
                 "volumes": [
                     {
                         "src_storage_uri": "storage://test-user/path_read_only",
                         "dst_path": "/container/read_only",
                         "read_only": True,
                     },
@@ -1465,15 +1462,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         volumes: List[Volume] = [
             Volume(
                 URL("storage://test-user/path_read_only"), "/container/read_only", True
             ),
             Volume(
                 URL("storage://test-user/path_read_write"),
                 "/container/path_read_write",
@@ -1519,17 +1516,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 7,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
 
@@ -1540,16 +1536,15 @@
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "http": {"port": 8181, "requires_auth": True},
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "name": "test-job-name",
             "description": "job description",
             "cluster_name": "default",
@@ -1560,15 +1555,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         container = Container(
             image=RemoteImage.new_external_image(name="submit-image-name"),
             command="submit-command",
             resources=resources,
             http=HTTPPort(8181),
         )
         ret = await client.jobs.run(
@@ -1603,17 +1598,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
 
@@ -1624,16 +1618,15 @@
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "http": {"port": 8181, "requires_auth": True},
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
                 "volumes": [
                     {
                         "src_storage_uri": "storage://default/test-project/path",
                         "dst_path": "/container/my_path",
                         "read_only": False,
                     },
@@ -1659,15 +1652,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         volumes: List[Volume] = [
             Volume(URL("storage:path"), "/container/my_path", False),
             Volume(
                 URL("storage:/otherproject/path"),
                 "/container/other_user_path",
                 True,
             ),
@@ -1711,17 +1704,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
 
@@ -1732,16 +1724,15 @@
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "http": {"port": 8181, "requires_auth": True},
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
                 "env": {"VAR": "VAL"},
                 "secret_env": {"SECRET_VAR": "secret://default/test-project/secret"},
                 "volumes": [
                     {
                         "src_storage_uri": "storage://default/test-project/path",
                         "dst_path": "/container/my_path",
@@ -1765,15 +1756,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         env = {"VAR": "VAL"}
         secret_env = {"SECRET_VAR": URL("secret:secret")}
         volumes = [Volume(URL("storage:path"), "/container/my_path", False)]
         secret_files = [
             SecretFile(URL("secret:secret"), "/secrets/my_path"),
         ]
         container = Container(
@@ -1813,17 +1804,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
             "disk_volumes": [
                 {
                     "src_disk_uri": "disk://default/test-project/disk-1",
                     "dst_path": "/container/my_path",
                     "read_only": False,
                 }
@@ -1841,16 +1831,15 @@
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "http": {"port": 8181, "requires_auth": True},
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
                 "disk_volumes": [
                     {
                         "src_disk_uri": "disk://default/test-project/disk-1",
                         "dst_path": "/container/my_path",
                         "read_only": False,
                     }
@@ -1866,15 +1855,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         disk_volumes = [
             DiskVolume(URL("disk:disk-1"), "/container/my_path"),
         ]
         container = Container(
             image=RemoteImage.new_external_image(name="submit-image-name"),
             command="submit-command",
             resources=resources,
@@ -1909,17 +1898,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "scheduler_enabled": True,
         "pass_config": False,
         "http_url": "http://my_host:8889",
     }
 
@@ -1930,16 +1918,15 @@
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "http": {"port": 8181, "requires_auth": True},
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
                 "volumes": [
                     {
                         "src_storage_uri": "storage://test-user/path_read_only",
                         "dst_path": "/container/read_only",
                         "read_only": True,
                     },
@@ -1962,15 +1949,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         volumes: List[Volume] = [
             Volume(
                 URL("storage://test-user/path_read_only"), "/container/read_only", True
             ),
             Volume(
                 URL("storage://test-user/path_read_write"),
                 "/container/path_read_write",
@@ -2016,17 +2003,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
         "schedule_timeout": 5,
     }
@@ -2037,16 +2023,15 @@
             "container": {
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                 },
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "schedule_timeout": 5,
             "cluster_name": "default",
             "project_name": "test-project",
@@ -2056,15 +2041,15 @@
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
+        resources = Resources(memory=16384 * 2**20, cpu=7, nvidia_gpu=1, shm=True)
         container = Container(
             image=RemoteImage.new_external_image(name="submit-image-name"),
             command="submit-command",
             resources=resources,
         )
         ret = await client.jobs.run(container=container, schedule_timeout=5)
 
@@ -2093,17 +2078,16 @@
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
+                "nvidia_gpu": 1,
                 "shm": False,
-                "gpu_model": "nvidia-tesla-p4",
                 "tpu": {"type": "v3-8", "software_version": "1.14"},
             },
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
         "pass_config": False,
     }
@@ -2114,16 +2098,15 @@
             "container": {
                 "image": "submit-image-name",
                 "command": "submit-command",
                 "resources": {
                     "memory": 16384 * 2**20,
                     "cpu": 7,
                     "shm": True,
-                    "gpu": 1,
-                    "gpu_model": "test-gpu-model",
+                    "nvidia_gpu": 1,
                     "tpu": {"type": "v3-8", "software_version": "1.14"},
                 },
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "schedule_timeout": 5,
             "cluster_name": "default",
@@ -2135,15 +2118,20 @@
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         resources = Resources(
-            16384 * 2**20, 7, 1, "test-gpu-model", True, "v3-8", "1.14"
+            memory=16384 * 2**20,
+            cpu=7,
+            nvidia_gpu=1,
+            shm=True,
+            tpu_type="v3-8",
+            tpu_software_version="1.14",
         )
         container = Container(
             image=RemoteImage.new_external_image(name="submit-image-name"),
             command="submit-command",
             resources=resources,
         )
         ret = await client.jobs.run(container=container, schedule_timeout=5)
@@ -2261,16 +2249,15 @@
         },
         "container": {
             "image": image,
             "command": "submit-command",
             "resources": {
                 "cpu": 1.0,
                 "memory": 16384 * 2**20,
-                "gpu": 1,
-                "gpu_model": "nvidia-tesla-v100",
+                "nvidia_gpu": 1,
             },
         },
         "scheduler_enabled": True,
         "pass_config": False,
         "owner": owner,
         "cluster_name": "default",
         "uri": f"job://default/{owner}/{id}",
```

### Comparing `neuro-sdk-24.2.0/tests/test_login.py` & `neuro_sdk-24.5.0/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_login_utils.py` & `neuro_sdk-24.5.0/tests/test_login_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import Decimal
 
 import aiohttp
 import pytest
 from aiohttp import web
 from yarl import URL
 
-from neuro_sdk import AuthError, Cluster, Preset, Project
+from neuro_sdk import AuthError, Cluster, Preset, Project, ResourcePool
 from neuro_sdk._login import _AuthConfig
 from neuro_sdk._server_cfg import _ServerConfig, get_server_config
 
 from tests import _TestClientFactory
 
 
 async def test_get_server_config_no_clusters(
@@ -143,42 +143,119 @@
                 "monitoring_url": monitoring_url,
                 "storage_url": storage_url,
                 "registry_url": registry_url,
                 "users_url": users_url,
                 "secrets_url": secrets_url,
                 "disks_url": disks_url,
                 "buckets_url": buckets_url,
+                "resource_pool_types": [
+                    {
+                        "name": "cpu",
+                        "min_size": 1,
+                        "max_size": 2,
+                        "cpu": 7,
+                        "memory": 14 * 2**30,
+                        "disk_size": 150 * 2**30,
+                    },
+                    {
+                        "name": "nvidia-gpu",
+                        "min_size": 0,
+                        "max_size": 1,
+                        "cpu": 7,
+                        "memory": 60 * 2**30,
+                        "disk_size": 150 * 2**30,
+                        "nvidia_gpu": 1,
+                    },
+                    {
+                        "name": "amd-gpu",
+                        "min_size": 0,
+                        "max_size": 1,
+                        "cpu": 7,
+                        "memory": 60 * 2**30,
+                        "disk_size": 150 * 2**30,
+                        "amd_gpu": 1,
+                    },
+                    {
+                        "name": "intel-gpu",
+                        "min_size": 0,
+                        "max_size": 1,
+                        "cpu": 7,
+                        "memory": 60 * 2**30,
+                        "disk_size": 150 * 2**30,
+                        "intel_gpu": 1,
+                    },
+                ],
                 "resource_presets": [
                     {
-                        "name": "gpu-small",
+                        "name": "nvidia-gpu-small",
                         "credits_per_hour": "10",
                         "cpu": 7,
                         "memory": 30 * 2**30,
-                        "gpu": 1,
-                        "gpu_model": "nvidia-tesla-k80",
+                        "nvidia_gpu": 1,
+                        "resource_pool_names": ["nvidia-gpu"],
+                        "available_resource_pool_names": ["nvidia-gpu"],
                     },
                     {
-                        "name": "gpu-large",
+                        "name": "nvidia-gpu-large",
                         "credits_per_hour": "10",
                         "cpu": 7,
                         "memory": 60 * 2**30,
-                        "gpu": 1,
-                        "gpu_model": "nvidia-tesla-v100",
+                        "nvidia_gpu": 1,
+                        "resource_pool_names": ["nvidia-gpu"],
+                        "available_resource_pool_names": ["nvidia-gpu"],
+                    },
+                    {
+                        "name": "amd-gpu-small",
+                        "credits_per_hour": "10",
+                        "cpu": 7,
+                        "memory": 30 * 2**30,
+                        "amd_gpu": 1,
+                        "resource_pool_names": ["amd-gpu"],
+                        "available_resource_pool_names": ["amd-gpu"],
+                    },
+                    {
+                        "name": "amd-gpu-large",
+                        "credits_per_hour": "10",
+                        "cpu": 7,
+                        "memory": 60 * 2**30,
+                        "amd_gpu": 1,
+                        "resource_pool_names": ["amd-gpu"],
+                        "available_resource_pool_names": ["amd-gpu"],
+                    },
+                    {
+                        "name": "intel-gpu-small",
+                        "credits_per_hour": "10",
+                        "cpu": 7,
+                        "memory": 30 * 2**30,
+                        "intel_gpu": 1,
+                        "resource_pool_names": ["intel-gpu"],
+                        "available_resource_pool_names": ["intel-gpu"],
+                    },
+                    {
+                        "name": "intel-gpu-large",
+                        "credits_per_hour": "10",
+                        "cpu": 7,
+                        "memory": 60 * 2**30,
+                        "intel_gpu": 1,
+                        "resource_pool_names": ["intel-gpu"],
+                        "available_resource_pool_names": ["intel-gpu"],
                     },
                     {
                         "name": "cpu-small",
                         "credits_per_hour": "10",
                         "cpu": 2,
                         "memory": 2 * 2**30,
+                        "available_resource_pool_names": ["cpu"],
                     },
                     {
                         "name": "cpu-large",
                         "credits_per_hour": "10",
                         "cpu": 3,
                         "memory": 14 * 2**30,
+                        "available_resource_pool_names": ["cpu"],
                     },
                     {
                         "name": "cpu-large-p",
                         "credits_per_hour": "10",
                         "cpu": 3,
                         "memory": 14 * 2**30,
                         "scheduler_enabled": True,
@@ -227,34 +304,99 @@
                 registry_url=URL(registry_url),
                 storage_url=URL(storage_url),
                 users_url=URL(users_url),
                 monitoring_url=URL(monitoring_url),
                 secrets_url=URL(secrets_url),
                 disks_url=URL(disks_url),
                 buckets_url=URL(buckets_url),
+                resource_pools={
+                    "cpu": ResourcePool(
+                        min_size=1,
+                        max_size=2,
+                        cpu=7,
+                        memory=14 * 2**30,
+                        disk_size=150 * 2**30,
+                    ),
+                    "nvidia-gpu": ResourcePool(
+                        min_size=0,
+                        max_size=1,
+                        cpu=7,
+                        memory=60 * 2**30,
+                        disk_size=150 * 2**30,
+                        nvidia_gpu=1,
+                    ),
+                    "amd-gpu": ResourcePool(
+                        min_size=0,
+                        max_size=1,
+                        cpu=7,
+                        memory=60 * 2**30,
+                        disk_size=150 * 2**30,
+                        amd_gpu=1,
+                    ),
+                    "intel-gpu": ResourcePool(
+                        min_size=0,
+                        max_size=1,
+                        cpu=7,
+                        memory=60 * 2**30,
+                        disk_size=150 * 2**30,
+                        intel_gpu=1,
+                    ),
+                },
                 presets={
-                    "gpu-small": Preset(
+                    "nvidia-gpu-small": Preset(
+                        credits_per_hour=Decimal("10"),
+                        cpu=7,
+                        memory=30 * 2**30,
+                        nvidia_gpu=1,
+                        resource_pool_names=["nvidia-gpu"],
+                    ),
+                    "nvidia-gpu-large": Preset(
+                        credits_per_hour=Decimal("10"),
+                        cpu=7,
+                        memory=60 * 2**30,
+                        nvidia_gpu=1,
+                        resource_pool_names=["nvidia-gpu"],
+                    ),
+                    "amd-gpu-small": Preset(
                         credits_per_hour=Decimal("10"),
                         cpu=7,
                         memory=30 * 2**30,
-                        gpu=1,
-                        gpu_model="nvidia-tesla-k80",
+                        amd_gpu=1,
+                        resource_pool_names=["amd-gpu"],
                     ),
-                    "gpu-large": Preset(
+                    "amd-gpu-large": Preset(
                         credits_per_hour=Decimal("10"),
                         cpu=7,
                         memory=60 * 2**30,
-                        gpu=1,
-                        gpu_model="nvidia-tesla-v100",
+                        amd_gpu=1,
+                        resource_pool_names=["amd-gpu"],
+                    ),
+                    "intel-gpu-small": Preset(
+                        credits_per_hour=Decimal("10"),
+                        cpu=7,
+                        memory=30 * 2**30,
+                        intel_gpu=1,
+                        resource_pool_names=["intel-gpu"],
+                    ),
+                    "intel-gpu-large": Preset(
+                        credits_per_hour=Decimal("10"),
+                        cpu=7,
+                        memory=60 * 2**30,
+                        intel_gpu=1,
+                        resource_pool_names=["intel-gpu"],
                     ),
                     "cpu-small": Preset(
-                        credits_per_hour=Decimal("10"), cpu=2, memory=2 * 2**30
+                        credits_per_hour=Decimal("10"),
+                        cpu=2,
+                        memory=2 * 2**30,
                     ),
                     "cpu-large": Preset(
-                        credits_per_hour=Decimal("10"), cpu=3, memory=14 * 2**30
+                        credits_per_hour=Decimal("10"),
+                        cpu=3,
+                        memory=14 * 2**30,
                     ),
                     "cpu-large-p": Preset(
                         credits_per_hour=Decimal("10"),
                         cpu=3,
                         memory=14 * 2**30,
                         scheduler_enabled=True,
                         preemptible_node=True,
```

### Comparing `neuro-sdk-24.2.0/tests/test_parser.py` & `neuro_sdk-24.5.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_plugins.py` & `neuro_sdk-24.5.0/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_public_names.py` & `neuro_sdk-24.5.0/tests/test_public_names.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_retry.py` & `neuro_sdk-24.5.0/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_secrets.py` & `neuro_sdk-24.5.0/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_service_accounts.py` & `neuro_sdk-24.5.0/tests/test_service_accounts.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_storage.py` & `neuro_sdk-24.5.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_storage_filestatus.py` & `neuro_sdk-24.5.0/tests/test_storage_filestatus.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_tools.py` & `neuro_sdk-24.5.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_url_utils.py` & `neuro_sdk-24.5.0/tests/test_url_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_users.py` & `neuro_sdk-24.5.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-24.2.0/tests/test_version_check.py` & `neuro_sdk-24.5.0/tests/test_version_check.py`

 * *Files identical despite different names*

