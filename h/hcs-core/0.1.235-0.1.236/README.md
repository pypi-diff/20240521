# Comparing `tmp/hcs_core-0.1.235.tar.gz` & `tmp/hcs_core-0.1.236.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs_core-0.1.235.tar", last modified: Mon May 20 22:38:06 2024, max compression
+gzip compressed data, was "hcs_core-0.1.236.tar", last modified: Mon May 20 23:16:32 2024, max compression
```

## Comparing `hcs_core-0.1.235.tar` & `hcs_core-0.1.236.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.107575 hcs_core-0.1.235/
--rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 22:38:06.106920 hcs_core-0.1.235/PKG-INFO
--rw-r--r--   0 nanw       (503) staff       (20)       25 2024-05-14 18:28:08.000000 hcs_core-0.1.235/README.md
--rw-r--r--   0 nanw       (503) staff       (20)        7 2024-05-20 22:38:02.000000 hcs_core-0.1.235/VERSION
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.066045 hcs_core-0.1.235/hcs_core/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/__init__.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.077944 hcs_core-0.1.235/hcs_core/ctxp/
--rw-r--r--   0 nanw       (503) staff       (20)      790 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 22:21:06.000000 hcs_core-0.1.235/hcs_core/ctxp/_init.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.082558 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     3086 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (503) staff       (20)     2387 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (503) staff       (20)     4034 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (503) staff       (20)     2274 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/cli_options.py
--rw-r--r--   0 nanw       (503) staff       (20)     5791 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (503) staff       (20)      931 2024-05-20 15:58:31.000000 hcs_core-0.1.235/hcs_core/ctxp/config.py
--rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 16:01:06.000000 hcs_core-0.1.235/hcs_core/ctxp/context.py
--rw-r--r--   0 nanw       (503) staff       (20)    14068 2024-05-20 15:59:29.000000 hcs_core-0.1.235/hcs_core/ctxp/data_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     2856 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/duration.py
--rw-r--r--   0 nanw       (503) staff       (20)     1658 2024-05-20 22:32:30.000000 hcs_core-0.1.235/hcs_core/ctxp/extension.py
--rw-r--r--   0 nanw       (503) staff       (20)     6801 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/fstore.py
--rw-r--r--   0 nanw       (503) staff       (20)     4666 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/jsondot.py
--rw-r--r--   0 nanw       (503) staff       (20)     6310 2024-05-20 22:36:14.000000 hcs_core-0.1.235/hcs_core/ctxp/logger.py
--rw-r--r--   0 nanw       (503) staff       (20)     6586 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/profile.py
--rw-r--r--   0 nanw       (503) staff       (20)     1565 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/profile_store.py
--rw-r--r--   0 nanw       (503) staff       (20)     1767 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/recent.py
--rw-r--r--   0 nanw       (503) staff       (20)     1619 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/state.py
--rw-r--r--   0 nanw       (503) staff       (20)     8036 2024-05-14 21:19:34.000000 hcs_core-0.1.235/hcs_core/ctxp/util.py
--rw-r--r--   0 nanw       (503) staff       (20)     3244 2024-05-20 16:02:07.000000 hcs_core-0.1.235/hcs_core/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.087013 hcs_core-0.1.235/hcs_core/plan/
--rw-r--r--   0 nanw       (503) staff       (20)      203 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)      125 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/actions.py
--rw-r--r--   0 nanw       (503) staff       (20)     1298 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/base_provider.py
--rw-r--r--   0 nanw       (503) staff       (20)      116 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/context.py
--rw-r--r--   0 nanw       (503) staff       (20)    20957 2024-05-17 23:12:51.000000 hcs_core-0.1.235/hcs_core/plan/core.py
--rw-r--r--   0 nanw       (503) staff       (20)    12966 2024-05-20 22:31:51.000000 hcs_core-0.1.235/hcs_core/plan/dag.py
--rw-r--r--   0 nanw       (503) staff       (20)     7784 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/helper.py
--rw-r--r--   0 nanw       (503) staff       (20)     5471 2024-05-20 22:19:59.000000 hcs_core-0.1.235/hcs_core/plan/kop.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.087671 hcs_core-0.1.235/hcs_core/plan/provider/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.089447 hcs_core-0.1.235/hcs_core/plan/provider/dev/
--rw-r--r--   0 nanw       (503) staff       (20)       30 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)       34 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (503) staff       (20)     1994 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (503) staff       (20)     1104 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.096287 hcs_core-0.1.235/hcs_core/sglib/
--rw-r--r--   0 nanw       (503) staff       (20)      654 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     5194 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/auth.py
--rw-r--r--   0 nanw       (503) staff       (20)     1796 2024-05-20 16:06:32.000000 hcs_core-0.1.235/hcs_core/sglib/cli_options.py
--rw-r--r--   0 nanw       (503) staff       (20)     8378 2024-05-20 22:12:17.000000 hcs_core-0.1.235/hcs_core/sglib/client_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     8043 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/csp.py
--rw-r--r--   0 nanw       (503) staff       (20)     5167 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/ez_client.py
--rw-r--r--   0 nanw       (503) staff       (20)      901 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/hcs_client.py
--rw-r--r--   0 nanw       (503) staff       (20)    10130 2024-05-20 16:05:14.000000 hcs_core-0.1.235/hcs_core/sglib/login_support.py
--rw-r--r--   0 nanw       (503) staff       (20)      689 2024-05-20 16:05:58.000000 hcs_core-0.1.235/hcs_core/sglib/payload_util.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.104814 hcs_core-0.1.235/hcs_core/util/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/__init__.py
--rwxr-xr-x   0 nanw       (503) staff       (20)     2535 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/check_license.py
--rw-r--r--   0 nanw       (503) staff       (20)     3482 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/duration.py
--rw-r--r--   0 nanw       (503) staff       (20)      838 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/exit.py
--rw-r--r--   0 nanw       (503) staff       (20)     1755 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/hcs_constants.py
--rw-r--r--   0 nanw       (503) staff       (20)     8438 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/job_view.py
--rw-r--r--   0 nanw       (503) staff       (20)     5288 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/pki_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     1946 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/query_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     2958 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/scheduler.py
--rw-r--r--   0 nanw       (503) staff       (20)     1239 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/ssl_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     1727 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/versions.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.106246 hcs_core-0.1.235/hcs_core.egg-info/
--rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (503) staff       (20)     1788 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (503) staff       (20)        1 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/requires.txt
--rw-r--r--   0 nanw       (503) staff       (20)        9 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/top_level.txt
--rw-r--r--   0 nanw       (503) staff       (20)     1250 2024-05-14 18:28:08.000000 hcs_core-0.1.235/pyproject.toml
--rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:28:08.000000 hcs_core-0.1.235/requirements.txt
--rw-r--r--   0 nanw       (503) staff       (20)       38 2024-05-20 22:38:06.107649 hcs_core-0.1.235/setup.cfg
--rw-r--r--   0 nanw       (503) staff       (20)      808 2024-05-14 18:28:08.000000 hcs_core-0.1.235/setup.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.302274 hcs_core-0.1.236/
+-rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 23:16:32.301372 hcs_core-0.1.236/PKG-INFO
+-rw-r--r--   0 nanw       (503) staff       (20)       25 2024-05-14 18:28:08.000000 hcs_core-0.1.236/README.md
+-rw-r--r--   0 nanw       (503) staff       (20)        7 2024-05-20 23:16:30.000000 hcs_core-0.1.236/VERSION
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.262908 hcs_core-0.1.236/hcs_core/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/__init__.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.275205 hcs_core-0.1.236/hcs_core/ctxp/
+-rw-r--r--   0 nanw       (503) staff       (20)      790 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 22:21:06.000000 hcs_core-0.1.236/hcs_core/ctxp/_init.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.278956 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3086 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2388 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)     4034 2024-05-20 22:44:20.000000 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2274 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5800 2024-05-20 23:02:06.000000 hcs_core-0.1.236/hcs_core/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (503) staff       (20)      931 2024-05-20 15:58:31.000000 hcs_core-0.1.236/hcs_core/ctxp/config.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 16:01:06.000000 hcs_core-0.1.236/hcs_core/ctxp/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)    14092 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/ctxp/data_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2856 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/duration.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1658 2024-05-20 22:32:30.000000 hcs_core-0.1.236/hcs_core/ctxp/extension.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6805 2024-05-20 22:48:34.000000 hcs_core-0.1.236/hcs_core/ctxp/fstore.py
+-rw-r--r--   0 nanw       (503) staff       (20)     4666 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6320 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/ctxp/logger.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6602 2024-05-20 23:02:31.000000 hcs_core-0.1.236/hcs_core/ctxp/profile.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1565 2024-05-20 22:51:09.000000 hcs_core-0.1.236/hcs_core/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1767 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/recent.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1619 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/state.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8036 2024-05-20 22:52:07.000000 hcs_core-0.1.236/hcs_core/ctxp/util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3244 2024-05-20 16:02:07.000000 hcs_core-0.1.236/hcs_core/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.283033 hcs_core-0.1.236/hcs_core/plan/
+-rw-r--r--   0 nanw       (503) staff       (20)      203 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)      125 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/actions.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1298 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/base_provider.py
+-rw-r--r--   0 nanw       (503) staff       (20)      116 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)    20957 2024-05-20 22:52:58.000000 hcs_core-0.1.236/hcs_core/plan/core.py
+-rw-r--r--   0 nanw       (503) staff       (20)    12950 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/plan/dag.py
+-rw-r--r--   0 nanw       (503) staff       (20)     7761 2024-05-20 22:55:21.000000 hcs_core-0.1.236/hcs_core/plan/helper.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5454 2024-05-20 22:55:35.000000 hcs_core-0.1.236/hcs_core/plan/kop.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.283569 hcs_core-0.1.236/hcs_core/plan/provider/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.285652 hcs_core-0.1.236/hcs_core/plan/provider/dev/
+-rw-r--r--   0 nanw       (503) staff       (20)       30 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)       34 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1982 2024-05-20 22:55:55.000000 hcs_core-0.1.236/hcs_core/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1104 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.289589 hcs_core-0.1.236/hcs_core/sglib/
+-rw-r--r--   0 nanw       (503) staff       (20)      654 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/sglib/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5169 2024-05-20 22:56:14.000000 hcs_core-0.1.236/hcs_core/sglib/auth.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1796 2024-05-20 16:06:32.000000 hcs_core-0.1.236/hcs_core/sglib/cli_options.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8379 2024-05-20 22:57:08.000000 hcs_core-0.1.236/hcs_core/sglib/client_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8053 2024-05-20 22:57:40.000000 hcs_core-0.1.236/hcs_core/sglib/csp.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5167 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/sglib/ez_client.py
+-rw-r--r--   0 nanw       (503) staff       (20)      901 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (503) staff       (20)    10128 2024-05-20 23:01:41.000000 hcs_core-0.1.236/hcs_core/sglib/login_support.py
+-rw-r--r--   0 nanw       (503) staff       (20)      683 2024-05-20 22:59:20.000000 hcs_core-0.1.236/hcs_core/sglib/payload_util.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.299356 hcs_core-0.1.236/hcs_core/util/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/__init__.py
+-rwxr-xr-x   0 nanw       (503) staff       (20)     2535 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/check_license.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3482 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/duration.py
+-rw-r--r--   0 nanw       (503) staff       (20)      838 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/exit.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1755 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/hcs_constants.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8395 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/util/job_view.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5281 2024-05-20 23:00:41.000000 hcs_core-0.1.236/hcs_core/util/pki_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1946 2024-05-20 23:01:09.000000 hcs_core-0.1.236/hcs_core/util/query_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2958 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/scheduler.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1239 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/ssl_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1727 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/versions.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.300480 hcs_core-0.1.236/hcs_core.egg-info/
+-rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (503) staff       (20)     1788 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (503) staff       (20)        1 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/requires.txt
+-rw-r--r--   0 nanw       (503) staff       (20)        9 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (503) staff       (20)     1250 2024-05-14 18:28:08.000000 hcs_core-0.1.236/pyproject.toml
+-rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:28:08.000000 hcs_core-0.1.236/requirements.txt
+-rw-r--r--   0 nanw       (503) staff       (20)       38 2024-05-20 23:16:32.302366 hcs_core-0.1.236/setup.cfg
+-rw-r--r--   0 nanw       (503) staff       (20)      808 2024-05-14 18:28:08.000000 hcs_core-0.1.236/setup.py
```

### Comparing `hcs_core-0.1.235/PKG-INFO` & `hcs_core-0.1.236/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.235
+Version: 0.1.236
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/__init__.py` & `hcs_core-0.1.236/hcs_core/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/_init.py` & `hcs_core-0.1.236/hcs_core/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/_ut.py` & `hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/context.py` & `hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     if data is None:
         return None
     return data.get(key)
 
 
 @context.command()
 @click.argument("name")
-@click.argument("key_value")  #'key value pair, example: k1=v1'
+@click.argument("key_value")  # 'key value pair, example: k1=v1'
 def set(name: str, key_value: str):
     """Set a context object by name."""
     parts = key_value.split("=")
     if len(parts) != 2:
         ctxp.panic("Invalid KEY_VALUE format. Valid example: key1=value1")
     k, v = parts
     data = ctxp.context.get(name, default={})
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/profile.py` & `hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
 
 @profile_cmd_group.command()
 @click.argument("name", required=False)
 def use(name: str):
     """Switch to a specific profile. If no name specified, launch interactive list to choose profile."""
 
     if name:
-        if profile.use(name) == None:
+        if profile.use(name) is None:
             panic("No such profile: " + name)
     else:
         current = profile.name()
         choices = profile.names()
         if not choices:
             panic("No profile available.")
 
         ret = questionary.select("Select profile", choices, default=current, show_selected=True).ask()
         if ret:
-            if profile.use(ret) == None:
+            if profile.use(ret) is None:
                 panic("No such profile: " + name)
         else:
             # aborted
             return "", 1
 
 
 @profile_cmd_group.command()
@@ -73,21 +73,21 @@
 
 @profile_cmd_group.command()
 @click.argument("name", required=False)
 def get(name: str):
     """Get content of a specific profile."""
     if name:
         data = profile.get(name)
-        if data == None:
+        if data is None:
             panic(
                 "Profile not found. Use 'hcs profile list' to show available profiles, or 'hcs profile init' to create one."
             )
     else:
         data = profile.current()
-        if data == None:
+        if data is None:
             panic(
                 "Default profile not set. Use 'hcs profile list' to show available profiles, 'hcs profile user <name>' to switch to a profile, or 'hcs profile init' to create one."
             )
 
     return data
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/cli_options.py` & `hcs_core-0.1.236/hcs_core/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/cli_processor.py` & `hcs_core-0.1.236/hcs_core/ctxp/cli_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """
 
 import click
 import sys
 from click.core import Group
 import os.path as path
 import os
+import re
 import importlib
 import importlib.util
 from pathlib import Path
 from .util import print_output, print_error, validate_error_return, avoid_trace_for_ctrl_c
 from .extension import ensure_extension
 
 _eager_loading = os.environ.get("_CTXP_EAGER_LOAD")
@@ -80,28 +81,26 @@
         return subgroup
 
     subgroup = LazyGroup(extension=extension, name=name, help=help, mod_path=mod_path)
     current.add_command(subgroup)
     return subgroup
 
 
-import re
-
 _property_pattern = re.compile("(.*)\\s*=\\s*(.*)$")
 
 
 def _read_group_meta(mod_path: Path) -> dict:
     meta_file = mod_path.absolute().joinpath("__init__.py")
 
     ret = {"help": None, "hidden": False, "extension": None}
     if meta_file.exists():
         with open(meta_file, "r") as f:
             lines = f.readlines()
-            for l in lines:
-                m = _property_pattern.match(l)
+            for line in lines:
+                m = _property_pattern.match(line)
                 if m:
                     name = m.group(1).strip()
                     value = eval(m.group(2))
                     ret[name] = value
     return ret
 
 
@@ -150,17 +149,17 @@
 
 def _process_result(result, **kwargs):
     if result is None:
         return
     if isinstance(result, tuple):
         data, return_code = result
 
-        is_error = isinstance(data, Exception) or return_code != None
+        is_error = isinstance(data, Exception) or return_code is not None
         if is_error:
-            if return_code == None:
+            if return_code is None:
                 return_code = 1
             validate_error_return(data, return_code)
             if isinstance(data, Exception):
                 print_error(data)
             else:
                 print_output(data, kwargs, file=sys.stderr)
             ctx = click.get_current_context()
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/config.py` & `hcs_core-0.1.236/hcs_core/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/context.py` & `hcs_core-0.1.236/hcs_core/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/data_util.py` & `hcs_core-0.1.236/hcs_core/ctxp/data_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import yaml
 import re
 from .util import CtxpException
 
 
 def load_data(file_name: str, class_type: str):
     data = load_data_file(file_name)
-    if data == None:
+    if data is None:
         return
     return strict_dict_to_class(data, class_type)
 
 
 def load_data_file(file, default=None, format="auto"):
 
     if isinstance(file, TextIOWrapper):
@@ -23,34 +23,34 @@
         if format == "json":
             data = json.loads(text)
         elif format == "yaml" or format == "yml":
             data = yaml.safe_load(text)
         else:
             try:
                 data = yaml.safe_load(text)
-            except:
+            except Exception:
                 data = json.loads(text)
-        return default if data == None else data
+        return default if data is None else data
     else:
         if not path.exists(file) or not path.isfile(file):
             return default
         with open(file, encoding="utf-8") as f:
             text = f.read()
 
         _, ext = path.splitext(file)
         if ext == ".json" or format == "json":
             if format != "auto" and format != "json":
                 raise CtxpException(f"File extension does not match specified format. File={file}, format={format}")
             data = json.loads(text)
-            return default if data == None else data  # handle empty file
+            return default if data is None else data  # handle empty file
         if ext == ".yaml" or ext == ".yml" or format == "yml" or format == "yaml":
             if format != "auto" and format != "yaml" and format != "yml":
                 raise CtxpException(f"File extension does not match specified format. File={file}, format={format}")
             data = yaml.safe_load(text)
-            return default if data == None else data  # handle empty file
+            return default if data is None else data  # handle empty file
     return text
 
 
 def save_data_file(data, file_name: str, format: str = "yaml", file_mod: int = 0):
     with open(file_name, "w") as file:
         if format == "yaml":
             # TODO
@@ -167,15 +167,15 @@
     name, array_index = _parse_array_property_name(k)
 
     if isinstance(o, dict):
         ret = o[name]
     else:
         ret = getattr(o, name)
 
-    if array_index != None:
+    if array_index is not None:
         ret = ret[array_index]
 
     return ret
 
 
 def _set_obj_attr(o, k, v):
     name, array_index = _parse_array_property_name(k)
@@ -229,20 +229,20 @@
                     collector.add(i)
 
     deep_iterate(obj, fn_on_value)
     return collector
 
 
 def process_variables(obj: dict, fn_get_var=None, use_env: bool = True):
-    if fn_get_var == None:
+    if fn_get_var is None:
 
         def _fn_get_var(name):
             try:
                 return deep_get_attr(obj, name), True
-            except:
+            except Exception:
                 return None, False
 
         fn_get_var = _fn_get_var
 
     if use_env:
         import os
 
@@ -322,15 +322,15 @@
         if not mapped_value.startswith(tmp_var_name + "."):
             raise CtxpException(
                 f"Unsupported expression. attr_path={referencing_attr_path}, src_var_name={src_var_name}"
             )
         new_attr_path = mapped_value[len(tmp_var_name) + 1 :]
         ret = []
         for i in target_value:
-            if i == None:
+            if i is None:
                 # raise CtxpException(f"Invalid value encountered during processing array expansion expression. The value in the referenced array is None. This is normally a problem of the data, not the caller. attr_path={referencing_attr_path}, src_var_name={src_var_name}")
                 # There are valid cases that some of such items are null. Raising exception
                 # makes the handling hard. Pass-on null in such scenario, so enable the downstream
                 # components to decide what to do with the null case.
                 item = None
             else:
                 item = deep_get_attr(i, new_attr_path)
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/duration.py` & `hcs_core-0.1.236/hcs_core/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/extension.py` & `hcs_core-0.1.236/hcs_core/ctxp/extension.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/fstore.py` & `hcs_core-0.1.236/hcs_core/ctxp/fstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     def get(self, key: str, reload: bool = False, format: str = "auto", default=None) -> dotdict:
         _validate_key(key)
         if self._path and (reload or key not in self._cache):
             file_path = self._get_path(key)
             log.debug(f"Read {file_path}")
             data = _load_file(file_path, format)
-            if data != None:
+            if data is not None:
                 self._cache[key] = data
         else:
             data = self._cache.get(key)
 
         if data is None and default is not None:
             return jsondot.dotify(default)
         return data
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/jsondot.py` & `hcs_core-0.1.236/hcs_core/ctxp/jsondot.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,43 +9,44 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import json
+import os.path
+import copy
+import time
+import random
+import portalocker
+from typing import Any
+
+
 """
 jsondot is utility to make json/dict object accessible in the "." way.
 
 ##########
 #Example 1: load, update, and save JSON file
 ##########
 
 data = jsondot.load('path/to/my.json')
 print(data.hello.message)
 data.hello.message = 'Hello, mortal.'
 jsondot.save(data, 'path/to/my.json')
-	
+
 
 ##########
 #Example 2: decorate an existing python dict
 ##########
 
 my_dict = jsondot.dotify(my_dict)
 print(my_dict.key1.key2)
 """
 
-import json
-import os.path
-import copy
-import time
-import random
-import portalocker
-from typing import Any
-
 
 class dotdict(dict):
     """dot.notation access to dictionary attributes"""
 
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/logger.py` & `hcs_core-0.1.236/hcs_core/ctxp/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def __init__(self, color, mask, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.color = color
         self.mask = mask
 
     def format(self, record, *args, **kwargs):
-        if self.color == True and record.levelno in self.COLOR_CODES:
+        if self.color is True and record.levelno in self.COLOR_CODES:
             record.color_on = self.COLOR_CODES[record.levelno]
             record.color_off = self.RESET_CODE
         else:
             record.color_on = ""
             record.color_off = ""
 
         record.name = _shorten_package_name(record.name, 16)
@@ -178,15 +178,15 @@
         logfile_handler = RotatingFileHandler(logfile_file, maxBytes=logfile_max_bytes, backupCount=logfile_max_count)
     except Exception as exception:
         print("Failed to set up log file: %s" % str(exception))
         raise
 
     try:
         logfile_handler.setLevel(logfile_log_level.upper())
-    except:
+    except Exception:
         print("Failed to set log file log level: invalid level: '%s'" % logfile_log_level)
         raise
 
     logfile_formatter = LogFormatter(fmt=log_line_template, color=logfile_log_color, mask=logfile_log_mask)
     logfile_handler.setFormatter(logfile_formatter)
     logger.addHandler(logfile_handler)
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/profile.py` & `hcs_core-0.1.236/hcs_core/ctxp/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             data["csp"] = csp_config
     return data
 
 
 def save():
     """Save the current profile"""
     global _data
-    if _data != None:
+    if _data is not None:
         save_data_file(_data, file(name()), "yaml", 0o600)
 
 
 def name() -> str:
     """Get the current active profile name"""
     global _active_profile_name
     if not _active_profile_name:
@@ -140,23 +140,23 @@
     shutil.rmtree(os.path.join(_repo_path, profile_name), ignore_errors=True)
 
 
 def get(profile_name: str, reload: bool = False, default=None) -> dotdict:
     """Get profile data by name"""
     if profile_name == name():
         global _data
-        if _data != None and not reload:
+        if _data is not None and not reload:
             return _data
         data = load_data_file(file(profile_name), default=default)
-        if data != None:
+        if data is not None:
             data = dotify(data)
             _data = data
     else:
         data = load_data_file(file(profile_name), default=default)
-        if data != None:
+        if data is not None:
             data = dotify(data)
     return data
 
 
 def file(profile_name: str) -> str:
     """Get the file path of a profile"""
     return os.path.join(_repo_path, profile_name, "profile.yml")
@@ -172,15 +172,15 @@
     @staticmethod
     def _file_name() -> str:
         return os.path.join(_repo_path, name(), ".auth")
 
     @staticmethod
     def get() -> dict:
         global _auth_cache
-        if _auth_cache == None:
+        if _auth_cache is None:
             _auth_cache = load_data_file(auth._file_name(), {}, "yaml")
         return dotify(deepcopy(_auth_cache))
 
     @staticmethod
     def set(data: dict) -> None:
         global _auth_cache
         import json
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/profile_store.py` & `hcs_core-0.1.236/hcs_core/ctxp/profile_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     if profile_name != _active_profile_name:
         # profile changed
         _active_profile_name = profile_name
         _store_map = {}
 
     ret = _store_map.get(store_name)
-    if ret == None:
+    if ret is None:
         ret = _store_from_profile_name(profile_name, store_name)
         _store_map[store_name] = ret
     return ret
 
 
 def _store_from_profile_name(profile_name: str, store_name: str) -> fstore:
     profile_path = profile.path(profile_name)
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/recent.py` & `hcs_core-0.1.236/hcs_core/ctxp/recent.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/state.py` & `hcs_core-0.1.236/hcs_core/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/util.py` & `hcs_core-0.1.236/hcs_core/ctxp/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     subprocess.call(cmd, shell=True)
 
 
 def choose(prompt: str, items: list, fn_get_text: Callable = None, selected=None, select_by_default=True):
     if len(items) == 0:
         panic(prompt + " ERROR: no item available.")
 
-    if fn_get_text == None:
+    if fn_get_text is None:
         fn_get_text = lambda t: str(t)
 
     if select_by_default and len(items) == 1:
         ret = items[0]
         print(prompt + " only one item available. Select by default: " + fn_get_text(ret))
         return ret
 
@@ -192,15 +192,15 @@
         # if label in choices:
         #    raise Exception("Problem with the provided fn_get_text: generates non-unique label. Item=" + label)
         choices.append(label)
 
     # hack workaround bug of the questionary lib
     selected_key = fn_get_text(selected) if selected else None
     k = questionary.select(prompt, choices, default=selected_key, show_selected=True).ask()
-    if k == None:
+    if k is None:
         panic()
     for i in range(size):
         if k == choices[i]:
             return items[i]
     raise Exception("This is a bug and should not happen")
```

### Comparing `hcs_core-0.1.235/hcs_core/ctxp/var_template.py` & `hcs_core-0.1.236/hcs_core/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/plan/base_provider.py` & `hcs_core-0.1.236/hcs_core/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/plan/core.py` & `hcs_core-0.1.236/hcs_core/plan/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,15 +256,15 @@
             with KOP(state, res["kind"], name) as kop2:
                 kop2.id(_get_res_text(handler, res_state))
                 kop2.start(KOP.MODE.delete, handler.eta(actions.delete, res_data, res_state))
                 handler.destroy(res_data, res_state, False)
             action = actions.create
 
         new_state = None
-        if action == actions.create or action == None:
+        if action == actions.create or action is None:
             kop.start(KOP.MODE.create, handler.eta(actions.create, res_data, res_state))
             if _has_save_state(handler.deploy):
                 new_state = handler.deploy(res_data, res_state, fn_set_state)
             else:
                 new_state = handler.deploy(res_data, res_state)
             kop.id(_get_res_text(handler, new_state))
         elif action == actions.update:
@@ -466,15 +466,15 @@
                     resource_state = output[i]
 
                     def _fn_set_state(o):
                         output[i] = deepcopy(o)
 
                     resource_data = deepcopy(data)
                     resource_data[for_var_name] = v
-                    if v == None:
+                    if v is None:
                         kop_per_item.skip("No input data")
                     else:
                         _handle_resource_1(resource_data, resource_state, _fn_set_state, kop_per_item)
         else:
             # Single resource
 
             resource_state = state["output"].get(name)
```

### Comparing `hcs_core-0.1.235/hcs_core/plan/dag.py` & `hcs_core-0.1.236/hcs_core/plan/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from copy import deepcopy
 import time
 import threading
 from graphlib import TopologicalSorter
 from graphviz import Digraph
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Callable
-import atexit
 from .helper import PlanException
 from hcs_core.ctxp import data_util
 from hcs_core.util import exit
 
 
 class walker:
     next = "next"
@@ -98,15 +97,15 @@
         while open_nodes:
             n = open_nodes.pop()
             if n in dependencies:
                 continue
             dependencies.add(n)
             open_nodes |= dag.graph[n]
 
-        to_delete = set(dag.graph.keys()) - dependencies
+        to_delete = all_nodes - dependencies
         for n in to_delete:
             del dag.graph[n]
             del dag.data[n]
     else:
         # keep only the target node
         dag.data = {target_node_name: dag.data[target_node_name]}
         dag.graph = {target_node_name: set()}
@@ -185,15 +184,15 @@
     return dag
 
 
 def _handle_priority_override(blueprint, dag):
     priority_list = []
     for k, v in blueprint["runtime"].items():
         p = v.get("destroyPriority")
-        if p != None:
+        if p is not None:
             priority_list.append({"priority": p, "name": k, "data": v})
 
     if not priority_list:
         return
 
     list.sort(priority_list, key=lambda i: i["priority"])
 
@@ -206,16 +205,16 @@
     for i in priority_list:
         dependencies = [last_priority] if last_priority else []
         name = "priority/" + i["name"]
         dag.add(name, _NodeType.runtime, i["data"], dependencies)
         last_priority = name
         dag.data[i["name"]]["ghost"] = True
 
-    for l in leaves:
-        dag.graph[l].add(last_priority)
+    for leaf in leaves:
+        dag.graph[leaf].add(last_priority)
 
 
 def _get_provider_id(node_data):
     kind = node_data["kind"]
     provider_type = kind[: kind.find("/")]
     if provider_type == "runtime":
         raise PlanException("This is a regression bug. Must not be runtime here")
```

### Comparing `hcs_core-0.1.235/hcs_core/plan/helper.py` & `hcs_core-0.1.236/hcs_core/plan/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 limitations under the License.
 """
 
 import json
 import yaml
 from typing import Tuple
 import os
-from hcs_core.ctxp.data_util import load_data_file, strict_dict_to_class, process_variables
+from hcs_core.ctxp.data_util import load_data_file, process_variables
 
 
 class PlanException(Exception):
     pass
 
 
 class PluginException(Exception):
@@ -37,22 +37,22 @@
     def __init__(self):
         self.var = {}
         self.default = {}
         self.provider = {}
         self.resource = {}
 
     def __repr__(self):
-        return f"Blueprint"
+        return "Blueprint"
 
 
 def load_files(files: list[str]) -> dict:
     ret = {}
     for file in files:
         data = load_data_file(file)
-        if data == None or isinstance(data, str):
+        if data is None or isinstance(data, str):
             raise FileNotFoundError("Fail loading file: " + file)
         ret = _merge_dict_fail_on_dup(ret, _smart_load_file(file))
     return ret
 
 
 def process_template(template, use_env: bool = True) -> Tuple[dict, dict]:
     # Ensure default sections are not None
```

### Comparing `hcs_core-0.1.235/hcs_core/plan/kop.py` & `hcs_core-0.1.236/hcs_core/plan/kop.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import time
 import traceback
-import traceback
 import logging
 from hcs_core.ctxp.util import error_details
 
 log = logging.getLogger(__name__)
 
 
 class KopException(Exception):
```

### Comparing `hcs_core-0.1.235/hcs_core/plan/provider/dev/dummy.py` & `hcs_core-0.1.236/hcs_core/plan/provider/dev/dummy.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import time
 from hcs_core.util import exit
 from copy import deepcopy
 from typing import Callable
 import hcs_core.ctxp.duration as duration
 from hcs_core.plan import actions
 from hcs_core.plan import PluginException
```

### Comparing `hcs_core-0.1.235/hcs_core/plan/provider/dev/fibonacci.py` & `hcs_core-0.1.236/hcs_core/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/sglib/__init__.py` & `hcs_core-0.1.236/hcs_core/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/sglib/auth.py` & `hcs_core-0.1.236/hcs_core/sglib/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import os
 import time
 import jwt
 import json
 import hashlib
 import logging
-from hcs_core.ctxp import profile, panic, jsondot, CtxpException
+from hcs_core.ctxp import profile, panic, jsondot
 from .csp import CspClient
 from .login_support import create_oauth_client, refresh_oauth_token
 
 log = logging.getLogger(__name__)
 
 
 def _get_profile_auth_hash():
```

### Comparing `hcs_core-0.1.235/hcs_core/sglib/cli_options.py` & `hcs_core-0.1.236/hcs_core/sglib/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/sglib/client_util.py` & `hcs_core-0.1.236/hcs_core/sglib/client_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     names = []
     for r in regions:
         names.append(r.name)
     panic(f"Region not found: {region_name}. Available regions: {names}")
 
 
 def regional_service_client(region_name: str, service_name: str):
-    #'https://dev1b-westus2-cp103a.azcp.horizon.vmware.com/vmhub'
+    # 'https://dev1b-westus2-cp103a.azcp.horizon.vmware.com/vmhub'
     url = _get_region_url(region_name)
     if not url:
         panic("Missing profile property: hcs.regions")
     if not url.endswith("/"):
         url += "/"
     url += service_name
     return hcs_client(url)
@@ -136,15 +136,15 @@
     polling_interval_seconds: int = 10,
     fn_is_error: Callable = None,
 ):
     timeout_seconds = _parse_timeout(timeout)
     start = time.time()
     while True:
         t = fn_get()
-        if t == None:
+        if t is None:
             return
         if fn_is_error:
             if fn_is_error(t):
                 msg = f"Failed deleting resource '{resource_name}', resource in Error state."
                 raise CtxpException(msg)
 
         now = time.time()
@@ -202,15 +202,15 @@
         if not is_error:
             raise CtxpException("Either status_map or is_error must be specified.")
         if not is_transition:
             raise CtxpException("Either status_map or is_transition must be specified.")
 
     while True:
         t = fn_get()
-        if t == None:
+        if t is None:
             if not_found_as_success:
                 return
             raise CtxpException(prefix + "Not found.")
         status = get_status(t)
         # print(f"DDD - status {status}")
         if is_error(status):
             msg = prefix + f"Status error. Actual={status}"
```

### Comparing `hcs_core-0.1.235/hcs_core/sglib/csp.py` & `hcs_core-0.1.236/hcs_core/sglib/csp.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     response.raise_for_status()
 
 
 def _try_formatting_json(text: str):
     try:
         return json.dumps(json.loads(text), indent=4)
-    except:
+    except Exception:
         return text
 
 
 def _log_request(request):
     if not log.isEnabledFor(logging.DEBUG):
         return
     log.debug("\n")
```

### Comparing `hcs_core-0.1.235/hcs_core/sglib/ez_client.py` & `hcs_core-0.1.236/hcs_core/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/sglib/hcs_client.py` & `hcs_core-0.1.236/hcs_core/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/sglib/login_support.py` & `hcs_core-0.1.236/hcs_core/sglib/login_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import threading
 import time
 from typing import Callable
 import webbrowser
 import secrets
 import logging
+from hcs_core.util.scheduler import ThreadPoolScheduler
 from authlib.integrations.httpx_client import OAuth2Client
 from authlib.oauth2.rfc7636 import create_s256_code_challenge
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from urllib.parse import urlparse, parse_qs
 
 log = logging.getLogger(__name__)
 
@@ -44,15 +45,15 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta charset="utf-8" />
     <title>Login successfully</title>
     <style>
         body {
-            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; 
+            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
         }
 
         code {
             font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace;
             display: inline-block;
             background-color: rgb(242, 242, 242);
             padding: 12px 16px;
@@ -235,16 +236,14 @@
             _register_custom_refresher(client, oauth_token, fn_on_new_oauth_token, fn_custom_refresh)
         else:
             # not even initialized.
             pass
     return client
 
 
-from hcs_core.util.scheduler import ThreadPoolScheduler
-
 _scheduler: ThreadPoolScheduler = None
 
 
 def _register_custom_refresher(
     client: OAuth2Client, oauth_token, fn_on_new_oauth_token: Callable, fn_custom_refresh: Callable
 ):
     global _scheduler
```

### Comparing `hcs_core-0.1.235/hcs_core/sglib/payload_util.py` & `hcs_core-0.1.236/hcs_core/sglib/payload_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         text = file_arg.read()
 
     try:
         payload = json.loads(text)
     except Exception as e1:
         try:
             payload = yaml.safe_load(text)
-        except Exception as e2:
+        except Exception:
             raise CtxpException("Invalid payload: " + str(e1))
 
     # Override org id, if specified explicitly on args.
     # Otherwise override using default, if not in payload.
     if org:
         payload["orgId"] = org
     else:
```

### Comparing `hcs_core-0.1.235/hcs_core/util/check_license.py` & `hcs_core-0.1.236/hcs_core/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/util/duration.py` & `hcs_core-0.1.236/hcs_core/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/util/exit.py` & `hcs_core-0.1.236/hcs_core/util/exit.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/util/hcs_constants.py` & `hcs_core-0.1.236/hcs_core/util/hcs_constants.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/util/job_view.py` & `hcs_core-0.1.236/hcs_core/util/job_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 import threading
 from time import sleep, monotonic
 import sys
 import os
 from rich.live import Live
 from rich.progress import Progress, Task, ProgressBar, SpinnerColumn, TextColumn, TimeRemainingColumn, ProgressColumn
 from rich.table import Column
-from rich.text import Text, TextType
-from rich.style import StyleType
+from rich.text import Text
 from rich.console import RenderableType
 import hcs_core.ctxp.duration as duration
 
 
 def _shorten_package_name(package_name, max_length):
     if len(package_name) <= max_length:
         return package_name
```

### Comparing `hcs_core-0.1.235/hcs_core/util/pki_util.py` & `hcs_core-0.1.236/hcs_core/util/pki_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         f.write(chain_pems[0])
     with open("temp_chain.pem", "w") as f:
         for pem in chain_pems[1:]:
             f.write(pem)
             f.write("\n")
     cmd = "openssl verify -verbose -CAfile temp_chain.pem temp_leaf.pem"
 
-    proc = subprocess.run(cmd, shell=True, check=True, capture_output=False)
+    subprocess.run(cmd, shell=True, check=True, capture_output=False)
 
     os.unlink("temp_leaf.pem")
     os.unlink("temp_chain.pem")
 
 
 # Generate pkey
 def generate_key(type=crypto.TYPE_RSA, bits: int = 4096):
```

### Comparing `hcs_core-0.1.235/hcs_core/util/query_util.py` & `hcs_core-0.1.236/hcs_core/util/query_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import Any, Callable
 
 
 def _remove_none(obj: dict):
     keys = list(obj.keys())
     for k in keys:
         v = obj[k]
-        if v == None:
+        if v is None:
             del obj[k]
     return obj
 
 
 def with_query(url: str, **kwargs: Any) -> str:
     qs = urlencode(_remove_none(dict(kwargs)))
     if qs:
```

### Comparing `hcs_core-0.1.235/hcs_core/util/scheduler.py` & `hcs_core-0.1.236/hcs_core/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/util/ssl_util.py` & `hcs_core-0.1.236/hcs_core/util/ssl_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core/util/versions.py` & `hcs_core-0.1.236/hcs_core/util/versions.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/hcs_core.egg-info/PKG-INFO` & `hcs_core-0.1.236/hcs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.235
+Version: 0.1.236
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs_core-0.1.235/hcs_core.egg-info/SOURCES.txt` & `hcs_core-0.1.236/hcs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/pyproject.toml` & `hcs_core-0.1.236/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.235/setup.py` & `hcs_core-0.1.236/setup.py`

 * *Files identical despite different names*

