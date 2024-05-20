# Comparing `tmp/hcs_core-0.1.234.tar.gz` & `tmp/hcs_core-0.1.235.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs_core-0.1.234.tar", last modified: Mon May 20 14:34:45 2024, max compression
+gzip compressed data, was "hcs_core-0.1.235.tar", last modified: Mon May 20 22:38:06 2024, max compression
```

## Comparing `hcs_core-0.1.234.tar` & `hcs_core-0.1.235.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.089896 hcs_core-0.1.234/
--rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 14:34:45.089411 hcs_core-0.1.234/PKG-INFO
--rw-r--r--   0 nanw       (503) staff       (20)       25 2024-05-14 18:28:08.000000 hcs_core-0.1.234/README.md
--rw-r--r--   0 nanw       (503) staff       (20)        7 2024-05-20 14:34:42.000000 hcs_core-0.1.234/VERSION
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.038888 hcs_core-0.1.234/hcs_core/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/__init__.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.055759 hcs_core-0.1.234/hcs_core/ctxp/
--rw-r--r--   0 nanw       (503) staff       (20)      790 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/_init.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.058927 hcs_core-0.1.234/hcs_core/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     3086 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (503) staff       (20)     2387 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (503) staff       (20)     4034 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (503) staff       (20)     2274 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/cli_options.py
--rw-r--r--   0 nanw       (503) staff       (20)     5791 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (503) staff       (20)      936 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/config.py
--rw-r--r--   0 nanw       (503) staff       (20)     1160 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/context.py
--rw-r--r--   0 nanw       (503) staff       (20)    14088 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/data_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     2856 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/duration.py
--rw-r--r--   0 nanw       (503) staff       (20)     1623 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/extension.py
--rw-r--r--   0 nanw       (503) staff       (20)     6801 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/fstore.py
--rw-r--r--   0 nanw       (503) staff       (20)     1200 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/init.py
--rw-r--r--   0 nanw       (503) staff       (20)     4666 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/jsondot.py
--rw-r--r--   0 nanw       (503) staff       (20)     6346 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/logger.py
--rw-r--r--   0 nanw       (503) staff       (20)     6586 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/profile.py
--rw-r--r--   0 nanw       (503) staff       (20)     1565 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/profile_store.py
--rw-r--r--   0 nanw       (503) staff       (20)     1767 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/recent.py
--rw-r--r--   0 nanw       (503) staff       (20)     1619 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/state.py
--rw-r--r--   0 nanw       (503) staff       (20)     8036 2024-05-14 21:19:34.000000 hcs_core-0.1.234/hcs_core/ctxp/util.py
--rw-r--r--   0 nanw       (503) staff       (20)     3245 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.069169 hcs_core-0.1.234/hcs_core/plan/
--rw-r--r--   0 nanw       (503) staff       (20)      203 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)      125 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/actions.py
--rw-r--r--   0 nanw       (503) staff       (20)     1298 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/base_provider.py
--rw-r--r--   0 nanw       (503) staff       (20)      116 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/context.py
--rw-r--r--   0 nanw       (503) staff       (20)    20957 2024-05-17 23:12:51.000000 hcs_core-0.1.234/hcs_core/plan/core.py
--rw-r--r--   0 nanw       (503) staff       (20)    12918 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/dag.py
--rw-r--r--   0 nanw       (503) staff       (20)     7784 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/helper.py
--rw-r--r--   0 nanw       (503) staff       (20)     5363 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/kop.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.069829 hcs_core-0.1.234/hcs_core/plan/provider/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.073121 hcs_core-0.1.234/hcs_core/plan/provider/dev/
--rw-r--r--   0 nanw       (503) staff       (20)       30 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)       34 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (503) staff       (20)     1994 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (503) staff       (20)     1104 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.081654 hcs_core-0.1.234/hcs_core/sglib/
--rw-r--r--   0 nanw       (503) staff       (20)      654 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     5194 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/auth.py
--rw-r--r--   0 nanw       (503) staff       (20)     1790 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/cli_options.py
--rw-r--r--   0 nanw       (503) staff       (20)     8378 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/client_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     8043 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/csp.py
--rw-r--r--   0 nanw       (503) staff       (20)     5167 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/ez_client.py
--rw-r--r--   0 nanw       (503) staff       (20)      901 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/hcs_client.py
--rw-r--r--   0 nanw       (503) staff       (20)    10128 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/login_support.py
--rw-r--r--   0 nanw       (503) staff       (20)      684 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/sglib/payload_util.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.087877 hcs_core-0.1.234/hcs_core/util/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/__init__.py
--rwxr-xr-x   0 nanw       (503) staff       (20)     2535 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/check_license.py
--rw-r--r--   0 nanw       (503) staff       (20)     3482 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/duration.py
--rw-r--r--   0 nanw       (503) staff       (20)      838 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/exit.py
--rw-r--r--   0 nanw       (503) staff       (20)     1755 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/hcs_constants.py
--rw-r--r--   0 nanw       (503) staff       (20)     8438 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/job_view.py
--rw-r--r--   0 nanw       (503) staff       (20)     5288 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/pki_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     1946 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/query_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     2958 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/scheduler.py
--rw-r--r--   0 nanw       (503) staff       (20)     1239 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/ssl_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     1727 2024-05-14 18:28:08.000000 hcs_core-0.1.234/hcs_core/util/versions.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 14:34:45.088569 hcs_core-0.1.234/hcs_core.egg-info/
--rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 14:34:44.000000 hcs_core-0.1.234/hcs_core.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (503) staff       (20)     1810 2024-05-20 14:34:45.000000 hcs_core-0.1.234/hcs_core.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (503) staff       (20)        1 2024-05-20 14:34:44.000000 hcs_core-0.1.234/hcs_core.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-20 14:34:44.000000 hcs_core-0.1.234/hcs_core.egg-info/requires.txt
--rw-r--r--   0 nanw       (503) staff       (20)        9 2024-05-20 14:34:44.000000 hcs_core-0.1.234/hcs_core.egg-info/top_level.txt
--rw-r--r--   0 nanw       (503) staff       (20)     1250 2024-05-14 18:28:08.000000 hcs_core-0.1.234/pyproject.toml
--rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:28:08.000000 hcs_core-0.1.234/requirements.txt
--rw-r--r--   0 nanw       (503) staff       (20)       38 2024-05-20 14:34:45.089961 hcs_core-0.1.234/setup.cfg
--rw-r--r--   0 nanw       (503) staff       (20)      808 2024-05-14 18:28:08.000000 hcs_core-0.1.234/setup.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.107575 hcs_core-0.1.235/
+-rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 22:38:06.106920 hcs_core-0.1.235/PKG-INFO
+-rw-r--r--   0 nanw       (503) staff       (20)       25 2024-05-14 18:28:08.000000 hcs_core-0.1.235/README.md
+-rw-r--r--   0 nanw       (503) staff       (20)        7 2024-05-20 22:38:02.000000 hcs_core-0.1.235/VERSION
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.066045 hcs_core-0.1.235/hcs_core/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/__init__.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.077944 hcs_core-0.1.235/hcs_core/ctxp/
+-rw-r--r--   0 nanw       (503) staff       (20)      790 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 22:21:06.000000 hcs_core-0.1.235/hcs_core/ctxp/_init.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.082558 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3086 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2387 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)     4034 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2274 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5791 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (503) staff       (20)      931 2024-05-20 15:58:31.000000 hcs_core-0.1.235/hcs_core/ctxp/config.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 16:01:06.000000 hcs_core-0.1.235/hcs_core/ctxp/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)    14068 2024-05-20 15:59:29.000000 hcs_core-0.1.235/hcs_core/ctxp/data_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2856 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/duration.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1658 2024-05-20 22:32:30.000000 hcs_core-0.1.235/hcs_core/ctxp/extension.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6801 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/fstore.py
+-rw-r--r--   0 nanw       (503) staff       (20)     4666 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6310 2024-05-20 22:36:14.000000 hcs_core-0.1.235/hcs_core/ctxp/logger.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6586 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/profile.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1565 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1767 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/recent.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1619 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/ctxp/state.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8036 2024-05-14 21:19:34.000000 hcs_core-0.1.235/hcs_core/ctxp/util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3244 2024-05-20 16:02:07.000000 hcs_core-0.1.235/hcs_core/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.087013 hcs_core-0.1.235/hcs_core/plan/
+-rw-r--r--   0 nanw       (503) staff       (20)      203 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)      125 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/actions.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1298 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/base_provider.py
+-rw-r--r--   0 nanw       (503) staff       (20)      116 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)    20957 2024-05-17 23:12:51.000000 hcs_core-0.1.235/hcs_core/plan/core.py
+-rw-r--r--   0 nanw       (503) staff       (20)    12966 2024-05-20 22:31:51.000000 hcs_core-0.1.235/hcs_core/plan/dag.py
+-rw-r--r--   0 nanw       (503) staff       (20)     7784 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/helper.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5471 2024-05-20 22:19:59.000000 hcs_core-0.1.235/hcs_core/plan/kop.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.087671 hcs_core-0.1.235/hcs_core/plan/provider/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.089447 hcs_core-0.1.235/hcs_core/plan/provider/dev/
+-rw-r--r--   0 nanw       (503) staff       (20)       30 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)       34 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1994 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1104 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.096287 hcs_core-0.1.235/hcs_core/sglib/
+-rw-r--r--   0 nanw       (503) staff       (20)      654 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5194 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/auth.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1796 2024-05-20 16:06:32.000000 hcs_core-0.1.235/hcs_core/sglib/cli_options.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8378 2024-05-20 22:12:17.000000 hcs_core-0.1.235/hcs_core/sglib/client_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8043 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/csp.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5167 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/ez_client.py
+-rw-r--r--   0 nanw       (503) staff       (20)      901 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (503) staff       (20)    10130 2024-05-20 16:05:14.000000 hcs_core-0.1.235/hcs_core/sglib/login_support.py
+-rw-r--r--   0 nanw       (503) staff       (20)      689 2024-05-20 16:05:58.000000 hcs_core-0.1.235/hcs_core/sglib/payload_util.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.104814 hcs_core-0.1.235/hcs_core/util/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/__init__.py
+-rwxr-xr-x   0 nanw       (503) staff       (20)     2535 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/check_license.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3482 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/duration.py
+-rw-r--r--   0 nanw       (503) staff       (20)      838 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/exit.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1755 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/hcs_constants.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8438 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/job_view.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5288 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/pki_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1946 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/query_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2958 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/scheduler.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1239 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/ssl_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1727 2024-05-14 18:28:08.000000 hcs_core-0.1.235/hcs_core/util/versions.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 22:38:06.106246 hcs_core-0.1.235/hcs_core.egg-info/
+-rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (503) staff       (20)     1788 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (503) staff       (20)        1 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/requires.txt
+-rw-r--r--   0 nanw       (503) staff       (20)        9 2024-05-20 22:38:06.000000 hcs_core-0.1.235/hcs_core.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (503) staff       (20)     1250 2024-05-14 18:28:08.000000 hcs_core-0.1.235/pyproject.toml
+-rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:28:08.000000 hcs_core-0.1.235/requirements.txt
+-rw-r--r--   0 nanw       (503) staff       (20)       38 2024-05-20 22:38:06.107649 hcs_core-0.1.235/setup.cfg
+-rw-r--r--   0 nanw       (503) staff       (20)      808 2024-05-14 18:28:08.000000 hcs_core-0.1.235/setup.py
```

### Comparing `hcs_core-0.1.234/PKG-INFO` & `hcs_core-0.1.235/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.234
+Version: 0.1.235
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/__init__.py` & `hcs_core-0.1.235/hcs_core/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/_init.py` & `hcs_core-0.1.235/hcs_core/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/built_in_cmds/_ut.py` & `hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/built_in_cmds/context.py` & `hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/built_in_cmds/profile.py` & `hcs_core-0.1.235/hcs_core/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/cli_options.py` & `hcs_core-0.1.235/hcs_core/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/cli_processor.py` & `hcs_core-0.1.235/hcs_core/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/config.py` & `hcs_core-0.1.235/hcs_core/ctxp/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     _store_impl = fstore(config_path)
 
 
 def get(name: str, reload: bool = False) -> dotdict:
     return _store_impl.get(name, reload)
 
 
-def list() -> list[str]:
+def list() -> list:
     return _store_impl.keys()
```

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/context.py` & `hcs_core-0.1.235/hcs_core/ctxp/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .profile_store import profile_store, fstore
 
 
 def _store() -> fstore:
     return profile_store("context")
 
 
-def list() -> list[str]:
+def list() -> list:
     return _store().keys()
 
 
 def get(name: str, reload: bool = False, default=None) -> dotdict:
     return _store().get(key=name, reload=reload, default=default)
```

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/data_util.py` & `hcs_core-0.1.235/hcs_core/ctxp/data_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         obj[path] = value
         return obj
 
     k = None
     try:
         for i in range(len(parts)):
             k = parts[i]
-            obj = _get_obj_attr(obj, k, raise_on_not_found)
+            obj = _get_obj_attr(obj, k)
 
             if i == len(parts) - 2:
                 # found the one before the leaf.
                 _set_obj_attr(obj, parts[i + 1], value)
                 break
         return obj
     except (KeyError, TypeError, IndexError) as e:
```

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/duration.py` & `hcs_core-0.1.235/hcs_core/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/extension.py` & `hcs_core-0.1.235/hcs_core/ctxp/extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import subprocess
 from importlib import reload, import_module
 import pkg_resources
 from .util import CtxpException
 
 
 def ensure_extension(required: str, parent_module_name: str = None):
-    installed = {pkg.key for pkg in pkg_resources.working_set}
+    installed = {pkg.key for pkg in pkg_resources.working_set}  # pylint: disable=not-an-iterable
     if required in installed:
         return
 
     msg = f"This command requires an extension: {required}. Install now?"
     click.confirm(click.style(msg, fg="yellow"), default=True, abort=True)
 
     cmd = f"pip install {required}"
```

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/fstore.py` & `hcs_core-0.1.235/hcs_core/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/jsondot.py` & `hcs_core-0.1.235/hcs_core/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/logger.py` & `hcs_core-0.1.235/hcs_core/ctxp/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         logging.INFO: "\033[0;37m",
         logging.DEBUG: "\033[1;30m",
     }
 
     RESET_CODE = "\033[0m"
 
     def __init__(self, color, mask, *args, **kwargs):
-        super(LogFormatter, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.color = color
         self.mask = mask
 
     def format(self, record, *args, **kwargs):
         if self.color == True and record.levelno in self.COLOR_CODES:
             record.color_on = self.COLOR_CODES[record.levelno]
             record.color_off = self.RESET_CODE
@@ -57,15 +57,15 @@
 
         msg = super(LogFormatter, self).format(record, *args, **kwargs)
         return mask_password(msg) if self.mask else msg
 
 
 class LogFormatterFixedNameWidth(logging.Formatter):
     def __init__(self, *args, **kwargs):
-        super(LogFormatter, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def format(self, record, *args, **kwargs):
         record.name = _shorten_package_name(record.name, 16)
         return super(LogFormatterFixedNameWidth, self).format(record, *args, **kwargs)
 
 
 def _shorten_package_name(package_name, max_length):
```

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/profile.py` & `hcs_core-0.1.235/hcs_core/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/profile_store.py` & `hcs_core-0.1.235/hcs_core/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/recent.py` & `hcs_core-0.1.235/hcs_core/ctxp/recent.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/state.py` & `hcs_core-0.1.235/hcs_core/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/util.py` & `hcs_core-0.1.235/hcs_core/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/ctxp/var_template.py` & `hcs_core-0.1.235/hcs_core/ctxp/var_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def _vars() -> dotdict:
     global _variables
     _variables = context.get(".variables")
     return _variables
 
 
 def _save():
-    context.save(".variables", _variables)
+    context.set(".variables", _variables)
 
 
 def set(name: str, value: Any):
     variables = _vars()
     if name in variables:
         existing = variables.get(name)
         if existing == value:
```

### Comparing `hcs_core-0.1.234/hcs_core/plan/base_provider.py` & `hcs_core-0.1.235/hcs_core/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/plan/core.py` & `hcs_core-0.1.235/hcs_core/plan/core.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/plan/dag.py` & `hcs_core-0.1.235/hcs_core/plan/dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,16 +301,17 @@
         exit.set()
         raise e
     except Exception as e:
         flag_stop.set()
         raise e
     finally:
         executor.shutdown(wait=False)
-        if flags["err"]:
-            raise flags["err"]
+        ex = flags["err"]
+        if ex:
+            raise ex  # pylint: disable=raising-bad-type
 
 
 def _has_indirect_dependency(tree: dict, from_node: str, to_node: str):
     deps = list(tree[from_node])
     deps.remove(to_node)
     while deps:
         n = deps.pop()
@@ -390,15 +391,15 @@
                 # This is an external dependency and not part of our node
                 pass
 
 
 def _test(reverse):
     print("reverse=", reverse)
     dag = DAG()
-    dag.add("a", "a")
+    dag.add("a", "a", None)
     dag.add("b1", "b1", {"a"})
     dag.add("b2", "b2", {"a"})
     dag.add("c", "c", {"b1"})
     dag.add("d", "d", {"b2", "c"})
 
     if reverse:
         _reverse_dag(dag)
```

### Comparing `hcs_core-0.1.234/hcs_core/plan/helper.py` & `hcs_core-0.1.235/hcs_core/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/plan/kop.py` & `hcs_core-0.1.235/hcs_core/plan/kop.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,29 +36,35 @@
     start = "start"
     success = "success"
     error = "error"
     skip = "skip"
 
 
 class _DummyJobView:
+    @staticmethod
     def add(id, name):
         pass
 
+    @staticmethod
     def update(id, text: str):
         pass
 
+    @staticmethod
     def start(id, eta: str):
         pass
 
+    @staticmethod
     def success(id):
         pass
 
+    @staticmethod
     def skip(id, reason):
         pass
 
+    @staticmethod
     def error(id, err):
         pass
 
 
 _job_view = _DummyJobView
```

### Comparing `hcs_core-0.1.234/hcs_core/plan/provider/dev/dummy.py` & `hcs_core-0.1.235/hcs_core/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/plan/provider/dev/fibonacci.py` & `hcs_core-0.1.235/hcs_core/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/sglib/__init__.py` & `hcs_core-0.1.235/hcs_core/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/sglib/auth.py` & `hcs_core-0.1.235/hcs_core/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/sglib/cli_options.py` & `hcs_core-0.1.235/hcs_core/sglib/cli_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
             # 4th priority: org from the current auth token
             from hcs_core.sglib import auth
 
             auth_info = auth.details(False)
             if not auth_info:
                 raise CtxpException("Not authorized. See 'hcs login --help'.")
-            org = auth_info.org.id
+            org = auth_info["org"]["id"]
             return org
         finally:
             if org:
                 r.set(org)
 
 
 def ensure_login():
```

### Comparing `hcs_core-0.1.234/hcs_core/sglib/client_util.py` & `hcs_core-0.1.235/hcs_core/sglib/client_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/sglib/csp.py` & `hcs_core-0.1.235/hcs_core/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/sglib/ez_client.py` & `hcs_core-0.1.235/hcs_core/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/sglib/hcs_client.py` & `hcs_core-0.1.235/hcs_core/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/sglib/login_support.py` & `hcs_core-0.1.235/hcs_core/sglib/login_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 state = states[0]
                 if _state != state:
                     _respond(401, "Response state mismatch")
                     return
 
                 code = codes[0]
                 # Process the authorization code
-                log.debug("auth code", code)
+                log.debug(f"auth code {code}")
                 _auth_code_event.value = code
 
                 # Send a response back to the client
                 _respond(200, _auth_success_html, "text/html")
             else:
                 _respond(404, "Not found")
         finally:
```

### Comparing `hcs_core-0.1.234/hcs_core/sglib/payload_util.py` & `hcs_core-0.1.235/hcs_core/sglib/payload_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with file_arg:
         text = file_arg.read()
 
     try:
         payload = json.loads(text)
     except Exception as e1:
         try:
-            payload = yaml.load(text)
+            payload = yaml.safe_load(text)
         except Exception as e2:
             raise CtxpException("Invalid payload: " + str(e1))
 
     # Override org id, if specified explicitly on args.
     # Otherwise override using default, if not in payload.
     if org:
         payload["orgId"] = org
```

### Comparing `hcs_core-0.1.234/hcs_core/util/check_license.py` & `hcs_core-0.1.235/hcs_core/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/duration.py` & `hcs_core-0.1.235/hcs_core/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/exit.py` & `hcs_core-0.1.235/hcs_core/util/exit.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/hcs_constants.py` & `hcs_core-0.1.235/hcs_core/util/hcs_constants.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/job_view.py` & `hcs_core-0.1.235/hcs_core/util/job_view.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/pki_util.py` & `hcs_core-0.1.235/hcs_core/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/query_util.py` & `hcs_core-0.1.235/hcs_core/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/scheduler.py` & `hcs_core-0.1.235/hcs_core/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/ssl_util.py` & `hcs_core-0.1.235/hcs_core/util/ssl_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core/util/versions.py` & `hcs_core-0.1.235/hcs_core/util/versions.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/hcs_core.egg-info/PKG-INFO` & `hcs_core-0.1.235/hcs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.234
+Version: 0.1.235
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs_core-0.1.234/hcs_core.egg-info/SOURCES.txt` & `hcs_core-0.1.235/hcs_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 hcs_core/ctxp/cli_processor.py
 hcs_core/ctxp/config.py
 hcs_core/ctxp/context.py
 hcs_core/ctxp/data_util.py
 hcs_core/ctxp/duration.py
 hcs_core/ctxp/extension.py
 hcs_core/ctxp/fstore.py
-hcs_core/ctxp/init.py
 hcs_core/ctxp/jsondot.py
 hcs_core/ctxp/logger.py
 hcs_core/ctxp/profile.py
 hcs_core/ctxp/profile_store.py
 hcs_core/ctxp/recent.py
 hcs_core/ctxp/state.py
 hcs_core/ctxp/util.py
```

### Comparing `hcs_core-0.1.234/pyproject.toml` & `hcs_core-0.1.235/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.234/setup.py` & `hcs_core-0.1.235/setup.py`

 * *Files identical despite different names*

