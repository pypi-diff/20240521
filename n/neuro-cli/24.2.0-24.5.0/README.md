# Comparing `tmp/neuro-cli-24.2.0.tar.gz` & `tmp/neuro_cli-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-cli-24.2.0.tar", last modified: Mon Feb 12 13:15:39 2024, max compression
+gzip compressed data, was "neuro_cli-24.5.0.tar", last modified: Tue May 21 09:59:54 2024, max compression
```

## Comparing `neuro-cli-24.2.0.tar` & `neuro_cli-24.5.0.tar`

### file list

```diff
@@ -1,813 +1,813 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.796729 neuro-cli-24.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    92728 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-12 13:15:39.796729 neuro-cli-24.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-02-12 13:15:39.796729 neuro-cli-24.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.652730 neuro-cli-24.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.664729 neuro-cli-24.2.0/src/neuro_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56931 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/ael.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/asyncio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36757 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    39766 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/click_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/docker_credential_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/file_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.668729 neuro-cli-24.2.0/src/neuro_cli/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18388 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/bucket_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    35648 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/formatters/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    44249 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19622 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/share.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    25962 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    20400 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)    22348 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/src/neuro_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.796729 neuro-cli-24.2.0/src/neuro_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-12 13:15:39.000000 neuro-cli-24.2.0/src/neuro_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    51234 2024-02-12 13:15:39.000000 neuro-cli-24.2.0/src/neuro_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 13:15:39.000000 neuro-cli-24.2.0/src/neuro_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-12 13:15:39.000000 neuro-cli-24.2.0/src/neuro_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 13:15:03.000000 neuro-cli-24.2.0/src/neuro_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-12 13:15:39.000000 neuro-cli-24.2.0/src/neuro_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-12 13:15:39.000000 neuro-cli-24.2.0/src/neuro_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.668729 neuro-cli-24.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.668729 neuro-cli-24.2.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.672729 neuro-cli-24.2.0/tests/e2e/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/assets/echo-tag.tar
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/clear-all-my-permissions.sh
--rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)    26067 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e_images.py
--rw-r--r--   0 runner    (1001) docker     (127)    39074 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e_share.py
--rw-r--r--   0 runner    (1001) docker     (127)    24817 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/test_e2e_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/e2e/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.676730 neuro-cli-24.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.748729 neuro-cli-24.2.0/tests/unit/ascii/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_delete_progress[True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[False-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_fail[True-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-False-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-False-True-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-False-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[False-True-True-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-False-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-False-True-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-False-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_nested[True-True-True-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-False-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[False-True-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-False-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/ascii/test_progress[True-True-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.748729 neuro-cli-24.2.0/tests/unit/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:15:39.796729 neuro-cli-24.2.0/tests/unit/formatters/ascii/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_zeroes_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestAliasesFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_rounding_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_5.ref
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_6.ref
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_7.ref
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_8.ref
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClusterOrgProjectsFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClusterOrgProjectsFormatter.test_output_with_current_project_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_no_user_info_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_with_user_info_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_tpu_presets_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_jobs_available_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_org_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_project_name_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_without_project_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_finished_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_started_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_save_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_commit_finished_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_commit_started_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_pull_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_pull_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_push_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_push_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_save_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_commit_finished_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_commit_started_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_save_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter0]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter1]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter2]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter0]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter1]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter2]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_files_and_folders[formatter1]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-someotherproject]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-test-user]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-someotherproject]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-test-user]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_begin_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_begin_with_name_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_end_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_step_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_begin_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_begin_with_name_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[cancelled]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[failed]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[pending]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[running]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[succeeded]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[suspended]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[cancelled]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[failed]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[pending]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[running]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[succeeded]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[suspended]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_detach_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[cancelled]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[failed]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[succeeded]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_kill_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_restart_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_step_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_detach_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[cancelled]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[failed]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[succeeded]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_kill_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_restart_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[pending]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[running]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[suspended]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_2.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_3.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_4.ref
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_finished[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_finished[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_not_finished[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_not_finished[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestNonePainter.test_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestOrgClusterFormatter.test_org_cluster_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestOrgClusterFormatter.test_org_cluster_formatter_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_cpu_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_credits_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_gpu_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_jobs_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_zeroes_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_spent_more_than_quota_left_zero_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_too_many_hours_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestSimpleJobsFormatter.test_empty_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestSimpleJobsFormatter.test_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_custom_columns[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_custom_columns[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_working_dir[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_working_dir[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestUsageFormatter.test_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestUsageFormatter.test_org_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/TestUsageFormatter.test_path_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_bucket_credentials_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_bucket_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_bucket_formatter_with_org_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_formatter_long_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_formatter_short_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disk_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disks_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disks_formatter_long_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disks_formatter_short_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disks_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_secrets_formatter_short_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_secrets_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_service_account_formatter[None]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_service_account_formatter[some-org]_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_service_account_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/ascii/test_service_accounts_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_admin_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_blob_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_bucket_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_config_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_images_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)   100930 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_jobs_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14657 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_storage_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/formatters/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    21084 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_ael.py
--rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_click_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_click_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_docker_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    58991 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_shell_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_storage_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    32211 2024-02-12 13:14:58.000000 neuro-cli-24.2.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.644852 neuro_cli-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    92906 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-21 09:59:54.644852 neuro_cli-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-21 09:59:54.648852 neuro_cli-24.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.492852 neuro_cli-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.504852 neuro_cli-24.5.0/src/neuro_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58104 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/ael.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/asyncio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36757 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39766 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/click_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/docker_credential_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/file_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.508852 neuro_cli-24.5.0/src/neuro_cli/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18388 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/bucket_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35937 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/formatters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44249 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19622 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25962 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20400 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22348 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/src/neuro_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.644852 neuro_cli-24.5.0/src/neuro_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-21 09:59:54.000000 neuro_cli-24.5.0/src/neuro_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    51234 2024-05-21 09:59:54.000000 neuro_cli-24.5.0/src/neuro_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:59:54.000000 neuro_cli-24.5.0/src/neuro_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 09:59:54.000000 neuro_cli-24.5.0/src/neuro_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:59:11.000000 neuro_cli-24.5.0/src/neuro_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-21 09:59:54.000000 neuro_cli-24.5.0/src/neuro_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 09:59:54.000000 neuro_cli-24.5.0/src/neuro_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.508852 neuro_cli-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.508852 neuro_cli-24.5.0/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.508852 neuro_cli-24.5.0/tests/e2e/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/assets/echo-tag.tar
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/clear-all-my-permissions.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26067 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39074 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e_share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24817 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/test_e2e_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/e2e/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.512852 neuro_cli-24.5.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.588852 neuro_cli-24.5.0/tests/unit/ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_delete_progress[True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[False-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_fail[True-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-False-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-False-True-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-False-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[False-True-True-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-False-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-False-True-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-False-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_nested[True-True-True-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-False-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[False-True-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-False-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/ascii/test_progress[True-True-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)    18203 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.588852 neuro_cli-24.5.0/tests/unit/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:54.644852 neuro_cli-24.5.0/tests/unit/formatters/ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_zeroes_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestAliasesFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_rounding_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClusterOrgProjectsFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClusterOrgProjectsFormatter.test_output_with_current_project_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_no_user_info_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_with_user_info_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_tpu_presets_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_jobs_available_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_org_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_project_name_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_without_project_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_finished_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_started_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_save_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_commit_finished_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_commit_started_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_pull_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_pull_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_push_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_push_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_save_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_commit_finished_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_commit_started_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_save_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter0]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter1]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter2]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter0]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter1]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter2]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_files_and_folders[formatter1]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-someotherproject]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-test-user]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-someotherproject]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-test-user]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_begin_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_begin_with_name_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_end_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_step_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_begin_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_begin_with_name_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[cancelled]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[failed]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[pending]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[running]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[succeeded]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[suspended]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[cancelled]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[failed]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[pending]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[running]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[succeeded]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[suspended]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_detach_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[cancelled]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[failed]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[succeeded]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_kill_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_restart_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_step_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_detach_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[cancelled]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[failed]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[succeeded]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_kill_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_restart_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[pending]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[running]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[suspended]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_finished[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_finished[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_not_finished[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_not_finished[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestNonePainter.test_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestOrgClusterFormatter.test_org_cluster_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestOrgClusterFormatter.test_org_cluster_formatter_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_cpu_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_credits_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_gpu_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_jobs_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_zeroes_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_spent_more_than_quota_left_zero_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_too_many_hours_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestSimpleJobsFormatter.test_empty_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestSimpleJobsFormatter.test_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_custom_columns[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_custom_columns[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_working_dir[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_working_dir[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestUsageFormatter.test_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestUsageFormatter.test_org_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/TestUsageFormatter.test_path_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_bucket_credentials_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_bucket_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_bucket_formatter_with_org_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_formatter_long_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_formatter_short_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disk_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disks_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disks_formatter_long_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disks_formatter_short_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disks_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_secrets_formatter_short_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_secrets_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_service_account_formatter[None]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_service_account_formatter[some-org]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_service_account_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/ascii/test_service_accounts_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_admin_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_blob_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_bucket_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_config_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_images_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100725 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_jobs_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14657 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_storage_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/formatters/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_ael.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_click_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_click_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10938 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_docker_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59041 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_shell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_storage_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32211 2024-05-21 09:59:06.000000 neuro_cli-24.5.0/tests/unit/test_utils.py
```

### Comparing `neuro-cli-24.2.0/CHANGELOG.md` & `neuro_cli-24.5.0/CHANGELOG.md`

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

### Comparing `neuro-cli-24.2.0/LICENSE` & `neuro_cli-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/PKG-INFO` & `neuro_cli-24.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-cli
-Version: 24.2.0
+Version: 24.5.0
 Summary: Neuro Platform client
 Home-page: https://github.com/neuro-inc/platform-client-python
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-jose>=3.0.0
 Requires-Dist: python-dateutil>=2.7.0
-Requires-Dist: neuro-sdk>=24.2.0
+Requires-Dist: neuro-sdk>=24.5.0
 Requires-Dist: click>=8.0
 Requires-Dist: humanize>=3.3
 Requires-Dist: typing_extensions>=3.7.4
 Requires-Dist: certifi
 Requires-Dist: wcwidth>=0.1.7
 Requires-Dist: prompt-toolkit>=3.0.13
 Requires-Dist: rich>=11.0.0
```

### Comparing `neuro-cli-24.2.0/README.md` & `neuro_cli-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/setup.cfg` & `neuro_cli-24.5.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neuro-cli
-version = 24.2.0
+version = 24.5.0
 description = Neuro Platform client
 url = https://github.com/neuro-inc/platform-client-python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Neu.ro Team
 author_email = team@neu.ro
 license = Apache 2
@@ -31,15 +31,15 @@
 packages = find:
 zip_safe = False
 python_requires = >=3.8.0
 include_package_data = True
 install_requires = 
 	python-jose>=3.0.0
 	python-dateutil>=2.7.0
-	neuro-sdk>=24.2.0
+	neuro-sdk>=24.5.0
 	click>=8.0
 	humanize>=3.3
 	typing_extensions>=3.7.4
 	certifi
 	wcwidth>=0.1.7
 	prompt-toolkit>=3.0.13
 	rich>=11.0.0
```

### Comparing `neuro-cli-24.2.0/src/neuro_cli/admin.py` & `neuro_cli-24.5.0/src/neuro_cli/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import configparser
 import json
 import logging
 import os
 import pathlib
 from dataclasses import replace
 from decimal import Decimal, InvalidOperation
-from typing import IO, Dict, Optional, Tuple
+from typing import IO, Any, Dict, Optional, Sequence, Tuple
 
 import click
 import yaml
 from prompt_toolkit import PromptSession
 from prompt_toolkit.patch_stdout import patch_stdout
 from rich.markup import escape as rich_escape
 
@@ -951,23 +951,30 @@
     type=MEMORY,
     help="Memory amount",
     default=JOB_MEMORY_AMOUNT,
     show_default=True,
 )
 @option(
     "-g",
-    "--gpu",
+    "--nvidia-gpu",
     metavar="NUMBER",
     type=int,
-    help="Number of GPUs",
+    help="Number of Nvidia GPUs",
 )
 @option(
-    "--gpu-model",
-    metavar="MODEL",
-    help="GPU model",
+    "--amd-gpu",
+    metavar="NUMBER",
+    type=int,
+    help="Number of AMD GPUs",
+)
+@option(
+    "--intel-gpu",
+    metavar="NUMBER",
+    type=int,
+    help="Number of Intel GPUs",
 )
 @option("--tpu-type", metavar="TYPE", type=str, help="TPU type")
 @option(
     "tpu_software_version",
     "--tpu-sw-version",
     metavar="VERSION",
     type=str,
@@ -982,26 +989,38 @@
 )
 @option(
     "--preemptible-node/--non-preemptible-node",
     help="Use a lower-cost preemptible instance",
     default=False,
     show_default=True,
 )
+@option(
+    "resource_pool_names",
+    "-r",
+    "--resource-pool",
+    help=(
+        "Name of the resource pool where job will be scheduled "
+        "(multiple values are supported)"
+    ),
+    multiple=True,
+)
 async def add_resource_preset(
     root: Root,
     preset_name: str,
     credits_per_hour: str,
     cpu: float,
     memory: int,
-    gpu: Optional[int],
-    gpu_model: Optional[str],
+    nvidia_gpu: Optional[int],
+    amd_gpu: Optional[int],
+    intel_gpu: Optional[int],
     tpu_type: Optional[str],
     tpu_software_version: Optional[str],
     scheduler: bool,
     preemptible_node: bool,
+    resource_pool_names: Sequence[str],
 ) -> None:
     """
     Add new resource preset
     """
     presets = dict(root.client.config.presets)
     if preset_name in presets:
         raise ValueError(f"Preset '{preset_name}' already exists")
@@ -1010,19 +1029,21 @@
     else:
         tpu_preset = None
     preset = _ResourcePreset(
         name=preset_name,
         credits_per_hour=_parse_finite_decimal(credits_per_hour),
         cpu=cpu,
         memory=memory,
-        gpu=gpu,
-        gpu_model=gpu_model,
+        nvidia_gpu=nvidia_gpu,
+        amd_gpu=amd_gpu,
+        intel_gpu=intel_gpu,
         tpu=tpu_preset,
         scheduler_enabled=scheduler,
         preemptible_node=preemptible_node,
+        resource_pool_names=resource_pool_names,
     )
     await root.client._clusters.add_resource_preset(
         root.client.config.cluster_name, preset
     )
     await root.client.config.fetch()
     if not root.quiet:
         root.print(
@@ -1052,23 +1073,30 @@
     "--memory",
     metavar="AMOUNT",
     type=MEMORY,
     help="Memory amount",
 )
 @option(
     "-g",
-    "--gpu",
+    "--nvidia-gpu",
     metavar="NUMBER",
     type=int,
-    help="Number of GPUs",
+    help="Number of Nvidia GPUs",
 )
 @option(
-    "--gpu-model",
-    metavar="MODEL",
-    help="GPU model",
+    "--amd-gpu",
+    metavar="NUMBER",
+    type=int,
+    help="Number of AMD GPUs",
+)
+@option(
+    "--intel-gpu",
+    metavar="NUMBER",
+    type=int,
+    help="Number of Intel GPUs",
 )
 @option("--tpu-type", metavar="TYPE", type=str, help="TPU type")
 @option(
     "tpu_software_version",
     "--tpu-sw-version",
     metavar="VERSION",
     type=str,
@@ -1081,48 +1109,62 @@
     default=None,
 )
 @option(
     "--preemptible-node/--non-preemptible-node",
     help="Use a lower-cost preemptible instance",
     default=None,
 )
+@option(
+    "resource_pool_names",
+    "-r",
+    "--resource-pool",
+    help=(
+        "Name of the resource pool where job will be scheduled "
+        "(multiple values are supported)"
+    ),
+    multiple=True,
+)
 async def update_resource_preset(
     root: Root,
     preset_name: str,
     credits_per_hour: Optional[str],
     cpu: Optional[float],
     memory: Optional[int],
-    gpu: Optional[int],
-    gpu_model: Optional[str],
+    nvidia_gpu: Optional[int],
+    amd_gpu: Optional[int],
+    intel_gpu: Optional[int],
     tpu_type: Optional[str],
     tpu_software_version: Optional[str],
     scheduler: Optional[bool],
     preemptible_node: Optional[bool],
+    resource_pool_names: Sequence[str],
 ) -> None:
     """
     Update existing resource preset
     """
     presets = dict(root.client.config.presets)
     try:
         preset = presets[preset_name]
     except KeyError:
         raise ValueError(f"Preset '{preset_name}' does not exists")
 
-    kwargs = {
+    kwargs: Dict[str, Any] = {
         "credits_per_hour": _parse_finite_decimal(credits_per_hour)
         if credits_per_hour is not None
         else None,
         "cpu": cpu,
         "memory": memory,
-        "gpu": gpu,
-        "gpu_model": gpu_model,
+        "nvidia_gpu": nvidia_gpu,
+        "amd_gpu": amd_gpu,
+        "intel_gpu": intel_gpu,
         "tpu_type": tpu_type,
         "tpu_software_version": tpu_software_version,
         "scheduler_enabled": scheduler,
         "preemptible_node": preemptible_node,
+        "resource_pool_names": resource_pool_names,
     }
     kwargs = {key: value for key, value in kwargs.items() if value is not None}
     preset = replace(preset, **kwargs)
     if preset.tpu_type and preset.tpu_software_version:
         tpu_preset = _TPUPreset(
             type=preset.tpu_type, software_version=preset.tpu_software_version
         )
@@ -1131,19 +1173,21 @@
     await root.client._clusters.update_resource_preset(
         root.client.config.cluster_name,
         _ResourcePreset(
             name=preset_name,
             credits_per_hour=preset.credits_per_hour,
             cpu=preset.cpu,
             memory=preset.memory,
-            gpu=preset.gpu,
-            gpu_model=preset.gpu_model,
+            nvidia_gpu=preset.nvidia_gpu,
+            amd_gpu=preset.amd_gpu,
+            intel_gpu=preset.intel_gpu,
             tpu=tpu_preset,
             scheduler_enabled=preset.scheduler_enabled,
             preemptible_node=preset.preemptible_node,
+            resource_pool_names=preset.resource_pool_names,
         ),
     )
     await root.client.config.fetch()
     if not root.quiet:
         root.print(
             f"Updated resource preset [b]{rich_escape(preset_name)}[/b] "
             f"in cluster [b]{rich_escape(root.client.config.cluster_name)}[/b]",
```

### Comparing `neuro-cli-24.2.0/src/neuro_cli/ael.py` & `neuro_cli-24.5.0/src/neuro_cli/ael.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/alias.py` & `neuro_cli-24.5.0/src/neuro_cli/alias.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/asyncio_utils.py` & `neuro_cli-24.5.0/src/neuro_cli/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/blob_storage.py` & `neuro_cli-24.5.0/src/neuro_cli/blob_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/click_types.py` & `neuro_cli-24.5.0/src/neuro_cli/click_types.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/completion.py` & `neuro_cli-24.5.0/src/neuro_cli/completion.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/config.py` & `neuro_cli-24.5.0/src/neuro_cli/config.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/disks.py` & `neuro_cli-24.5.0/src/neuro_cli/disks.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/docker_credential_helper.py` & `neuro_cli-24.5.0/src/neuro_cli/docker_credential_helper.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/file_logging.py` & `neuro_cli-24.5.0/src/neuro_cli/file_logging.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/admin.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/admin.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/blob_storage.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/blob_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/bucket_credentials.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/bucket_credentials.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/buckets.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/buckets.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/config.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,17 +84,19 @@
         default_org: Optional[str],
     ) -> RenderableType:
         out: List[RenderableType] = [Text("Available clusters:", style="i")]
         for cluster in clusters:
             name: Union[str, Text] = cluster.name or ""
             pre = "  "
             org_names: List[Text] = [
-                Text(org or OrgType.NO_ORG_STR, style="u")
-                if org == default_org and cluster.name == default_cluster
-                else Text(org or OrgType.NO_ORG_STR)
+                (
+                    Text(org or OrgType.NO_ORG_STR, style="u")
+                    if org == default_org and cluster.name == default_cluster
+                    else Text(org or OrgType.NO_ORG_STR)
+                )
                 for org in cluster.orgs
             ]
             if cluster.name == default_cluster:
                 name = Text(cluster.name, style="u")
                 pre = "* "
             out.append(Text.assemble(pre, Text("Name"), ": ", name))
             out.append(
@@ -104,62 +106,69 @@
         return RichGroup(*out)
 
 
 def _format_presets(
     presets: Mapping[str, Preset],
     available_jobs_counts: Optional[Mapping[str, int]],
 ) -> Table:
-    has_tpu = False
-    for preset in presets.values():
-        if preset.tpu_type:
-            has_tpu = True
-            break
+    has_nvidia_gpu = any(p.nvidia_gpu for p in presets.values())
+    has_amd_gpu = any(p.amd_gpu for p in presets.values())
+    has_intel_gpu = any(p.intel_gpu for p in presets.values())
+    has_tpu = any(p.tpu_type for p in presets.values())
 
     table = Table(
         title="Resource Presets:",
         title_justify="left",
         box=box.SIMPLE_HEAVY,
         show_edge=False,
     )
     table.add_column("Name", style="bold", justify="left")
     table.add_column("#CPU", justify="right")
     table.add_column("Memory", justify="right")
+    if has_nvidia_gpu:
+        table.add_column("Nvidia GPU", justify="center")
+    if has_amd_gpu:
+        table.add_column("AMD GPU", justify="center")
+    if has_intel_gpu:
+        table.add_column("Intel GPU", justify="center")
+    if has_tpu:
+        table.add_column("TPU", justify="left")
+    table.add_column("Resource Pools", justify="left")
     table.add_column("Round Robin", justify="center")
     table.add_column("Preemptible Node", justify="center")
-    table.add_column("GPU", justify="left")
     if available_jobs_counts:
         table.add_column("Jobs Avail", justify="right")
-    if has_tpu:
-        table.add_column("TPU", justify="left")
     table.add_column("Credits per hour", justify="left")
 
     for name, preset in presets.items():
-        gpu = ""
-        if preset.gpu:
-            gpu = f"{preset.gpu} x {preset.gpu_model}"
-        row = [
-            name,
-            str(preset.cpu),
-            format_size(preset.memory),
-            "√" if preset.scheduler_enabled else "×",
-            "√" if preset.preemptible_node else "×",
-            gpu,
-        ]
+        row = [name, str(preset.cpu), format_size(preset.memory)]
+        if has_nvidia_gpu:
+            row.append(str(preset.nvidia_gpu) if preset.nvidia_gpu else "")
+        if has_amd_gpu:
+            row.append(str(preset.amd_gpu) if preset.amd_gpu else "")
+        if has_intel_gpu:
+            row.append(str(preset.intel_gpu) if preset.intel_gpu else "")
         if has_tpu:
             tpu = (
                 f"{preset.tpu_type}/{preset.tpu_software_version}"
                 if preset.tpu_type
                 else ""
             )
             row.append(tpu)
+        row.append("\n".join(preset.resource_pool_names))
+        row.append("√" if preset.scheduler_enabled else "×")
+        row.append(
+            "√" if preset.preemptible_node else "×",
+        )
         if available_jobs_counts:
-            if name in available_jobs_counts:
-                row.append(str(available_jobs_counts[name]))
-            else:
-                row.append("")
+            row.append(
+                str(available_jobs_counts[name])
+                if name in available_jobs_counts
+                else ""
+            )
         row.append(str(preset.credits_per_hour))
         table.add_row(*row)
 
     return table
 
 
 def _format_cluster_energy(cluster: _ConfigCluster) -> Sequence[RenderableType]:
```

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/disks.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/disks.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/images.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/images.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/jobs.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,19 +122,25 @@
         table.add_row("Current cost", f"{job_status.total_price_credits:.4f}")
 
         resources = Table(box=None, show_header=False, show_edge=False)
         resources.add_column()
         resources.add_column(style="bold", justify="right")
         resources.add_row("Memory", format_size(job_status.container.resources.memory))
         resources.add_row("CPU", f"{job_status.container.resources.cpu:0.1f}")
-        if job_status.container.resources.gpu:
+        if job_status.container.resources.nvidia_gpu:
             resources.add_row(
-                "GPU",
-                f"{job_status.container.resources.gpu:0.1f} x "
-                f"{job_status.container.resources.gpu_model}",
+                "Nvidia GPU", f"{job_status.container.resources.nvidia_gpu:0.1f}"
+            )
+        if job_status.container.resources.amd_gpu:
+            resources.add_row(
+                "AMD GPU", f"{job_status.container.resources.amd_gpu:0.1f}"
+            )
+        if job_status.container.resources.intel_gpu:
+            resources.add_row(
+                "Intel GPU", f"{job_status.container.resources.intel_gpu:0.1f}"
             )
 
         if job_status.container.resources.tpu_type:
             resources.add_row(
                 "TPU",
                 f"{job_status.container.resources.tpu_type}/"
                 f"{job_status.container.resources.tpu_software_version}",
```

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/secrets.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/secrets.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/service_accounts.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/service_accounts.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/storage.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/formatters/utils.py` & `neuro_cli-24.5.0/src/neuro_cli/formatters/utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/image.py` & `neuro_cli-24.5.0/src/neuro_cli/image.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/job.py` & `neuro_cli-24.5.0/src/neuro_cli/job.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/log_formatter.py` & `neuro_cli-24.5.0/src/neuro_cli/log_formatter.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/main.py` & `neuro_cli-24.5.0/src/neuro_cli/main.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/parse_utils.py` & `neuro_cli-24.5.0/src/neuro_cli/parse_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/plugin.py` & `neuro_cli-24.5.0/src/neuro_cli/plugin.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/root.py` & `neuro_cli-24.5.0/src/neuro_cli/root.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/secrets.py` & `neuro_cli-24.5.0/src/neuro_cli/secrets.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/service_accounts.py` & `neuro_cli-24.5.0/src/neuro_cli/service_accounts.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/share.py` & `neuro_cli-24.5.0/src/neuro_cli/share.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/stats.py` & `neuro_cli-24.5.0/src/neuro_cli/stats.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/storage.py` & `neuro_cli-24.5.0/src/neuro_cli/storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/topics.py` & `neuro_cli-24.5.0/src/neuro_cli/topics.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli/utils.py` & `neuro_cli-24.5.0/src/neuro_cli/utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/src/neuro_cli.egg-info/PKG-INFO` & `neuro_cli-24.5.0/src/neuro_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-cli
-Version: 24.2.0
+Version: 24.5.0
 Summary: Neuro Platform client
 Home-page: https://github.com/neuro-inc/platform-client-python
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-jose>=3.0.0
 Requires-Dist: python-dateutil>=2.7.0
-Requires-Dist: neuro-sdk>=24.2.0
+Requires-Dist: neuro-sdk>=24.5.0
 Requires-Dist: click>=8.0
 Requires-Dist: humanize>=3.3
 Requires-Dist: typing_extensions>=3.7.4
 Requires-Dist: certifi
 Requires-Dist: wcwidth>=0.1.7
 Requires-Dist: prompt-toolkit>=3.0.13
 Requires-Dist: rich>=11.0.0
```

### Comparing `neuro-cli-24.2.0/src/neuro_cli.egg-info/SOURCES.txt` & `neuro_cli-24.5.0/src/neuro_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/__init__.py` & `neuro_cli-24.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/assets/echo-tag.tar` & `neuro_cli-24.5.0/tests/e2e/assets/echo-tag.tar`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/conftest.py` & `neuro_cli-24.5.0/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e_admin.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e_admin.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e_blob_storage.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e_blob_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e_disks.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e_disks.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e_images.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e_images.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e_jobs.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e_jobs.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e_secrets.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e_secrets.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e_share.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e_share.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/test_e2e_storage.py` & `neuro_cli-24.5.0/tests/e2e/test_e2e_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/e2e/utils.py` & `neuro_cli-24.5.0/tests/e2e/utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/conftest.py` & `neuro_cli-24.5.0/tests/unit/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, Callable, DefaultDict, Iterator, List, Optional, Set, Union
 
 import click
 import pytest
 from rich.console import Console, RenderableType
 from yarl import URL
 
-from neuro_sdk import Cluster, Factory, Preset, Project
+from neuro_sdk import Cluster, Factory, Preset, Project, ResourcePool
 from neuro_sdk._config import _AuthConfig, _AuthToken, _ConfigData
 
 from neuro_cli import __version__
 from neuro_cli.const import EX_OK
 from neuro_cli.main import main
 from neuro_cli.root import Root
 from neuro_cli.utils import Command, Context
@@ -32,50 +32,126 @@
         registry_url=URL("https://registry-dev.neu.ro"),
         storage_url=URL("https://storage-dev.neu.ro"),
         users_url=URL("https://users-dev.neu.ro"),
         monitoring_url=URL("https://monitoring-dev.neu.ro"),
         secrets_url=URL("https://secrets-dev.neu.ro"),
         disks_url=URL("https://disks-dev.neu.ro"),
         buckets_url=URL("https://buckets-dev.neu.ro"),
+        resource_pools={
+            "cpu": ResourcePool(
+                min_size=1,
+                max_size=2,
+                cpu=7,
+                memory=14 * 2**30,
+                disk_size=150 * 2**30,
+            ),
+            "nvidia-gpu": ResourcePool(
+                min_size=0,
+                max_size=1,
+                cpu=7,
+                memory=60 * 2**30,
+                disk_size=150 * 2**30,
+                nvidia_gpu=1,
+            ),
+            "amd-gpu": ResourcePool(
+                min_size=0,
+                max_size=1,
+                cpu=7,
+                memory=60 * 2**30,
+                disk_size=150 * 2**30,
+                amd_gpu=1,
+            ),
+            "intel-gpu": ResourcePool(
+                min_size=0,
+                max_size=1,
+                cpu=7,
+                memory=60 * 2**30,
+                disk_size=150 * 2**30,
+                intel_gpu=1,
+            ),
+        },
         presets={
-            "gpu-small": Preset(
+            "nvidia-gpu-small": Preset(
                 credits_per_hour=Decimal("10"),
                 cpu=7,
                 memory=30 * 2**30,
-                gpu=1,
-                gpu_model="nvidia-tesla-k80",
+                nvidia_gpu=1,
+                resource_pool_names=["nvidia-gpu"],
             ),
-            "gpu-large": Preset(
+            "nvidia-gpu-large": Preset(
                 credits_per_hour=Decimal("10"),
                 cpu=7,
                 memory=60 * 2**30,
-                gpu=1,
-                gpu_model="nvidia-tesla-v100",
+                nvidia_gpu=1,
+                resource_pool_names=["nvidia-gpu"],
+            ),
+            "amd-gpu-small": Preset(
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=30 * 2**30,
+                amd_gpu=1,
+                resource_pool_names=["amd-gpu"],
+            ),
+            "amd-gpu-large": Preset(
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=60 * 2**30,
+                amd_gpu=1,
+                resource_pool_names=["amd-gpu"],
+            ),
+            "intel-gpu-small": Preset(
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=30 * 2**30,
+                intel_gpu=1,
+                resource_pool_names=["intel-gpu"],
+            ),
+            "intel-gpu-large": Preset(
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=60 * 2**30,
+                intel_gpu=1,
+                resource_pool_names=["intel-gpu"],
             ),
             "cpu-small": Preset(
-                credits_per_hour=Decimal("10"), cpu=7, memory=2 * 2**30
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=2 * 2**30,
             ),
             "cpu-large": Preset(
-                credits_per_hour=Decimal("10"), cpu=7, memory=14 * 2**30
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=14 * 2**30,
             ),
         },
         name="default",
         orgs=[None, "org"],
     )
     cluster2_config = Cluster(
         registry_url=URL("https://registry2-dev.neu.ro"),
         storage_url=URL("https://storage2-dev.neu.ro"),
         users_url=URL("https://users2-dev.neu.ro"),
         monitoring_url=URL("https://monitoring2-dev.neu.ro"),
         secrets_url=URL("https://secrets2-dev.neu.ro"),
         disks_url=URL("https://disks2-dev.neu.ro"),
         buckets_url=URL("https://buckets2-dev.neu.ro"),
+        resource_pools={
+            "cpu": ResourcePool(
+                min_size=1,
+                max_size=2,
+                cpu=7,
+                memory=14 * 2**30,
+                disk_size=150 * 2**30,
+            ),
+        },
         presets={
             "cpu-small": Preset(
-                credits_per_hour=Decimal("10"), cpu=7, memory=2 * 2**30
+                credits_per_hour=Decimal("10"),
+                cpu=7,
+                memory=2 * 2**30,
             ),
         },
         name="other",
         orgs=[None],
     )
     config = _ConfigData(
         auth_config=auth_config,
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_with_user_info_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_with_user_info_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_project_name_0.ref`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 User Configuration:                               
  User Name            user                        
  Current Cluster      default                     
  Current Org          <no-org>                    
- Current Project      project                     
+ Current Project      main                        
  Credits Quota        500.00                      
  Jobs Quota           10                          
  API URL              https://dev.neu.ro/api/v1   
  Docker Registry URL  https://registry-dev.neu.ro 
-Resource Presets:                                                                                       
- Name        #CPU    Memory   Round Robin   Preemptible Node   GPU                     Credits per hour 
-━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- gpu-small      7   32.2 GB        ×               ×           1 x nvidia-tesla-k80    10               
- gpu-large      7   64.4 GB        ×               ×           1 x nvidia-tesla-v100   10               
- cpu-small      7    2.1 GB        ×               ×                                   10               
- cpu-large      7   15.0 GB        ×               ×                                   10
+Resource Presets:                                                                                         
+ Name          #CPU    Memory   Round Robin   Preemptible Node   GPU                     Credits per hour 
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ gpu-small        7   32.2 GB        ×               ×           1 x nvidia-tesla-k80    10               
+ gpu-large        7   64.4 GB        ×               ×           1 x nvidia-tesla-v100   10               
+ cpu-small        7    2.1 GB        ×               ×                                   10               
+ cpu-large        7   15.0 GB        ×               ×                                   10               
+ cpu-large-p      7   15.0 GB        √               √                                   10
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,25 @@
  Current Cluster      default                     
  Current Org          <no-org>                    
  Current Project      project                     
  Credits Quota        500.00                      
  Jobs Quota           10                          
  API URL              https://dev.neu.ro/api/v1   
  Docker Registry URL  https://registry-dev.neu.ro 
-Resource Presets:                                                                                       
- Name        #CPU    Memory   Round Robin   Preemptible Node   GPU                     Credits per hour 
-━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- gpu-small      7   32.2 GB        ×               ×           1 x nvidia-tesla-k80    10               
- gpu-large      7   64.4 GB        ×               ×           1 x nvidia-tesla-v100   10               
- cpu-small      7    2.1 GB        ×               ×                                   10               
- cpu-large      7   15.0 GB        ×               ×                                   10               
+Resource Presets:                                                                                                                          
+ Name               #CPU    Memory   Nvidia GPU   AMD GPU   Intel GPU   Resource Pools   Round Robin   Preemptible Node   Credits per hour 
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ nvidia-gpu-small      7   32.2 GB       1                              nvidia-gpu            ×               ×           10               
+ nvidia-gpu-large      7   64.4 GB       1                              nvidia-gpu            ×               ×           10               
+ amd-gpu-small         7   32.2 GB                   1                  amd-gpu               ×               ×           10               
+ amd-gpu-large         7   64.4 GB                   1                  amd-gpu               ×               ×           10               
+ intel-gpu-small       7   32.2 GB                              1       intel-gpu             ×               ×           10               
+ intel-gpu-large       7   64.4 GB                              1       intel-gpu             ×               ×           10               
+ cpu-small             7    2.1 GB                                                            ×               ×           10               
+ cpu-large             7   15.0 GB                                                            ×               ×           10               
 Cluster energy parameters:         
  CO2 eq g/kWh:                40.4 
  Cluster location timezone:   UTC  
 Energy schedules:                                                                     
  Name        Price (kW/h)   Start time   End time                Weekday              
 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  DEFAULT         10.4         00:00       23:59     Mon, Tue, Wed, Thu, Fri, Sat, Sun
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-someotherproject]_0.ref`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Job                     test-job                                    
- Owner                   test-user                                   
- Project                                                             
- Cluster                 default                                     
- Description             test job description                        
- Status                  succeeded                                   
- Image                   test-image                                  
- Command                 test-command                                
- Priority                Normal                                      
- Price (credits / hour)  15.0000                                     
- Current cost            150.0000                                    
- Resources                Memory                           16 Bytes  
-                          CPU                                   0.1  
-                          GPU                 4.0 x nvidia-tesla-p4  
-                          TPU                             v2-8/1.14  
-                          Extended SHM space                   True  
- TTY                     False                                       
- Http URL                http://local.host.test/                     
- Created                 Sep 25 2018 at 12:28                        
- Started                 Sep 25 2018 at 12:28                        
- Finished                Sep 25 2018 at 12:28                        
+Job                     test-job                        
+ Owner                   test-user                       
+ Project                 someotherproject                
+ Cluster                 default                         
+ Description             test job description            
+ Status                  succeeded                       
+ Image                   test-image                      
+ Command                 test-command                    
+ Priority                Normal                          
+ Price (credits / hour)  15.0000                         
+ Current cost            150.0000                        
+ Resources                Memory               16 Bytes  
+                          CPU                       0.1  
+                          Nvidia GPU                4.0  
+                          AMD GPU                   5.0  
+                          Intel GPU                 6.0  
+                          TPU                 v2-8/1.14  
+                          Extended SHM space       True  
+ TTY                     False                           
+ Http URL                http://local.host.test/         
+ Created                 Sep 25 2018 at 12:28            
+ Started                 Sep 25 2018 at 12:28            
+ Finished                Sep 25 2018 at 12:28            
  Exit code               None
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-someotherproject]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-]_0.ref`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Job                     test-job                                    
- Owner                   test-user                                   
- Project                 someotherproject                            
- Cluster                 default                                     
- Description             test job description                        
- Status                  succeeded                                   
- Image                   test-image                                  
- Command                 test-command                                
- Priority                Normal                                      
- Price (credits / hour)  15.0000                                     
- Current cost            150.0000                                    
- Resources                Memory                           16 Bytes  
-                          CPU                                   0.1  
-                          GPU                 4.0 x nvidia-tesla-p4  
-                          TPU                             v2-8/1.14  
-                          Extended SHM space                   True  
- TTY                     False                                       
- Http URL                http://local.host.test/                     
- Created                 Sep 25 2018 at 12:28                        
- Started                 Sep 25 2018 at 12:28                        
- Finished                Sep 25 2018 at 12:28                        
+Job                     test-job                        
+ Owner                   test-user                       
+ Project                                                 
+ Cluster                 default                         
+ Description             test job description            
+ Status                  succeeded                       
+ Image                   test-image                      
+ Command                 test-command                    
+ Priority                Normal                          
+ Price (credits / hour)  15.0000                         
+ Current cost            150.0000                        
+ Resources                Memory               16 Bytes  
+                          CPU                       0.1  
+                          Nvidia GPU                4.0  
+                          AMD GPU                   5.0  
+                          Intel GPU                 6.0  
+                          TPU                 v2-8/1.14  
+                          Extended SHM space       True  
+ TTY                     False                           
+ Http URL                http://local.host.test/         
+ Created                 Sep 25 2018 at 12:28            
+ Started                 Sep 25 2018 at 12:28            
+ Finished                Sep 25 2018 at 12:28            
  Exit code               None
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-test-user]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-test-user]_0.ref`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Job                     test-job                                    
- Owner                   test-user                                   
- Project                 test-user                                   
- Cluster                 default                                     
- Description             test job description                        
- Status                  succeeded                                   
- Image                   test-image                                  
- Command                 test-command                                
- Priority                Normal                                      
- Price (credits / hour)  15.0000                                     
- Current cost            150.0000                                    
- Resources                Memory                           16 Bytes  
-                          CPU                                   0.1  
-                          GPU                 4.0 x nvidia-tesla-p4  
-                          TPU                             v2-8/1.14  
-                          Extended SHM space                   True  
- TTY                     False                                       
- Http URL                http://local.host.test/                     
- Created                 Sep 25 2018 at 12:28                        
- Started                 Sep 25 2018 at 12:28                        
- Finished                Sep 25 2018 at 12:28                        
+Job                     test-job                         
+ Owner                   test-user                        
+ Project                 test-user                        
+ Cluster                 default                          
+ Description             test job description             
+ Status                  succeeded                        
+ Image                   test-image                       
+ Command                 test-command                     
+ Priority                Normal                           
+ Price (credits / hour)  15.0000                          
+ Current cost            150.0000                         
+ Resources                Memory               16 Bytes   
+                          CPU                       0.1   
+                          Nvidia GPU                4.0   
+                          AMD GPU                   5.0   
+                          Intel GPU                 6.0   
+                          TPU                 v2-8/1.14   
+                          Extended SHM space       True   
+ TTY                     False                            
+ Http URL                http://local.host.test/          
+ Created                 2018-09-25T12:28:21.298672+00:00 
+ Started                 2018-09-25T12:28:59.759433+00:00 
+ Finished                2018-09-25T12:28:59.759433+00:00 
  Exit code               None
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[iso]_0.ref`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Job                     test-job                                    
- Owner                   test-user                                   
- Project                                                             
- Cluster                 default                                     
- Description             test job description                        
- Status                  succeeded                                   
- Image                   test-image                                  
- Command                 test-command                                
- Priority                Normal                                      
- Price (credits / hour)  15.0000                                     
- Current cost            150.0000                                    
- Resources                Memory                           16 Bytes  
-                          CPU                                   0.1  
-                          GPU                 4.0 x nvidia-tesla-p4  
-                          TPU                             v2-8/1.14  
-                          Extended SHM space                   True  
- TTY                     False                                       
- Http URL                http://local.host.test/                     
- Created                 2018-09-25T12:28:21.298672+00:00            
- Started                 2018-09-25T12:28:59.759433+00:00            
- Finished                2018-09-25T12:28:59.759433+00:00            
- Exit code               None
+Job                     test-job                         
+ Owner                   test-user                        
+ Project                 myproject                        
+ Cluster                 default                          
+ Description             test job description             
+ Status                  failed (ErrorReason)             
+ Image                   test-image                       
+ Command                 test-command                     
+ Priority                Normal                           
+ Price (credits / hour)  15.0000                          
+ Current cost            150.0000                         
+ Resources                Memory  16.8 MB                 
+                          CPU         0.1                 
+ TTY                     False                            
+ Http URL                http://local.host.test/          
+ Http port               80                               
+ Http authentication     True                             
+ Created                 2018-09-25T12:28:21.298672+00:00 
+ Started                 2018-09-25T12:28:59.759433+00:00 
+ Finished                2018-09-25T12:28:59.759433+00:00 
+ Exit code               321                              
+ Description             ErrorDesc
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-someotherproject]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[iso]_0.ref`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Job                     test-job                                    
- Owner                   test-user                                   
- Project                 someotherproject                            
- Cluster                 default                                     
- Description             test job description                        
- Status                  succeeded                                   
- Image                   test-image                                  
- Command                 test-command                                
- Priority                Normal                                      
- Price (credits / hour)  15.0000                                     
- Current cost            150.0000                                    
- Resources                Memory                           16 Bytes  
-                          CPU                                   0.1  
-                          GPU                 4.0 x nvidia-tesla-p4  
-                          TPU                             v2-8/1.14  
-                          Extended SHM space                   True  
- TTY                     False                                       
- Http URL                http://local.host.test/                     
- Created                 2018-09-25T12:28:21.298672+00:00            
- Started                 2018-09-25T12:28:59.759433+00:00            
- Finished                2018-09-25T12:28:59.759433+00:00            
- Exit code               None
+Job                     test-job                         
+ Name                    test-job-name                    
+ Owner                   test-user                        
+ Project                 myproject                        
+ Cluster                 default                          
+ Description             test job description             
+ Status                  failed (ErrorReason)             
+ Image                   image:test-image:sometag         
+ Command                 test-command                     
+ Working dir             /working/dir                     
+ Priority                Normal                           
+ Price (credits / hour)  15.0000                          
+ Current cost            150.0000                         
+ Resources                Memory  16.8 MB                 
+                          CPU         0.1                 
+ TTY                     False                            
+ Http URL                http://local.host.test/          
+ Http port               80                               
+ Http authentication     True                             
+ Created                 2018-09-25T12:28:21.298672+00:00 
+ Started                 2018-09-25T12:28:59.759433+00:00 
+ Finished                2018-09-25T12:28:59.759433+00:00 
+ Exit code               123                              
+ Description             ErrorDesc
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-test-user]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-someotherproject]_0.ref`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Job                     test-job                                    
- Owner                   test-user                                   
- Project                 test-user                                   
- Cluster                 default                                     
- Description             test job description                        
- Status                  succeeded                                   
- Image                   test-image                                  
- Command                 test-command                                
- Priority                Normal                                      
- Price (credits / hour)  15.0000                                     
- Current cost            150.0000                                    
- Resources                Memory                           16 Bytes  
-                          CPU                                   0.1  
-                          GPU                 4.0 x nvidia-tesla-p4  
-                          TPU                             v2-8/1.14  
-                          Extended SHM space                   True  
- TTY                     False                                       
- Http URL                http://local.host.test/                     
- Created                 2018-09-25T12:28:21.298672+00:00            
- Started                 2018-09-25T12:28:59.759433+00:00            
- Finished                2018-09-25T12:28:59.759433+00:00            
+Job                     test-job                         
+ Owner                   test-user                        
+ Project                 someotherproject                 
+ Cluster                 default                          
+ Description             test job description             
+ Status                  succeeded                        
+ Image                   test-image                       
+ Command                 test-command                     
+ Priority                Normal                           
+ Price (credits / hour)  15.0000                          
+ Current cost            150.0000                         
+ Resources                Memory               16 Bytes   
+                          CPU                       0.1   
+                          Nvidia GPU                4.0   
+                          AMD GPU                   5.0   
+                          Intel GPU                 6.0   
+                          TPU                 v2-8/1.14   
+                          Extended SHM space       True   
+ TTY                     False                            
+ Http URL                http://local.host.test/          
+ Created                 2018-09-25T12:28:21.298672+00:00 
+ Started                 2018-09-25T12:28:59.759433+00:00 
+ Finished                2018-09-25T12:28:59.759433+00:00 
  Exit code               None
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[iso]_0.ref`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 Job                     test-job                         
- Name                    test-job-name                    
  Owner                   test-user                        
  Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
- Status                  failed (ErrorReason)             
- Image                   image:test-image:sometag         
+ Status                  running (ContainerRunning)       
+ Image                   test-image                       
  Command                 test-command                     
- Working dir             /working/dir                     
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
  TTY                     False                            
+ Internal Hostname       host.local                       
  Http URL                http://local.host.test/          
- Http port               80                               
- Http authentication     True                             
  Created                 2018-09-25T12:28:21.298672+00:00 
- Started                 2018-09-25T12:28:59.759433+00:00 
- Finished                2018-09-25T12:28:59.759433+00:00 
- Exit code               123                              
- Description             ErrorDesc
+ Started                 2018-09-25T12:28:24.759433+00:00
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-]_0.ref`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Job                     test-job                         
  Owner                   test-user                        
- Project                 myproject                        
+ Project                                                  
  Cluster                 default                          
  Description             test job description             
- Status                  failed (ErrorReason)             
+ Status                  succeeded                        
  Image                   test-image                       
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
- Resources                Memory  16.8 MB                 
-                          CPU         0.1                 
+ Resources                Memory               16 Bytes   
+                          CPU                       0.1   
+                          Nvidia GPU                4.0   
+                          AMD GPU                   5.0   
+                          Intel GPU                 6.0   
+                          TPU                 v2-8/1.14   
+                          Extended SHM space       True   
  TTY                     False                            
  Http URL                http://local.host.test/          
- Http port               80                               
- Http authentication     True                             
  Created                 2018-09-25T12:28:21.298672+00:00 
  Started                 2018-09-25T12:28:59.759433+00:00 
  Finished                2018-09-25T12:28:59.759433+00:00 
- Exit code               321                              
- Description             ErrorDesc
+ Exit code               None
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[iso]_0.ref`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Job                     test-job                         
- Owner                   test-user                        
- Project                 myproject                        
- Cluster                 default                          
- Description             test job description             
- Status                  running (ContainerRunning)       
- Image                   test-image                       
- Command                 test-command                     
- Priority                Normal                           
- Price (credits / hour)  15.0000                          
- Current cost            150.0000                         
- Resources                Memory  16.8 MB                 
-                          CPU         0.1                 
- TTY                     False                            
- Internal Hostname       host.local                       
- Http URL                http://local.host.test/          
- Created                 2018-09-25T12:28:21.298672+00:00 
- Started                 2018-09-25T12:28:24.759433+00:00
+Job                      test-job                         
+ Name                     test-job                         
+ Owner                    test-user                        
+ Project                  myproject                        
+ Cluster                  default                          
+ Description              test job description             
+ Status                   running (ContainerRunning)       
+ Image                    test-image                       
+ Command                  test-command                     
+ Priority                 Normal                           
+ Price (credits / hour)   15.0000                          
+ Current cost             150.0000                         
+ Resources                 Memory  16.8 MB                 
+                           CPU         0.1                 
+ TTY                      False                            
+ Internal Hostname        host.local                       
+ Internal Hostname Named  test-job--test-owner.local       
+ Http URL                 http://local.host.test/          
+ Created                  2018-09-25T12:28:21.298672+00:00 
+ Started                  2018-09-25T12:28:24.759433+00:00
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_2.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_2.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_3.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_3.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_4.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_4.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_2.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_2.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_3.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_3.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_4.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_4.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[human]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[iso]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[0-owner-#less#you#more#]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[0-owner-#less#you#more#]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[1-alice-alice]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[1-alice-alice]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-1-alice-alice]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-1-alice-alice]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-0-owner-#less#you#more#]_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-0-owner-#less#you#more#]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-1-alice-alice]_1.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-1-alice-alice]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_bucket_credentials_formatter_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_bucket_credentials_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_bucket_formatter_with_org_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_bucket_formatter_with_org_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_formatter_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_formatter_long_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_formatter_long_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_buckets_formatter_short_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_buckets_formatter_short_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disk_formatter_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disk_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disks_formatter_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disks_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disks_formatter_long_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disks_formatter_long_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/ascii/test_disks_formatter_short_0.ref` & `neuro_cli-24.5.0/tests/unit/formatters/ascii/test_disks_formatter_short_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_admin_formatters.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_admin_formatters.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_blob_formatters.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_blob_formatters.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_bucket_credentials.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_bucket_credentials.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_buckets.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_buckets.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_config_formatters.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_config_formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,24 +70,27 @@
         presets["tpu-small"] = Preset(
             credits_per_hour=Decimal("10"),
             cpu=2,
             memory=2 * 2**30,
             scheduler_enabled=False,
             tpu_type="v3-8",
             tpu_software_version="1.14",
+            resource_pool_names=["tpu"],
         )
         presets["hybrid"] = Preset(
             credits_per_hour=Decimal("10"),
             cpu=4,
             memory=30 * 2**30,
             scheduler_enabled=False,
-            gpu=2,
-            gpu_model="nvidia-tesla-v100",
+            nvidia_gpu=1,
+            amd_gpu=2,
+            intel_gpu=3,
             tpu_type="v3-64",
             tpu_software_version="1.14",
+            resource_pool_names=["gpu-small", "gpu-large"],
         )
         new_config = replace(cluster_config, presets=presets)
 
         client = make_client(
             "https://dev.neu.ro/api/v1", clusters={new_config.name: new_config}
         )
         out = ConfigFormatter()(
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_disks.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_disks.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_images_formatters.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_images_formatters.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_jobs_formatters.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_jobs_formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             description="ErrorDesc",
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
             finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
         ),
         container=Container(
             image=RemoteImage.new_external_image(name="ubuntu", tag="latest"),
-            resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+            resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
         ),
         scheduler_enabled=True,
         pass_config=True,
         total_price_credits=Decimal("150"),
         price_credits_per_hour=Decimal("15"),
     )
 
@@ -136,15 +136,15 @@
             description="ErrorDesc",
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
             finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
         ),
         container=Container(
             image=RemoteImage.new_external_image(name="ubuntu", tag="latest"),
-            resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+            resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
         ),
         scheduler_enabled=True,
         pass_config=True,
         total_price_credits=Decimal("150"),
         price_credits_per_hour=Decimal("15"),
     )
 
@@ -181,19 +181,20 @@
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
             finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
         ),
         container=Container(
             command="test-command",
             image=RemoteImage.new_external_image(name="test-image"),
             resources=Resources(
-                16,
-                0.1,
-                4,
-                "nvidia-tesla-p4",
-                True,
+                memory=16,
+                cpu=0.1,
+                nvidia_gpu=4,
+                amd_gpu=5,
+                intel_gpu=6,
+                shm=True,
                 tpu_type="v2-8",
                 tpu_software_version="1.14",
             ),
         ),
         scheduler_enabled=False,
         pass_config=True,
         life_span=life_span,
@@ -426,15 +427,15 @@
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 exit_code=123,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -470,15 +471,15 @@
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 exit_code=123,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
                 volumes=[
                     Volume(
                         storage_uri=URL("storage://default/test-org/test-user/folder"),
                         container_path="/mnt/storage",
                     )
                 ],
@@ -519,15 +520,15 @@
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 exit_code=123,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -562,15 +563,15 @@
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 exit_code=123,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -604,15 +605,15 @@
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 exit_code=123,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             life_span=1.0 * ((60 * 60 * 24 * 1) + (60 * 60 * 2) + (60 * 3) + 4),
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
@@ -647,15 +648,15 @@
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 exit_code=123,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             life_span=0.0,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
@@ -691,15 +692,15 @@
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 exit_code=123,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             restart_policy=JobRestartPolicy.ALWAYS,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
@@ -734,15 +735,15 @@
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 exit_code=321,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -770,15 +771,15 @@
                 created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                 started_at=None,
                 finished_at=None,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=True,
             pass_config=True,
             project_name="myproject",
             owner="owner",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
@@ -809,15 +810,15 @@
                 created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                 started_at=None,
                 finished_at=None,
             ),
             container=Container(
                 image=RemoteImage.new_external_image(name="test-image"),
                 command="test-command",
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 tty=True,
             ),
             scheduler_enabled=True,
             pass_config=True,
             owner="owner",
             project_name="myproject",
             cluster_name="default",
@@ -849,15 +850,15 @@
                 created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                 started_at=None,
                 finished_at=None,
             ),
             container=Container(
                 image=RemoteImage.new_external_image(name="test-image"),
                 command="test-command",
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=True,
             pass_config=True,
             owner="owner",
             project_name="myproject",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
@@ -893,15 +894,15 @@
                 started_at=isoparse("2018-09-25T12:28:24.759433+00:00"),
                 finished_at=None,
             ),
             http_url=URL("http://local.host.test/"),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             internal_hostname="host.local",
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -955,15 +956,15 @@
                     ),
                 ],
             ),
             http_url=URL("http://local.host.test/"),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             internal_hostname="host.local",
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -997,15 +998,15 @@
                 started_at=isoparse("2018-09-25T12:28:24.759433+00:00"),
                 finished_at=None,
             ),
             http_url=URL("http://local.host.test/"),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             internal_hostname="host.local",
             internal_hostname_named="test-job--test-owner.local",
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
@@ -1040,15 +1041,15 @@
                 finished_at=None,
             ),
             http_url=URL("http://local.host.test/"),
             container=Container(
                 entrypoint="/usr/bin/make",
                 command="test",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             internal_hostname="host.local",
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -1090,15 +1091,15 @@
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
                     cluster_name="test-cluster",
                     org_name=None,
                     project_name="test-project",
                 ),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
                 env={"ENV_NAME_1": "__value1__", "ENV_NAME_2": "**value2**"},
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
@@ -1141,15 +1142,15 @@
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
                     cluster_name="test-cluster",
                     org_name=None,
                     project_name="test-project",
                 ),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
                 volumes=[
                     Volume(
                         storage_uri=URL("storage://test-cluster/otherproject/_ro_"),
                         container_path="/mnt/_ro_",
                         read_only=True,
                     ),
@@ -1208,15 +1209,15 @@
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
                     cluster_name="test-cluster",
                     org_name=None,
                     project_name="test-project",
                 ),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
                 volumes=[
                     Volume(
                         storage_uri=URL("storage://test-cluster/otherproject/ro"),
                         container_path="/mnt/ro",
                         read_only=True,
                     ),
@@ -1267,15 +1268,15 @@
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
                     cluster_name="test-cluster",
                     org_name=None,
                     project_name="test-project",
                 ),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
                 volumes=[
                     Volume(
                         storage_uri=URL("storage://test-cluster/test-project/rw"),
                         container_path="/mnt/rw",
                         read_only=False,
                     ),
@@ -1344,15 +1345,15 @@
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
                     cluster_name="test-cluster",
                     org_name=None,
                     project_name="test-project",
                 ),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
                 disk_volumes=[
                     DiskVolume(
                         URL("disk://test-cluster/test-project/disk1"),
                         "/mnt/disk1",
                         read_only=True,
                     ),
@@ -1412,15 +1413,15 @@
                     tag="sometag",
                     registry="https://registry.neu.ro",
                     cluster_name="test-cluster",
                     org_name=None,
                     project_name="test-project",
                 ),
                 working_dir="/working/dir",
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -1449,15 +1450,15 @@
                 started_at=None,
                 finished_at=None,
             ),
             preset_name="cpu-small",
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             project_name="myproject",
             owner="owner",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
@@ -1488,15 +1489,15 @@
                 created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                 started_at=None,
                 finished_at=None,
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=True,
             preemptible_node=True,
             pass_config=True,
             project_name="myproject",
             owner="owner",
             cluster_name="default",
@@ -1534,15 +1535,15 @@
                 started_at=isoparse("2018-09-25T12:28:24.759433+00:00"),
                 finished_at=None,
             ),
             http_url=URL("http://local.host.test/"),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
@@ -1575,15 +1576,15 @@
                 started_at=isoparse("2018-09-25T12:28:24.759433+00:00"),
                 finished_at=None,
             ),
             http_url=URL("http://local.host.test/"),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal(150 / 15000),
             price_credits_per_hour=Decimal(15 / 15000),
         )
 
@@ -1611,15 +1612,15 @@
                 started_at=None,
                 finished_at=None,
             ),
             preset_name="cpu-small",
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=True,
             energy_schedule_name="some-schedule",
             pass_config=True,
             project_name="myproject",
             owner="owner",
             cluster_name="default",
@@ -1900,15 +1901,15 @@
                     description="ErrorDesc",
                     created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                     started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                     finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 ),
                 container=Container(
                     image=RemoteImage.new_external_image(name="ubuntu", tag="latest"),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 ),
                 scheduler_enabled=True,
                 pass_config=True,
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
             ),
             JobDescription(
@@ -1925,15 +1926,15 @@
                     description="ErrorDesc",
                     created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                     started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                     finished_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 ),
                 container=Container(
                     image=RemoteImage.new_external_image(name="ubuntu", tag="latest"),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 ),
                 scheduler_enabled=True,
                 pass_config=True,
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
             ),
         ]
@@ -1965,15 +1966,15 @@
                 description="ErrorDesc",
                 created_at=isoparse("2017-01-02T12:28:21.298672+00:00"),
                 started_at=isoparse("2017-02-03T12:28:59.759433+00:00"),
                 finished_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
             ),
             container=Container(
                 image=remote_image,
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 command="ls",
             ),
             scheduler_enabled=True,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -2110,15 +2111,15 @@
                 description="ErrorDesc",
                 created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
             ),
             container=Container(
                 image=RemoteImage.new_external_image(name="i", tag="l"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 command="c",
             ),
             scheduler_enabled=True,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -2162,15 +2163,15 @@
                     started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                     finished_at=isoparse("2017-09-25T12:28:59.759433+00:00"),
                 ),
                 container=Container(
                     image=RemoteImage.new_external_image(
                         name="some-image-name", tag="with-long-tag"
                     ),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                     command="ls -la /some/path",
                 ),
                 scheduler_enabled=True,
                 pass_config=True,
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
             ),
@@ -2199,15 +2200,15 @@
                         name="some-image-name",
                         tag="with-long-tag",
                         registry="https://registry.neu.ro",
                         cluster_name="test-cluster",
                         org_name=None,
                         project_name="test-project",
                     ),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                     command="ls -la /some/path",
                 ),
                 scheduler_enabled=True,
                 pass_config=True,
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
             ),
@@ -2238,15 +2239,15 @@
                 description="ErrorDesc",
                 created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
             ),
             container=Container(
                 image=RemoteImage.new_external_image(name="i", tag="l"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 command="c",
             ),
             scheduler_enabled=True,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -2280,15 +2281,15 @@
                     description="ErrorDesc",
                     created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                     started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                     finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
                 ),
                 container=Container(
                     image=RemoteImage.new_external_image(name="i", tag="l"),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                     command="c",
                 ),
                 scheduler_enabled=True,
                 pass_config=True,
                 life_span=life_span,
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
@@ -2349,15 +2350,15 @@
                 id=f"job-{i}",
                 uri=URL(f"job://default/test-user/job-{i}"),
                 description=None,
                 history=item,
                 container=Container(
                     command="test-command",
                     image=RemoteImage.new_external_image(name="test-image"),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 ),
                 scheduler_enabled=False,
                 pass_config=True,
                 internal_hostname="host.local",
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
             )
@@ -2393,15 +2394,15 @@
                     created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                     started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                     finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
                 ),
                 container=Container(
                     command="test-command",
                     image=RemoteImage.new_external_image(name="test-image"),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                     working_dir=working_dir,
                 ),
                 scheduler_enabled=False,
                 pass_config=True,
                 internal_hostname="host.local",
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
@@ -2436,15 +2437,15 @@
                     created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                     started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                     finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
                 ),
                 container=Container(
                     command="test-command",
                     image=RemoteImage.new_external_image(name="test-image"),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 ),
                 scheduler_enabled=False,
                 pass_config=True,
                 internal_hostname="host.local",
                 preset_name=preset_name,
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
@@ -2482,15 +2483,15 @@
                     created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                     started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                     finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
                 ),
                 container=Container(
                     command="test-command",
                     image=RemoteImage.new_external_image(name="test-image"),
-                    resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                    resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
                 ),
                 scheduler_enabled=False,
                 pass_config=True,
                 internal_hostname="host.local",
                 preset_name=None,
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
@@ -2580,15 +2581,15 @@
                         transition_time=isoparse("2018-09-25T12:28:24.759433+00:00"),
                     ),
                 ],
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             life_span=360000,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
@@ -2616,15 +2617,15 @@
                 created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
                 started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
                 finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
-                resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
+                resources=Resources(memory=16 * 2**20, cpu=0.1, shm=False),
             ),
             scheduler_enabled=False,
             pass_config=True,
             life_span=3600,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
```

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_secrets.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_secrets.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_service_accounts.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_service_accounts.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_storage_formatters.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_storage_formatters.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/formatters/test_utils.py` & `neuro_cli-24.5.0/tests/unit/formatters/test_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_admin.py` & `neuro_cli-24.5.0/tests/unit/test_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,16 +362,17 @@
         ) -> None:
             assert cluster_name == "default"
             assert preset == _ResourcePreset(
                 name="cpu-micro",
                 credits_per_hour=Decimal("10"),
                 cpu=0.1,
                 memory=100 * 10**6,
-                gpu=1,
-                gpu_model="nvidia-tesla-k80",
+                nvidia_gpu=1,
+                amd_gpu=2,
+                intel_gpu=3,
                 tpu=_TPUPreset(
                     type="v2-8",
                     software_version="1.14",
                 ),
                 scheduler_enabled=True,
                 preemptible_node=True,
             )
@@ -391,16 +392,18 @@
                 "10.00",
                 "-c",
                 "0.1",
                 "-m",
                 "100Mb",
                 "-g",
                 "1",
-                "--gpu-model",
-                "nvidia-tesla-k80",
+                "--amd-gpu",
+                "2",
+                "--intel-gpu",
+                "3",
                 "--tpu-type",
                 "v2-8",
                 "--tpu-sw-version",
                 "1.14",
                 "-p",
                 "--preemptible-node",
             ]
@@ -450,16 +453,17 @@
             assert cluster_name == "default"
             assert p.name == "cpu-small"
             nonlocal preset
             preset = Preset(
                 credits_per_hour=p.credits_per_hour,
                 cpu=p.cpu,
                 memory=p.memory,
-                gpu=p.gpu,
-                gpu_model=p.gpu_model,
+                nvidia_gpu=p.nvidia_gpu,
+                amd_gpu=p.amd_gpu,
+                intel_gpu=p.intel_gpu,
                 tpu_type=p.tpu.type if p.tpu else None,
                 tpu_software_version=p.tpu.software_version if p.tpu else None,
                 preemptible_node=p.preemptible_node,
                 scheduler_enabled=p.scheduler_enabled,
             )
 
         async def fetch() -> None:
@@ -491,16 +495,18 @@
                 "122.00",
                 "-c",
                 "0.1",
                 "-m",
                 "100Mb",
                 "-g",
                 "1",
-                "--gpu-model",
-                "nvidia-tesla-k80",
+                "--amd-gpu",
+                "2",
+                "--intel-gpu",
+                "3",
                 "--tpu-type",
                 "v2-8",
                 "--tpu-sw-version",
                 "1.14",
                 "-p",
                 "--preemptible-node",
             ]
@@ -508,16 +514,17 @@
         assert capture.code == 0, capture.out + capture.err
         assert preset == Preset(
             credits_per_hour=Decimal("122.00"),
             cpu=0.1,
             memory=10**8,
             scheduler_enabled=True,
             preemptible_node=True,
-            gpu=1,
-            gpu_model="nvidia-tesla-k80",
+            nvidia_gpu=1,
+            amd_gpu=2,
+            intel_gpu=3,
             tpu_type="v2-8",
             tpu_software_version="1.14",
         )
 
 
 def test_add_resource_preset_print_result(run_cli: _RunCli) -> None:
     with ExitStack() as exit_stack:
```

### Comparing `neuro-cli-24.2.0/tests/unit/test_ael.py` & `neuro_cli-24.5.0/tests/unit/test_ael.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_alias.py` & `neuro_cli-24.5.0/tests/unit/test_alias.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_click_types.py` & `neuro_cli-24.5.0/tests/unit/test_click_types.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_click_utils.py` & `neuro_cli-24.5.0/tests/unit/test_click_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_config.py` & `neuro_cli-24.5.0/tests/unit/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Callable
 from unittest import mock
 
 import pytest
 from yarl import URL
 
-from neuro_sdk import Client, Cluster, Preset, Project
+from neuro_sdk import Client, Cluster, Preset, Project, ResourcePool
 
 from neuro_cli.config import prompt_cluster, prompt_project
 from neuro_cli.root import Root
 from neuro_cli.utils import Command, Context
 
 
 async def cmd() -> None:
@@ -28,14 +28,23 @@
             registry_url=URL("https://registry-dev.neu.ro"),
             storage_url=URL("https://storage-dev.neu.ro"),
             users_url=URL("https://users-dev.neu.ro"),
             monitoring_url=URL("https://monitoring-dev.neu.ro"),
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
+                ),
+            },
             presets={
                 "cpu-small": Preset(
                     credits_per_hour=Decimal("10"), cpu=1, memory=2**30
                 )
             },
             name="first",
             orgs=[None],
@@ -44,14 +53,23 @@
             registry_url=URL("https://registry2-dev.neu.ro"),
             storage_url=URL("https://storage2-dev.neu.ro"),
             users_url=URL("https://users2-dev.neu.ro"),
             monitoring_url=URL("https://monitoring2-dev.neu.ro"),
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
+                ),
+            },
             presets={
                 "cpu-small": Preset(
                     credits_per_hour=Decimal("10"), cpu=2, memory=2**30
                 )
             },
             name="second",
             orgs=[None],
@@ -102,14 +120,23 @@
             registry_url=URL("https://registry-dev.neu.ro"),
             storage_url=URL("https://storage-dev.neu.ro"),
             users_url=URL("https://users-dev.neu.ro"),
             monitoring_url=URL("https://monitoring-dev.neu.ro"),
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
+                ),
+            },
             presets={
                 "cpu-small": Preset(
                     credits_per_hour=Decimal("10"), cpu=1, memory=2**30
                 )
             },
             name="first",
             orgs=[None],
@@ -118,14 +145,23 @@
             registry_url=URL("https://registry2-dev.neu.ro"),
             storage_url=URL("https://storage2-dev.neu.ro"),
             users_url=URL("https://users2-dev.neu.ro"),
             monitoring_url=URL("https://monitoring2-dev.neu.ro"),
             secrets_url=URL("https://secrets2-dev.neu.ro"),
             disks_url=URL("https://disks2-dev.neu.ro"),
             buckets_url=URL("https://disks2-dev.neu.ro"),
+            resource_pools={
+                "cpu": ResourcePool(
+                    min_size=1,
+                    max_size=2,
+                    cpu=7,
+                    memory=14 * 2**30,
+                    disk_size=150 * 2**30,
+                ),
+            },
             presets={
                 "cpu-small": Preset(
                     credits_per_hour=Decimal("10"), cpu=2, memory=2**30
                 )
             },
             name="second",
             orgs=[None],
@@ -178,14 +214,23 @@
             registry_url=URL("https://registry-dev.neu.ro"),
             storage_url=URL("https://storage-dev.neu.ro"),
             users_url=URL("https://users-dev.neu.ro"),
             monitoring_url=URL("https://monitoring-dev.neu.ro"),
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
+                ),
+            },
             presets={
                 "cpu-small": Preset(
                     credits_per_hour=Decimal("10"), cpu=1, memory=2**30
                 )
             },
             orgs=[None],
         ),
@@ -238,14 +283,23 @@
             registry_url=URL("https://registry-dev.neu.ro"),
             storage_url=URL("https://storage-dev.neu.ro"),
             users_url=URL("https://users-dev.neu.ro"),
             monitoring_url=URL("https://monitoring-dev.neu.ro"),
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
+                ),
+            },
             presets={
                 "cpu-small": Preset(
                     credits_per_hour=Decimal("10"), cpu=1, memory=2**30
                 )
             },
             orgs=[None],
         ),
```

### Comparing `neuro-cli-24.2.0/tests/unit/test_docker_helper.py` & `neuro_cli-24.5.0/tests/unit/test_docker_helper.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_job.py` & `neuro_cli-24.5.0/tests/unit/test_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,27 +206,25 @@
     }
     assert env == {"ENV_VAR_2": "value2", "ENV_VAR_4": "value4"}
 
 
 async def test_calc_ps_columns_section_doesnt_exist(
     monkeypatch: Any, tmp_path: Path, make_client: _MakeClient
 ) -> None:
-
     async with make_client("https://example.com") as client:
         monkeypatch.chdir(tmp_path)
         local_conf = tmp_path / ".neuro.toml"
         # empty config
         local_conf.write_text("")
         assert await calc_ps_columns(client, None) == get_default_ps_columns()
 
 
 async def test_calc_top_columns_section_doesnt_exist(
     monkeypatch: Any, tmp_path: Path, make_client: _MakeClient
 ) -> None:
-
     async with make_client("https://example.com") as client:
         monkeypatch.chdir(tmp_path)
         local_conf = tmp_path / ".neuro.toml"
         # empty config
         local_conf.write_text("")
         assert await calc_top_columns(client, None) == get_default_top_columns()
 
@@ -296,15 +294,15 @@
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
             finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
         ),
         container=Container(
             command="test-command",
             image=RemoteImage.new_external_image(name="test-image"),
-            resources=Resources(16, 0.1, 0, None, True, None, None),
+            resources=Resources(memory=16, cpu=0.1, shm=True),
         ),
         scheduler_enabled=False,
         pass_config=False,
         preset_name="testing",
         total_price_credits=Decimal("150"),
         price_credits_per_hour=Decimal("15"),
     )
@@ -335,15 +333,15 @@
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
             finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
         ),
         container=Container(
             command="test-command",
             image=RemoteImage.new_external_image(name="test-image"),
-            resources=Resources(16, 0.1, 0, None, True, None, None),
+            resources=Resources(memory=16, cpu=0.1, shm=True),
             env={
                 "NEURO_PASSED_CONFIG": "base64 data here",
             },
         ),
         scheduler_enabled=False,
         pass_config=True,
         preset_name="testing",
@@ -381,15 +379,15 @@
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
             finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
         ),
         container=Container(
             command="test-command",
             image=RemoteImage.new_external_image(name="test-image"),
-            resources=Resources(16, 0.1, 0, None, False, None, None),
+            resources=Resources(memory=16, cpu=0.1, shm=False),
             working_dir="/mnt/test",
             volumes=[
                 Volume(
                     storage_uri=URL("storage://test-cluster/test-user/_ro_"),
                     container_path="/mnt/_ro_",
                     read_only=True,
                 ),
@@ -510,15 +508,15 @@
             description="ErrorDesc",
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
             finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
         ),
         container=Container(
             image=RemoteImage.new_external_image(name="test-image"),
-            resources=Resources(16, 0.1, 0, None, True, None, None),
+            resources=Resources(memory=16, cpu=0.1, shm=True),
         ),
         scheduler_enabled=False,
         pass_config=False,
         preset_name="testing",
         total_price_credits=Decimal("150"),
         price_credits_per_hour=Decimal("15"),
     )
```

### Comparing `neuro-cli-24.2.0/tests/unit/test_parse_utils.py` & `neuro_cli-24.5.0/tests/unit/test_parse_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_root.py` & `neuro_cli-24.5.0/tests/unit/test_root.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_shell_completion.py` & `neuro_cli-24.5.0/tests/unit/test_shell_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,17 +227,19 @@
         @asyncgeneratorcontextmanager
         async def list(uri: URL) -> AsyncIterator[FileStatus]:
             uri = normalize_storage_path_uri(uri, "test-user", "default", org_name=None)
             for name in tree[uri]:
                 child = uri / name
                 yield FileStatus(
                     path=name,
-                    type=FileStatusType.DIRECTORY
-                    if is_dir(child)
-                    else FileStatusType.FILE,
+                    type=(
+                        FileStatusType.DIRECTORY
+                        if is_dir(child)
+                        else FileStatusType.FILE
+                    ),
                     size=0,
                     modification_time=1234567890,
                     permission=Action.WRITE,
                     uri=child,
                 )
 
         mocked_stat.side_effect = stat
@@ -617,15 +619,15 @@
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
             finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
         ),
         container=Container(
             command="test-command",
             image=RemoteImage.new_external_image(name="test-image"),
-            resources=Resources(16, 0.1, 0, None, True, None, None),
+            resources=Resources(memory=16, cpu=0.1, shm=True),
         ),
         scheduler_enabled=False,
         pass_config=False,
         preset_name="testing",
         total_price_credits=Decimal("150"),
         price_credits_per_hour=Decimal("15"),
     )
```

### Comparing `neuro-cli-24.2.0/tests/unit/test_stats.py` & `neuro_cli-24.5.0/tests/unit/test_stats.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_storage.py` & `neuro_cli-24.5.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_storage_progress.py` & `neuro_cli-24.5.0/tests/unit/test_storage_progress.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-24.2.0/tests/unit/test_utils.py` & `neuro_cli-24.5.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

