# Comparing `tmp/hcs_core-0.1.236.tar.gz` & `tmp/hcs_core-0.1.237.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs_core-0.1.236.tar", last modified: Mon May 20 23:16:32 2024, max compression
+gzip compressed data, was "hcs_core-0.1.237.tar", last modified: Tue May 21 00:26:06 2024, max compression
```

## Comparing `hcs_core-0.1.236.tar` & `hcs_core-0.1.237.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.302274 hcs_core-0.1.236/
--rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 23:16:32.301372 hcs_core-0.1.236/PKG-INFO
--rw-r--r--   0 nanw       (503) staff       (20)       25 2024-05-14 18:28:08.000000 hcs_core-0.1.236/README.md
--rw-r--r--   0 nanw       (503) staff       (20)        7 2024-05-20 23:16:30.000000 hcs_core-0.1.236/VERSION
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.262908 hcs_core-0.1.236/hcs_core/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/__init__.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.275205 hcs_core-0.1.236/hcs_core/ctxp/
--rw-r--r--   0 nanw       (503) staff       (20)      790 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 22:21:06.000000 hcs_core-0.1.236/hcs_core/ctxp/_init.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.278956 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     3086 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (503) staff       (20)     2388 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (503) staff       (20)     4034 2024-05-20 22:44:20.000000 hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (503) staff       (20)     2274 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/cli_options.py
--rw-r--r--   0 nanw       (503) staff       (20)     5800 2024-05-20 23:02:06.000000 hcs_core-0.1.236/hcs_core/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (503) staff       (20)      931 2024-05-20 15:58:31.000000 hcs_core-0.1.236/hcs_core/ctxp/config.py
--rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 16:01:06.000000 hcs_core-0.1.236/hcs_core/ctxp/context.py
--rw-r--r--   0 nanw       (503) staff       (20)    14092 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/ctxp/data_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     2856 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/duration.py
--rw-r--r--   0 nanw       (503) staff       (20)     1658 2024-05-20 22:32:30.000000 hcs_core-0.1.236/hcs_core/ctxp/extension.py
--rw-r--r--   0 nanw       (503) staff       (20)     6805 2024-05-20 22:48:34.000000 hcs_core-0.1.236/hcs_core/ctxp/fstore.py
--rw-r--r--   0 nanw       (503) staff       (20)     4666 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/ctxp/jsondot.py
--rw-r--r--   0 nanw       (503) staff       (20)     6320 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/ctxp/logger.py
--rw-r--r--   0 nanw       (503) staff       (20)     6602 2024-05-20 23:02:31.000000 hcs_core-0.1.236/hcs_core/ctxp/profile.py
--rw-r--r--   0 nanw       (503) staff       (20)     1565 2024-05-20 22:51:09.000000 hcs_core-0.1.236/hcs_core/ctxp/profile_store.py
--rw-r--r--   0 nanw       (503) staff       (20)     1767 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/recent.py
--rw-r--r--   0 nanw       (503) staff       (20)     1619 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/ctxp/state.py
--rw-r--r--   0 nanw       (503) staff       (20)     8036 2024-05-20 22:52:07.000000 hcs_core-0.1.236/hcs_core/ctxp/util.py
--rw-r--r--   0 nanw       (503) staff       (20)     3244 2024-05-20 16:02:07.000000 hcs_core-0.1.236/hcs_core/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.283033 hcs_core-0.1.236/hcs_core/plan/
--rw-r--r--   0 nanw       (503) staff       (20)      203 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)      125 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/actions.py
--rw-r--r--   0 nanw       (503) staff       (20)     1298 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/base_provider.py
--rw-r--r--   0 nanw       (503) staff       (20)      116 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/context.py
--rw-r--r--   0 nanw       (503) staff       (20)    20957 2024-05-20 22:52:58.000000 hcs_core-0.1.236/hcs_core/plan/core.py
--rw-r--r--   0 nanw       (503) staff       (20)    12950 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/plan/dag.py
--rw-r--r--   0 nanw       (503) staff       (20)     7761 2024-05-20 22:55:21.000000 hcs_core-0.1.236/hcs_core/plan/helper.py
--rw-r--r--   0 nanw       (503) staff       (20)     5454 2024-05-20 22:55:35.000000 hcs_core-0.1.236/hcs_core/plan/kop.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.283569 hcs_core-0.1.236/hcs_core/plan/provider/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.285652 hcs_core-0.1.236/hcs_core/plan/provider/dev/
--rw-r--r--   0 nanw       (503) staff       (20)       30 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)       34 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (503) staff       (20)     1982 2024-05-20 22:55:55.000000 hcs_core-0.1.236/hcs_core/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (503) staff       (20)     1104 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.289589 hcs_core-0.1.236/hcs_core/sglib/
--rw-r--r--   0 nanw       (503) staff       (20)      654 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/sglib/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     5169 2024-05-20 22:56:14.000000 hcs_core-0.1.236/hcs_core/sglib/auth.py
--rw-r--r--   0 nanw       (503) staff       (20)     1796 2024-05-20 16:06:32.000000 hcs_core-0.1.236/hcs_core/sglib/cli_options.py
--rw-r--r--   0 nanw       (503) staff       (20)     8379 2024-05-20 22:57:08.000000 hcs_core-0.1.236/hcs_core/sglib/client_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     8053 2024-05-20 22:57:40.000000 hcs_core-0.1.236/hcs_core/sglib/csp.py
--rw-r--r--   0 nanw       (503) staff       (20)     5167 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/sglib/ez_client.py
--rw-r--r--   0 nanw       (503) staff       (20)      901 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/sglib/hcs_client.py
--rw-r--r--   0 nanw       (503) staff       (20)    10128 2024-05-20 23:01:41.000000 hcs_core-0.1.236/hcs_core/sglib/login_support.py
--rw-r--r--   0 nanw       (503) staff       (20)      683 2024-05-20 22:59:20.000000 hcs_core-0.1.236/hcs_core/sglib/payload_util.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.299356 hcs_core-0.1.236/hcs_core/util/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/__init__.py
--rwxr-xr-x   0 nanw       (503) staff       (20)     2535 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/check_license.py
--rw-r--r--   0 nanw       (503) staff       (20)     3482 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/duration.py
--rw-r--r--   0 nanw       (503) staff       (20)      838 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/exit.py
--rw-r--r--   0 nanw       (503) staff       (20)     1755 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/hcs_constants.py
--rw-r--r--   0 nanw       (503) staff       (20)     8395 2024-05-20 23:16:24.000000 hcs_core-0.1.236/hcs_core/util/job_view.py
--rw-r--r--   0 nanw       (503) staff       (20)     5281 2024-05-20 23:00:41.000000 hcs_core-0.1.236/hcs_core/util/pki_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     1946 2024-05-20 23:01:09.000000 hcs_core-0.1.236/hcs_core/util/query_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     2958 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/scheduler.py
--rw-r--r--   0 nanw       (503) staff       (20)     1239 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/ssl_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     1727 2024-05-14 18:28:08.000000 hcs_core-0.1.236/hcs_core/util/versions.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-20 23:16:32.300480 hcs_core-0.1.236/hcs_core.egg-info/
--rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (503) staff       (20)     1788 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (503) staff       (20)        1 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/requires.txt
--rw-r--r--   0 nanw       (503) staff       (20)        9 2024-05-20 23:16:32.000000 hcs_core-0.1.236/hcs_core.egg-info/top_level.txt
--rw-r--r--   0 nanw       (503) staff       (20)     1250 2024-05-14 18:28:08.000000 hcs_core-0.1.236/pyproject.toml
--rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:28:08.000000 hcs_core-0.1.236/requirements.txt
--rw-r--r--   0 nanw       (503) staff       (20)       38 2024-05-20 23:16:32.302366 hcs_core-0.1.236/setup.cfg
--rw-r--r--   0 nanw       (503) staff       (20)      808 2024-05-14 18:28:08.000000 hcs_core-0.1.236/setup.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.109035 hcs_core-0.1.237/
+-rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-21 00:26:06.108376 hcs_core-0.1.237/PKG-INFO
+-rw-r--r--   0 nanw       (503) staff       (20)       25 2024-05-14 18:28:08.000000 hcs_core-0.1.237/README.md
+-rw-r--r--   0 nanw       (503) staff       (20)        7 2024-05-21 00:26:03.000000 hcs_core-0.1.237/VERSION
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.050113 hcs_core-0.1.237/hcs_core/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/__init__.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.067826 hcs_core-0.1.237/hcs_core/ctxp/
+-rw-r--r--   0 nanw       (503) staff       (20)      790 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/ctxp/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 22:21:06.000000 hcs_core-0.1.237/hcs_core/ctxp/_init.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.073272 hcs_core-0.1.237/hcs_core/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3086 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2388 2024-05-20 23:16:24.000000 hcs_core-0.1.237/hcs_core/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)     4034 2024-05-20 22:44:20.000000 hcs_core-0.1.237/hcs_core/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2274 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5800 2024-05-20 23:02:06.000000 hcs_core-0.1.237/hcs_core/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (503) staff       (20)      931 2024-05-20 15:58:31.000000 hcs_core-0.1.237/hcs_core/ctxp/config.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 16:01:06.000000 hcs_core-0.1.237/hcs_core/ctxp/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)    14092 2024-05-20 23:16:24.000000 hcs_core-0.1.237/hcs_core/ctxp/data_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2856 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/ctxp/duration.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1658 2024-05-20 22:32:30.000000 hcs_core-0.1.237/hcs_core/ctxp/extension.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6805 2024-05-20 22:48:34.000000 hcs_core-0.1.237/hcs_core/ctxp/fstore.py
+-rw-r--r--   0 nanw       (503) staff       (20)     4666 2024-05-20 23:16:24.000000 hcs_core-0.1.237/hcs_core/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6320 2024-05-20 23:16:24.000000 hcs_core-0.1.237/hcs_core/ctxp/logger.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6714 2024-05-21 00:25:57.000000 hcs_core-0.1.237/hcs_core/ctxp/profile.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1565 2024-05-20 22:51:09.000000 hcs_core-0.1.237/hcs_core/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1767 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/ctxp/recent.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1619 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/ctxp/state.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8036 2024-05-20 22:52:07.000000 hcs_core-0.1.237/hcs_core/ctxp/util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3244 2024-05-20 16:02:07.000000 hcs_core-0.1.237/hcs_core/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.078884 hcs_core-0.1.237/hcs_core/plan/
+-rw-r--r--   0 nanw       (503) staff       (20)      203 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/plan/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)      125 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/plan/actions.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1298 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/plan/base_provider.py
+-rw-r--r--   0 nanw       (503) staff       (20)      116 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/plan/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)    20957 2024-05-20 22:52:58.000000 hcs_core-0.1.237/hcs_core/plan/core.py
+-rw-r--r--   0 nanw       (503) staff       (20)    12950 2024-05-20 23:16:24.000000 hcs_core-0.1.237/hcs_core/plan/dag.py
+-rw-r--r--   0 nanw       (503) staff       (20)     7761 2024-05-20 22:55:21.000000 hcs_core-0.1.237/hcs_core/plan/helper.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5454 2024-05-20 22:55:35.000000 hcs_core-0.1.237/hcs_core/plan/kop.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.080454 hcs_core-0.1.237/hcs_core/plan/provider/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.082751 hcs_core-0.1.237/hcs_core/plan/provider/dev/
+-rw-r--r--   0 nanw       (503) staff       (20)       30 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)       34 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1982 2024-05-20 22:55:55.000000 hcs_core-0.1.237/hcs_core/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1104 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.097339 hcs_core-0.1.237/hcs_core/sglib/
+-rw-r--r--   0 nanw       (503) staff       (20)      654 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/sglib/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5169 2024-05-20 22:56:14.000000 hcs_core-0.1.237/hcs_core/sglib/auth.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1796 2024-05-20 16:06:32.000000 hcs_core-0.1.237/hcs_core/sglib/cli_options.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8379 2024-05-20 22:57:08.000000 hcs_core-0.1.237/hcs_core/sglib/client_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8053 2024-05-20 22:57:40.000000 hcs_core-0.1.237/hcs_core/sglib/csp.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5167 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/sglib/ez_client.py
+-rw-r--r--   0 nanw       (503) staff       (20)      901 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (503) staff       (20)    10128 2024-05-20 23:01:41.000000 hcs_core-0.1.237/hcs_core/sglib/login_support.py
+-rw-r--r--   0 nanw       (503) staff       (20)      683 2024-05-20 22:59:20.000000 hcs_core-0.1.237/hcs_core/sglib/payload_util.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.105952 hcs_core-0.1.237/hcs_core/util/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/util/__init__.py
+-rwxr-xr-x   0 nanw       (503) staff       (20)     2535 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/util/check_license.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3482 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/util/duration.py
+-rw-r--r--   0 nanw       (503) staff       (20)      838 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/util/exit.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1755 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/util/hcs_constants.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8395 2024-05-20 23:16:24.000000 hcs_core-0.1.237/hcs_core/util/job_view.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5281 2024-05-20 23:00:41.000000 hcs_core-0.1.237/hcs_core/util/pki_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1946 2024-05-20 23:01:09.000000 hcs_core-0.1.237/hcs_core/util/query_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2958 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/util/scheduler.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1239 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/util/ssl_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1727 2024-05-14 18:28:08.000000 hcs_core-0.1.237/hcs_core/util/versions.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 00:26:06.107286 hcs_core-0.1.237/hcs_core.egg-info/
+-rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-21 00:26:06.000000 hcs_core-0.1.237/hcs_core.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (503) staff       (20)     1788 2024-05-21 00:26:06.000000 hcs_core-0.1.237/hcs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (503) staff       (20)        1 2024-05-21 00:26:06.000000 hcs_core-0.1.237/hcs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-21 00:26:06.000000 hcs_core-0.1.237/hcs_core.egg-info/requires.txt
+-rw-r--r--   0 nanw       (503) staff       (20)        9 2024-05-21 00:26:06.000000 hcs_core-0.1.237/hcs_core.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (503) staff       (20)     1250 2024-05-14 18:28:08.000000 hcs_core-0.1.237/pyproject.toml
+-rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:28:08.000000 hcs_core-0.1.237/requirements.txt
+-rw-r--r--   0 nanw       (503) staff       (20)       38 2024-05-21 00:26:06.109138 hcs_core-0.1.237/setup.cfg
+-rw-r--r--   0 nanw       (503) staff       (20)      808 2024-05-14 18:28:08.000000 hcs_core-0.1.237/setup.py
```

### Comparing `hcs_core-0.1.236/PKG-INFO` & `hcs_core-0.1.237/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.236
+Version: 0.1.237
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/__init__.py` & `hcs_core-0.1.237/hcs_core/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/_init.py` & `hcs_core-0.1.237/hcs_core/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/_ut.py` & `hcs_core-0.1.237/hcs_core/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/context.py` & `hcs_core-0.1.237/hcs_core/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/built_in_cmds/profile.py` & `hcs_core-0.1.237/hcs_core/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/cli_options.py` & `hcs_core-0.1.237/hcs_core/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/cli_processor.py` & `hcs_core-0.1.237/hcs_core/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/config.py` & `hcs_core-0.1.237/hcs_core/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/context.py` & `hcs_core-0.1.237/hcs_core/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/data_util.py` & `hcs_core-0.1.237/hcs_core/ctxp/data_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/duration.py` & `hcs_core-0.1.237/hcs_core/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/extension.py` & `hcs_core-0.1.237/hcs_core/ctxp/extension.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/fstore.py` & `hcs_core-0.1.237/hcs_core/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/jsondot.py` & `hcs_core-0.1.237/hcs_core/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/logger.py` & `hcs_core-0.1.237/hcs_core/ctxp/logger.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/profile.py` & `hcs_core-0.1.237/hcs_core/ctxp/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,22 @@
             data["csp"] = csp_config
     return data
 
 
 def save():
     """Save the current profile"""
     global _data
-    if _data is not None:
-        save_data_file(_data, file(name()), "yaml", 0o600)
+    if _data is None:
+        return
+    write(name(), _data)
+
+
+def write(profile_name: str, data: dict):
+    """Save profile by name"""
+    save_data_file(data, file(profile_name), "yaml", 0o600)
 
 
 def name() -> str:
     """Get the current active profile name"""
     global _active_profile_name
     if not _active_profile_name:
         _active_profile_name = state.get("active_profile", default="default")
```

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/profile_store.py` & `hcs_core-0.1.237/hcs_core/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/recent.py` & `hcs_core-0.1.237/hcs_core/ctxp/recent.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/state.py` & `hcs_core-0.1.237/hcs_core/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/util.py` & `hcs_core-0.1.237/hcs_core/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/ctxp/var_template.py` & `hcs_core-0.1.237/hcs_core/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/plan/base_provider.py` & `hcs_core-0.1.237/hcs_core/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/plan/core.py` & `hcs_core-0.1.237/hcs_core/plan/core.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/plan/dag.py` & `hcs_core-0.1.237/hcs_core/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/plan/helper.py` & `hcs_core-0.1.237/hcs_core/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/plan/kop.py` & `hcs_core-0.1.237/hcs_core/plan/kop.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/plan/provider/dev/dummy.py` & `hcs_core-0.1.237/hcs_core/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/plan/provider/dev/fibonacci.py` & `hcs_core-0.1.237/hcs_core/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/__init__.py` & `hcs_core-0.1.237/hcs_core/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/auth.py` & `hcs_core-0.1.237/hcs_core/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/cli_options.py` & `hcs_core-0.1.237/hcs_core/sglib/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/client_util.py` & `hcs_core-0.1.237/hcs_core/sglib/client_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/csp.py` & `hcs_core-0.1.237/hcs_core/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/ez_client.py` & `hcs_core-0.1.237/hcs_core/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/hcs_client.py` & `hcs_core-0.1.237/hcs_core/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/login_support.py` & `hcs_core-0.1.237/hcs_core/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/sglib/payload_util.py` & `hcs_core-0.1.237/hcs_core/sglib/payload_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/check_license.py` & `hcs_core-0.1.237/hcs_core/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/duration.py` & `hcs_core-0.1.237/hcs_core/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/exit.py` & `hcs_core-0.1.237/hcs_core/util/exit.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/hcs_constants.py` & `hcs_core-0.1.237/hcs_core/util/hcs_constants.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/job_view.py` & `hcs_core-0.1.237/hcs_core/util/job_view.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/pki_util.py` & `hcs_core-0.1.237/hcs_core/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/query_util.py` & `hcs_core-0.1.237/hcs_core/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/scheduler.py` & `hcs_core-0.1.237/hcs_core/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/ssl_util.py` & `hcs_core-0.1.237/hcs_core/util/ssl_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core/util/versions.py` & `hcs_core-0.1.237/hcs_core/util/versions.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/hcs_core.egg-info/PKG-INFO` & `hcs_core-0.1.237/hcs_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.236
+Version: 0.1.237
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs_core-0.1.236/hcs_core.egg-info/SOURCES.txt` & `hcs_core-0.1.237/hcs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/pyproject.toml` & `hcs_core-0.1.237/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.236/setup.py` & `hcs_core-0.1.237/setup.py`

 * *Files identical despite different names*

