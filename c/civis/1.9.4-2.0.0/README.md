# Comparing `tmp/civis-1.9.4.tar.gz` & `tmp/civis-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/civis-1.9.4.tar", last modified: Thu Feb 28 22:08:31 2019, max compression
+gzip compressed data, was "civis-2.0.0.tar", last modified: Tue May 21 13:12:26 2024, max compression
```

## Comparing `civis-1.9.4.tar` & `civis-2.0.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/
--rw-r--r--   0 mheilman   (502) staff       (20)     9097 2019-02-28 22:08:31.000000 civis-1.9.4/PKG-INFO
--rw-r--r--   0 mheilman   (502) staff       (20)     1501 2017-04-05 14:45:03.000000 civis-1.9.4/LICENSE.md
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/
--rw-r--r--   0 mheilman   (502) staff       (20)     9097 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/PKG-INFO
--rw-r--r--   0 mheilman   (502) staff       (20)     1374 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/SOURCES.txt
--rw-r--r--   0 mheilman   (502) staff       (20)      100 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/entry_points.txt
--rw-r--r--   0 mheilman   (502) staff       (20)      297 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/requires.txt
--rw-r--r--   0 mheilman   (502) staff       (20)        6 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/top_level.txt
--rw-r--r--   0 mheilman   (502) staff       (20)        1 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/dependency_links.txt
--rw-r--r--   0 mheilman   (502) staff       (20)      344 2017-10-13 15:03:53.000000 civis-1.9.4/requirements.txt
--rw-r--r--   0 mheilman   (502) staff       (20)      178 2017-10-13 15:03:53.000000 civis-1.9.4/MANIFEST.in
--rw-r--r--   0 mheilman   (502) staff       (20)     2517 2019-02-07 15:06:59.000000 civis-1.9.4/setup.py
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/
--rw-r--r--   0 mheilman   (502) staff       (20)     2754 2018-03-13 15:42:03.000000 civis-1.9.4/civis/compat.py
--rw-r--r--   0 mheilman   (502) staff       (20)      413 2017-04-05 14:45:03.000000 civis-1.9.4/civis/pubnub.py
--rw-r--r--   0 mheilman   (502) staff       (20)       22 2019-02-28 22:06:09.000000 civis-1.9.4/civis/_version.py
--rw-r--r--   0 mheilman   (502) staff       (20)     2660 2018-04-12 19:51:26.000000 civis-1.9.4/civis/_deprecation.py
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/resources/
--rw-r--r--   0 mheilman   (502) staff       (20)      425 2017-10-13 15:03:53.000000 civis-1.9.4/civis/resources/__init__.py
--rw-r--r--   0 mheilman   (502) staff       (20)    21655 2018-04-18 16:25:07.000000 civis-1.9.4/civis/resources/_resources.py
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/io/
--rw-r--r--   0 mheilman   (502) staff       (20)     5716 2018-04-12 19:51:26.000000 civis-1.9.4/civis/io/_databases.py
--rw-r--r--   0 mheilman   (502) staff       (20)    42712 2018-11-30 18:10:19.000000 civis-1.9.4/civis/io/_tables.py
--rw-r--r--   0 mheilman   (502) staff       (20)      185 2017-06-29 13:59:33.000000 civis-1.9.4/civis/io/__init__.py
--rw-r--r--   0 mheilman   (502) staff       (20)    16709 2018-12-03 17:53:14.000000 civis-1.9.4/civis/io/_files.py
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/tests/
--rw-r--r--   0 mheilman   (502) staff       (20)    14921 2017-11-14 23:00:55.000000 civis-1.9.4/civis/tests/test_resources.py
--rw-r--r--   0 mheilman   (502) staff       (20)     2733 2017-11-14 22:41:19.000000 civis-1.9.4/civis/tests/test_utils.py
--rw-r--r--   0 mheilman   (502) staff       (20)     5556 2019-02-28 19:44:50.000000 civis-1.9.4/civis/tests/test_response.py
--rw-r--r--   0 mheilman   (502) staff       (20)     1465 2017-04-05 14:45:03.000000 civis-1.9.4/civis/tests/testcase.py
--rw-r--r--   0 mheilman   (502) staff       (20)    18162 2018-03-13 14:47:28.000000 civis-1.9.4/civis/tests/test_futures.py
--rw-r--r--   0 mheilman   (502) staff       (20)       68 2017-10-13 15:03:53.000000 civis-1.9.4/civis/tests/__init__.py
--rw-r--r--   0 mheilman   (502) staff       (20)      804 2019-02-28 15:46:05.000000 civis-1.9.4/civis/tests/test_civis.py
--rw-r--r--   0 mheilman   (502) staff       (20)      487 2017-10-13 15:03:53.000000 civis-1.9.4/civis/tests/test_mocks.py
--rw-r--r--   0 mheilman   (502) staff       (20)    23475 2018-12-03 17:53:14.000000 civis-1.9.4/civis/tests/test_io.py
--rw-r--r--   0 mheilman   (502) staff       (20)     3221 2017-04-05 14:45:03.000000 civis-1.9.4/civis/tests/petstore.json
--rw-r--r--   0 mheilman   (502) staff       (20)    19629 2018-01-24 15:33:19.000000 civis-1.9.4/civis/tests/test_parallel.py
--rw-r--r--   0 mheilman   (502) staff       (20)      537 2017-11-14 23:00:55.000000 civis-1.9.4/civis/tests/test_compat.py
--rw-r--r--   0 mheilman   (502) staff       (20)  2070045 2019-02-07 15:06:59.000000 civis-1.9.4/civis/tests/civis_api_spec_channels.json
--rw-r--r--   0 mheilman   (502) staff       (20)     2140 2018-04-12 19:51:26.000000 civis-1.9.4/civis/tests/test_deprecate.py
--rw-r--r--   0 mheilman   (502) staff       (20)  2068020 2019-02-07 15:06:59.000000 civis-1.9.4/civis/tests/civis_api_spec.json
--rw-r--r--   0 mheilman   (502) staff       (20)     1398 2017-10-13 15:03:53.000000 civis-1.9.4/civis/tests/test_client.py
--rw-r--r--   0 mheilman   (502) staff       (20)     4224 2019-02-07 15:06:59.000000 civis-1.9.4/civis/tests/test_cli.py
--rw-r--r--   0 mheilman   (502) staff       (20)      665 2017-06-29 13:59:33.000000 civis-1.9.4/civis/tests/test_base.py
--rw-r--r--   0 mheilman   (502) staff       (20)     3573 2018-09-24 13:52:12.000000 civis-1.9.4/civis/tests/test_polling.py
--rw-r--r--   0 mheilman   (502) staff       (20)     1415 2018-04-12 19:51:26.000000 civis-1.9.4/civis/tests/mocks.py
--rw-r--r--   0 mheilman   (502) staff       (20)      259 2017-10-13 15:03:53.000000 civis-1.9.4/civis/__init__.py
--rw-r--r--   0 mheilman   (502) staff       (20)     6352 2019-02-28 19:44:50.000000 civis-1.9.4/civis/response.py
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/utils/
--rw-r--r--   0 mheilman   (502) staff       (20)       50 2017-04-05 14:45:03.000000 civis-1.9.4/civis/utils/__init__.py
--rw-r--r--   0 mheilman   (502) staff       (20)     1015 2018-04-12 19:51:26.000000 civis-1.9.4/civis/utils/_jobs.py
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/cli/
--rw-r--r--   0 mheilman   (502) staff       (20)       73 2017-04-05 14:45:03.000000 civis-1.9.4/civis/cli/__init__.py
--rw-r--r--   0 mheilman   (502) staff       (20)     5526 2018-02-01 14:15:15.000000 civis-1.9.4/civis/cli/_cli_commands.py
--rwxr-xr-x   0 mheilman   (502) staff       (20)    11341 2018-04-18 16:25:23.000000 civis-1.9.4/civis/cli/__main__.py
--rw-r--r--   0 mheilman   (502) staff       (20)    28092 2018-04-12 19:51:26.000000 civis-1.9.4/civis/futures.py
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/ml/
-drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/ml/tests/
--rw-r--r--   0 mheilman   (502) staff       (20)    39390 2019-02-07 15:06:59.000000 civis-1.9.4/civis/ml/tests/test_model.py
--rw-r--r--   0 mheilman   (502) staff       (20)        0 2017-11-14 23:00:55.000000 civis-1.9.4/civis/ml/tests/__init__.py
--rw-r--r--   0 mheilman   (502) staff       (20)       71 2017-06-29 13:59:33.000000 civis-1.9.4/civis/ml/__init__.py
--rw-r--r--   0 mheilman   (502) staff       (20)    62356 2019-02-07 15:06:59.000000 civis-1.9.4/civis/ml/_model.py
--rwxr-xr-x   0 mheilman   (502) staff       (20)     4292 2017-10-13 15:03:53.000000 civis-1.9.4/civis/run_joblib_func.py
--rw-r--r--   0 mheilman   (502) staff       (20)     8484 2017-11-14 23:00:55.000000 civis-1.9.4/civis/polling.py
--rw-r--r--   0 mheilman   (502) staff       (20)    40356 2018-04-12 19:51:26.000000 civis-1.9.4/civis/parallel.py
--rw-r--r--   0 mheilman   (502) staff       (20)     7709 2017-11-15 16:50:42.000000 civis-1.9.4/civis/base.py
--rw-r--r--   0 mheilman   (502) staff       (20)     4673 2018-01-24 15:33:19.000000 civis-1.9.4/civis/_utils.py
--rw-r--r--   0 mheilman   (502) staff       (20)    13632 2019-02-28 15:46:05.000000 civis-1.9.4/civis/civis.py
--rw-r--r--   0 mheilman   (502) staff       (20)       99 2019-02-28 22:08:31.000000 civis-1.9.4/setup.cfg
--rw-r--r--   0 mheilman   (502) staff       (20)     6657 2019-02-07 15:06:59.000000 civis-1.9.4/README.rst
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.220872 civis-2.0.0/
+-rw-r--r--   0 jlee       (503) staff       (20)     1501 2023-06-28 16:43:32.000000 civis-2.0.0/LICENSE.md
+-rw-r--r--   0 jlee       (503) staff       (20)     9387 2024-05-21 13:12:26.219983 civis-2.0.0/PKG-INFO
+-rw-r--r--   0 jlee       (503) staff       (20)     7512 2024-05-20 21:42:07.000000 civis-2.0.0/README.rst
+-rw-r--r--   0 jlee       (503) staff       (20)     1990 2024-05-20 21:42:07.000000 civis-2.0.0/pyproject.toml
+-rw-r--r--   0 jlee       (503) staff       (20)       38 2024-05-21 13:12:26.221035 civis-2.0.0/setup.cfg
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.122045 civis-2.0.0/src/
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.158128 civis-2.0.0/src/civis/
+-rw-r--r--   0 jlee       (503) staff       (20)      446 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3171 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/_deprecation.py
+-rw-r--r--   0 jlee       (503) staff       (20)     5387 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/_utils.py
+-rw-r--r--   0 jlee       (503) staff       (20)    10829 2024-05-20 02:15:26.000000 civis-2.0.0/src/civis/base.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.167149 civis-2.0.0/src/civis/cli/
+-rw-r--r--   0 jlee       (503) staff       (20)       73 2024-05-13 18:11:55.000000 civis-2.0.0/src/civis/cli/__init__.py
+-rwxr-xr-x   0 jlee       (503) staff       (20)    11639 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/cli/__main__.py
+-rw-r--r--   0 jlee       (503) staff       (20)    11849 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/cli/_cli_commands.py
+-rw-r--r--   0 jlee       (503) staff       (20)    10665 2024-05-20 13:20:42.000000 civis-2.0.0/src/civis/client.py
+-rw-r--r--   0 jlee       (503) staff       (20)  2306264 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/client.pyi
+-rw-r--r--   0 jlee       (503) staff       (20)    27130 2024-05-20 21:42:07.000000 civis-2.0.0/src/civis/futures.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.171973 civis-2.0.0/src/civis/io/
+-rw-r--r--   0 jlee       (503) staff       (20)      145 2024-05-13 18:11:55.000000 civis-2.0.0/src/civis/io/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     5229 2024-05-20 21:42:07.000000 civis-2.0.0/src/civis/io/_databases.py
+-rw-r--r--   0 jlee       (503) staff       (20)    21558 2024-05-20 21:42:07.000000 civis-2.0.0/src/civis/io/_files.py
+-rw-r--r--   0 jlee       (503) staff       (20)    55786 2024-05-20 21:42:07.000000 civis-2.0.0/src/civis/io/_tables.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3223 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/loggers.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.175851 civis-2.0.0/src/civis/ml/
+-rw-r--r--   0 jlee       (503) staff       (20)      110 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/ml/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)    12005 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/ml/_helper.py
+-rw-r--r--   0 jlee       (503) staff       (20)    63734 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/ml/_model.py
+-rw-r--r--   0 jlee       (503) staff       (20)    41253 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/parallel.py
+-rw-r--r--   0 jlee       (503) staff       (20)     8573 2024-05-16 14:28:12.000000 civis-2.0.0/src/civis/polling.py
+-rw-r--r--   0 jlee       (503) staff       (20)        0 2024-05-13 18:11:55.000000 civis-2.0.0/src/civis/py.typed
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.183233 civis-2.0.0/src/civis/resources/
+-rw-r--r--   0 jlee       (503) staff       (20)      357 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/resources/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3686 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/resources/_client_pypi.py
+-rw-r--r--   0 jlee       (503) staff       (20)    22167 2024-05-20 13:20:42.000000 civis-2.0.0/src/civis/resources/_resources.py
+-rw-r--r--   0 jlee       (503) staff       (20)  2375407 2024-05-13 18:11:55.000000 civis-2.0.0/src/civis/resources/civis_api_spec.json
+-rw-r--r--   0 jlee       (503) staff       (20)    10531 2024-05-20 21:42:07.000000 civis-2.0.0/src/civis/response.py
+-rwxr-xr-x   0 jlee       (503) staff       (20)     5054 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/run_joblib_func.py
+-rw-r--r--   0 jlee       (503) staff       (20)     7684 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/service_client.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.192573 civis-2.0.0/src/civis/tests/
+-rw-r--r--   0 jlee       (503) staff       (20)      165 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/tests/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3414 2024-05-20 21:42:07.000000 civis-2.0.0/src/civis/tests/mocks.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.194520 civis-2.0.0/src/civis/utils/
+-rw-r--r--   0 jlee       (503) staff       (20)       91 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/utils/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3272 2024-05-15 13:36:23.000000 civis-2.0.0/src/civis/utils/_jobs.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.217119 civis-2.0.0/src/civis.egg-info/
+-rw-r--r--   0 jlee       (503) staff       (20)     9387 2024-05-21 13:12:26.000000 civis-2.0.0/src/civis.egg-info/PKG-INFO
+-rw-r--r--   0 jlee       (503) staff       (20)     1423 2024-05-21 13:12:26.000000 civis-2.0.0/src/civis.egg-info/SOURCES.txt
+-rw-r--r--   0 jlee       (503) staff       (20)        1 2024-05-21 13:12:26.000000 civis-2.0.0/src/civis.egg-info/dependency_links.txt
+-rw-r--r--   0 jlee       (503) staff       (20)       99 2024-05-21 13:12:26.000000 civis-2.0.0/src/civis.egg-info/entry_points.txt
+-rw-r--r--   0 jlee       (503) staff       (20)      381 2024-05-21 13:12:26.000000 civis-2.0.0/src/civis.egg-info/requires.txt
+-rw-r--r--   0 jlee       (503) staff       (20)        6 2024-05-21 13:12:26.000000 civis-2.0.0/src/civis.egg-info/top_level.txt
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-21 13:12:26.215867 civis-2.0.0/tests/
+-rw-r--r--   0 jlee       (503) staff       (20)     1494 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_base.py
+-rw-r--r--   0 jlee       (503) staff       (20)     6635 2024-05-20 21:42:07.000000 civis-2.0.0/tests/test_cli.py
+-rw-r--r--   0 jlee       (503) staff       (20)     2341 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_client.py
+-rw-r--r--   0 jlee       (503) staff       (20)     4101 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_deprecate.py
+-rw-r--r--   0 jlee       (503) staff       (20)    15467 2024-05-16 15:37:34.000000 civis-2.0.0/tests/test_futures.py
+-rw-r--r--   0 jlee       (503) staff       (20)    52275 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_io.py
+-rw-r--r--   0 jlee       (503) staff       (20)     4599 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_jobs.py
+-rw-r--r--   0 jlee       (503) staff       (20)     2999 2024-05-13 18:11:55.000000 civis-2.0.0/tests/test_loggers.py
+-rw-r--r--   0 jlee       (503) staff       (20)      487 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_mocks.py
+-rw-r--r--   0 jlee       (503) staff       (20)    22269 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_parallel.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3590 2024-05-16 14:28:12.000000 civis-2.0.0/tests/test_polling.py
+-rw-r--r--   0 jlee       (503) staff       (20)    30060 2024-05-20 13:20:42.000000 civis-2.0.0/tests/test_resources.py
+-rw-r--r--   0 jlee       (503) staff       (20)    10975 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_response.py
+-rw-r--r--   0 jlee       (503) staff       (20)      181 2024-05-20 21:42:07.000000 civis-2.0.0/tests/test_run_joblib_func.py
+-rw-r--r--   0 jlee       (503) staff       (20)    10238 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_service_client.py
+-rw-r--r--   0 jlee       (503) staff       (20)    11118 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_utils.py
+-rw-r--r--   0 jlee       (503) staff       (20)      560 2024-05-15 13:36:23.000000 civis-2.0.0/tests/test_version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `civis-1.9.4/LICENSE.md` & `civis-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `civis-1.9.4/civis/resources/_resources.py` & `civis-2.0.0/src/civis/resources/_resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,246 +1,269 @@
 from collections import OrderedDict
+from functools import lru_cache
 import json
 import os
 import re
 import textwrap
-try:
-    from inspect import Signature, Parameter
-except ImportError:
-    from funcsigs import Signature, Parameter
+from inspect import Signature, Parameter
 
 from jsonref import JsonRef
 import requests
-import six
+from requests import Request
 
-from civis.base import Endpoint, get_base_url
-from civis.compat import lru_cache
-from civis._deprecation import deprecate_param
-from civis._utils import (camel_to_snake, to_camelcase,
-                          open_session, get_api_key)
-
-
-API_VERSIONS = ["1.0"]
-BASE_RESOURCES_V1 = [
-    'announcements',
-    'apps',
-    'civis',
-    'clusters',
-    'codes',
-    'credentials',
-    'databases',
-    'endpoints',
-    'enhancements',
-    'exports',
-    'files',
-    'groups',
-    'imports',
-    'jobs',
-    'match_targets',
-    'media',
-    'models',
-    'notebooks',
-    'notifications',
-    'ontology',
-    'predictions',
-    'projects',
-    'queries',
-    'remote_hosts',
-    'reports',
-    'results',
-    'scripts',
-    'search',
-    'tables',
-    'templates',
-    'users',
-    'workflows'
-]
+from civis.base import Endpoint, get_base_url, open_session
+from civis._utils import camel_to_snake, get_api_key, retry_request, MAX_RETRIES
 
-TYPE_MAP = {"array": "list", "object": "dict"}
+
+API_VERSIONS = frozenset({"1.0"})
+
+# civis_api_spec.json can be updated
+# by running the tools/update_civis_api_spec_json.py script.
+API_SPEC_PATH = os.path.join(
+    os.path.dirname(os.path.realpath(__file__)),
+    "civis_api_spec.json",
+)
+with open(API_SPEC_PATH) as f:
+    API_SPEC = json.load(f, object_pairs_hook=OrderedDict)
+BASE_RESOURCES_V1 = sorted(
+    r
+    for r in set(path.split("/", 2)[1] for path in API_SPEC["paths"].keys())
+    # "feature_flags" has a name collision with an APIClient instance
+    if r != "feature_flags"
+)
+
+
+TYPE_MAP = {
+    "array": "list",
+    "object": "dict",
+    "integer": "int",
+    "number": "float",
+    "string": "str",
+    "boolean": "bool",
+}
 ITERATOR_PARAM_DESC = (
     "iterator : bool, optional\n"
     "    If True, return a generator to iterate over all responses. Use when\n"
     "    more results than the maximum allowed by limit are needed. When\n"
-    "    True, limit and page_num are ignored. Defaults to False.\n")
-MAX_RETRIES = 10
-CACHED_SPEC_PATH = os.path.join(os.path.expanduser('~'),
-                                ".civis_api_spec.json")
+    "    True, limit and page_num are ignored. Defaults to False.\n"
+)
+CACHED_SPEC_PATH = os.path.join(os.path.expanduser("~"), ".civis_api_spec.json")
+DEFAULT_ARG_VALUE = None
 
 
-@deprecate_param('v2.0.0', 'resources')
-def exclude_resource(path, api_version, resources):
-    if api_version == "1.0" and resources == "base":
-        include = any([path.startswith(x) for x in BASE_RESOURCES_V1])
+def exclude_resource(path, api_version):
+    if api_version == "1.0":
+        include = any(path.startswith(x) for x in BASE_RESOURCES_V1)
     else:
         include = True
     return not include
 
 
 def get_properties(x):
     return x.get("properties") or x.get("items", {}).get("properties")
 
 
 def property_type(props):
-    t = TYPE_MAP.get(props['type'], props['type'])
+    t = type_from_param(props)
     fmt = props.get("format")
-    return "{}/{}".format(t, fmt) if fmt else t
+    return "{} ({})".format(t, fmt) if fmt else t
 
 
-def name_and_type_doc(name, prop, child, level, optional=False):
-    """ Create a doc string element that includes a parameter's name
-    and its type. This is intented to be combined with another
+def name_and_type_doc(name, prop, level, optional=False):
+    """Create a doc string element that includes a parameter's name
+    and its type. This is intended to be combined with another
     doc string element that gives a description of the parameter.
     """
     prop_type = property_type(prop)
     snake_name = camel_to_snake(name)
     indent = " " * level * 4
     dash = "- " if level > 0 else ""
-    colons = "::" if child else ""
     opt_str = ", optional" if optional else ""
-    doc = "{}{}{} : {}{}{}"
-    return doc.format(indent, dash, snake_name, prop_type, opt_str, colons)
+    doc = "{}{}{} : {}{}"
+    return doc.format(indent, dash, snake_name, prop_type, opt_str)
 
 
 def docs_from_property(name, prop, properties, level, optional=False):
-    """ Create a list of doc string elements from a single property
+    """Create a list of doc string elements from a single property
     object. Avoids infinite recursion when a property contains a
     circular reference to its parent.
     """
     docs = []
     child_properties = get_properties(prop)
     child = None if child_properties == properties else child_properties
-    docs.append(name_and_type_doc(name, prop, child, level, optional))
+    docs.append(name_and_type_doc(name, prop, level, optional))
     doc_str = prop.get("description")
     if doc_str:
         indent = 4 * (level + 1) * " "
-        doc_wrap = textwrap.fill(doc_str,
-                                 initial_indent=indent,
-                                 subsequent_indent=indent,
-                                 width=79)
-        docs.append(doc_wrap)
+        doc_wrap = textwrap.fill(
+            doc_str, initial_indent=indent, subsequent_indent=indent, width=79
+        )
+        docs.append(f"{doc_wrap}\n") if child else docs.append(doc_wrap)
     if child:
         child_docs = docs_from_properties(child, level + 1)
         docs.append("\n".join(child_docs))
     return docs
 
 
 def docs_from_properties(properties, level=0):
-    """ Return doc string elements from a dictionary of properties."""
+    """Return doc string elements from a dictionary of properties."""
     docs = []
     for name, prop in properties.items():
         doc_list = docs_from_property(name, prop, properties, level)
         docs.extend(doc_list)
     return docs
 
 
-def doc_from_responses(responses):
-    """ Return a doc string element from a responses object. The
+def deprecated_notice(deprecation_warning):
+    """Return a doc string element for the deprecation notice. The
+    doc string can be an empty string if the warning is None
+    """
+    if deprecation_warning is None:
+        return ""
+
+    return f"\n.. warning::\n\n    {deprecation_warning}\n"
+
+
+def doc_from_responses(responses, is_iterable):
+    """Return a doc string element from a responses object. The
     doc string describes the returned objects of a function.
     """
     response_code, response_object = next(iter(responses.items()))
-    schema = response_object.get('schema', {})
+    schema = response_object.get("schema", {})
     properties = get_properties(schema)
     if properties:
-        result_doc = "\n".join(docs_from_properties(properties))
+        if is_iterable:
+            resp_type = ":class:`civis.response.PaginatedResponse`\n"
+        else:
+            resp_type = ":class:`civis.response.Response`\n"
+        result_doc = resp_type + ("\n".join(docs_from_properties(properties, level=1)))
     else:
-        description = response_object['description']
+        description = response_object["description"]
         result_doc_fmt = "None\n    Response code {}: {}"
         result_doc = result_doc_fmt.format(response_code, description)
     return "Returns\n-------\n" + result_doc
 
 
 def join_doc_elements(*args):
     return "\n".join(args).rstrip()
 
 
+def type_from_param(param):
+    main_type = TYPE_MAP[param["type"]]
+    item_type = None
+    if main_type == "list":
+        items = param.get("items", {})
+        if "type" in items:
+            item_type = TYPE_MAP[items["type"]]
+        elif "$ref" in items:
+            item_type = "dict"
+    return f"{main_type}[{item_type}]" if item_type else main_type
+
+
 def doc_from_param(param):
-    """ Return a doc string element for a single parameter.
+    """Return a doc string element for a single parameter.
     Intended to be joined with other doc string elements to
     form a complete docstring of the accepted parameters of
     a function.
     """
-    snake_name = camel_to_snake(param['name'])
-    param_type = param['type']
-    desc = param.get('description')
+    snake_name = camel_to_snake(param["name"])
+    param_type = type_from_param(param)
+    desc = param.get("description")
     optional = "" if param["required"] else ", optional"
     doc_body = ""
     if desc:
         indent = " " * 4
-        doc_wrap = textwrap.fill(desc,
-                                 initial_indent=indent,
-                                 subsequent_indent=indent,
-                                 width=79)
+        doc_wrap = textwrap.fill(
+            desc, initial_indent=indent, subsequent_indent=indent, width=79
+        )
         doc_body += doc_wrap
         doc_body += "\n"
     doc_head = "{} : {}{}\n".format(snake_name, param_type, optional)
     return doc_head + doc_body
 
 
 def iterable_method(method, params):
     """Determine whether it is possible for this endpoint to return an iterated
     response.
     """
-    required_params = ('limit', 'page_num')
+    required_params = ("limit", "page_num")
     params_present = all(param in params for param in required_params)
-    return (method.lower() == 'get' and params_present)
+    return method.lower() == "get" and params_present
 
 
-def create_signature(args, optional_args):
-    """ Dynamically create a signature for a function from strings.
+def create_signature(args, optional_args, prepend_self=False):
+    """Dynamically create a signature for a function from strings.
 
     This function can be used to create a signature for a dynamically
     generated function without generating a string representation of
     the function code and making an explicit eval call.
 
     Parameters
     ----------
-    args : list
-        List of strings that name the required arguments of a function.
-    optional_args : list
-        List of strings that name the optional arguments of a function.
+    args : dict
+        Dict of strings that name the required arguments of a function.
+    optional_args : dict
+        Dict of strings that name the optional arguments of a function,
+        and their default values.
+    prepend_self : bool, optional
+        If True, add the "self" arg as the first arg for a class method.
 
     Returns
     -------
     Signature(p) : inspect.Signature instance
         A Signature object that can be used to validate arguments in
         a dynamically created function.
     """
-    p = [Parameter(x, Parameter.POSITIONAL_OR_KEYWORD) for x in args]
-    if six.PY3:
-        opt_par_type = Parameter.KEYWORD_ONLY
-    else:
-        opt_par_type = Parameter.POSITIONAL_OR_KEYWORD
-    p += [Parameter(x, opt_par_type, default='DEFAULT')
-          for x in optional_args]
+    p = []
+    if prepend_self:
+        p += [Parameter("self", Parameter.POSITIONAL_OR_KEYWORD)]
+    p += [
+        Parameter(name, Parameter.POSITIONAL_OR_KEYWORD, annotation=arg["type"])
+        for name, arg in args.items()
+    ]
+    p += [
+        Parameter(
+            name,
+            Parameter.KEYWORD_ONLY,
+            default=arg["default"],
+            annotation=arg["type"],
+        )
+        for name, arg in optional_args.items()
+    ]
     return Signature(p)
 
 
 def split_method_params(params):
-    args = []
-    optional_args = []
+    args = {}
+    optional_args = {}
     body_params = []
     query_params = []
     path_params = []
     for param in params:
         name = param["name"]
         if param["required"]:
-            args.append(name)
+            args[name] = {"type": param.get("type")}
         else:
-            optional_args.append(name)
+            optional_args[name] = {
+                "default": param.get("default", DEFAULT_ARG_VALUE),
+                "type": param.get("type"),
+            }
         if param["in"] == "body":
             body_params.append(name)
         elif param["in"] == "query":
             query_params.append(name)
         elif param["in"] == "path":
             path_params.append(name)
     return args, optional_args, body_params, query_params, path_params
 
 
-def create_method(params, verb, method_name, path, doc):
-    """ Dynamically create a function to make an API call.
+def create_method(
+    params, verb, method_name, path, deprecation_warning, param_doc, response_doc
+):
+    """Dynamically create a function to make an API call.
 
     The returned function accepts required parameters as positional arguments
     and optional parameters as kwargs.  The function passes these parameters
     into the appropriate place (path, query or body) in the API call,
     depending on the criteria of the API endpoint.
 
     Parameters
@@ -251,95 +274,117 @@
     verb : str
         HTTP verb to call
     method_name : str
         The name to give the returned function f
     path : str
         Endpoint path, possibly including replacement fields
         (i.e. scripts/{id})
-    doc : str
-        Documentation string for the returned function f
-
+    deprecation_warning : str or None
+        Deprecation warning, if applicable, for the method
+    param_doc : str
+        Documentation string for the returned function f's parameters
+    response_doc : str
+        Documentation string for the returned function f's response
 
     Returns
     ------
     f : function
         A function which will make an API call
     """
+    doc = join_doc_elements(
+        deprecated_notice(deprecation_warning), param_doc, response_doc
+    )
     elements = split_method_params(params)
     sig_args, sig_opt_args, body_params, query_params, path_params = elements
     sig = create_signature(sig_args, sig_opt_args)
     is_iterable = iterable_method(verb, query_params)
 
     def f(self, *args, **kwargs):
-        raise_for_unexpected_kwargs(method_name, kwargs, sig_args,
-                                    sig_opt_args, is_iterable)
+        raise_for_unexpected_kwargs(
+            method_name, kwargs, sig_args, sig_opt_args, is_iterable
+        )
 
-        iterator = kwargs.pop('iterator', False)
+        iterator = kwargs.pop("iterator", False)
         arguments = sig.bind(*args, **kwargs).arguments
         if arguments.get("kwargs"):
             arguments.update(arguments.pop("kwargs"))
         body = {x: arguments[x] for x in body_params if x in arguments}
         query = {x: arguments[x] for x in query_params if x in arguments}
         path_vals = {x: arguments[x] for x in path_params if x in arguments}
         url = path.format(**path_vals) if path_vals else path
-        return self._call_api(verb, url, query, body, iterator=iterator)
+        return self._call_api(
+            verb, url, query, body, deprecation_warning, iterator=iterator
+        )
 
     # Add signature to function, including 'self' for class method
-    sig_self = create_signature(["self"] + sig_args, sig_opt_args)
+    sig_self = create_signature(sig_args, sig_opt_args, prepend_self=True)
     f.__signature__ = sig_self
     f.__doc__ = doc
     f.__name__ = str(method_name)
     return f
 
 
-def raise_for_unexpected_kwargs(method_name, arguments, sig_args, sig_kwargs,
-                                is_iterable):
+def raise_for_unexpected_kwargs(
+    method_name, arguments, sig_args, sig_kwargs, is_iterable
+):
     """Raise TypeError if arguments are not in sig_args or sig_kwargs."""
-    expected = set(sig_args) | set(sig_kwargs)
+    expected = set(sig_args.keys()) | set(sig_kwargs.keys())
     if is_iterable:
-        expected |= {'iterator'}
+        expected |= {"iterator"}
     unexpected = set(arguments.keys()) - expected
     if unexpected:
         msg_fmt = "{}() got an unexpected keyword argument(s) {}"
         raise TypeError(msg_fmt.format(method_name, str(unexpected)))
 
 
 def bracketed(x):
     return re.search("^{.*}$", x)
 
 
 def parse_param(param):
-    """ Parse a parameter into a list of dictionaries which can
+    """Parse a parameter into a list of dictionaries which can
     be used to add the parameter to a dynamically generated function.
     """
-    doc = ""
     args = []
-    param_in = param['in']
-    if param_in == 'body':
+    param_in = param["in"]
+    if param_in == "body":
         body_args = parse_param_body(param)
         args.extend(body_args)
     else:
-        snake_name = camel_to_snake(param['name'])
-        req = param['required']
+        snake_name = camel_to_snake(param["name"])
+        req = param["required"]
         doc = doc_from_param(param)
-        a = {"name": snake_name, "in": param_in, "required": req, "doc": doc}
+        a = {
+            "name": snake_name,
+            "in": param_in,
+            "required": req,
+            "doc": doc,
+            "type": type_from_param(param),
+        }
+        if not req:
+            a["default"] = param.get("default", DEFAULT_ARG_VALUE)
         args.append(a)
     return args
 
 
 def parse_params(parameters, summary, verb):
-    """ Parse the parameters of a function specification into a list
+    """Parse the parameters of a function specification into a list
     of dictionaries which are used to generate the function at runtime.
     """
     args = []
     for param in parameters:
         args.extend(parse_param(param))
     if iterable_method(verb, (x["name"] for x in args)):
-        iter_arg = {"name": "iterator", "in": None,
-                    "required": False, "doc": ITERATOR_PARAM_DESC}
+        iter_arg = {
+            "name": "iterator",
+            "in": None,
+            "required": False,
+            "doc": ITERATOR_PARAM_DESC,
+            "type": "bool",
+        }
         args.append(iter_arg)
     req_docs = [x["doc"] for x in args if x["required"]]
     opt_docs = [x["doc"] for x in args if not x["required"]]
     param_docs = "".join(req_docs + opt_docs)
     if summary:
         summary_str = "{}\n".format(textwrap.fill(summary, width=79))
     else:
@@ -348,34 +393,46 @@
         docs = "{}\nParameters\n----------\n{}".format(summary_str, param_docs)
     elif summary:
         docs = summary_str
     return args, docs
 
 
 def parse_param_body(parameter):
-    """ Parse the nested element of a parameter into a list of dictionaries
+    """Parse the nested element of a parameter into a list of dictionaries
     which can be used to add the parameter to a dynamically generated
     function.
     """
-    schema = parameter['schema']
-    properties = schema['properties']
-    req = schema.get('required', [])
+    schema = parameter["schema"]
+    try:
+        properties = schema["properties"]
+    except KeyError:
+        print(schema)
+        raise
+    req = schema.get("required", [])
     arguments = []
     for name, prop in properties.items():
         snake_name = camel_to_snake(name)
         is_req = name in req
         doc_list = docs_from_property(name, prop, properties, 0, not is_req)
         doc = "\n".join(doc_list) + "\n"
-        a = {"name": snake_name, "in": "body", "required": is_req, "doc": doc}
+        a = {
+            "name": snake_name,
+            "in": "body",
+            "required": is_req,
+            "doc": doc,
+            "type": type_from_param(prop),
+        }
+        if not is_req:
+            a["default"] = prop.get("default", DEFAULT_ARG_VALUE)
         arguments.append(a)
     return arguments
 
 
 def parse_method_name(verb, path):
-    """ Create method name from endpoint path
+    """Create method name from endpoint path
 
     Create method name as the http verb (method) followed by
     any static path parameters. As there is ambiguity where
     a path may optionally have a path parameter passed (i.e.
     GET reports/ and GET reports/{id}), any GET method is changed
     to "list" for endpoints where the final path parameter is
     static.
@@ -394,88 +451,93 @@
     path_elems = path.split("/")[1:]
     name_elems = []
     for i, elem in enumerate(path_elems):
         prev_elem = path_elems[i - 1] if i > 0 else None
         if not bracketed(elem):
             name_elems.append(elem)
         elif prev_elem and bracketed(prev_elem):
-            name_elems.append(prev_elem.strip('{|}'))
+            name_elems.append(prev_elem.strip("{|}"))
     final_elem = path_elems[-1] if path_elems else ""
     verb = "list" if verb == "get" and (not bracketed(final_elem)) else verb
     path_name = "_".join(name_elems)
     method_name = "_".join((verb, path_name)) if path_name else verb
     return re.sub("-", "_", method_name)
 
 
 def parse_method(verb, operation, path):
-    """ Generate a python function from a specification of that function."""
+    """Generate a python function from a specification of that function."""
     summary = operation["summary"]
-    params = operation["parameters"]
+    params = operation.get("parameters", [])
     responses = operation["responses"]
-    deprecated = operation.get('deprecated', False)
-    if 'deprecated' in summary.lower() or deprecated:
+    deprecation_warning = operation.get("x-deprecation-warning", None)
+    if "deprecated" in summary.lower():
         return None
 
     args, param_doc = parse_params(params, summary, verb)
-    response_doc = doc_from_responses(responses)
-    docs = join_doc_elements(param_doc, response_doc)
+    elements = split_method_params(params)
+    _, _, _, query_params, _ = elements
+    is_iterable = iterable_method(verb, query_params)
+    response_doc = doc_from_responses(responses, is_iterable)
     name = parse_method_name(verb, path)
 
-    method = create_method(args, verb, name, path, docs)
+    method = create_method(
+        args, verb, name, path, deprecation_warning, param_doc, response_doc
+    )
     return name, method
 
 
-@deprecate_param('v2.0.0', 'resources')
-def parse_path(path, operations, api_version, resources):
-    """ Parse an endpoint into a class where each valid http request
+def parse_path(path, operations, api_version):
+    """Parse an endpoint into a class where each valid http request
     on that endpoint is converted into a convenience function and
     attached to the class as a method.
     """
-    path = path.strip('/')
-    modified_base_path = re.sub("-", "_", path.split('/')[0].lower())
+    path = path.strip("/")
+    modified_base_path = re.sub("-", "_", path.split("/")[0].lower())
     methods = []
-    if exclude_resource(path, api_version, resources):
+    if exclude_resource(path, api_version):
         return modified_base_path, methods
     for verb, op in operations.items():
         method = parse_method(verb, op, path)
         if method is None:
             continue
         methods.append(method)
     return modified_base_path, methods
 
 
-@deprecate_param('v2.0.0', 'resources')
-def parse_api_spec(api_spec, api_version, resources):
-    """ Dynamically create classes to interface with the Civis API.
+def parse_api_spec(api_spec, api_version):
+    """Dynamically create classes to interface with the Civis API.
 
     Parse an OpenAPI (Swagger) specification into a dictionary of classes
     where each class represents an endpoint resource and contains
     methods to make http requests on that resource.
 
     Parameters
     ----------
     api_spec : OrderedDict
         The Civis API specification to parse.  References should be resolved
         before passing, typically using jsonref.JsonRef().
     api_version : string, optional
         The version of endpoints to call. May instantiate multiple client
         objects with different versions.  Currently only "1.0" is supported.
-    resources : string, optional
-        When set to "base", only the default endpoints will be exposed in the
-        client object.  Set to "all" to include all endpoints available for
-        a given user, including those that may be in development and subject
-        to breaking changes at a later date.
     """
-    paths = api_spec['paths']
+    paths = api_spec["paths"]
     classes = {}
     for path, ops in paths.items():
-        base_path, methods = parse_path(path, ops, api_version, resources)
-        class_name = to_camelcase(base_path)
+        base_path, methods = parse_path(path, ops, api_version)
+        class_name = base_path.title()
         if methods and classes.get(base_path) is None:
-            classes[base_path] = type(str(class_name), (Endpoint,), {})
+            cls = type(class_name, (Endpoint,), {})
+            cls.__doc__ = (
+                "Examples\n"
+                "--------\n"
+                ">>> import civis\n"
+                ">>> client = civis.APIClient()\n"
+                f">>> client.{base_path}.{methods[0][0]}(...)"
+            )
+            classes[base_path] = cls
         for method_name, method in methods:
             setattr(classes[base_path], method_name, method)
     return classes
 
 
 @lru_cache(maxsize=4)
 def get_api_spec(api_key, api_version="1.0", user_agent="civis-python"):
@@ -489,31 +551,32 @@
         The version of endpoints to call. May instantiate multiple client
         objects with different versions.  Currently only "1.0" is supported.
     user_agent : string, optional
         Provide this user agent to the the Civis API, along with an
         API client version tag and ``requests`` version tag.
     """
     if api_version == "1.0":
-        with open_session(api_key, MAX_RETRIES, user_agent=user_agent) as sess:
-            response = sess.get("{}endpoints".format(get_base_url()))
+        with open_session(api_key, user_agent=user_agent) as sess:
+            request = Request("GET", "{}endpoints".format(get_base_url()))
+            pre_request = sess.prepare_request(request)
+            response = retry_request("get", pre_request, sess, MAX_RETRIES)
     else:
         msg = "API specification for api version {} cannot be found"
         raise ValueError(msg.format(api_version))
     if response.status_code in (401, 403):
         msg = "{} error downloading API specification. API key may be expired."
         raise requests.exceptions.HTTPError(msg.format(response.status_code))
     response.raise_for_status()
     spec = response.json(object_pairs_hook=OrderedDict)
     return spec
 
 
 @lru_cache(maxsize=4)
-@deprecate_param('v2.0.0', 'resources')
-def generate_classes(api_key, api_version="1.0", resources="all"):
-    """ Dynamically create classes to interface with the Civis API.
+def generate_classes(api_key, api_version="1.0"):
+    """Dynamically create classes to interface with the Civis API.
 
     The Civis API documents behavior using an OpenAPI/Swagger specification.
     This function parses the specification and returns a dictionary of
     classes to provide a convenient method to make requests to the Civis
     API and to view documentation.
 
     https://github.com/OAI/OpenAPI-Specification
@@ -521,27 +584,23 @@
     Parameters
     ----------
     api_key : str
         Your API key obtained from the Civis Platform.
     api_version : string, optional
         The version of endpoints to call. May instantiate multiple client
         objects with different versions.  Currently only "1.0" is supported.
-    resources : string, optional
-        When set to "base", only the default endpoints will be exposed in the
-        client object.  Set to "all" to include all endpoints available for
-        a given user, including those that may be in development and subject
-        to breaking changes at a later date.
-    """
-    assert api_version in API_VERSIONS, (
-        "APIClient api_version must be one of {}".format(API_VERSIONS))
-    assert resources in ["base", "all"], (
-        "resources must be one of {}".format(["base", "all"]))
+    """
+    if api_version not in API_VERSIONS:
+        raise ValueError(
+            f"APIClient api_version must be one of {set(API_VERSIONS)}: "
+            f"{api_version}"
+        )
     raw_spec = get_api_spec(api_key, api_version)
     spec = JsonRef.replace_refs(raw_spec)
-    return parse_api_spec(spec, api_version, resources)
+    return parse_api_spec(spec, api_version)
 
 
 def cache_api_spec(cache=CACHED_SPEC_PATH, api_key=None, api_version="1.0"):
     """Cache a local copy of the Civis Data Science API spec
 
     Parameters
     ----------
@@ -556,47 +615,23 @@
     """
     api_key = get_api_key(api_key)
     spec = get_api_spec(api_key, api_version=api_version)
     with open(cache, "wt") as _fout:
         json.dump(spec, _fout)
 
 
-@deprecate_param('v2.0.0', 'resources')
-def generate_classes_maybe_cached(cache, api_key, api_version, resources):
+def generate_classes_maybe_cached(cache, api_key, api_version):
     """Generate class objects either from /endpoints or a local cache."""
     if cache is None:
-        classes = generate_classes(api_key, api_version, resources)
+        classes = generate_classes(api_key, api_version)
     else:
         if isinstance(cache, OrderedDict):
             raw_spec = cache
         elif isinstance(cache, str):
             with open(cache, "r") as f:
                 raw_spec = json.load(f, object_pairs_hook=OrderedDict)
         else:
             msg = "cache must be an OrderedDict or str, given {}"
             raise ValueError(msg.format(type(cache)))
         spec = JsonRef.replace_refs(raw_spec)
-        classes = parse_api_spec(spec, api_version, resources)
-    classes_ = _add_no_underscore_compatibility(classes)
-    return classes_
-
-
-def _add_no_underscore_compatibility(classes):
-    """ Add class names without underscores for compatibility.
-
-    Previously, no resources had underscores in APIClient.  Parsing of
-    resources has been fixed so now these resources will have underscores.
-    This adds an extra class for those resources without an underscore
-    for compatibility. Additionally, this removes the resource "feature_flags"
-    as APIClient has a name collision with this resource. This will
-    be removed in v2.0.0.
-    """
-    new = ["bocce_clusters", "match_targets", "remote_hosts", "feature_flags"]
-    classes_ = {}
-    class_names = list(classes.keys())
-    for class_name in class_names:
-        if class_name != "feature_flags":
-            classes_[class_name] = classes[class_name]
-        if class_name in new:
-            class_name_no_us = "".join(class_name.split("_"))
-            classes_[class_name_no_us] = classes[class_name]
-    return classes_
+        classes = parse_api_spec(spec, api_version)
+    return classes
```

### Comparing `civis-1.9.4/civis/io/_databases.py` & `civis-2.0.0/src/civis/io/_databases.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from __future__ import absolute_import
+import logging
 
 from civis import APIClient
 from civis._utils import maybe_get_random_name
 from civis.futures import CivisFuture
-from civis._deprecation import deprecate_param
 
+log = logging.getLogger(__name__)
 
-@deprecate_param('v2.0.0', 'api_key')
-def query_civis(sql, database, api_key=None, client=None, credential_id=None,
-                preview_rows=10, polling_interval=None, hidden=True):
+
+def query_civis(
+    sql,
+    database,
+    client=None,
+    credential_id=None,
+    preview_rows=10,
+    polling_interval=None,
+    hidden=True,
+):
     """Execute a SQL statement as a Civis query.
 
     Run a query that may return no results or where only a small
     preview is required. To execute a query that returns a large number
     of rows, see :func:`~civis.io.read_civis_sql`.
 
     Parameters
     ----------
     sql : str
         The SQL statement to execute.
     database : str or int
         The name or ID of the database.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     credential_id : str or int, optional
         The ID of the database credential. If ``None``, the default
         credential will be used.
     preview_rows : int, optional
@@ -41,35 +45,46 @@
     Returns
     -------
     results : :class:`~civis.futures.CivisFuture`
         A `CivisFuture` object.
 
     Examples
     --------
-    >>> run = query_civis(sql="DELETE schema.table", database='database')
+    >>> import civis
+    >>> run = civis.io.query_civis(sql="DELETE schema.table", database='database')
     >>> run.result()  # Wait for query to complete
     """
     if client is None:
-        client = APIClient(api_key=api_key)
+        client = APIClient()
     database_id = client.get_database_id(database)
     cred_id = credential_id or client.default_credential
-    resp = client.queries.post(database_id,
-                               sql,
-                               preview_rows,
-                               credential=cred_id,
-                               hidden=hidden)
-    return CivisFuture(client.queries.get, (resp.id, ), polling_interval,
-                       client=client, poll_on_creation=False)
-
-
-@deprecate_param('v2.0.0', 'api_key')
-def transfer_table(source_db, dest_db, source_table, dest_table,
-                   job_name=None, api_key=None, client=None,
-                   source_credential_id=None, dest_credential_id=None,
-                   polling_interval=None, **advanced_options):
+    resp = client.queries.post(
+        database_id, sql, preview_rows, credential=cred_id, hidden=hidden
+    )
+    return CivisFuture(
+        client.queries.get,
+        (resp.id,),
+        polling_interval,
+        client=client,
+        poll_on_creation=False,
+    )
+
+
+def transfer_table(
+    source_db,
+    dest_db,
+    source_table,
+    dest_table,
+    job_name=None,
+    client=None,
+    source_credential_id=None,
+    dest_credential_id=None,
+    polling_interval=None,
+    **advanced_options,
+):
     """Transfer a table from one location to another.
 
     Parameters
     ----------
     source_db : str or int
         The name of the database where the source table is located.
         Optionally, could be the database ID.
@@ -80,17 +95,14 @@
         Full name of the table to transfer, e.g., ``'schema.table'``.
     dest_table : str
         Full name of the table in the destination database, e.g.,
         ``'schema.table'``.
     job_name : str, optional
         A name to give the job. If omitted, a random job name will be
         used.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     source_credential_id : str or int, optional
         Optional credential ID for the source database. If ``None``, the
         default credential will be used.
     dest_credential_id : str or int, optional
@@ -105,36 +117,44 @@
     Returns
     -------
     results : :class:`~civis.futures.CivisFuture`
         A `CivisFuture` object.
 
     Examples
     --------
-    >>> transfer_table(source_db='Cluster A', dest_db='Cluster B',
-    ...                source_table='schma.tbl', dest_table='schma.tbl')
+    >>> import civis
+    >>> civis.io.transfer_table(source_db='Cluster A', dest_db='Cluster B',
+    ...                         source_table='schma.tbl', dest_table='schma.tbl')
     """
     if client is None:
-        client = APIClient(api_key=api_key)
+        client = APIClient()
     source_cred_id = source_credential_id or client.default_credential
     dest_cred_id = dest_credential_id or client.default_credential
     job_name = maybe_get_random_name(job_name)
     source = {
-        'remote_host_id': client.get_database_id(source_db),
-        'credential_id': source_cred_id
+        "remote_host_id": client.get_database_id(source_db),
+        "credential_id": source_cred_id,
     }
     destination = {
-        'remote_host_id': client.get_database_id(dest_db),
-        'credential_id': dest_cred_id
+        "remote_host_id": client.get_database_id(dest_db),
+        "credential_id": dest_cred_id,
     }
-    job_id = client.imports.post(job_name, "Dbsync", True, source=source,
-                                 destination=destination).id
-
-    client.imports.post_syncs(id=job_id,
-                              source={'path': source_table},
-                              destination={'path': dest_table},
-                              advanced_options=advanced_options)
+    job_id = client.imports.post(
+        job_name, "Dbsync", True, source=source, destination=destination
+    ).id
+
+    client.imports.post_syncs(
+        id=job_id,
+        source={"path": source_table},
+        destination={"path": dest_table},
+        advanced_options=advanced_options,
+    )
     run_id = client.imports.post_runs(id=job_id).run_id
-
-    fut = CivisFuture(client.imports.get_files_runs, (job_id, run_id),
-                      polling_interval=polling_interval, client=client,
-                      poll_on_creation=False)
+    log.debug("Started run %d of sync for import %d", run_id, job_id)
+    fut = CivisFuture(
+        client.imports.get_files_runs,
+        (job_id, run_id),
+        polling_interval=polling_interval,
+        client=client,
+        poll_on_creation=False,
+    )
     return fut
```

### Comparing `civis-1.9.4/civis/io/_tables.py` & `civis-2.0.0/src/civis/io/_tables.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,77 @@
+import collections
 import json
+import concurrent.futures
 import csv
 from os import path
 import io
 import logging
 import os
-import re
-import six
 import shutil
+from tempfile import TemporaryDirectory
 import warnings
 import zlib
 
+from typing import Dict, List
+
 import gzip
 import zipfile
 
 from civis import APIClient
 from civis._utils import maybe_get_random_name
-from civis.base import EmptyResultError
-from civis.compat import TemporaryDirectory
+from civis.base import EmptyResultError, CivisImportError, CivisAPIError
 from civis.futures import CivisFuture
-from civis.io import civis_to_file, file_to_civis, query_civis
-from civis._deprecation import deprecate_param
+from civis.io import civis_to_file, file_to_civis
+from civis.utils import run_job
 
 import requests
 
 try:
-    from io import StringIO
-except ImportError:
-    from cStringIO import StringIO
-try:
     import pandas as pd
+
     NO_PANDAS = False
 except ImportError:
     NO_PANDAS = True
 
 CHUNK_SIZE = 32 * 1024
 log = logging.getLogger(__name__)
-__all__ = ['read_civis', 'read_civis_sql', 'civis_to_csv',
-           'civis_to_multifile_csv', 'dataframe_to_civis', 'csv_to_civis',
-           'civis_file_to_table', 'split_schema_tablename',
-           'export_to_civis_file']
+__all__ = [
+    "read_civis",
+    "read_civis_sql",
+    "civis_to_csv",
+    "civis_to_multifile_csv",
+    "dataframe_to_civis",
+    "csv_to_civis",
+    "civis_file_to_table",
+    "split_schema_tablename",
+    "export_to_civis_file",
+]
 
 DELIMITERS = {
-    ',': 'comma',
-    '\t': 'tab',
-    '|': 'pipe',
+    ",": "comma",
+    "\t": "tab",
+    "|": "pipe",
 }
 
+_File = collections.namedtuple("_File", "id name detected_info")
+
 
-@deprecate_param('v2.0.0', 'api_key')
-def read_civis(table, database, columns=None, use_pandas=False,
-               job_name=None, api_key=None, client=None, credential_id=None,
-               polling_interval=None, archive=False, hidden=True, **kwargs):
+def read_civis(
+    table,
+    database,
+    columns=None,
+    use_pandas=False,
+    encoding=None,
+    job_name=None,
+    client=None,
+    credential_id=None,
+    polling_interval=None,
+    hidden=True,
+    **kwargs,
+):
     """Read data from a Civis table.
 
     Parameters
     ----------
     table : str
         Name of table, including schema, in the database. E.g.
         ``'my_schema.my_table'``. Schemas or tablenames with periods must
@@ -63,95 +80,111 @@
         Read data from this database. Can be the database name or ID.
     columns : list, optional
         A list of column names. Column SQL transformations are possible.
         If omitted, all columns are exported.
     use_pandas : bool, optional
         If ``True``, return a :class:`pandas:pandas.DataFrame`. Otherwise,
         return a list of results from :func:`python:csv.reader`.
+    encoding : str, optional
+        If ``use_pandas`` is ``True``, this parameter is passed to
+        the ``encoding`` kwarg of :func:`pandas:pandas.read_csv`.
+        If ``use_pandas`` is ``False``, and if this parameter isn't provided,
+        then the UTF-8 encoding is assumed. In case you encounter
+        a ``UnicodeDecodeError``, consider choosing an encoding suitable
+        for your data; see the `list of standard encodings
+        <https://docs.python.org/3/library/codecs.html#standard-encodings>`_.
     job_name : str, optional
         A name to give the job. If omitted, a random job name will be
         used.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     credential_id : str or int, optional
         The database credential ID.  If ``None``, the default credential
         will be used.
     polling_interval : int or float, optional
         Number of seconds to wait between checks for query completion.
-    archive : bool, optional (deprecated)
-        If ``True``, archive the import job as soon as it completes.
     hidden : bool, optional
         If ``True`` (the default), this job will not appear in the Civis UI.
     **kwargs : kwargs
         Extra keyword arguments are passed into
-        :func:`pandas:pandas.read_csv` if `use_pandas` is ``True`` or
-        passed into :func:`python:csv.reader` if `use_pandas` is
+        :func:`pandas:pandas.read_csv` if ``use_pandas`` is ``True`` or
+        passed into :func:`python:csv.reader` if ``use_pandas`` is
         ``False``.
 
     Returns
     -------
     data : :class:`pandas:pandas.DataFrame` or list
-        A list of rows (with header as first row) if `use_pandas` is
-        ``False``, otherwise a `pandas` `DataFrame`. Note that if
-        `use_pandas` is ``False``, no parsing of types is performed and
+        A list of rows (with header as first row) if ``use_pandas`` is
+        ``False``, otherwise a :class:`pandas:pandas.DataFrame`. Note that if
+        ``use_pandas`` is ``False``, no parsing of types is performed and
         each row will be a list of strings.
 
     Raises
     ------
     ImportError
-        If `use_pandas` is ``True`` and `pandas` is not installed.
+        If ``use_pandas`` is ``True`` and pandas is not installed.
+    EmptyResultError
+        If the table is empty.
 
     Examples
     --------
+    >>> import civis
     >>> table = "schema.table"
     >>> database = "my_data"
     >>> columns = ["column_a", "ROW_NUMBER() OVER(ORDER BY date) AS order"]
-    >>> data = read_civis(table, database, columns=columns)
+    >>> data = civis.io.read_civis(table, database, columns=columns)
     >>> columns = data.pop(0)
     >>> col_a_index = columns.index("column_a")
     >>> col_a = [row[col_a_index] for row in data]
 
-    >>> df = read_civis("schema.table", "my_data", use_pandas=True)
+    >>> df = civis.io.read_civis("schema.table", "my_data", use_pandas=True)
     >>> col_a = df["column_a"]
 
     See Also
     --------
     civis.io.read_civis_sql : Read directly into memory using SQL.
     civis.io.civis_to_csv : Write directly to csv.
     civis.io.export_to_civis_file : Store a SQL query's results in a Civis file
     """
     if use_pandas and NO_PANDAS:
         raise ImportError("use_pandas is True but pandas is not installed.")
-    if archive:
-        warnings.warn("`archive` is deprecated and will be removed in v2.0.0. "
-                      "Use `hidden` instead.", FutureWarning)
     if client is None:
-        # Instantiate client here in case users provide a (deprecated) api_key
-        client = APIClient(api_key=api_key)
+        client = APIClient()
     sql = _get_sql_select(table, columns)
-    data = read_civis_sql(sql=sql, database=database, use_pandas=use_pandas,
-                          job_name=job_name, client=client,
-                          credential_id=credential_id,
-                          polling_interval=polling_interval,
-                          archive=archive, hidden=hidden, **kwargs)
+    data = read_civis_sql(
+        sql=sql,
+        database=database,
+        use_pandas=use_pandas,
+        encoding=encoding,
+        job_name=job_name,
+        client=client,
+        credential_id=credential_id,
+        polling_interval=polling_interval,
+        hidden=hidden,
+        **kwargs,
+    )
     return data
 
 
-def export_to_civis_file(sql, database, job_name=None, client=None,
-                         credential_id=None, polling_interval=None,
-                         hidden=True, csv_settings=None):
+def export_to_civis_file(
+    sql,
+    database,
+    job_name=None,
+    client=None,
+    credential_id=None,
+    polling_interval=None,
+    hidden=True,
+    csv_settings=None,
+):
     """Store results of a query to a Civis file
 
     Parameters
     ----------
-    sql : str, optional
+    sql : str
         The SQL select string to be executed.
     database : str or int
         Execute the query against this database. Can be the database name
         or ID.
     job_name : str, optional
         A name to give the job. If omitted, a random job name will be
         used.
@@ -174,218 +207,218 @@
     fut : :class:`~civis.futures.CivisFuture`
         A future which returns the response from
         :func:`civis.APIClient.scripts.get_sql_runs` after the sql query
         has completed and the result has been stored as a Civis file.
 
     Examples
     --------
+    >>> import civis
     >>> sql = "SELECT * FROM schema.table"
-    >>> fut = export_to_civis_file(sql, "my_database")
+    >>> fut = civis.io.export_to_civis_file(sql, "my_database")
     >>> file_id = fut.result()['output'][0]["file_id"]
 
 
     See Also
     --------
     civis.io.read_civis : Read directly into memory without SQL.
     civis.io.read_civis_sql : Read results of a SQL query into memory.
     civis.io.civis_to_csv : Write directly to a CSV file.
     civis.io.civis_file_to_table : Upload a Civis file to a Civis table
     """
     client = client or APIClient()
-    script_id, run_id = _sql_script(client=client,
-                                    sql=sql,
-                                    database=database,
-                                    job_name=job_name,
-                                    credential_id=credential_id,
-                                    csv_settings=csv_settings,
-                                    hidden=hidden)
-    fut = CivisFuture(client.scripts.get_sql_runs, (script_id, run_id),
-                      polling_interval=polling_interval, client=client,
-                      poll_on_creation=False)
+    script_id, run_id = _sql_script(
+        client=client,
+        sql=sql,
+        database=database,
+        job_name=job_name,
+        credential_id=credential_id,
+        csv_settings=csv_settings,
+        hidden=hidden,
+    )
+    fut = CivisFuture(
+        client.scripts.get_sql_runs,
+        (script_id, run_id),
+        polling_interval=polling_interval,
+        client=client,
+        poll_on_creation=False,
+    )
     return fut
 
 
-@deprecate_param('v2.0.0', 'api_key')
-def read_civis_sql(sql, database, use_pandas=False, job_name=None,
-                   api_key=None, client=None, credential_id=None,
-                   polling_interval=None, archive=False,
-                   hidden=True, **kwargs):
+def read_civis_sql(
+    sql,
+    database,
+    use_pandas=False,
+    encoding=None,
+    job_name=None,
+    client=None,
+    credential_id=None,
+    polling_interval=None,
+    hidden=True,
+    **kwargs,
+):
     """Read data from Civis using a custom SQL string.
 
-    The custom SQL string will be executed twice; once to attempt to
-    retrieve headers and once to retrieve the data. This is done to
-    use a more performant method for retrieving the data. The first
-    execution of the custom SQL is controlled such that changes in
-    state cannot occur (e.g., INSERT, UPDATE, DELETE, etc.).
+    If no data is expected to return from the query,
+    consider :func:`~civis.io.query_civis` instead.
 
     Parameters
     ----------
-    sql : str, optional
+    sql : str
         The SQL select string to be executed.
     database : str or int
         Execute the query against this database. Can be the database name
         or ID.
     use_pandas : bool, optional
         If ``True``, return a :class:`pandas:pandas.DataFrame`. Otherwise,
         return a list of results from :func:`python:csv.reader`.
+    encoding : str, optional
+        If ``use_pandas`` is ``True``, this parameter is passed to
+        the ``encoding`` kwarg of :func:`pandas:pandas.read_csv`.
+        If ``use_pandas`` is ``False``, and if this parameter isn't provided,
+        then the UTF-8 encoding is assumed. In case you encounter
+        a ``UnicodeDecodeError``, consider choosing an encoding suitable
+        for your data; see the `list of standard encodings
+        <https://docs.python.org/3/library/codecs.html#standard-encodings>`_.
     job_name : str, optional
         A name to give the job. If omitted, a random job name will be
         used.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     credential_id : str or int, optional
         The database credential ID.  If ``None``, the default credential
         will be used.
     polling_interval : int or float, optional
         Number of seconds to wait between checks for query completion.
-    archive : bool, optional (deprecated)
-        If ``True``, archive the import job as soon as it completes.
     hidden : bool, optional
         If ``True`` (the default), this job will not appear in the Civis UI.
     **kwargs : kwargs
         Extra keyword arguments are passed into
-        :func:`pandas:pandas.read_csv` if `use_pandas` is ``True`` or
-        passed into :func:`python:csv.reader` if `use_pandas` is
+        :func:`pandas:pandas.read_csv` if ``use_pandas`` is ``True`` or
+        passed into :func:`python:csv.reader` if ``use_pandas`` is
         ``False``.
 
     Returns
     -------
     data : :class:`pandas:pandas.DataFrame` or list
-        A list of rows (with header as first row) if `use_pandas` is
-        ``False``, otherwise a `pandas` `DataFrame`. Note that if
-        `use_pandas` is ``False``, no parsing of types is performed and
+        A list of rows (with header as first row) if ``use_pandas`` is
+        ``False``, otherwise a :class:`pandas:pandas.DataFrame`. Note that if
+        ``use_pandas`` is ``False``, no parsing of types is performed and
         each row will be a list of strings.
 
     Raises
     ------
     ImportError
-        If `use_pandas` is ``True`` and `pandas` is not installed.
+        If ``use_pandas`` is ``True`` and pandas is not installed.
+    EmptyResultError
+        If no rows were returned as a result of the query.
 
     Examples
     --------
+    >>> import civis
     >>> sql = "SELECT * FROM schema.table"
-    >>> df = read_civis_sql(sql, "my_database", use_pandas=True)
+    >>> df = civis.io.read_civis_sql(sql, "my_database", use_pandas=True)
     >>> col_a = df["column_a"]
 
-    >>> data = read_civis_sql(sql, "my_database")
+    >>> data = civis.io.read_civis_sql(sql, "my_database")
     >>> columns = data.pop(0)
     >>> col_a_index = columns.index("column_a")
     >>> col_a = [row[col_a_index] for row in data]
 
     Notes
     -----
     This reads the data into memory.
 
     See Also
     --------
     civis.io.read_civis : Read directly into memory without SQL.
     civis.io.civis_to_csv : Write directly to a CSV file.
     """
     if client is None:
-        client = APIClient(api_key=api_key)
+        client = APIClient()
     if use_pandas and NO_PANDAS:
         raise ImportError("use_pandas is True but pandas is not installed.")
-    if archive:
-        warnings.warn("`archive` is deprecated and will be removed in v2.0.0. "
-                      "Use `hidden` instead.", FutureWarning)
 
     db_id = client.get_database_id(database)
     credential_id = credential_id or client.default_credential
 
-    # determine if we can request headers separately; if we can then Platform
-    # will perform a parallel unload which is significantly more performant
-    # we start by assuming headers are requested
-    ovrd_include_header, headers = _include_header(client, sql, True,
-                                                   db_id, credential_id,
-                                                   polling_interval)
-
-    # if we retrieved headers then we are performing a parallel unload
-    # in which case we need to specify backslash as the escapechar
-    if headers is not None:
-        kwargs['escapechar'] = '\\'
-
-    csv_settings = dict(include_header=ovrd_include_header,
-                        compression='gzip')
-
-    script_id, run_id = _sql_script(client, sql, db_id,
-                                    job_name, credential_id,
-                                    csv_settings=csv_settings,
-                                    hidden=hidden)
-    fut = CivisFuture(client.scripts.get_sql_runs, (script_id, run_id),
-                      polling_interval=polling_interval, client=client,
-                      poll_on_creation=False)
-    if archive:
-
-        def f(x):
-            return client.scripts.put_sql_archive(script_id, True)
-
-        fut.add_done_callback(f)
+    script_id, run_id = _sql_script(
+        client,
+        sql,
+        db_id,
+        job_name,
+        credential_id,
+        csv_settings={"compression": "gzip"},
+        hidden=hidden,
+    )
+    fut = CivisFuture(
+        client.scripts.get_sql_runs,
+        (script_id, run_id),
+        polling_interval=polling_interval,
+        client=client,
+        poll_on_creation=False,
+    )
     fut.result()
     outputs = client.scripts.get_sql_runs(script_id, run_id)["output"]
     if not outputs:
-        raise EmptyResultError("Query {} returned no output."
-                               .format(script_id))
+        raise EmptyResultError("Query {} returned no output.".format(script_id))
 
     url = outputs[0]["path"]
     file_id = outputs[0]["file_id"]
-    log.debug('Exported results to Civis file %s (%s)',
-              outputs[0]["output_name"], file_id)
+    log.debug(
+        "Exported results to Civis file %s (%s)", outputs[0]["output_name"], file_id
+    )
 
     if use_pandas:
-        # allows users to enter their own names parameter
-        _kwargs = {'names': headers}
-        _kwargs.update(kwargs)
-        _kwargs['compression'] = 'gzip'
+        kwargs["compression"] = "gzip"
+        kwargs["encoding"] = encoding
 
-        data = pd.read_csv(url, **_kwargs)
+        data = pd.read_csv(url, **kwargs)
     else:
-        response = requests.get(url, stream=True)
+        response = requests.get(url, stream=True, timeout=60)
         response.raise_for_status()
 
-        with StringIO() as buf:
-            if headers:
-                buf.write(','.join(headers) + '\n')
-            _decompress_stream(response, buf, write_bytes=False)
+        with io.StringIO() as buf:
+            _decompress_stream(
+                response, buf, write_bytes=False, encoding=encoding or "utf-8"
+            )
             buf.seek(0)
             data = list(csv.reader(buf, **kwargs))
 
     return data
 
 
-@deprecate_param('v2.0.0', 'api_key')
-def civis_to_csv(filename, sql, database, job_name=None, api_key=None,
-                 client=None, credential_id=None, include_header=True,
-                 compression='none', delimiter=',', unquoted=False,
-                 archive=False, hidden=True, polling_interval=None):
+def civis_to_csv(
+    filename,
+    sql,
+    database,
+    job_name=None,
+    client=None,
+    credential_id=None,
+    include_header=True,
+    compression="none",
+    delimiter=",",
+    unquoted=False,
+    hidden=True,
+    polling_interval=None,
+):
     """Export data from Civis to a local CSV file.
 
-    The custom SQL string will be executed twice; once to attempt to
-    retrieve headers and once to retrieve the data. This is done to
-    use a more performant method for retrieving the data. The first
-    execution of the custom SQL is controlled such that changes in
-    state cannot occur (e.g., INSERT, UPDATE, DELETE, etc.).
-
     Parameters
     ----------
     filename : str
         Download exported data into this file.
-    sql : str, optional
+    sql : str
         The SQL select string to be executed.
     database : str or int
         Export data from this database. Can be the database name or ID.
     job_name : str, optional
         A name to give the job. If omitted, a random job name will be
         used.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     credential_id : str or int, optional
         The ID of the database credential.  If ``None``, the default
         credential will be used.
     include_header: bool, optional
@@ -400,114 +433,128 @@
     delimiter: str, optional
         Which delimiter to use, if any. One of ``','``, ``'\t'``, or
         ``'|'``. Default: ``','``.
     unquoted: bool, optional
         Whether or not to quote fields. Default: ``False``.
     polling_interval : int or float, optional
         Number of seconds to wait between checks for query completion.
-    archive : bool, optional (deprecated)
-        If ``True``, archive the import job as soon as it completes.
     hidden : bool, optional
         If ``True`` (the default), this job will not appear in the Civis UI.
 
     Returns
     -------
     results : :class:`~civis.futures.CivisFuture`
-        A `CivisFuture` object.
+        A ``CivisFuture`` object that represents the SQL query that unloads data
+        from Civis Platform. Note that this unloading process has an arbitrary
+        filename assigned and made available through the ``CivisFuture`` object,
+        which is not the same as the `filename` parameter. It is recommended
+        that a separate variable is used to store the desired filename beforehand
+        so that it's accessible after this function finishes,
+        see the code example below.
 
     Examples
     --------
+    >>> import civis
     >>> sql = "SELECT * FROM schema.table"
-    >>> fut = civis_to_csv("file.csv", sql, "my_database")
+    >>> file_path = "file.csv"
+    >>> fut = civis.io.civis_to_csv(file_path, sql, "my_database")
     >>> fut.result()  # Wait for job to complete
+    >>> import pandas as pd  # Let's say we want to read the data into a DataFrame
+    >>> df = pd.read_csv(file_path)
 
     See Also
     --------
     civis.io.read_civis : Read table contents into memory.
     civis.io.read_civis_sql : Read results of a SQL query into memory.
     civis.io.export_to_civis_file : Store a SQL query's results in a Civis file
     """
-    if archive:
-        warnings.warn("`archive` is deprecated and will be removed in v2.0.0. "
-                      "Use `hidden` instead.", FutureWarning)
     if client is None:
-        client = APIClient(api_key=api_key)
+        client = APIClient()
 
     db_id = client.get_database_id(database)
     credential_id = credential_id or client.default_credential
 
     # don't fix bug that would cause breaking change for now
     # when gzip compression is requested, a gzip file is not actually returned
     # instead the gzip file is decompressed during download
-    if compression == 'gzip' and include_header:
-        compression = 'none'
+    if compression == "gzip" and include_header:
+        compression = "none"
 
     # don't support parallel unload; the output format
     # is different which would introduce a breaking change
-    headers = b''
+    headers = b""
 
     delimiter = DELIMITERS.get(delimiter)
     if not delimiter:
-        raise ValueError("delimiter must be one of {}"
-                         .format(DELIMITERS.keys()))
+        raise ValueError("delimiter must be one of {}".format(DELIMITERS.keys()))
 
     # always set compression to gzip to reduce I/O
-    csv_settings = dict(include_header=include_header,
-                        compression='gzip',
-                        column_delimiter=delimiter,
-                        unquoted=unquoted,
-                        filename_prefix=None,
-                        force_multifile=False)
-
-    script_id, run_id = _sql_script(client, sql, db_id, job_name,
-                                    credential_id, hidden=hidden,
-                                    csv_settings=csv_settings)
-    fut = CivisFuture(client.scripts.get_sql_runs, (script_id, run_id),
-                      polling_interval=polling_interval, client=client,
-                      poll_on_creation=False)
-    download = _download_callback(script_id, run_id, filename,
-                                  headers, compression)
+    csv_settings = dict(
+        include_header=include_header,
+        compression="gzip",
+        column_delimiter=delimiter,
+        unquoted=unquoted,
+        filename_prefix=None,
+        force_multifile=False,
+    )
+
+    script_id, run_id = _sql_script(
+        client,
+        sql,
+        db_id,
+        job_name,
+        credential_id,
+        hidden=hidden,
+        csv_settings=csv_settings,
+    )
+    fut = CivisFuture(
+        client.scripts.get_sql_runs,
+        (script_id, run_id),
+        polling_interval=polling_interval,
+        client=client,
+        poll_on_creation=False,
+    )
+    download = _download_callback(script_id, run_id, filename, headers, compression)
     fut.add_done_callback(download)
-    if archive:
-
-        def f(x):
-            return client.scripts.put_sql_archive(script_id, True)
-
-        fut.add_done_callback(f)
 
     return fut
 
 
-@deprecate_param('v2.0.0', 'api_key')
-def civis_to_multifile_csv(sql, database, job_name=None, api_key=None,
-                           client=None, credential_id=None,
-                           include_header=True,
-                           compression='none', delimiter='|',
-                           unquoted=False, prefix=None,
-                           polling_interval=None, hidden=True):
+def civis_to_multifile_csv(
+    sql,
+    database,
+    job_name=None,
+    client=None,
+    credential_id=None,
+    include_header=True,
+    compression="none",
+    delimiter="|",
+    max_file_size=None,
+    unquoted=False,
+    prefix=None,
+    polling_interval=None,
+    hidden=True,
+):
     """Unload the result of SQL query and return presigned urls.
 
     This function is intended for unloading large queries/tables from redshift
     as it uses a 'PARALLEL ON' S3 unload. It returns a similar manifest file
     to conventional S3 UNLOAD statements except the CSV parts are accessible
     via both files endpoint IDs and presigned S3 urls.
 
     Parameters
     ----------
-    sql : str, optional
+    sql : str
         The SQL select string to be executed.
     database : str or int
         Execute the query against this database. Can be the database name
         or ID.
     job_name : str, optional
         A name to give the job. If omitted, a random job name will be
         used.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     credential_id : str or int, optional
         The database credential ID.  If ``None``, the default credential
         will be used.
     include_header: bool, optional
@@ -515,14 +562,16 @@
         of column names. Default: ``True``.
     compression: str, optional
         Type of compression to use, if any. One of ``'none'``, ``'zip'``, or
         ``'gzip'``. Default ``'none'``.
     delimiter: str, optional
         Which delimiter to use, if any. One of ``','``, ``'\t'``, or
         ``'|'``. Default: ``'|'``.
+    max_file_size: int, optional
+        Maximum number of Megabytes each created file will be.
     unquoted: bool, optional
         Whether or not to quote fields. Default: ``False``.
     prefix: str, optional
         A user specified filename prefix for the output file to have. Default:
         ``None``.
     polling_interval : int or float, optional
         Number of seconds to wait between checks for query completion.
@@ -561,301 +610,475 @@
             Type of compression used.
 
         'delimiter': str
             Delimiter that separates the cells.
 
     Examples
     --------
+    >>> import io
+    >>> import civis
+    >>> import pandas as pd
     >>> sql = "SELECT * FROM schema.my_big_table"
     >>> database = "my_database"
     >>> delimiter = "|"
-    >>> manifest = civis_to_multifile_csv(sql, database, delimiter=delimiter)
+    >>> manifest = civis.io.civis_to_multifile_csv(sql, database, delimiter=delimiter)
     >>> ids = [entry['id'] for entry in manifest['entries']]
-    >>> buf = BytesIO()
-    >>> civis_to_file(ids[0], buf)
-    >>> buf.seek(0)
-    >>> df = pd.read_csv(buf, delimiter=delimiter)
+    >>> for file_id in ids:
+    >>>     buf = io.BytesIO()
+    >>>     civis.io.civis_to_file(file_id, buf)
+    >>>     buf.seek(0)
+    >>>     # Process the data in `buf` for your own application, e.g.:
+    >>>     df = pd.read_csv(buf, delimiter=delimiter)
 
     See Also
     --------
     civis.APIClient.scripts.post_sql
     """
     if client is None:
-        client = APIClient(api_key=api_key)
+        client = APIClient()
     delimiter = DELIMITERS.get(delimiter)
-    assert delimiter, "delimiter must be one of {}".format(DELIMITERS.keys())
+    if not delimiter:
+        raise ValueError(f"delimiter must be one of {DELIMITERS.keys()}: {delimiter}")
 
-    csv_settings = dict(include_header=include_header,
-                        compression=compression,
-                        column_delimiter=delimiter,
-                        unquoted=unquoted,
-                        filename_prefix=prefix,
-                        force_multifile=True)
-    script_id, run_id = _sql_script(client, sql, database, job_name,
-                                    credential_id, hidden,
-                                    csv_settings=csv_settings)
-
-    fut = CivisFuture(client.scripts.get_sql_runs, (script_id, run_id),
-                      polling_interval=polling_interval, client=client,
-                      poll_on_creation=False)
+    csv_settings = dict(
+        include_header=include_header,
+        compression=compression,
+        column_delimiter=delimiter,
+        unquoted=unquoted,
+        filename_prefix=prefix,
+        force_multifile=True,
+        max_file_size=max_file_size,
+    )
+    script_id, run_id = _sql_script(
+        client,
+        sql,
+        database,
+        job_name,
+        credential_id,
+        hidden,
+        csv_settings=csv_settings,
+    )
+
+    fut = CivisFuture(
+        client.scripts.get_sql_runs,
+        (script_id, run_id),
+        polling_interval=polling_interval,
+        client=client,
+        poll_on_creation=False,
+    )
 
     outputs = fut.result()["output"]
     if not outputs:
-        raise EmptyResultError("Unload query {} returned no manifest."
-                               .format(script_id))
+        raise EmptyResultError(
+            "Unload query {} returned no manifest.".format(script_id)
+        )
 
     buf = io.BytesIO()
-    civis_to_file(outputs[0]['file_id'], buf, client=client)
-    txt = io.TextIOWrapper(buf, encoding='utf-8')
+    civis_to_file(outputs[0]["file_id"], buf, client=client)
+    txt = io.TextIOWrapper(buf, encoding="utf-8")
     txt.seek(0)
     unload_manifest = json.load(txt)
 
     return unload_manifest
 
 
-@deprecate_param('v2.0.0', 'api_key')
-def dataframe_to_civis(df, database, table, api_key=None, client=None,
-                       max_errors=None, existing_table_rows="fail",
-                       diststyle=None, distkey=None,
-                       sortkey1=None, sortkey2=None,
-                       headers=None, credential_id=None,
-                       polling_interval=None,
-                       archive=False, hidden=True, **kwargs):
-    """Upload a `pandas` `DataFrame` into a Civis table.
-
-    The `DataFrame`'s index will not be included. To store the index
-    along with the other values, use `df.reset_index()` instead
-    of `df` as the first argument to this function.
+def dataframe_to_civis(
+    df,
+    database,
+    table,
+    client=None,
+    max_errors=None,
+    existing_table_rows="fail",
+    diststyle=None,
+    distkey=None,
+    sortkey1=None,
+    sortkey2=None,
+    table_columns=None,
+    credential_id=None,
+    primary_keys=None,
+    last_modified_keys=None,
+    execution="immediate",
+    polling_interval=None,
+    hidden=True,
+    **kwargs,
+):
+    """Upload a pandas dataframe into a Civis table.
+
+    The dataframe's index will not be included. To store the index
+    along with the other values, use ``df.reset_index()`` instead
+    of ``df`` as the first argument to this function.
 
     Parameters
     ----------
     df : :class:`pandas:pandas.DataFrame`
         The `DataFrame` to upload to Civis.
     database : str or int
         Upload data into this database. Can be the database name or ID.
     table : str
         The schema and table you want to upload to. E.g.,
         ``'scratch.table'``. Schemas or tablenames with periods must
         be double quoted, e.g. ``'scratch."my.table"'``.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     max_errors : int, optional
         The maximum number of rows with errors to remove from the import
         before failing.
     existing_table_rows : str, optional
         The behaviour if a table with the requested name already exists.
-        One of ``'fail'``, ``'truncate'``, ``'append'`` or ``'drop'``.
-        Defaults to ``'fail'``.
+        One of ``'fail'``, ``'truncate'``, ``'append'``, ``'drop'``, or
+        ``'upsert'``. Defaults to ``'fail'``.
     diststyle : str, optional
         The distribution style for the table.
         One of ``'even'``, ``'all'`` or ``'key'``.
     distkey : str, optional
         The column to use as the distkey for the table.
     sortkey1 : str, optional
         The column to use as the sortkey for the table.
     sortkey2 : str, optional
         The second column in a compound sortkey for the table.
-    headers : bool, optional
-        Whether or not the first row of the file should be treated as
-        headers. The default, ``None``, attempts to autodetect whether
-        or not the first row contains headers.
+    table_columns : list[Dict[str, str]], optional
+        A list of dictionaries, ordered so each dictionary corresponds
+        to a column in the order that it appears in the source file. Each dict
+        should have a key "name" that corresponds to the column name in the
+        destination table, and a key "sql_type" corresponding to the intended
+        column data type in the destination table. The "sql_type" key is not
+        required when appending to an existing table. The table_columns
+        parameter is required if the table does not exist, the table is being
+        dropped, or the columns in the source file do not appear in the same
+        order as in the destination table. Example:
+        ``[{"name": "foo", "sql_type": "INT"}, {"name": "bar", "sql_type": "VARCHAR"}]``
     credential_id : str or int, optional
         The ID of the database credential.  If ``None``, the default
         credential will be used.
+    primary_keys: list[str], optional
+        A list of the primary key column(s) of the destination table that
+        uniquely identify a record. These columns must not contain null values.
+        If existing_table_rows is "upsert", this
+        field is required. Note that this is true regardless of whether the
+        destination database itself requires a primary key.
+    last_modified_keys: list[str], optional
+        A list of the columns indicating a record has been updated. If
+        existing_table_rows is "upsert", this field is required.
+    execution: string, optional, default "immediate"
+        One of "delayed" or "immediate". If "immediate", refresh column
+        statistics as part of the run. If "delayed", flag the table for a
+        deferred statistics update; column statistics may not be available
+        for up to 24 hours. In addition, if existing_table_rows is "upsert",
+        delayed executions move data from staging table to final table after a
+        brief delay, in order to accommodate multiple concurrent imports to the
+        same destination table.
     polling_interval : int or float, optional
         Number of seconds to wait between checks for job completion.
-    archive : bool, optional (deprecated)
-        If ``True``, archive the import job as soon as it completes.
     hidden : bool, optional
         If ``True`` (the default), this job will not appear in the Civis UI.
     **kwargs : kwargs
         Extra keyword arguments will be passed to
         :meth:`pandas:pandas.DataFrame.to_csv`.
 
     Returns
     -------
     fut : :class:`~civis.futures.CivisFuture`
-        A `CivisFuture` object.
+        A ``CivisFuture`` object.
 
     Examples
     --------
+    >>> import civis
     >>> import pandas as pd
     >>> df = pd.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 6]})
     >>> fut = civis.io.dataframe_to_civis(df, 'my-database',
     ...                                   'scratch.df_table')
     >>> fut.result()
-    """
+
+    See Also
+    --------
+    :func:`~pandas.DataFrame.to_csv`
+    """  # noqa: E501
     if client is None:
-        client = APIClient(api_key=api_key)
-    if archive:
-        warnings.warn("`archive` is deprecated and will be removed in v2.0.0. "
-                      "Use `hidden` instead.", FutureWarning)
+        client = APIClient()
 
+    headers = False if kwargs.get("header") is False else True
     with TemporaryDirectory() as tmp_dir:
-        tmp_path = os.path.join(tmp_dir, 'dataframe_to_civis.csv')
-        to_csv_kwargs = {'encoding': 'utf-8', 'index': False}
+        tmp_path = os.path.join(tmp_dir, "dataframe_to_civis.csv")
+        to_csv_kwargs = {"encoding": "utf-8", "index": False}
         to_csv_kwargs.update(kwargs)
         df.to_csv(tmp_path, **to_csv_kwargs)
         _, name = split_schema_tablename(table)
         file_id = file_to_civis(tmp_path, name, client=client)
 
-    delimiter = ','
-    fut = civis_file_to_table(file_id, database, table,
-                              client=client, max_errors=max_errors,
-                              existing_table_rows=existing_table_rows,
-                              diststyle=diststyle, distkey=distkey,
-                              sortkey1=sortkey1, sortkey2=sortkey2,
-                              delimiter=delimiter, headers=headers,
-                              credential_id=credential_id,
-                              polling_interval=polling_interval,
-                              hidden=hidden)
+    delimiter = ","
+    fut = civis_file_to_table(
+        file_id,
+        database,
+        table,
+        client=client,
+        max_errors=max_errors,
+        existing_table_rows=existing_table_rows,
+        diststyle=diststyle,
+        distkey=distkey,
+        sortkey1=sortkey1,
+        sortkey2=sortkey2,
+        table_columns=table_columns,
+        delimiter=delimiter,
+        headers=headers,
+        credential_id=credential_id,
+        primary_keys=primary_keys,
+        last_modified_keys=last_modified_keys,
+        escaped=False,
+        execution=execution,
+        polling_interval=polling_interval,
+        hidden=hidden,
+    )
 
     return fut
 
 
-@deprecate_param('v2.0.0', 'api_key')
-def csv_to_civis(filename, database, table, api_key=None, client=None,
-                 max_errors=None, existing_table_rows="fail",
-                 diststyle=None, distkey=None,
-                 sortkey1=None, sortkey2=None,
-                 delimiter=",", headers=None,
-                 credential_id=None, polling_interval=None,
-                 archive=False, hidden=True):
+def csv_to_civis(
+    filename,
+    database,
+    table,
+    client=None,
+    max_errors=None,
+    existing_table_rows="fail",
+    diststyle=None,
+    distkey=None,
+    sortkey1=None,
+    sortkey2=None,
+    table_columns=None,
+    delimiter=",",
+    headers=None,
+    primary_keys=None,
+    last_modified_keys=None,
+    escaped=False,
+    execution="immediate",
+    credential_id=None,
+    polling_interval=None,
+    hidden=True,
+):
     """Upload the contents of a local CSV file to Civis.
 
     Parameters
     ----------
     filename : str
         Upload the contents of this file.
     database : str or int
         Upload data into this database. Can be the database name or ID.
     table : str
         The schema and table you want to upload to. E.g.,
         ``'scratch.table'``.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     max_errors : int, optional
         The maximum number of rows with errors to remove from the import
         before failing.
     existing_table_rows : str, optional
         The behaviour if a table with the requested name already exists.
-        One of ``'fail'``, ``'truncate'``, ``'append'`` or ``'drop'``.
-        Defaults to ``'fail'``.
+        One of ``'fail'``, ``'truncate'``, ``'append'``, ``'drop'``, or
+        ``'upsert'``. Defaults to ``'fail'``.
     diststyle : str, optional
         The distribution style for the table.
         One of ``'even'``, ``'all'`` or ``'key'``.
     distkey : str, optional
         The column to use as the distkey for the table.
     sortkey1 : str, optional
         The column to use as the sortkey for the table.
     sortkey2 : str, optional
         The second column in a compound sortkey for the table.
+    table_columns : list[Dict[str, str]], optional
+        A list of dictionaries, ordered so each dictionary corresponds
+        to a column in the order that it appears in the source file. Each dict
+        should have a key "name" that corresponds to the column name in the
+        destination table, and a key "sql_type" corresponding to the intended
+        column data type in the destination table. The "sql_type" key is not
+        required when appending to an existing table. The table_columns
+        parameter is required if the table does not exist, the table is being
+        dropped, or the columns in the source file do not appear in the same
+        order as in the destination table. Example:
+        ``[{"name": "foo", "sql_type": "INT"}, {"name": "bar", "sql_type": "VARCHAR"}]``
     delimiter : string, optional
         The column delimiter. One of ``','``, ``'\\t'`` or ``'|'``.
     headers : bool, optional
         Whether or not the first row of the file should be treated as
         headers. The default, ``None``, attempts to autodetect whether
         or not the first row contains headers.
+    primary_keys: list[str], optional
+        A list of the primary key column(s) of the destination table that
+        uniquely identify a record. These columns must not contain null values.
+        If existing_table_rows is "upsert", this
+        field is required. Note that this is true regardless of whether the
+        destination database itself requires a primary key.
+    last_modified_keys: list[str], optional
+        A list of the columns indicating a record has been updated. If
+        existing_table_rows is "upsert", this field is required.
+    escaped: bool, optional
+        A boolean value indicating whether or not the source file has quotes
+        escaped with a backslash. Defaults to false.
+    execution: string, optional, default "immediate"
+        One of "delayed" or "immediate". If "immediate", refresh column
+        statistics as part of the run. If "delayed", flag the table for a
+        deferred statistics update; column statistics may not be available
+        for up to 24 hours. In addition, if existing_table_rows is "upsert",
+        delayed executions move data from staging table to final table after a
+        brief delay, in order to accommodate multiple concurrent imports to the
+        same destination table.
     credential_id : str or int, optional
         The ID of the database credential.  If ``None``, the default
         credential will be used.
     polling_interval : int or float, optional
         Number of seconds to wait between checks for job completion.
-    archive : bool, optional (deprecated)
-        If ``True``, archive the import job as soon as it completes.
     hidden : bool, optional
         If ``True`` (the default), this job will not appear in the Civis UI.
 
     Returns
     -------
     results : :class:`~civis.futures.CivisFuture`
         A `CivisFuture` object.
 
     Notes
     -----
     This reads the contents of `filename` into memory.
 
     Examples
     --------
+    >>> import civis
     >>> with open('input_file.csv', 'w') as _input:
     ...     _input.write('a,b,c\\n1,2,3')
     >>> fut = civis.io.csv_to_civis('input_file.csv',
     ...                             'my-database',
     ...                             'scratch.my_data')
     >>> fut.result()
-    """
+    """  # noqa: E501
     if client is None:
-        client = APIClient(api_key=api_key)
-    if archive:
-        warnings.warn("`archive` is deprecated and will be removed in v2.0.0. "
-                      "Use `hidden` instead.", FutureWarning)
+        client = APIClient()
 
     name = path.basename(filename)
     with open(filename, "rb") as data:
         file_id = file_to_civis(data, name, client=client)
-        log.debug('Uploaded file %s to Civis file %s', filename, file_id)
-        fut = civis_file_to_table(file_id, database, table,
-                                  client=client, max_errors=max_errors,
-                                  existing_table_rows=existing_table_rows,
-                                  diststyle=diststyle, distkey=distkey,
-                                  sortkey1=sortkey1, sortkey2=sortkey2,
-                                  delimiter=delimiter, headers=headers,
-                                  credential_id=credential_id,
-                                  polling_interval=polling_interval,
-                                  hidden=hidden)
+        log.debug("Uploaded file %s to Civis file %s", filename, file_id)
+        fut = civis_file_to_table(
+            file_id,
+            database,
+            table,
+            client=client,
+            max_errors=max_errors,
+            existing_table_rows=existing_table_rows,
+            diststyle=diststyle,
+            distkey=distkey,
+            sortkey1=sortkey1,
+            sortkey2=sortkey2,
+            table_columns=table_columns,
+            delimiter=delimiter,
+            headers=headers,
+            credential_id=credential_id,
+            primary_keys=primary_keys,
+            last_modified_keys=last_modified_keys,
+            escaped=escaped,
+            execution=execution,
+            polling_interval=polling_interval,
+            hidden=hidden,
+        )
     return fut
 
 
-def civis_file_to_table(file_id, database, table, client=None,
-                        max_errors=None, existing_table_rows="fail",
-                        diststyle=None, distkey=None,
-                        sortkey1=None, sortkey2=None,
-                        delimiter=",", headers=None,
-                        credential_id=None, polling_interval=None,
-                        hidden=True):
-    """Upload the contents of a Civis file to a Civis table.
+def civis_file_to_table(
+    file_id,
+    database,
+    table,
+    client=None,
+    max_errors=None,
+    existing_table_rows="fail",
+    diststyle=None,
+    distkey=None,
+    sortkey1=None,
+    sortkey2=None,
+    table_columns=None,
+    primary_keys=None,
+    last_modified_keys=None,
+    escaped=False,
+    execution="immediate",
+    delimiter=None,
+    headers=None,
+    credential_id=None,
+    polling_interval=None,
+    hidden=True,
+):
+    """Upload the contents of one or more Civis files to a Civis table.
+    All provided files will be loaded as an atomic unit in parallel, and
+    should share the same columns in the same order, and be in the same
+    format.
+
+    .. note::
+        The input Civis files must be in a CSV-like delimiter separated format and
+        will be accepted in both uncompressed and compressed format
+        (.zip, .gz).
 
     Parameters
     ----------
-    file_id : int
-        Civis file ID.
+    file_id : int or list[int]
+        Civis file ID or a list of Civis file IDs.
     database : str or int
         Upload data into this database. Can be the database name or ID.
     table : str
         The schema and table you want to upload to. E.g.,
         ``'scratch.table'``.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     max_errors : int, optional
         The maximum number of rows with errors to remove from the import
-        before failing.
+        before failing. If multiple files are provided, this limit applies
+        across all files combined.
     existing_table_rows : str, optional
         The behaviour if a table with the requested name already exists.
-        One of ``'fail'``, ``'truncate'``, ``'append'`` or ``'drop'``.
-        Defaults to ``'fail'``.
+        One of ``'fail'``, ``'truncate'``, ``'append'``, ``'drop'``, or
+        ``'upsert'``. Defaults to ``'fail'``.
     diststyle : str, optional
         The distribution style for the table.
         One of ``'even'``, ``'all'`` or ``'key'``.
     distkey : str, optional
         The column to use as the distkey for the table.
     sortkey1 : str, optional
         The column to use as the sortkey for the table.
     sortkey2 : str, optional
         The second column in a compound sortkey for the table.
+    table_columns : list[Dict[str, str]], optional
+        A list of dictionaries, ordered so each dictionary corresponds
+        to a column in the order that it appears in the source file. Each dict
+        should have a key "name" that corresponds to the column name in the
+        destination table, and a key "sql_type" corresponding to the intended
+        column data type in the destination table. The "sql_type" key is not
+        required when appending to an existing table. The table_columns
+        parameter is required if the table does not exist, the table is being
+        dropped, or the columns in the source file do not appear in the same
+        order as in the destination table. Example:
+        ``[{"name": "foo", "sql_type": "INT"}, {"name": "bar", "sql_type": "VARCHAR"}]``
+    primary_keys: list[str], optional
+        A list of the primary key column(s) of the destination table that
+        uniquely identify a record. These columns must not contain null values.
+        If existing_table_rows is "upsert", this
+        field is required. Note that this is true regardless of whether the
+        destination database itself requires a primary key.
+    last_modified_keys: list[str], optional
+        A list of the columns indicating a record has been updated. If
+        existing_table_rows is "upsert", this field is required.
+    escaped: bool, optional
+        A boolean value indicating whether or not the source file(s) escape
+        quotes with a backslash. Defaults to false.
+    execution: string, optional, default "immediate"
+        One of "delayed" or "immediate". If "immediate", refresh column
+        statistics as part of the run. If "delayed", flag the table for a
+        deferred statistics update; column statistics may not be available
+        for up to 24 hours. In addition, if existing_table_rows is "upsert",
+        delayed executions move data from staging table to final table after a
+        brief delay, in order to accommodate multiple concurrent imports to the
+        same destination table.
     delimiter : string, optional
-        The column delimiter. One of ``','``, ``'\\t'`` or ``'|'``.
+        The column delimiter. One of ``','``, ``'\\t'`` or ``'|'``. If not
+        provided, will attempt to auto-detect.
     headers : bool, optional
         Whether or not the first row of the file should be treated as
         headers. The default, ``None``, attempts to autodetect whether
         or not the first row contains headers.
     credential_id : str or int, optional
         The ID of the database credential.  If ``None``, the default
         credential will be used.
@@ -865,118 +1088,189 @@
         If ``True`` (the default), this job will not appear in the Civis UI.
 
     Returns
     -------
     results : :class:`~civis.futures.CivisFuture`
         A `CivisFuture` object.
 
+    Raises
+    ------
+    CivisImportError
+        If multiple files are given and determined to be incompatible for
+        import. This may be the case if their columns have different types,
+        their delimiters are different, headers are present in some but not
+        others, or compressions do not match.
+    TypeError
+        If the type of the file_id parameter is a string. This situation may
+        arise when the file ID comes from an environment variable and is not
+        cast from string to integer before being passed to civis_file_to_table.
+
     Examples
     --------
+    >>> import civis
     >>> file_id = 100
     >>> fut = civis.io.civis_file_to_table(file_id,
     ...                                    'my-database',
     ...                                    'scratch.my_data')
     >>> fut.result()
-    """
+    """  # noqa: E501
     if client is None:
         client = APIClient()
 
-    schema, table = split_schema_tablename(table)
+    if type(file_id) is str:
+        raise TypeError("Invalid type for file_id: str. " "Must be int or list[int]")
+
+    schema, table_name = split_schema_tablename(table)
+    if isinstance(file_id, int):
+        file_id = [file_id]
+    if not file_id:
+        raise ValueError("Provide one or multiple meaningful input file IDs.")
     if schema is None:
         raise ValueError("Provide a schema as part of the `table` input.")
     db_id = client.get_database_id(database)
     cred_id = credential_id or client.default_credential
-    delimiter = DELIMITERS.get(delimiter)
-    assert delimiter, "delimiter must be one of {}".format(DELIMITERS.keys())
-
-    destination = dict(remote_host_id=db_id, credential_id=cred_id)
-    import_name = 'CSV import to {}.{}'.format(schema, table)
-    import_job = client.imports.post(import_name, 'AutoImport',
-                                     is_outbound=False,
-                                     destination=destination,
-                                     hidden=hidden)
-
-    options = dict(max_errors=max_errors,
-                   existing_table_rows=existing_table_rows,
-                   diststyle=diststyle, distkey=distkey,
-                   sortkey1=sortkey1, sortkey2=sortkey2,
-                   column_delimiter=delimiter, first_row_is_header=headers)
-
-    client.imports.post_syncs(
-        import_job.id,
-        source=dict(file=dict(id=file_id)),
-        destination=dict(database_table=dict(schema=schema, table=table)),
-        advanced_options=options)
-
-    run = client.jobs.post_runs(import_job.id)
-    fut = CivisFuture(client.jobs.get_runs,
-                      (import_job.id, run['id']),
-                      polling_interval=polling_interval,
-                      client=client,
-                      poll_on_creation=False)
+    if delimiter is not None:  # i.e. it was provided as an argument
+        delimiter = DELIMITERS.get(delimiter)
+        if not delimiter:
+            raise ValueError(
+                f"delimiter must be one of {DELIMITERS.keys()}: {delimiter}"
+            )
+    if table_columns:
+        # If the data cleaning code doesn't find a "sql_type" for each
+        # entry, it will silently replace the input table_columns with
+        # an inferred table_columns. Make sure there's no typos in the input.
+        keys = set(key for hash in table_columns for key in hash)
+        valid_keys = {"name", "sql_type"}
+        invalid_keys = keys - valid_keys
+        if invalid_keys:
+            # Sort the sets for display to allow for deterministic testing in
+            # Python versions < 3.7.
+            raise ValueError(
+                "Keys of the dictionaries contained in `table_columns` must "
+                "be one of {}. The input `table_columns` also has "
+                "{}.".format(tuple(sorted(valid_keys)), tuple(sorted(invalid_keys)))
+            )
 
+    try:
+        client.databases.get_schemas_tables(db_id, schema, table_name)
+        log.debug(
+            "Table {table} already exists - skipping column "
+            "detection".format(table=table)
+        )
+        table_exists = True
+    except CivisAPIError as e:
+        table_exists = False
+        if e.status_code != 404:
+            warnings.warn(
+                "Unexpected error when checking if table %s.%s "
+                "exists on database %d:\n%s" % (schema, table_name, db_id, str(e))
+            )
+
+    sql_types_provided = False
+    if table_columns:
+        sql_type_cnt = sum(1 for col in table_columns if col.get("sql_type"))
+        if sql_type_cnt == len(table_columns):
+            sql_types_provided = True
+        elif sql_type_cnt != 0:
+            error_message = (
+                "Some table columns " "have a sql type provided, " "but others do not."
+            )
+            raise ValueError(error_message)
+
+    # Use Preprocess endpoint to get the table columns as needed
+    # and perform necessary file cleaning
+    need_table_columns = (not table_exists or existing_table_rows == "drop") and (
+        not sql_types_provided
+    )
+
+    cleaning_futures = _run_cleaning(
+        file_id, client, need_table_columns, headers, delimiter, hidden
+    )
+
+    (cleaned_file_ids, headers, compression, delimiter, cleaned_table_columns) = (
+        _process_cleaning_results(
+            cleaning_futures, client, headers, need_table_columns, delimiter
+        )
+    )
+
+    table_columns = cleaned_table_columns if need_table_columns else table_columns
+
+    source = dict(file_ids=cleaned_file_ids)
+    destination = dict(
+        schema=schema,
+        table=table_name,
+        remote_host_id=db_id,
+        credential_id=cred_id,
+        primary_keys=primary_keys,
+        last_modified_keys=last_modified_keys,
+    )
+
+    redshift_options = dict(
+        distkey=distkey, sortkeys=[sortkey1, sortkey2], diststyle=diststyle
+    )
+
+    import_name = "CSV import to {}.{}".format(schema, table_name)
+    import_job = client.imports.post_files_csv(
+        source,
+        destination,
+        headers,
+        name=import_name,
+        max_errors=max_errors,
+        existing_table_rows=existing_table_rows,
+        column_delimiter=delimiter,
+        compression=compression,
+        escaped=escaped,
+        execution=execution,
+        # If the user hasn't explicitly provided table column info,
+        # then there might be differences in their precisions/lengths.
+        # Setting this option will allow the Civis API
+        # to increase these values for the data types provided,
+        # and decreases the risk of a length-related import failure
+        # when types are inferred.
+        loosen_types=need_table_columns,
+        table_columns=table_columns,
+        redshift_destination_options=redshift_options,
+        hidden=hidden,
+    )
+    fut = run_job(import_job.id, client=client, polling_interval=polling_interval)
+    log.debug("Started run %d for import %d", fut.run_id, import_job.id)
     return fut
 
 
-def _sql_script(client, sql, database, job_name, credential_id, hidden=False,
-                csv_settings=None):
+def _sql_script(
+    client, sql, database, job_name, credential_id, hidden=False, csv_settings=None
+):
     job_name = maybe_get_random_name(job_name)
     db_id = client.get_database_id(database)
     credential_id = credential_id or client.default_credential
     csv_settings = csv_settings or {}
 
-    export_job = client.scripts.post_sql(job_name,
-                                         remote_host_id=db_id,
-                                         credential_id=credential_id,
-                                         sql=sql,
-                                         hidden=hidden,
-                                         csv_settings=csv_settings)
+    export_job = client.scripts.post_sql(
+        job_name,
+        remote_host_id=db_id,
+        credential_id=credential_id,
+        sql=sql,
+        hidden=hidden,
+        csv_settings=csv_settings,
+    )
 
     run_job = client.scripts.post_sql_runs(export_job.id)
-
+    log.debug("Started run %d of SQL script %d", run_job.id, export_job.id)
     return export_job.id, run_job.id
 
 
 def _get_sql_select(table, columns=None):
     if columns and not isinstance(columns, (list, tuple)):
         raise TypeError("columns must be a list, tuple or None")
     select = ", ".join(columns) if columns is not None else "*"
-    sql = "select {} from {}".format(select, table)
+    sql = "select {} from {}".format(select, table)  # nosec
     return sql
 
 
-def _get_headers(client, sql, database, credential_id, polling_interval=None):
-    # use 'begin read only;' to ensure we can't change state
-    sql = 'begin read only; select * from ({}) limit 1'.format(sql)
-    fut = query_civis(sql, database, client=client,
-                      credential_id=credential_id,
-                      polling_interval=polling_interval)
-    return fut.result()['result_columns']
-
-
-def _include_header(client, sql, include_header, database, credential_id,
-                    polling_interval=None):
-    headers = None
-
-    # can't do a parallel unload when sql contains an order by
-    if not include_header or re.search(r'order\s+by', sql, re.I | re.M):
-        return include_header, headers
-
-    try:
-        # if _get_headers throws an error then assume sql is not read only
-        headers = _get_headers(client, sql, database, credential_id,
-                               polling_interval=polling_interval)
-        include_header = False
-    except Exception as exc:  # NOQA
-        log.debug("Failed to retrieve headers due to %s", str(exc))
-
-    return include_header, headers
-
-
-def _decompress_stream(response, buf, write_bytes=True):
+def _decompress_stream(response, buf, write_bytes=True, encoding="utf-8"):
 
     # use response.raw for a more consistent approach
     # if content-encoding is specified in the headers
     # then response.iter_content will decompress the stream
     # however, our use of content-encoding is inconsistent
     chunk = response.raw.read(CHUNK_SIZE)
     d = zlib.decompressobj(zlib.MAX_WBITS | 32)
@@ -986,66 +1280,67 @@
             to_decompress = d.unused_data + chunk
             d = zlib.decompressobj(zlib.MAX_WBITS | 32)
         else:
             to_decompress = d.unconsumed_tail + chunk
         if write_bytes:
             buf.write(d.decompress(to_decompress))
         else:
-            buf.write(d.decompress(to_decompress).decode('utf-8'))
+            buf.write(d.decompress(to_decompress).decode(encoding))
         chunk = response.raw.read(CHUNK_SIZE)
 
 
 def _download_file(url, local_path, headers, compression):
-    response = requests.get(url, stream=True)
+    response = requests.get(url, stream=True, timeout=60)
     response.raise_for_status()
 
     # gzipped buffers can be concatenated so write headers as gzip
-    if compression == 'gzip':
-        with gzip.open(local_path, 'wb') as fout:
+    if compression == "gzip":
+        with gzip.open(local_path, "wb") as fout:
             fout.write(headers)
-        with open(local_path, 'ab') as fout:
+        with open(local_path, "ab") as fout:
             shutil.copyfileobj(response.raw, fout, CHUNK_SIZE)
 
     # write headers and decompress the stream
-    elif compression == 'none':
-        with open(local_path, 'wb') as fout:
+    elif compression == "none":
+        with open(local_path, "wb") as fout:
             fout.write(headers)
             _decompress_stream(response, fout)
 
     # decompress the stream, write headers, and zip the file
-    elif compression == 'zip':
+    elif compression == "zip":
         with TemporaryDirectory() as tmp_dir:
-            tmp_path = path.join(tmp_dir, 'civis_to_csv.csv')
-            with open(tmp_path, 'wb') as tmp_file:
+            tmp_path = path.join(tmp_dir, "civis_to_csv.csv")
+            with open(tmp_path, "wb") as tmp_file:
                 tmp_file.write(headers)
                 _decompress_stream(response, tmp_file)
 
-            with zipfile.ZipFile(local_path, 'w') as fout:
+            with zipfile.ZipFile(local_path, "w") as fout:
                 arcname = path.basename(local_path)
-                if arcname.split('.')[-1] == 'zip':
-                    arcname = arcname.split('.')[0] + '.csv'
+                if arcname.split(".")[-1] == "zip":
+                    arcname = arcname.split(".")[0] + ".csv"
                 fout.write(tmp_path, arcname, zipfile.ZIP_DEFLATED)
 
 
 def _download_callback(job_id, run_id, filename, headers, compression):
 
     def callback(future):
         if not future.succeeded():
             return
         outputs = future.result().get("output")
         if not outputs:
-            warnings.warn("Job %s, run %s does not have any output to "
-                          "download. Not creating file %s."
-                          % (job_id, run_id, filename),
-                          RuntimeWarning)
+            warnings.warn(
+                "Job %s, run %s does not have any output to "
+                "download. Not creating file %s." % (job_id, run_id, filename),
+                RuntimeWarning,
+            )
             return
         else:
             url = outputs[0]["path"]
             file_id = outputs[0]["file_id"]
-            log.debug('Exported results to Civis file %s', file_id)
+            log.debug("Exported results to Civis file %s", file_id)
             return _download_file(url, filename, headers, compression)
 
     return callback
 
 
 def split_schema_tablename(table):
     """Split a Redshift 'schema.tablename' string
@@ -1067,19 +1362,197 @@
 
     Raises
     ------
     ValueError
         If the input ``table`` is not separable into a schema and
         table name.
     """
-    reader = csv.reader(StringIO(six.text_type(table)),
-                        delimiter=".",
-                        doublequote=True,
-                        quotechar='"')
+    reader = csv.reader(
+        io.StringIO(str(table)), delimiter=".", doublequote=True, quotechar='"'
+    )
     schema_name_tup = next(reader)
     if len(schema_name_tup) == 1:
         schema_name_tup = (None, schema_name_tup[0])
     if len(schema_name_tup) != 2:
-        raise ValueError("Cannot parse schema and table. "
-                         "Does '{}' follow the pattern 'schema.table'?"
-                         .format(table))
+        raise ValueError(
+            "Cannot parse schema and table. "
+            "Does '{}' follow the pattern 'schema.table'?".format(table)
+        )
     return tuple(schema_name_tup)
+
+
+def _run_cleaning(
+    file_ids,
+    client,
+    need_table_columns,
+    headers,
+    delimiter,
+    hidden,
+    polling_interval=None,
+):
+    cleaning_futures = []
+    for fid in file_ids:
+        cleaner_job = client.files.post_preprocess_csv(
+            file_id=fid,
+            in_place=False,
+            detect_table_columns=need_table_columns,
+            force_character_set_conversion=True,
+            include_header=headers,
+            column_delimiter=delimiter,
+            hidden=hidden,
+        )
+        fut = run_job(cleaner_job.id, client=client, polling_interval=polling_interval)
+        log.debug(
+            "Started CSV preprocess job %d run %d for file %d (%s)",
+            cleaner_job.id,
+            fut.run_id,
+            fid,
+            client.files.get(fid).name,
+        )
+        cleaning_futures.append(fut)
+    return cleaning_futures
+
+
+def _process_cleaning_results(
+    cleaning_futures, client, headers, need_table_columns, delimiter
+):
+    futures, _ = concurrent.futures.wait(cleaning_futures)
+    files: List[_File] = []
+
+    job_run_ids_no_output = []
+    for fut in futures:
+        objs = client.jobs.list_runs_outputs(fut.job_id, fut.run_id)
+        if not objs:
+            job_run_ids_no_output.append((fut.job_id, fut.run_id))
+            continue
+        # `objs` is guaranteed to have exactly one file output.
+        f = client.files.get(objs[0].object_id)
+        files.append(_File(id=f.id, name=f.name, detected_info=f.detected_info))
+    if job_run_ids_no_output:
+        job_run_ids_in_err_msg = "\n".join(
+            f"\tjob {j} run {r}" for j, r in job_run_ids_no_output
+        )
+        raise CivisImportError(
+            "No CSV preprocess output found for "
+            f"these runs:\n{job_run_ids_in_err_msg}"
+        )
+
+    if need_table_columns:
+        table_columns, allow_inconsistent_headers = _check_column_types(files)
+    else:
+        table_columns = None
+        allow_inconsistent_headers = False
+
+    try:
+        headers = _check_detected_info(files, "includeHeader", headers)
+    except CivisImportError:
+        if allow_inconsistent_headers:
+            headers = True
+        else:
+            raise
+
+    delimiter = _check_detected_info(files, "columnDelimiter", delimiter)
+    compression = _check_detected_info(files, "compression")
+
+    cleaned_file_ids = [f.id for f in files]
+
+    return cleaned_file_ids, headers, compression, delimiter, table_columns
+
+
+def _check_detected_info(files: List[_File], attr: str, value_from_user=None):
+    values_detected = [f.detected_info[attr] for f in files]
+    err_msg = _err_msg_if_inconsistent(values_detected, files)
+    if err_msg:
+        raise CivisImportError(
+            f"All detected values for '{attr}' must be the same, "
+            f"however --\n{err_msg}"
+        )
+
+    value_detected = values_detected[0]
+
+    # The user cannot specify "compression" from civis_file_to_table.
+    if attr == "compression" or value_from_user is None:
+        return value_detected
+
+    if value_detected != value_from_user:
+        raise CivisImportError(
+            f"All detected values for '{attr}' in your files "
+            f"are {value_detected}, which doesn't match "
+            f"your provided value of {value_from_user}"
+        )
+    else:
+        return value_detected
+
+
+def _check_column_types(files: List[_File]):
+    cols_by_file: List[List[Dict[str, str]]]
+    cols_by_file = [f.detected_info["tableColumns"] for f in files]
+
+    col_counts = [len(cols) for cols in cols_by_file]
+    err_msg = _err_msg_if_inconsistent(col_counts, files)
+    if err_msg:
+        raise CivisImportError(
+            f"All files must have the same number of columns, " f"however --\n{err_msg}"
+        )
+
+    # Transpose cols_by_file to get cols_by_col
+    # https://stackoverflow.com/q/6473679
+    cols_by_col: List[List[Dict[str, str]]]
+    cols_by_col = list(map(list, zip(*cols_by_file)))
+
+    table_columns: List[Dict[str, str]] = []
+    allow_inconsistent_headers = False
+    err_msgs: List[str] = []
+
+    for i, cols in enumerate(cols_by_col, 1):
+        col_name = next((c.get("name") for c in cols if c.get("name")), f"column_{i}")
+
+        sql_base_types = [col["sql_type"].split("(", 1)[0].upper() for col in cols]
+        err_msg = _err_msg_if_inconsistent(sql_base_types, files)
+        if err_msg and "VARCHAR" not in sql_base_types:
+            err_msgs.append(
+                f"All sql_types for column '{col_name}' must be the same, "
+                f"however --\n{err_msg}"
+            )
+            continue
+        if err_msg:
+            # If the sql_types are inconsistent and at least one of them
+            # is a VARCHAR, then simply use VARCHAR
+            # for this column across all files.
+            sql_type = "VARCHAR"
+            # The one single file that originally had sql_type as VARCHAR
+            # has the detected "first row is headers" to be false
+            # (i.e., the detection thought the first row was first row of data,
+            # because it can't reliably tell when it comes to VARCHAR),
+            # whereas for all the other files where the sql_type for this
+            # column isn't VARCHAR, the detected "first row is headers" is
+            # true instead. Due to this expected inconsistency,
+            # we need to pass a flag out of this function to signal
+            # that we can allow `headers` to be True.
+            allow_inconsistent_headers = True
+        else:
+            sql_type = cols[0]["sql_type"]
+        table_columns.append({"name": col_name, "sql_type": sql_type})
+
+    if err_msgs:
+        raise CivisImportError("\n".join(err_msgs))
+
+    return table_columns, allow_inconsistent_headers
+
+
+def _err_msg_if_inconsistent(items: List, files: List[_File]):
+    if len(set(items)) <= 1:
+        return
+    values_to_indices = collections.defaultdict(list)
+    for i, value in enumerate(items):
+        values_to_indices[value].append(i)
+    msg_for_each_value = [
+        f"\t{v} from: {_format_files_for_err_msg(files, indices)}"
+        for v, indices in values_to_indices.items()
+    ]
+    err_msg = "\n".join(msg_for_each_value)
+    return err_msg
+
+
+def _format_files_for_err_msg(files: List[_File], indices):
+    files_in_str = [f"file {files[i].id} ({files[i].name})" for i in indices]
+    return ", ".join(files_in_str)
```

### Comparing `civis-1.9.4/civis/io/_files.py` & `civis-2.0.0/src/civis/io/_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,213 +4,256 @@
 import json
 import logging
 import math
 from multiprocessing.dummy import Pool
 import os
 import re
 import shutil
-import six
+from tempfile import TemporaryDirectory
+
 import requests
 from requests import HTTPError
 
 from civis import APIClient, find_one
 from civis.base import CivisAPIError, EmptyResultError
-from civis.compat import FileNotFoundError, TemporaryDirectory
-from civis._deprecation import deprecate_param
 from civis._utils import BufferedPartialReader, retry
 
 try:
     import pandas as pd
+
     HAS_PANDAS = True
 except ImportError:
     HAS_PANDAS = False
 
-MIN_MULTIPART_SIZE = 50 * 2 ** 20  # 50MB
-MIN_PART_SIZE = 5 * 2 ** 20  # 5MB
-MAX_PART_SIZE = 5 * 2 ** 30  # 5GB
-MAX_FILE_SIZE = 5 * 2 ** 40  # 5TB
+MIN_MULTIPART_SIZE = 50 * 2**20  # 50MB
+MIN_PART_SIZE = 5 * 2**20  # 5MB
+MAX_PART_SIZE = 5 * 2**30  # 5GB
+MAX_FILE_SIZE = 5 * 2**40  # 5TB
 MAX_THREADS = 4
 
-RETRY_EXCEPTIONS = (requests.HTTPError,
-                    requests.ConnectionError,
-                    requests.ConnectTimeout)
+RETRY_EXCEPTIONS = (
+    requests.HTTPError,
+    requests.ConnectionError,
+    requests.ConnectTimeout,
+)
 
 log = logging.getLogger(__name__)
 # standard chunk size; provides good performance across various buffer sizes
 CHUNK_SIZE = 32 * 1024
-__all__ = ['file_to_civis', 'civis_to_file', 'file_id_from_run_output',
-           'file_to_dataframe', 'file_to_json']
+__all__ = [
+    "file_to_civis",
+    "civis_to_file",
+    "file_id_from_run_output",
+    "file_to_dataframe",
+    "dataframe_to_file",
+    "file_to_json",
+    "json_to_file",
+]
 
 
 def _get_aws_error_message(response):
     # Amazon gives back informative error messages
     # http://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html
     # NOTE: This is cribbed from response.raise_for_status with AWS
     # message appended
-    msg = ''
+    msg = ""
 
     if 400 <= response.status_code < 500:
-        msg = '%s Client Error: %s for url: %s' % (response.status_code,
-                                                   response.reason,
-                                                   response.url)
+        msg = "%s Client Error: %s for url: %s" % (
+            response.status_code,
+            response.reason,
+            response.url,
+        )
 
     elif 500 <= response.status_code < 600:
-        msg = '%s Server Error: %s for url: %s' % (response.status_code,
-                                                   response.reason,
-                                                   response.url)
+        msg = "%s Server Error: %s for url: %s" % (
+            response.status_code,
+            response.reason,
+            response.url,
+        )
 
-    msg += '\nAWS Content: %s' % response.content
+    msg += "\nAWS Content: %s" % response.content
 
     return msg
 
 
 def _buf_len(buf):
-    if hasattr(buf, '__len__'):
+    if hasattr(buf, "__len__"):
         return len(buf)
 
-    if hasattr(buf, 'len'):
+    if hasattr(buf, "len"):
         return buf.len
 
-    if hasattr(buf, 'fileno'):
+    if hasattr(buf, "fileno"):
         try:
             fileno = buf.fileno()
         except io.UnsupportedOperation:
             pass
         else:
             return os.fstat(fileno).st_size
 
-    if hasattr(buf, 'getvalue'):
+    if hasattr(buf, "getvalue"):
         # e.g. BytesIO, cStringIO.StringIO
         return len(buf.getvalue())
 
     return None
 
 
 def _single_upload(buf, name, client, **kwargs):
     file_response = client.files.post(name, **kwargs)
 
     # Platform has given us a URL to which we can upload a file.
     # The file must be uploaded with a POST formatted as per
     # http://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-post-example.html
     # Note that the payload must have "key" first and "file" last.
     url = file_response.upload_url
-    form = file_response.upload_fields
-    form_key = OrderedDict(key=form.pop('key'))
+    form = file_response.upload_fields._data_snake
+    form_key = OrderedDict(key=form.pop("key"))
     form_key.update(form)
 
     # Store the current buffer position in case we need to retry below.
     buf_orig_position = buf.tell()
 
     @retry(RETRY_EXCEPTIONS)
     def _post():
         # Reset the buffer in case we had to retry.
         buf.seek(buf_orig_position)
 
-        form_key['file'] = buf
+        form_key["file"] = buf
         # requests will not stream multipart/form-data, but _single_upload
         # is only used for small file objects or non-seekable file objects
         # which can't be streamed with using requests-toolbelt anyway
-        response = requests.post(url, files=form_key)
+        response = requests.post(url, files=form_key, timeout=60)
 
         if not response.ok:
             msg = _get_aws_error_message(response)
             raise HTTPError(msg, response=response)
 
     _post()
 
+    log.debug("Uploaded File %d", file_response.id)
     return file_response.id
 
 
 def _multipart_upload(buf, name, file_size, client, **kwargs):
     # scale the part size based on file size
-    part_size = max(int(math.sqrt(MIN_PART_SIZE) * math.sqrt(file_size)),
-                    MIN_PART_SIZE)
+    part_size = max(int(math.sqrt(MIN_PART_SIZE) * math.sqrt(file_size)), MIN_PART_SIZE)
     num_parts = int(math.ceil((file_size) / float(part_size)))
 
-    log.debug('Uploading file with %s bytes using %s file parts with a part '
-              'size of %s bytes', file_size, num_parts, part_size)
-    file_response = client.files.post_multipart(name=name, num_parts=num_parts,
-                                                **kwargs)
+    log.debug(
+        "Uploading file with %s bytes using %s file parts with a part "
+        "size of %s bytes",
+        file_size,
+        num_parts,
+        part_size,
+    )
+    file_response = client.files.post_multipart(
+        name=name, num_parts=num_parts, **kwargs
+    )
 
     # Platform will give us a URL for each file part
     urls = file_response.upload_urls
-    assert num_parts == len(urls), \
-        "There are {} file parts but only {} urls".format(num_parts, len(urls))
+    if num_parts != len(urls):
+        raise ValueError(f"There are {num_parts} file parts but only {len(urls)} urls")
 
     # upload function wrapped with a retry decorator
     @retry(RETRY_EXCEPTIONS)
     def _upload_part_base(item, file_path, part_size, file_size):
         part_num, part_url = item[0], item[1]
         offset = part_size * part_num
         num_bytes = min(part_size, file_size - offset)
 
-        log.debug('Uploading file part %s', part_num)
-        with open(file_path, 'rb') as fin:
+        log.debug("Uploading file part %s", part_num)
+        with open(file_path, "rb") as fin:
             fin.seek(offset)
             partial_buf = BufferedPartialReader(fin, num_bytes)
-            part_response = requests.put(part_url, data=partial_buf)
+            part_response = requests.put(part_url, data=partial_buf, timeout=60)
 
         if not part_response.ok:
             msg = _get_aws_error_message(part_response)
             raise HTTPError(msg, response=part_response)
 
-        log.debug('Completed upload of file part %s', part_num)
+        log.debug("Completed upload of file part %s", part_num)
 
     # upload each part
     try:
         pool = Pool(MAX_THREADS)
-        _upload_part = partial(_upload_part_base, file_path=buf.name,
-                               part_size=part_size, file_size=file_size)
+        _upload_part = partial(
+            _upload_part_base,
+            file_path=buf.name,
+            part_size=part_size,
+            file_size=file_size,
+        )
         pool.map(_upload_part, enumerate(urls))
 
     # complete the multipart upload; an abort will be triggered
     # if any part except the last failed to upload at least 5MB
     finally:
         pool.terminate()
         client.files.post_multipart_complete(file_response.id)
 
+    log.debug("Uploaded File %d", file_response.id)
     return file_response.id
 
 
-@deprecate_param('v2.0.0', 'api_key')
-def file_to_civis(buf, name, api_key=None, client=None, **kwargs):
+def file_to_civis(buf, name=None, client=None, **kwargs):
     """Upload a file to Civis.
 
     Parameters
     ----------
     buf : file-like object or str
-        The file or other buffer that you wish to upload. Strings will be
-        treated as paths to local files to open.
-    name : str
-        The name you wish to give the file.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
+        Either a file-like object for a buffer or a string for a local file
+        path.
+        Note that if a file-like object is provided and it's not
+        an :class:`io.BufferedReader <io.BufferedReader>`
+        or :class:`io.TextIoWrapper <io.TextIoWrapper>` object,
+        the current implementation requires extra disk space
+        (which could be an issue if your file is large).
+    name : str, optional
+        The name you wish to give the file. If not given, it will be inferred
+        from the basename of ``buf`` (if ``buf`` is a string for a file path)
+        or ``buf.name`` (if ``buf`` is a file-like object).
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     **kwargs : kwargs
         Extra keyword arguments will be passed to the file creation
         endpoint. See :func:`~civis.resources._resources.Files.post`.
+        In particular, ``expires_at`` can be specified for
+        the date and time the file will expire. If not specified, the file
+        will expire in 30 days. To keep a file indefinitely, specify ``None``.
+        To specify a date and time, format it by the ISO 8601 standard,
+        e.g., ``"2020-12-31"``, ``"2020-12-31T23:03:40Z"``,
+        and what the ``isoformat()`` method returns from
+        a :class:`datetime.date <datetime.date>`
+        or :class:`datetime.datetime <datetime.datetime>` object.
 
     Returns
     -------
     file_id : int
         The new Civis file ID.
 
+    Raises
+    ------
+    TypeError
+        If ``name`` is not provided and cannot be inferred from ``buf``
+
     Examples
     --------
+    >>> import civis
     >>> # Upload file at a given path on the local filesystem.
-    >>> file_id = file_to_civis("my_data.csv", 'my_data')
+    >>> file_id = civis.io.file_to_civis("my_data.csv", 'my_data')
+    >>> # If not given, ``name`` will be the basename of the given file path.
+    >>> file_id = civis.io.file_to_civis("foo/bar/data.csv")  # ``name`` is 'data.csv'
     >>> # Upload file which expires in 30 days
     >>> with open("my_data.csv", "r") as f:
-    ...     file_id = file_to_civis(f, 'my_data')
+    ...     file_id = civis.io.file_to_civis(f, 'my_data')
     >>> # Upload file which never expires
     >>> with open("my_data.csv", "r") as f:
-    ...     file_id = file_to_civis(f, 'my_data', expires_at=None)
+    ...     file_id = civis.io.file_to_civis(f, 'my_data', expires_at=None)
 
     Notes
     -----
     If you are opening a binary file (e.g., a compressed archive) to
     pass to this function, do so using the ``'rb'`` (read binary)
     mode (e.g., ``open('myfile.zip', 'rb')``).
 
@@ -219,121 +262,132 @@
 
     This facilitates retries and is used to chunk files for multipart
     uploads for improved performance.
 
     Small or non-seekable file-like objects will be uploaded with a
     single post.
     """
-    if isinstance(buf, six.string_types):
-        with open(buf, 'rb') as f:
-            return _file_to_civis(
-                f, name, api_key=api_key, client=client, **kwargs)
+    if name is None:
+        if isinstance(buf, str):
+            name = os.path.basename(buf)
+        elif hasattr(buf, "name"):
+            name = buf.name
+        else:
+            msg = (
+                "`buf` is a file-like object, but its name cannot be inferred."
+                " Please provide `name` explicitly."
+            )
+            raise TypeError(msg)
+
+    if isinstance(buf, str):
+        with open(buf, "rb") as f:
+            return _file_to_civis(f, name, client=client, **kwargs)
 
     # we should only pass _file_to_civis a file-like object that is
     # on disk, seekable and at position 0
-    if not isinstance(buf, (io.BufferedReader, io.TextIOWrapper)) or \
-            buf.tell() != 0:
+    if not isinstance(buf, (io.BufferedReader, io.TextIOWrapper)) or buf.tell() != 0:
         # determine mode for writing
-        mode = 'w'
-        if isinstance(buf.read(0), six.binary_type):
-            mode += 'b'
+        mode = "w"
+        if isinstance(buf.read(0), bytes):
+            mode += "b"
         with TemporaryDirectory() as tmp_dir:
-            tmp_path = os.path.join(tmp_dir, 'file_to_civis.csv')
+            tmp_path = os.path.join(tmp_dir, "file_to_civis.csv")
             with open(tmp_path, mode) as fout:
                 shutil.copyfileobj(buf, fout, CHUNK_SIZE)
-            with open(tmp_path, 'rb') as fin:
-                return _file_to_civis(
-                    fin, name, api_key=api_key, client=client, **kwargs)
+            with open(tmp_path, "rb") as fin:
+                return _file_to_civis(fin, name, client=client, **kwargs)
     else:
-        return _file_to_civis(
-            buf, name, api_key=api_key, client=client, **kwargs)
+        return _file_to_civis(buf, name, client=client, **kwargs)
 
 
-def _file_to_civis(buf, name, api_key=None, client=None, **kwargs):
+def _file_to_civis(buf, name, client=None, **kwargs):
     if client is None:
-        client = APIClient(api_key=api_key)
+        client = APIClient()
 
     file_size = _buf_len(buf)
-    if not file_size:
-        log.warning('Could not determine file size; defaulting to '
-                    'single post. Files over 5GB will fail.')
+    if file_size == 0:
+        log.warning("Warning: file size is zero bytes.")
+    elif not file_size:
+        log.warning(
+            "Could not determine file size; defaulting to "
+            "single post. Files over 5GB will fail."
+        )
 
     if not file_size or file_size <= MIN_MULTIPART_SIZE:
         return _single_upload(buf, name, client, **kwargs)
     elif file_size > MAX_FILE_SIZE:
         msg = "File is greater than the maximum allowable file size (5TB)"
         raise ValueError(msg)
     else:
         return _multipart_upload(buf, name, file_size, client, **kwargs)
 
 
-@deprecate_param('v2.0.0', 'api_key')
-def civis_to_file(file_id, buf, api_key=None, client=None):
+def civis_to_file(file_id, buf, client=None):
     """Download a file from Civis.
 
     Parameters
     ----------
     file_id : int
         The Civis file ID.
     buf : file-like object or str
         A buffer or path specifying where to write the contents of the Civis
         file. Strings will be treated as paths to local files to open.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
 
     Returns
     -------
     None
 
     Examples
     --------
+    >>> import civis
     >>> file_id = 100
     >>> # Download a file to a path on the local filesystem.
-    >>> civis_to_file(file_id, "my_file.txt")
+    >>> civis.io.civis_to_file(file_id, "my_file.txt")
     >>> # Download a file to a file object.
     >>> with open("my_file.txt", "wb") as f:
-    ...    civis_to_file(file_id, f)
+    ...    civis.io.civis_to_file(file_id, f)
     >>> # Download a file as a bytes object.
     >>> import io
     >>> buf = io.BytesIO()
-    >>> civis_to_file(file_id, buf)
+    >>> civis.io.civis_to_file(file_id, buf)
     >>> # Note that s could be converted to a string with s.decode('utf-8').
     >>> s = buf.read()
     """
-    if isinstance(buf, six.string_types):
-        with open(buf, 'wb') as f:
-            _civis_to_file(file_id, f, api_key=api_key, client=client)
+    if isinstance(buf, str):
+        with open(buf, "wb") as f:
+            _civis_to_file(file_id, f, client=client)
     else:
-        _civis_to_file(file_id, buf, api_key=api_key, client=client)
+        _civis_to_file(file_id, buf, client=client)
         buf.flush()
 
 
-def _civis_to_file(file_id, buf, api_key=None, client=None):
+def _civis_to_file(file_id, buf, client=None):
     if client is None:
-        client = APIClient(api_key=api_key)
+        client = APIClient()
     files_response = client.files.get(file_id)
     url = files_response.file_url
     if not url:
-        raise EmptyResultError('Unable to locate file {}. If it previously '
-                               'existed, it may have '
-                               'expired.'.format(file_id))
+        raise EmptyResultError(
+            "Unable to locate file {}. If it previously "
+            "existed, it may have "
+            "expired.".format(file_id)
+        )
 
     # Store the current buffer position in case we need to retry below.
     buf_orig_position = buf.tell()
 
     @retry(RETRY_EXCEPTIONS)
     def _download_url_to_buf():
         # Reset the buffer in case we had to retry.
         buf.seek(buf_orig_position)
 
-        response = requests.get(url, stream=True)
+        response = requests.get(url, stream=True, timeout=60)
         response.raise_for_status()
         chunked = response.iter_content(CHUNK_SIZE)
         for lines in chunked:
             buf.write(lines)
 
     _download_url_to_buf()
 
@@ -344,74 +398,82 @@
     The run output is required to have type "File".
     If using an approximate match and multiple names match the
     provided string, return only the first file ID.
 
     Parameters
     ----------
     name : str
-        The "name" field of the run output you wish to retrieve
+        The "name" field of the run output you wish to retrieve. If
+        `.*?` is passed in and regex is set to True, this will
+        retrieve the file ID of the first run output
     job_id : int
     run_id : int
     regex : bool, optional
         If False (the default), require an exact string match between
         ``name`` and the name of the run output. If True, search for a
         name which matches the regular expression ``name`` and
         retrieve the first found.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
 
     Returns
     -------
     file_id : int
-        The ID of a Civis File with name matching ``name``
+        The ID of a Civis File with name matching ``name`` or, if
+        name = `".*?"` and regex = True, the ID of the first run
+        output
 
     Raises
     ------
     IOError
         If the provided job ID and run ID combination can't be found
     FileNotFoundError
         If the run exists, but ``name`` isn't in its run outputs
 
     See Also
     --------
-    APIClient.scripts.list_containers.runs_outputs
+    :func:`civis.APIClient.jobs.list_runs_outputs`
     """
     client = APIClient() if client is None else client
     # Retrieve run outputs
     try:
-        outputs = client.scripts.list_containers_runs_outputs(job_id, run_id)
+        outputs = client.jobs.list_runs_outputs(job_id, run_id)
     except CivisAPIError as err:
         if err.status_code == 404:
-            six.raise_from(IOError('Could not find job/run ID {}/{}'
-                           .format(job_id, run_id)), err)
+            raise IOError(
+                "Could not find job/run ID {}/{}".format(job_id, run_id)
+            ) from err
         else:
             raise
 
     # Find file in the run outputs.
     if not regex:
         # Require an exact match on the "name" string.
-        obj = find_one(outputs, name=name, object_type='File')
+        obj = find_one(outputs, name=name, object_type="File")
     else:
         # Search for a filename which contains the "name" string
-        obj_matches = [o for o in outputs
-                       if re.search(name, o.name) and o.object_type == 'File']
+        obj_matches = [
+            o for o in outputs if re.search(name, o.name) and o.object_type == "File"
+        ]
         if len(obj_matches) > 1:
-            log.warning('Found %s matches to "%s". Returning the first.',
-                        len(obj_matches), name)
+            log.warning(
+                'Found %s matches to "%s". Returning the first.', len(obj_matches), name
+            )
         obj = None if not obj_matches else obj_matches[0]
     if obj is None:
         prefix = "A file containing the pattern" if regex else "File"
-        raise FileNotFoundError('{} "{}" is not an output of job/run ID '
-                                '{}/{}.'.format(prefix, name, job_id, run_id))
-    return obj['object_id']
+        raise FileNotFoundError(
+            '{} "{}" is not an output of job/run ID '
+            "{}/{}.".format(prefix, name, job_id, run_id)
+        )
+    return obj["object_id"]
 
 
-def file_to_dataframe(file_id, compression='infer', client=None,
-                      **read_kwargs):
+def file_to_dataframe(file_id, compression="infer", client=None, **read_kwargs):
     """Load a :class:`~pandas.DataFrame` from a CSV stored in a Civis File
 
     The :class:`~pandas.DataFrame` will be read directly from Civis
     without copying the CSV to a local file on disk.
 
     Parameters
     ----------
@@ -438,28 +500,81 @@
         If ``pandas`` is not available
 
     See Also
     --------
     pandas.read_csv
     """
     if not HAS_PANDAS:
-        raise ImportError('file_to_dataframe requires pandas to be installed.')
+        raise ImportError("file_to_dataframe requires pandas to be installed.")
     client = APIClient() if client is None else client
     file_info = client.files.get(file_id)
     file_url = file_info.file_url
+    if not file_url:
+        raise EmptyResultError(
+            "Unable to locate file {}. If it previously "
+            "existed, it may have "
+            "expired.".format(file_id)
+        )
     file_name = file_info.name
-    if compression == 'infer':
-        comp_exts = {'.gz': 'gzip', '.xz': 'xz', '.bz2': 'bz2', '.zip': 'zip'}
+    if compression == "infer":
+        comp_exts = {".gz": "gzip", ".xz": "xz", ".bz2": "bz2", ".zip": "zip"}
         ext = os.path.splitext(file_name)[-1]
         if ext in comp_exts:
             compression = comp_exts[ext]
 
     return pd.read_csv(file_url, compression=compression, **read_kwargs)
 
 
+def dataframe_to_file(
+    df, name="data.csv", expires_at="DEFAULT", client=None, **to_csv_kws
+):
+    """Store a :class:`~pandas.DataFrame` as a CSV in Civis Platform
+
+    Parameters
+    ----------
+    df : :class:`~pandas.DataFrame`
+        The table to upload.
+    name : str, optional
+        The name of the Civis File
+    expires_at : str, optional
+        The date and time the file will expire. If not specified, the file
+        will expire in 30 days. To keep a file indefinitely, specify ``None``.
+        To specify a date and time, format it by the ISO 8601 standard,
+        e.g., ``"2020-12-31"``, ``"2020-12-31T23:03:40Z"``,
+        and what the ``isoformat()`` method returns from
+        a :class:`datetime.date <datetime.date>`
+        or :class:`datetime.datetime <datetime.datetime>` object.
+    client : :class:`civis.APIClient`, optional
+        If not provided, an :class:`civis.APIClient` object will be
+        created from the :envvar:`CIVIS_API_KEY`.
+    **to_csv_kws
+        Additional keyword parameters will be passed directly to
+        :func:`~pandas.DataFrame.to_csv`.
+
+    Returns
+    -------
+    file_id : int
+        The integer ID of the new Civis File object
+
+    See Also
+    --------
+    :func:`file_to_civis`
+    :func:`~pandas.DataFrame.to_csv`
+    """
+    with TemporaryDirectory() as tdir:
+        path = os.path.join(tdir, name)
+        df.to_csv(path, **to_csv_kws)
+        file_kwargs = {"name": name}
+        if expires_at != "DEFAULT":
+            # A missing parameter signifies the default value here.
+            file_kwargs["expires_at"] = expires_at
+        fid = file_to_civis(path, client=client, **file_kwargs)
+    return fid
+
+
 def file_to_json(file_id, client=None, **json_kwargs):
     """Restore JSON stored in a Civis File
 
     Parameters
     ----------
     file_id : int
         ID of a JSON-formatted Civis File
@@ -477,10 +592,59 @@
     See Also
     --------
     :func:`civis_to_file`
     :func:`json.load`
     """
     buf = io.BytesIO()
     civis_to_file(file_id, buf, client=client)
-    txt = io.TextIOWrapper(buf, encoding='utf-8')
+    txt = io.TextIOWrapper(buf, encoding="utf-8")
     txt.seek(0)
     return json.load(txt, **json_kwargs)
+
+
+def json_to_file(
+    obj, name="file.json", expires_at="DEFAULT", client=None, **json_kwargs
+):
+    """Store a JSON-serializable object in a Civis File
+
+    Parameters
+    ----------
+    obj
+        The object to be JSON-serialized and stored in a Civis File
+    name : str, optional
+        The name of the Civis File
+    expires_at : str, optional
+        The date and time the file will expire. If not specified, the file
+        will expire in 30 days. To keep a file indefinitely, specify ``None``.
+        To specify a date and time, format it by the ISO 8601 standard,
+        e.g., ``"2020-12-31"``, ``"2020-12-31T23:03:40Z"``,
+        and what the ``isoformat()`` method returns from
+        a :class:`datetime.date <datetime.date>`
+        or :class:`datetime.datetime <datetime.datetime>` object.
+    client : :class:`civis.APIClient`, optional
+        If not provided, an :class:`civis.APIClient` object will be
+        created from the :envvar:`CIVIS_API_KEY`.
+    **json_kwargs
+        Additional keyword arguments will be passed directly to
+        :func:`json.dump`.
+
+    Returns
+    -------
+    file_id : int
+        The integer ID of the new Civis File object
+
+    See Also
+    --------
+    :func:`file_to_civis`
+    :func:`json.dump`
+    """
+    buf = io.BytesIO()
+    txt = io.TextIOWrapper(buf, encoding="utf-8")
+    json.dump(obj, txt, **json_kwargs)
+    txt.seek(0)
+
+    file_kwargs = {"name": name}
+    if expires_at != "DEFAULT":
+        # A missing parameter signifies the default value here.
+        file_kwargs["expires_at"] = expires_at
+    fid = file_to_civis(txt.buffer, client=client, **file_kwargs)
+    return fid
```

### Comparing `civis-1.9.4/civis/tests/test_futures.py` & `civis-2.0.0/tests/test_futures.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,331 +1,226 @@
-import os
 import json
-from collections import OrderedDict
+import warnings
+from operator import itemgetter
+from unittest import mock
 
 import pytest
+import requests
 
 from civis import APIClient, response
 from civis.base import CivisAPIError, CivisJobFailure
-from civis.compat import mock
-from civis.resources._resources import get_api_spec, generate_classes
-from civis.futures import (ContainerFuture,
-                           _ContainerShellExecutor,
-                           CustomScriptExecutor,
-                           _create_docker_command)
-
-from civis.futures import (CivisFuture,
-                           JobCompleteListener,
-                           _LONG_POLLING_INTERVAL)
-from civis.tests import TEST_SPEC
-from pubnub.enums import PNStatusCategory
-
-from civis.tests.testcase import CivisVCRTestCase
-
-api_import_str = 'civis.resources._resources.get_api_spec'
-THIS_DIR = os.path.dirname(os.path.realpath(__file__))
-with open(TEST_SPEC) as f:
-    civis_api_spec_base = json.load(f, object_pairs_hook=OrderedDict)
-
-with open(os.path.join(THIS_DIR, "civis_api_spec_channels.json")) as f:
-    civis_api_spec_channels = json.load(f, object_pairs_hook=OrderedDict)
-
-
-def clear_lru_cache():
-    # LRU cache persists between tests so these caches need to be cleared
-    # when different api specs are used in different test cases
-    get_api_spec.cache_clear()
-    generate_classes.cache_clear()
-
-
-def setup_listener_status_mocks(status_category):
-    match = mock.Mock()
-    callback = mock.Mock()
-    disconnect = mock.Mock()
-    listener = JobCompleteListener(match, callback, disconnect)
-    status = mock.Mock()
-    status.category = status_category
-    return match, callback, disconnect, listener, status
-
-
-class CivisFutureTests(CivisVCRTestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        clear_lru_cache()
-
-    @classmethod
-    def tearDownClass(cls):
-        clear_lru_cache()
-
-    def test_listener_calls_callback_when_message_matches(self):
-        match = mock.Mock()
-        match.return_value = True
-        callback = mock.Mock()
-        listener = JobCompleteListener(match, callback)
-        message = mock.Mock()
-        message.message.return_value = 'test message'
-
-        listener.message(None, message)
-        match.assert_called_with(message.message)
-        self.assertEqual(callback.call_count, 1)
-
-    def test_listener_does_not_call_callback(self):
-        match = mock.Mock()
-        match.return_value = False
-        callback = mock.Mock()
-        listener = JobCompleteListener(match, callback)
-        message = mock.Mock()
-        message.message.return_value = 'test message'
-
-        listener.message(None, message)
-        match.assert_called_with(message.message)
-        self.assertEqual(callback.call_count, 0)
-
-    def test_listener_calls_disconnect_callback_when_status_disconnect(self):
-        disconnect_categories = [
-            PNStatusCategory.PNTimeoutCategory,
-            PNStatusCategory.PNNetworkIssuesCategory,
-            PNStatusCategory.PNUnexpectedDisconnectCategory,
-        ]
-        for category in disconnect_categories:
-            mocks = setup_listener_status_mocks(category)
-            _, _, disconnect, listener, status = mocks
-            listener.status(None, status)
-            assert disconnect.call_count == 1
-
-    def test_listener_does_note_call_disconnect_callback_on_other_status(self):
-        nondisconnect_categories = [
-            PNStatusCategory.PNAcknowledgmentCategory,
-            PNStatusCategory.PNConnectedCategory,
-            PNStatusCategory.PNReconnectedCategory,
-        ]
-        for category in nondisconnect_categories:
-            mocks = setup_listener_status_mocks(category)
-            _, _, disconnect, listener, status = mocks
-            listener.status(None, status)
-            assert disconnect.call_count == 0
-
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_check_message(self, *mocks):
-        result = CivisFuture(lambda x: x, (1, 20))
-        message = {
-            'object': {
-                'id': 1
-            },
-            'run': {
-                'id': 20,
-                'state': 'succeeded'
-            }
-        }
-        self.assertTrue(result._check_message(message))
+from civis.futures import (
+    ContainerFuture,
+    _ContainerShellExecutor,
+    CustomScriptExecutor,
+    _create_docker_command,
+)
 
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_check_message_with_different_run_id(self, *mocks):
-        result = CivisFuture(lambda x: x, (1, 20))
-        message = {
-            'object': {
-                'id': 2
-            },
-            'run': {
-                'id': 20,
-                'state': 'succeeded'
-            }
-        }
-        self.assertFalse(result._check_message(message))
+from civis.futures import CivisFuture
+from civis.tests import create_client_mock, create_client_mock_for_container_tests
+
+
+def _create_poller_mock(state: str) -> mock.Mock:
+    api_result = mock.Mock(state=state)
+    poller = mock.Mock(return_value=api_result)
+    return poller
+
+
+def test_check_message():
+    mock_civis = create_client_mock()
+    result = CivisFuture(lambda x: x, (1, 20), client=mock_civis)
+    message = {"object": {"id": 1}, "run": {"id": 20, "state": "succeeded"}}
+    assert result._check_message(message) is True
+
+
+def test_check_message_with_different_run_id():
+    mock_civis = create_client_mock()
+    result = CivisFuture(lambda x: x, (1, 20), client=mock_civis)
+    message = {"object": {"id": 2}, "run": {"id": 20, "state": "succeeded"}}
+    assert result._check_message(message) is False
 
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_check_message_when_job_is_running(self, *mocks):
-        result = CivisFuture(lambda x: x, (1, 20))
-        message = {
-            'object': {
-                'id': 1
-            },
-            'run': {
-                'id': 20,
-                'state': 'running'
-            }
-        }
-        self.assertFalse(result._check_message(message))
 
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_set_api_result_result_succeeded(self, mock_subscribe, mock_api):
-        mock_pubnub = mock.Mock()
-        mock_pubnub.unsubscribe_all.return_value = None
-        mock_subscribe.return_value = mock_pubnub
-        poller = mock.Mock()
-        api_result = mock.Mock()
-        api_result.state = 'succeeded'
-
-        result = CivisFuture(poller, (1, 2))
-        result._set_api_result(api_result)
-        assert poller.call_count == 0
-        assert mock_pubnub.unsubscribe_all.call_count == 1
-        assert result._state == 'FINISHED'
-
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_set_api_result_failed(self, mock_subscribe, mock_api):
-        mock_pubnub = mock.Mock()
-        mock_pubnub.unsubscribe_all.return_value = None
-        mock_subscribe.return_value = mock_pubnub
-        poller = mock.Mock()
-        api_result = mock.Mock()
-        api_result.state = 'failed'
-
-        result = CivisFuture(poller, (1, 2))
-        result._set_api_result(api_result)
-        assert mock_pubnub.unsubscribe_all.call_count == 1
-        assert result._state == 'FINISHED'
-        with pytest.raises(CivisJobFailure):
-            result.result()
-
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_subscribed_with_channels(self, *mocks):
-        future = CivisFuture(lambda x: x,
-                             (1, 20))
-        future._pubnub.get_subscribed_channels.return_value = [1]
-        assert future.subscribed is True
-
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_subscribed_with_no_subscription(self, *mocks):
-        future = CivisFuture(lambda x: x,
-                             (1, 20))
-        future._pubnub.get_subscribed_channels.return_value = []
-        assert future.subscribed is False
-
-    @mock.patch(api_import_str, return_value=civis_api_spec_base)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_subscribed_with_no_channels(self, *mocks):
-        clear_lru_cache()
-        future = CivisFuture(lambda x: x,
-                             (1, 20))
-        assert future.subscribed is False
-        clear_lru_cache()
-
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_overwrite_polling_interval_with_channels(self, *mocks):
-        future = CivisFuture(lambda x: x, (1, 20))
-        assert future.polling_interval == _LONG_POLLING_INTERVAL
-        assert hasattr(future, '_pubnub')
-
-    @mock.patch(api_import_str, return_value=civis_api_spec_channels)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_explicit_polling_interval_with_channels(self, *mocks):
-        future = CivisFuture(lambda x: x, (1, 20), polling_interval=5)
-        assert future.polling_interval == 5
-        assert hasattr(future, '_pubnub')
-
-    @mock.patch(api_import_str, return_value=civis_api_spec_base)
-    @mock.patch.object(CivisFuture, '_subscribe')
-    def test_polling_interval(self, *mocks):
-        # This tests the fallback to polling when channels is not available.
-        # It uses a different api spec than the other tests so it
-        # should clear the cached values before and after
-        clear_lru_cache()
-
-        polling_interval = 30
-        future = CivisFuture(lambda x: x,
-                             (1, 20),
-                             polling_interval=polling_interval)
-        assert future.polling_interval == polling_interval
-        assert hasattr(future, '_pubnub') is False
+def test_check_message_when_job_is_running():
+    mock_civis = create_client_mock()
+    result = CivisFuture(lambda x: x, (1, 20), client=mock_civis)
+    message = {"object": {"id": 1}, "run": {"id": 20, "state": "running"}}
+    assert result._check_message(message) is False
 
-        clear_lru_cache()
+
+def test_poller_call_count_poll_on_creation_true():
+    mock_civis = create_client_mock()
+    poller = _create_poller_mock("succeeded")
+    CivisFuture(poller, (1, 2), poll_on_creation=True, client=mock_civis)
+    assert poller.call_count == 1
+
+
+def test_poller_call_count_poll_on_creation_false():
+    mock_civis = create_client_mock()
+    poller = _create_poller_mock("succeeded")
+    CivisFuture(poller, (1, 2), poll_on_creation=False, client=mock_civis)
+    assert poller.call_count == 0
+
+
+def test_set_api_result_succeeded():
+    mock_civis = create_client_mock()
+    poller = _create_poller_mock("succeeded")
+    result = CivisFuture(poller, (1, 2), client=mock_civis)
+    assert result._state == "FINISHED"
+
+
+@mock.patch("civis.futures.time.sleep", side_effect=lambda x: None)
+def test_set_api_result_failed(m_sleep):
+    mock_civis = create_client_mock()
+    poller = _create_poller_mock("failed")
+    result = CivisFuture(poller, (1, 2), client=mock_civis)
+    assert result._state == "FINISHED"
+    with pytest.raises(CivisJobFailure):
+        result.result()
+    with pytest.raises(CivisJobFailure):
+        result.outputs()
+
+
+def test_outputs_succeeded():
+    poller = _create_poller_mock("succeeded")
+    mock_client = create_client_mock()
+    expected_return = [{"test": "test_result"}]
+    mock_client.jobs.list_runs_outputs.return_value = expected_return
+
+    result = CivisFuture(poller, (1, 2), client=mock_client)
+    assert result.outputs() == expected_return
+
+
+def test_polling_interval():
+    mock_client = create_client_mock()
+    polling_interval = 30
+    future = CivisFuture(
+        lambda x: x, (1, 20), polling_interval=polling_interval, client=mock_client
+    )
+    assert future.polling_interval == polling_interval
 
 
 def _check_executor(from_template_id=None):
     job_id, run_id = 42, 43
     c = _setup_client_mock(job_id, run_id, n_failures=0)
     mock_run = c.scripts.post_containers_runs()
     if from_template_id:
-        bpe = CustomScriptExecutor(from_template_id=from_template_id,
-                                   client=c, polling_interval=0.01)
-        future = bpe.submit(my_param='spam')
+        bpe = CustomScriptExecutor(
+            from_template_id=from_template_id, client=c, polling_interval=0.01
+        )
+        future = bpe.submit(my_param="spam")
     else:
         bpe = _ContainerShellExecutor(client=c, polling_interval=0.01)
         future = bpe.submit("foo")
 
     # Mock and test running, future.job_id, and done()
-    mock_run.state = "running"
+    mock_run._replace("state", "running")
     assert future.running(), "future is incorrectly marked as not running"
     assert future.job_id == job_id, "job_id not stored properly"
     assert not future.done(), "future is incorrectly marked as done"
 
     future.cancel()
 
     # Mock and test cancelled()
     assert future.cancelled(), "cancelled() did not return True as expected"
     assert not future.running(), "running() did not return False as expected"
 
     # Mock and test done()
-    mock_run.state = "succeeded"
+    mock_run._replace("state", "succeeded")
     assert future.done(), "done() did not return True as expected"
 
     # Test cancelling all jobs.
-    mock_run.state = "running"
+    mock_run._replace("state", "running")
     bpe.cancel_all()
     assert future.cancelled(), "cancel_all() failed"
 
     # Test shutdown method.
     bpe.shutdown(wait=True)
     assert future.done(), "shutdown() failed"
 
     return c
 
 
+@pytest.mark.parametrize(
+    "poller_args,expected_job_id,expected_run_id",
+    [((123, 456), 123, 456), ((123,), 123, None)],
+)
+def test_future_job_id_run_id(poller_args, expected_job_id, expected_run_id):
+    result = CivisFuture(
+        poller=_create_poller_mock("succeeded"),
+        poller_args=poller_args,
+        client=create_client_mock(),
+    )
+    assert result.job_id == expected_job_id
+    assert result.run_id == expected_run_id
+    assert result.job_url == (
+        f"https://platform.civisanalytics.com/spa/#/jobs/{expected_job_id}"
+    )
+
+
+def test_container_future_job_id_run_id():
+    job_id, run_id = 123, 456
+    result = ContainerFuture(
+        job_id=job_id,
+        run_id=run_id,
+        client=create_client_mock_for_container_tests(),
+    )
+    assert result.job_id == job_id
+    assert result.run_id == run_id
+    assert result.job_url == f"https://platform.civisanalytics.com/spa/#/jobs/{job_id}"
+
+
 def test_container_scripts():
     c = _check_executor()
     assert c.scripts.post_custom.call_count == 0
     assert c.scripts.post_containers.call_count > 0
 
 
 def test_custom_scripts():
-    with mock.patch.dict('os.environ', {'CIVIS_JOB_ID': '12',
-                                        'CIVIS_RUN_ID': '40'}):
+    with mock.patch.dict("os.environ", {"CIVIS_JOB_ID": "12", "CIVIS_RUN_ID": "40"}):
         c = _check_executor(133)
     assert c.scripts.post_custom.call_count > 0
     assert c.scripts.post_containers.call_count == 0
 
     # Verify that this script's job and run ID are passed to arguments
-    args = c.scripts.post_custom.call_args[1].get('arguments')
-    for k, v in (('CIVIS_PARENT_JOB_ID', '12'), ('CIVIS_PARENT_RUN_ID', '40')):
+    args = c.scripts.post_custom.call_args[1].get("arguments")
+    for k, v in (("CIVIS_PARENT_JOB_ID", "12"), ("CIVIS_PARENT_RUN_ID", "40")):
         assert args.get(k) == v
 
 
-def test_container_script_param_injection():
+@pytest.mark.parametrize("is_child_job", [False, True])
+def test_container_script_param_injection(is_child_job):
     # Test that child jobs created by the shell executor have the
     # job and run IDs of the script which created them (if any).
-    job_id, run_id = '123', '13'
+    job_id, run_id = "123", "13"
     c = _setup_client_mock(42, 43, n_failures=0)
-    with mock.patch.dict('os.environ', {'CIVIS_JOB_ID': job_id,
-                                        'CIVIS_RUN_ID': run_id}):
-        bpe = _ContainerShellExecutor(client=c, polling_interval=0.01)
+    mock_env = {"CIVIS_JOB_ID": job_id, "CIVIS_RUN_ID": run_id}
+
+    with mock.patch.dict("os.environ", mock_env):
+        init_kwargs = dict(client=c, polling_interval=0.01)
+        if is_child_job:
+            init_kwargs["params"] = [
+                {"name": "CIVIS_PARENT_JOB_ID", "type": "integer", "value": "888"},
+                {"name": "CIVIS_PARENT_RUN_ID", "type": "integer", "value": "999"},
+            ]
+        bpe = _ContainerShellExecutor(**init_kwargs)
         bpe.submit("foo")
 
-    params = c.scripts.post_containers.call_args[1].get('params')
-    assert params is not None
-    assert {'name': 'CIVIS_PARENT_JOB_ID', 'type': 'integer',
-            'value': job_id} in params, \
-        "The creator's job ID wasn't passed to the child."
-    assert {'name': 'CIVIS_PARENT_RUN_ID', 'type': 'integer',
-            'value': run_id} in params, \
-        "The creator's run ID wasn't passed to the child."
+    params = sorted(
+        c.scripts.post_containers.call_args[1].get("params"), key=itemgetter("name")
+    )
+    assert params == [
+        {"name": "CIVIS_PARENT_JOB_ID", "type": "integer", "value": job_id},
+        {"name": "CIVIS_PARENT_RUN_ID", "type": "integer", "value": run_id},
+    ], "The parent job parameters were not set correctly."
 
 
 def test_create_docker_command():
-    res = _create_docker_command("foo.sh", "bar", "baz", wibble="wibble1",
-                                 wobble="wobble1")
+    res = _create_docker_command(
+        "foo.sh", "bar", "baz", wibble="wibble1", wobble="wobble1"
+    )
     assert res == "foo.sh bar baz --wibble wibble1 --wobble wobble1"
 
 
 # A function to raise fake API errors the first
 # num_failures times it is called.
 def _make_error_func(num_failures, failure_is_error=False):
     """Raise API errors multiple times before succeeding
@@ -342,34 +237,34 @@
 
     Returns
     -------
     MockRun
         Mock which imitates the result of a `post_containers_runs`
         or `get_containers_runs` call
     """
-    counter = {'failures': 0}  # Use a dict so we can modify it in the closure
+    counter = {"failures": 0}  # Use a dict so we can modify it in the closure
 
     def mock_api_error(job_id, run_id):
-        if counter['failures'] < num_failures:
-            counter['failures'] += 1
+        if counter["failures"] < num_failures:
+            counter["failures"] += 1
             if failure_is_error:
                 raise CivisAPIError(mock.MagicMock())
             else:
-                return response.Response({'id': run_id,
-                                          'container_id': job_id,
-                                          'state': 'failed'})
+                return response.Response(
+                    {"id": run_id, "container_id": job_id, "state": "failed"}
+                )
         else:
-            return response.Response({'id': run_id,
-                                      'container_id': job_id,
-                                      'state': 'succeeded'})
+            return response.Response(
+                {"id": run_id, "container_id": job_id, "state": "succeeded"}
+            )
+
     return mock_api_error
 
 
-def _setup_client_mock(job_id=-10, run_id=100, n_failures=8,
-                       failure_is_error=False):
+def _setup_client_mock(job_id=-10, run_id=100, n_failures=8, failure_is_error=False):
     """Return a Mock set up for use in testing container scripts
 
     Parameters
     ----------
     job_id: int
         Mock-create containers with this ID when calling `post_containers`
         or `post_containers_runs`.
@@ -386,55 +281,63 @@
     `unittest.mock.Mock`
         With `post_containers`, `post_containers_runs`, and
         `get_containers_runs` methods set up.
     """
     c = mock.Mock()
     c.__class__ = APIClient
 
-    mock_container = response.Response({'id': job_id})
+    mock_container = response.Response({"id": job_id})
     c.scripts.post_containers.return_value = mock_container
     c.scripts.post_custom.return_value = mock_container
-    mock_container_run = response.Response({'id': run_id,
-                                            'container_id': job_id,
-                                            'state': 'queued'})
+    mock_container_run = response.Response(
+        {"id": run_id, "container_id": job_id, "state": "queued"}
+    )
     c.scripts.post_containers_runs.return_value = mock_container_run
     c.jobs.post_runs.return_value = mock_container_run
     c.scripts.get_containers_runs.side_effect = _make_error_func(
-        n_failures, failure_is_error)
+        n_failures, failure_is_error
+    )
 
     def change_state_to_cancelled(job_id):
-        mock_container_run.state = "cancelled"
+        mock_container_run._replace("state", "cancelled")
         return mock_container_run
 
     c.scripts.post_cancel.side_effect = change_state_to_cancelled
-    del c.channels  # Remove "channels" endpoint to fall back on polling
 
     return c
 
 
 def test_cancel_finished_job():
     # If we try to cancel a completed job, we get a 404 error.
     # That shouldn't be sent to the user.
 
     # Set up a mock client which will give an exception when
     # you try to cancel any job.
     c = _setup_client_mock()
-    err_resp = response.Response({
-        'status_code': 404,
-        'error': 'not_found',
-        'errorDescription': 'The requested resource could not be found.',
-        'content': True})
-    err_resp.json = lambda: err_resp.json_data
+    err_resp = requests.Response()
+    status_code = 404
+    err_resp.status_code = status_code
+    err_resp._content = json.dumps(
+        {
+            "status_code": status_code,
+            "error": "not_found",
+            "errorDescription": "The requested resource could not be found.",
+            "content": True,
+        }
+    ).encode()
     c.scripts.post_cancel.side_effect = CivisAPIError(err_resp)
-    c.scripts.post_containers_runs.return_value.state = 'running'
-
-    fut = ContainerFuture(-10, 100, polling_interval=1, client=c,
-                          poll_on_creation=False)
+    c.scripts.post_containers_runs.return_value._replace("state", "running")
+    fut = ContainerFuture(
+        -10, 100, polling_interval=1, client=c, poll_on_creation=False
+    )
     assert not fut.done()
-    assert fut.cancel() is False
+    with warnings.catch_warnings():
+        # Check that no warnings are raised.
+        warnings.simplefilter("error")
+        assert fut.cancel() is False
 
 
 def test_future_no_retry_error():
     # Verify that with no retries, exceptions on job polling
     #  are raised to the user
     c = _setup_client_mock(failure_is_error=True)
     fut = ContainerFuture(-10, 100, polling_interval=0.001, client=c)
@@ -451,37 +354,88 @@
         fut.result()
 
 
 def test_future_not_enough_retry_error():
     # Verify that if polling the run is still erroring after all retries
     # are exhausted, the error will be raised for the user.
     c = _setup_client_mock(failure_is_error=True)
-    fut = ContainerFuture(-10, 100, max_n_retries=3, polling_interval=0.01,
-                          client=c)
+    fut = ContainerFuture(-10, 100, max_n_retries=3, polling_interval=0.01, client=c)
     with pytest.raises(CivisAPIError):
         fut.result()
 
 
 def test_future_not_enough_retry_failure():
     # Verify that if the job is still failing after all retries
     # are exhausted, the job failure will be raised for the user.
     c = _setup_client_mock(failure_is_error=False)
-    fut = ContainerFuture(-10, 100, max_n_retries=3, polling_interval=0.01,
-                          client=c)
+    fut = ContainerFuture(-10, 100, max_n_retries=3, polling_interval=0.01, client=c)
     with pytest.raises(CivisJobFailure):
         fut.result()
 
 
 def test_future_retry_failure():
     # Verify that we can retry through API errors until a job succeeds
     c = _setup_client_mock(failure_is_error=False)
-    fut = ContainerFuture(-10, 100, max_n_retries=10, polling_interval=0.01,
-                          client=c)
-    assert fut.result().state == 'succeeded'
+    fut = ContainerFuture(-10, 100, max_n_retries=10, polling_interval=0.01, client=c)
+    assert fut.result().state == "succeeded"
 
 
 def test_future_retry_error():
     # Verify that we can retry through job failures until it succeeds
     c = _setup_client_mock(failure_is_error=True)
-    fut = ContainerFuture(-10, 100, max_n_retries=10, polling_interval=0.01,
-                          client=c)
-    assert fut.result().state == 'succeeded'
+    fut = ContainerFuture(-10, 100, max_n_retries=10, polling_interval=0.01, client=c)
+    assert fut.result().state == "succeeded"
+
+
+@mock.patch("civis.futures.time.sleep", side_effect=lambda x: None)
+def test_container_exception_no_result_logs(m_sleep):
+    # If the job errored with no output but with logs,
+    # we should return error logs with the future exception.
+    mem_msg = "Run used approximately 2 millicores " "of its 256 millicore CPU limit"
+    failed_msg = "Failed: The job container failed. Exit code 1"
+    logs = [
+        {"id": 111, "created_at": "abc", "message": mem_msg, "level": "info"},
+        {"id": 222, "created_at": "def", "message": failed_msg, "level": "error"},
+    ]
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="failed", run_outputs=[], log_outputs=logs
+    )
+    fut = ContainerFuture(1, 2, client=mock_client)
+
+    with pytest.raises(CivisJobFailure) as err:
+        fut.result()
+    expected_msg = "(From job 1 / run 2) " + "\n".join([failed_msg, mem_msg, ""])
+    assert expected_msg == str(fut._exception.error_message)
+    assert str(err.value) == expected_msg
+
+
+@mock.patch("civis.futures.time.sleep", side_effect=lambda x: None)
+def test_container_exception_memory_error(m_sleep):
+    err_msg = "Process ran out of its allowed 3000 MiB of " "memory and was killed."
+    logs = [
+        {
+            "created_at": "2017-05-10T12:00:00.000Z",
+            "id": 10005,
+            "level": "error",
+            "message": "Failed",
+        },
+        {
+            "created_at": "2017-05-10T12:00:00.000Z",
+            "id": 10003,
+            "level": "error",
+            "message": "Error on job: Process ended with an " "error, exiting: 137.",
+        },
+        {
+            "created_at": "2017-05-10T12:00:00.000Z",
+            "id": 10000,
+            "level": "error",
+            "message": err_msg,
+        },
+    ]
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="failed", run_outputs=[], log_outputs=logs
+    )
+    fut = ContainerFuture(1, 2, client=mock_client)
+
+    with pytest.raises(MemoryError) as err:
+        fut.result()
+    assert str(err.value) == f"(From job 1 / run 2) {err_msg}"
```

### Comparing `civis-1.9.4/civis/tests/test_parallel.py` & `civis-2.0.0/tests/test_parallel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,65 @@
 from math import sqrt
 import io
 import pickle
-from civis.compat import mock
+import warnings
+from unittest import mock
 
 import pytest
 from joblib import delayed, Parallel
 from joblib import parallel_backend, register_parallel_backend
-from joblib.my_exceptions import TransportableException
-from civis.base import CivisAPIError
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore", DeprecationWarning)
+    from joblib.my_exceptions import TransportableException
+
+from civis.base import CivisAPIError, CivisJobFailure
 from civis.response import Response
 import requests
 
 import civis.parallel
 from civis.futures import ContainerFuture
+from civis.tests import create_client_mock, create_client_mock_for_container_tests
+
+
+_MOCK_JOB_KWARGS = dict(
+    from_template_id=None,
+    id="42",
+    required_resources={"cpu": 11},
+    docker_image_name="image_name",
+    docker_image_tag="tag",
+    repo_http_uri="cabbage",
+    repo_ref="servant",
+    remote_host_credential_id=171,
+    git_credential_id=213,
+    cancel_timeout=23,
+    time_zone="America/Chicago",
+)
 
 
 @pytest.fixture
 def mock_job():
-    return Response(dict(from_template_id=None,
-                         id='42',
-                         required_resources={'cpu': 11},
-                         params=[{'name': 'spam'}],
-                         arguments={'spam': 'eggs'},
-                         docker_image_name='image_name',
-                         docker_image_tag='tag',
-                         repo_http_uri='cabbage',
-                         repo_ref='servant',
-                         remote_host_credential_id=171,
-                         git_credential_id=213,
-                         cancel_timeout=23,
-                         time_zone="America/Chicago",
-                         ))
+    return Response(
+        dict(params=[{"name": "spam"}], arguments={"spam": "eggs"}, **_MOCK_JOB_KWARGS)
+    )
 
 
-def test_retries():
+@pytest.fixture
+def mock_child_job():
+    params = [
+        {"name": "spam"},
+        {"name": "CIVIS_PARENT_JOB_ID", "value": "123"},
+        {"name": "CIVIS_PARENT_RUN_ID", "value": "456"},
+    ]
+    args = {"spam": "eggs"}
+    return Response(dict(params=params, arguments=args, **_MOCK_JOB_KWARGS))
+
+
+@mock.patch("civis.futures.time.sleep", side_effect=lambda x: None)
+def test_retries(m_sleep):
     """Make sure that job submission retry behavior works."""
 
     # Test that submission doesn't fail when there are no mock API errors.
     _test_retries_helper(0, 0, False, None)
     _test_retries_helper(0, 5, False, None)
 
     # Test that submission fails when there are API errors and too few retries.
@@ -53,449 +75,529 @@
 
 def test_from_template_id():
     _test_retries_helper(0, 5, False, 13)
     _test_retries_helper(1, 5, False, 13)
     _test_retries_helper(1, 0, True, 13)
 
 
-@mock.patch.object(civis.parallel, '_ContainerShellExecutor')
-@mock.patch.object(civis.parallel, 'CustomScriptExecutor')
-@mock.patch.object(civis.parallel, '_CivisBackendResult')
-@mock.patch.object(civis.parallel.civis.io, 'file_to_civis', autospec=True)
-def _test_retries_helper(num_failures, max_submit_retries,
-                         should_fail, from_template_id,
-                         mock_file_to_civis, mock_result_cls,
-                         mock_custom_exec_cls, mock_executor_cls):
+@mock.patch.object(civis.parallel, "_ContainerShellExecutor")
+@mock.patch.object(civis.parallel, "CustomScriptExecutor")
+@mock.patch.object(civis.parallel, "_CivisBackendResult")
+@mock.patch.object(civis.parallel.civis.io, "file_to_civis", autospec=True)
+def _test_retries_helper(
+    num_failures,
+    max_submit_retries,
+    should_fail,
+    from_template_id,
+    mock_file_to_civis,
+    mock_result_cls,
+    mock_custom_exec_cls,
+    mock_executor_cls,
+):
 
     mock_file_to_civis.return_value = 0
-    mock_result_cls.get.return_value = 123
+    mock_result_cls.return_value.get.return_value = [123]
 
     # A function to raise fake API errors the first num_failures times it is
     # called.
-    counter = {'n_failed': 0}
+    counter = {"n_failed": 0}
 
-    def mock_submit(fn='', *args, **kwargs):
-        if counter['n_failed'] < num_failures:
-            counter['n_failed'] += 1
+    def mock_submit(fn="", *args, **kwargs):
+        if counter["n_failed"] < num_failures:
+            counter["n_failed"] += 1
             raise CivisAPIError(mock.MagicMock())
         else:
             return mock.MagicMock(spec=ContainerFuture)
 
     mock_custom_exec_cls.return_value.submit.side_effect = mock_submit
     mock_executor_cls.return_value.submit.side_effect = mock_submit
 
     if from_template_id:
         factory = civis.parallel.make_backend_template_factory(
             from_template_id=from_template_id,
             max_submit_retries=max_submit_retries,
-            client=mock.Mock())
+            client=create_client_mock(),
+        )
     else:
         factory = civis.parallel.make_backend_factory(
-            max_submit_retries=max_submit_retries, client=mock.Mock())
-    register_parallel_backend('civis', factory)
-    with parallel_backend('civis'):
-        parallel = Parallel(n_jobs=5, pre_dispatch='n_jobs')
+            max_submit_retries=max_submit_retries, client=create_client_mock()
+        )
+    register_parallel_backend("civis", factory)
+    with parallel_backend("civis"):
+        # NB: joblib >v0.11 relies on callbacks from the result object to
+        # decide when it's done consuming inputs. We've mocked the result
+        # object here, so Parallel must be called either with n_jobs=1 or
+        # pre_dispatch='all' to consume the inputs all at once.
+        parallel = Parallel(n_jobs=1, pre_dispatch="n_jobs")
         if should_fail:
             with pytest.raises(civis.parallel.JobSubmissionError):
-                parallel(delayed(sqrt)(i ** 2) for i in range(3))
+                parallel(delayed(sqrt)(i**2) for i in range(3))
         else:
-            parallel(delayed(sqrt)(i ** 2) for i in range(3))
+            parallel(delayed(sqrt)(i**2) for i in range(3))
 
 
-@mock.patch.object(civis.parallel, 'CustomScriptExecutor')
-@mock.patch.object(civis.parallel, '_CivisBackendResult')
-@mock.patch.object(civis.parallel.civis.io, 'file_to_civis', autospec=True)
+@mock.patch.object(civis.parallel, "CustomScriptExecutor")
+@mock.patch.object(civis.parallel, "_CivisBackendResult")
+@mock.patch.object(civis.parallel.civis.io, "file_to_civis", autospec=True)
 def test_template_submit(mock_file, mock_result, mock_pool):
     # Verify that creating child jobs from a template looks like we expect
     file_id = 17
-    mock_client = mock.Mock()
+    mock_client = create_client_mock()
     mock_file.return_value = file_id
 
     factory = civis.parallel.make_backend_template_factory(
-        from_template_id=1234, client=mock_client)
+        from_template_id=1234, client=mock_client
+    )
 
     n_calls = 3
-    register_parallel_backend('civis', factory)
-    with parallel_backend('civis'):
-        parallel = Parallel(n_jobs=5, pre_dispatch='n_jobs')
-        parallel(delayed(sqrt)(i ** 2) for i in range(n_calls))
+    register_parallel_backend("civis", factory)
+    with parallel_backend("civis"):
+        # NB: joblib >v0.11 relies on callbacks from the result object to
+        # decide when it's done consuming inputs. We've mocked the result
+        # object here, so Parallel must be called either with n_jobs=1 or
+        # pre_dispatch='all' to consume the inputs all at once.
+        parallel = Parallel(n_jobs=1, pre_dispatch="n_jobs")
+        parallel(delayed(sqrt)(i**2) for i in range(n_calls))
 
     assert mock_file.call_count == 3, "Upload 3 functions to run"
     assert mock_pool().submit.call_count == n_calls, "Run 3 functions"
     for this_call in mock_pool().submit.call_args_list:
         assert this_call == mock.call(JOBLIB_FUNC_FILE_ID=file_id)
     assert mock_result.call_count == 3, "Create 3 results"
 
 
-@mock.patch.object(civis.parallel, '_CivisBackend')
+@mock.patch.object(civis.parallel, "_CivisBackend")
 def test_make_template(mock_backend):
     # Verify that the input setup command is recognized
     func = civis.parallel.make_backend_template_factory(1234)
 
     assert mock_backend.call_count == 0
     func()
     assert mock_backend.call_count == 1
-    assert mock_backend.call_args_list[0][1].get('from_template_id') == 1234
+    assert mock_backend.call_args_list[0][1].get("from_template_id") == 1234
 
 
-@mock.patch.object(civis.parallel, '_CivisBackend')
+@mock.patch.object(civis.parallel, "_CivisBackend")
 def test_setup_cmd(mock_backend):
     # Verify that the input setup command is recognized
-    func = civis.parallel.make_backend_factory(setup_cmd='sample')
+    func = civis.parallel.make_backend_factory(setup_cmd="sample")
 
     assert mock_backend.call_count == 0
     func()
     assert mock_backend.call_count == 1
-    assert mock_backend.call_args_list[0][1].get('setup_cmd') == 'sample'
+    assert mock_backend.call_args_list[0][1].get("setup_cmd") == "sample"
 
 
-@mock.patch.object(civis.parallel, '_CivisBackend')
+@mock.patch.object(civis.parallel, "_CivisBackend")
 def test_default_setup_cmd_no_repo(mock_backend):
     # Check that the setup command has the expected
     # default when the user does not input a GitHub repo
     func = civis.parallel.make_backend_factory()
 
     func()
     assert mock_backend.call_count == 1
-    assert mock_backend.call_args_list[0][1].get('setup_cmd') == ":"
+    assert mock_backend.call_args_list[0][1].get("setup_cmd") == ":"
 
 
-@mock.patch.object(civis.parallel, '_CivisBackend')
+@mock.patch.object(civis.parallel, "_CivisBackend")
 def test_default_setup_cmd_with_repo(mock_backend):
     # Check that the default setup command will attempt to install
     # a supplied GitHub repo.
-    func = civis.parallel.make_backend_factory(repo_http_uri='potato')
+    func = civis.parallel.make_backend_factory(repo_http_uri="potato")
 
     func()
     assert mock_backend.call_count == 1
-    assert mock_backend.call_args_list[0][1].get('setup_cmd') == \
-        "cd /app; python setup.py install; cd /"
+    assert (
+        mock_backend.call_args_list[0][1].get("setup_cmd")
+        == "cd /app; pip install .; cd /"
+    )
 
 
-@mock.patch.object(civis.parallel, 'make_backend_factory')
+@mock.patch.object(civis.parallel, "make_backend_factory")
 def test_infer_no_job_id_error(mock_make_factory, mock_job):
     # The `infer_backend_factory` should give a RuntimeError
     # if there's no CIVIS_JOB_ID in the environment.
-    mock_client = mock.MagicMock()
+    mock_client = create_client_mock()
     mock_client.scripts.get_containers.return_value = mock_job
-    with mock.patch.dict('os.environ', {}, clear=True):
+    with mock.patch.dict("os.environ", {}, clear=True):
         with pytest.raises(RuntimeError):
             civis.parallel.infer_backend_factory(client=mock_client)
 
 
-@mock.patch.object(civis.parallel, 'make_backend_factory')
+@mock.patch.object(civis.parallel, "make_backend_factory")
 def test_infer(mock_make_factory, mock_job):
     # Verify that `infer_backend_factory` passes through
     # the expected arguments to `make_backend_factory`.
-    mock_client = mock.MagicMock()
+    mock_client = create_client_mock()
     mock_client.scripts.get_containers.return_value = mock_job
-    with mock.patch.dict('os.environ', {'CIVIS_JOB_ID': "test_job",
-                                        'CIVIS_RUN_ID': "test_run"}):
+    with mock.patch.dict(
+        "os.environ", {"CIVIS_JOB_ID": "test_job", "CIVIS_RUN_ID": "test_run"}
+    ):
         civis.parallel.infer_backend_factory(client=mock_client)
 
-    expected = dict(mock_job)
-    del expected['from_template_id']
-    del expected['id']
+    expected = mock_job._data_snake
+    del expected["from_template_id"]
+    del expected["id"]
     mock_make_factory.assert_called_once_with(
         client=mock_client,
         setup_cmd=None,
         polling_interval=None,
         max_submit_retries=0,
         max_job_retries=0,
         hidden=True,
-        remote_backend='sequential',
-        **expected)
+        remote_backend="sequential",
+        **expected,
+    )
 
 
-@mock.patch.object(civis.parallel, 'make_backend_factory')
+@mock.patch.object(civis.parallel, "make_backend_factory")
 def test_infer_new_params(mock_make_factory, mock_job):
     # Test overwriting existing job parameters with new parameters
-    mock_client = mock.MagicMock()
+    mock_client = create_client_mock()
     mock_client.scripts.get_containers.return_value = mock_job
-    new_params = [{'name': 'spam', 'type': 'fun'},
-                  {'name': 'foo', 'type': 'bar'}]
-    with mock.patch.dict('os.environ', {'CIVIS_JOB_ID': "test_job",
-                                        'CIVIS_RUN_ID': "test_run"}):
-        civis.parallel.infer_backend_factory(
-            client=mock_client, params=new_params)
+    new_params = [{"name": "spam", "type": "fun"}, {"name": "foo", "type": "bar"}]
+    with mock.patch.dict(
+        "os.environ", {"CIVIS_JOB_ID": "test_job", "CIVIS_RUN_ID": "test_run"}
+    ):
+        civis.parallel.infer_backend_factory(client=mock_client, params=new_params)
 
-    assert mock_make_factory.call_args[1]['params'] == new_params
+    assert mock_make_factory.call_args[1]["params"] == new_params
 
 
-@mock.patch.object(civis.parallel, 'make_backend_factory')
+@mock.patch.object(civis.parallel, "make_backend_factory")
 def test_infer_extra_param(mock_make_factory, mock_job):
     # Test adding a new parameter and keeping
     # the existing parameter unchanged.
-    mock_client = mock.MagicMock()
+    mock_client = create_client_mock()
     mock_client.scripts.get_containers.return_value = mock_job
-    new_params = [{'name': 'foo', 'type': 'bar'}]
-    with mock.patch.dict('os.environ', {'CIVIS_JOB_ID': "test_job",
-                                        'CIVIS_RUN_ID': "test_run"}):
-        civis.parallel.infer_backend_factory(
-            client=mock_client, params=new_params)
+    new_params = [{"name": "foo", "type": "bar"}]
+    with mock.patch.dict(
+        "os.environ", {"CIVIS_JOB_ID": "test_job", "CIVIS_RUN_ID": "test_run"}
+    ):
+        civis.parallel.infer_backend_factory(client=mock_client, params=new_params)
+
+    assert mock_make_factory.call_args[1]["params"] == [
+        {"name": "spam"},
+        {"name": "foo", "type": "bar"},
+    ]
 
-    assert mock_make_factory.call_args[1]['params'] == \
-        [{'name': 'spam'}, {'name': 'foo', 'type': 'bar'}]
 
-
-@mock.patch.object(civis.parallel, 'make_backend_factory')
+@mock.patch.object(civis.parallel, "make_backend_factory")
 def test_infer_update_resources(mock_make_factory, mock_job):
     # Verify that users can modify requested resources for jobs.
-    mock_client = mock.MagicMock()
+    mock_client = create_client_mock()
     mock_client.scripts.get_containers.return_value = mock_job
-    with mock.patch.dict('os.environ', {'CIVIS_JOB_ID': "test_job",
-                                        'CIVIS_RUN_ID': "test_run"}):
+    with mock.patch.dict(
+        "os.environ", {"CIVIS_JOB_ID": "test_job", "CIVIS_RUN_ID": "test_run"}
+    ):
         civis.parallel.infer_backend_factory(
-            client=mock_client, required_resources={'cpu': -11})
+            client=mock_client, required_resources={"cpu": -11}
+        )
 
-    assert mock_make_factory.call_args[1]['required_resources'] == \
-        {'cpu': -11}
+    assert mock_make_factory.call_args[1]["required_resources"] == {"cpu": -11}
 
 
-@mock.patch.object(civis.parallel, 'make_backend_factory')
+@mock.patch.object(civis.parallel, "make_backend_factory")
 def test_infer_update_args(mock_make_factory, mock_job):
     # Verify that users can modify the existing job's
     # arguments for sub-processes.
-    mock_client = mock.MagicMock()
+    mock_client = create_client_mock()
     mock_client.scripts.get_containers.return_value = mock_job
-    with mock.patch.dict('os.environ', {'CIVIS_JOB_ID': "test_job",
-                                        'CIVIS_RUN_ID': "test_run"}):
+    with mock.patch.dict(
+        "os.environ", {"CIVIS_JOB_ID": "test_job", "CIVIS_RUN_ID": "test_run"}
+    ):
         civis.parallel.infer_backend_factory(
-            client=mock_client, arguments={'foo': 'bar'})
+            client=mock_client, arguments={"foo": "bar"}
+        )
 
-    assert mock_make_factory.call_args[1]['arguments'] == \
-        {'spam': 'eggs', 'foo': 'bar'}
+    assert mock_make_factory.call_args[1]["arguments"] == {"spam": "eggs", "foo": "bar"}
 
 
-@mock.patch.object(civis.parallel, 'make_backend_factory')
-def test_infer_from_custom_job(mock_make_factory):
+@mock.patch.object(civis.parallel, "make_backend_factory")
+def test_infer_from_custom_job(mock_make_factory, mock_job):
     # Test that `infer_backend_factory` can find needed
     # parameters if it's run inside a custom job created
     # from a template.
-    mock_client = mock.MagicMock()
-    mock_custom = Response(dict(from_template_id=999, id=42,
-                                required_resources=None,
-                                params=[{'name': 'spam'}],
-                                arguments={'spam': 'eggs'},
-                                docker_image_name='image_name',
-                                docker_image_tag='tag',
-                                repo_http_uri='cabbage', repo_ref='servant'))
-    mock_script = mock_job()
+    mock_client = create_client_mock()
+    mock_custom = Response(
+        dict(
+            from_template_id=999,
+            id=42,
+            required_resources=None,
+            params=[{"name": "spam"}],
+            arguments={"spam": "eggs"},
+            docker_image_name="image_name",
+            docker_image_tag="tag",
+            repo_http_uri="cabbage",
+            repo_ref="servant",
+        )
+    )
     mock_template = Response(dict(id=999, script_id=171))
 
     def _get_container(job_id):
         if int(job_id) == 42:
             return mock_custom
         elif int(job_id) == 171:
-            return mock_script
+            return mock_job
         else:
             raise ValueError("Got job_id {}".format(job_id))
 
     mock_client.scripts.get_containers.side_effect = _get_container
     mock_client.templates.get_scripts.return_value = mock_template
-    with mock.patch.dict('os.environ', {'CIVIS_JOB_ID': "42",
-                                        'CIVIS_RUN_ID': "test_run"}):
-        civis.parallel.infer_backend_factory(
-            client=mock_client)
+    with mock.patch.dict(
+        "os.environ", {"CIVIS_JOB_ID": "42", "CIVIS_RUN_ID": "test_run"}
+    ):
+        civis.parallel.infer_backend_factory(client=mock_client)
 
     # We should have called `get_containers` twice now -- once for
     # the container we're running in, and a second time for the
     # container which backs the template this job was created from.
     # The backing script has settings which aren't visible from
     # the container which was created from it.
     assert mock_client.scripts.get_containers.call_count == 2
     mock_client.templates.get_scripts.assert_called_once_with(999)
-    expected_kwargs = {'required_resources': {'cpu': 11},
-                       'params': [{'name': 'spam'}],
-                       'arguments': {'spam': 'eggs'},
-                       'client': mock.ANY,
-                       'polling_interval': mock.ANY,
-                       'setup_cmd': None,
-                       'max_submit_retries': mock.ANY,
-                       'max_job_retries': mock.ANY,
-                       'hidden': True,
-                       'remote_backend': 'sequential'}
+    expected_kwargs = {
+        "required_resources": {"cpu": 11},
+        "params": [{"name": "spam"}],
+        "arguments": {"spam": "eggs"},
+        "client": mock.ANY,
+        "polling_interval": mock.ANY,
+        "setup_cmd": None,
+        "max_submit_retries": mock.ANY,
+        "max_job_retries": mock.ANY,
+        "hidden": True,
+        "remote_backend": "sequential",
+    }
     for key in civis.parallel.KEYS_TO_INFER:
-        expected_kwargs[key] = mock_script[key]
+        expected_kwargs[key] = mock_job[key]
     mock_make_factory.assert_called_once_with(**expected_kwargs)
 
 
+@mock.patch.object(civis.parallel, "make_backend_factory")
+def test_infer_in_child_job(mock_make_factory, mock_child_job):
+    # Verify that infer_backend_factory doesn't include CIVIS_PARENT_JOB_ID and
+    # CIVIS_PARENT_RUN_ID since those will be automatically added later.
+    mock_client = create_client_mock()
+    mock_client.scripts.get_containers.return_value = mock_child_job
+    mock_env = {"CIVIS_JOB_ID": "test_job", "CIVIS_RUN_ID": "test_run"}
+    with mock.patch.dict("os.environ", mock_env):
+        civis.parallel.infer_backend_factory(client=mock_client)
+
+    assert mock_make_factory.call_args[1]["params"] == [{"name": "spam"}]
+
+
 def make_to_file_mock(result, max_n_err=0, exc=None):
-    cnt = {'err': 0}
+    cnt = {"err": 0}
 
     def mock_civis_to_file(file_id, buf, client=None):
-        if cnt['err'] < max_n_err:
-            cnt['err'] += 1
+        if cnt["err"] < max_n_err:
+            cnt["err"] += 1
             raise exc
         else:
             buf.write(pickle.dumps(result))
+
     return mock_civis_to_file
 
 
-@mock.patch.object(civis.parallel, 'civis')
+@mock.patch.object(civis.parallel, "civis")
 def test_result_success(mock_civis):
     # Test that we can get a result back from a succeeded job.
     callback = mock.MagicMock()
-    mock_civis.io.civis_to_file.side_effect = make_to_file_mock('spam')
-    fut = ContainerFuture(1, 2, client=mock.MagicMock())
-    fut.set_result(Response({'state': 'success'}))
+    mock_civis.io.civis_to_file.side_effect = make_to_file_mock("spam")
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="success", run_outputs=mock.MagicMock()
+    )
+    fut = ContainerFuture(1, 2, client=mock_client)
     res = civis.parallel._CivisBackendResult(fut, callback)
 
-    assert res.get() == 'spam'
+    assert res.get() == "spam"
     assert callback.call_count == 1
 
 
-@mock.patch.object(civis.parallel, 'civis')
+@mock.patch.object(civis.parallel, "civis")
 def test_result_callback_no_get(mock_civis):
     # Test that the completed callback happens even if we don't call `get`
     callback = mock.MagicMock()
-    mock_civis.io.civis_to_file.side_effect = make_to_file_mock('spam')
-    fut = ContainerFuture(1, 2, client=mock.MagicMock())
-    fut.set_result(Response({'state': 'success'}))
-
+    mock_civis.io.civis_to_file.side_effect = make_to_file_mock("spam")
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="success", run_outputs=mock.MagicMock()
+    )
+    fut = ContainerFuture(1, 2, client=mock_client)
     civis.parallel._CivisBackendResult(fut, callback)
     assert callback.call_count == 1
 
 
-@mock.patch.object(civis.parallel, 'civis')
-def test_result_exception(mock_civis):
+@mock.patch.object(civis.parallel, "civis")
+@mock.patch("civis.futures.time.sleep", side_effect=lambda x: None)
+def test_result_exception(m_sleep, mock_civis):
     # An error in the job should be raised by the result
     callback = mock.MagicMock()
     exc = ZeroDivisionError()
     mock_civis.io.civis_to_file.side_effect = make_to_file_mock(exc)
-    fut = ContainerFuture(1, 2, client=mock.MagicMock())
-    fut._set_api_exception(Response({'state': 'failed'}))
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="failed", run_outputs=mock.MagicMock()
+    )
+    fut = ContainerFuture(1, 2, client=mock_client)
     res = civis.parallel._CivisBackendResult(fut, callback)
 
     with pytest.raises(ZeroDivisionError):
         res.get()
     assert callback.call_count == 0
 
 
-def test_result_exception_no_result():
+@mock.patch("civis.futures.time.sleep", side_effect=lambda x: None)
+def test_result_exception_no_result(m_sleep):
     # If the job errored but didn't write an output, we should get
     # a generic TransportableException back.
     callback = mock.MagicMock()
 
-    # Passing the client mock as an argument instead of globally
-    # patching the client tests that the _CivisBackendResult
-    # uses the client object on the input CivisFuture.
-    mock_client = mock.MagicMock().APIClient()
-    mock_client.scripts.list_containers_runs_outputs.return_value = []
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="failed", run_outputs=[]
+    )
     fut = ContainerFuture(1, 2, client=mock_client)
-    fut._set_api_exception(Response({'state': 'failed'}))
     res = civis.parallel._CivisBackendResult(fut, callback)
+    fut._set_api_exception(CivisJobFailure(Response({"state": "failed"})))
 
     with pytest.raises(TransportableException) as exc:
         res.get()
+
     assert "{'state': 'failed'}" in str(exc.value)
     assert callback.call_count == 0
 
 
-@mock.patch.object(civis.parallel, 'civis')
+@mock.patch.object(civis.parallel, "civis")
 def test_result_callback_exception(mock_civis):
     # An error in the result retrieval should be raised by .get
     callback = mock.MagicMock()
     exc = ZeroDivisionError()
     mock_civis.io.civis_to_file.side_effect = exc
-    fut = ContainerFuture(1, 2, client=mock.MagicMock())
-
     # We're simulating a job which succeeded but generated an
     # exception when we try to download the outputs.
-    fut._set_api_exception(Response({'state': 'succeeded'}))
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="succeeded", run_outputs=mock.MagicMock()
+    )
+    fut = ContainerFuture(1, 2, client=mock_client)
+
     res = civis.parallel._CivisBackendResult(fut, callback)
 
     with pytest.raises(ZeroDivisionError):
         res.get()
     assert callback.call_count == 0
 
 
-@mock.patch.object(civis.parallel, 'civis')
-def test_result_eventual_success(mock_civis):
+@mock.patch.object(civis.parallel, "civis")
+@mock.patch("civis.futures.time.sleep", side_effect=lambda x: None)
+def test_result_eventual_success(m_sleep, mock_civis):
     # Test that we can get a result back from a succeeded job,
     # even if we need to retry a few times to succeed with the download.
     callback = mock.MagicMock()
     exc = requests.ConnectionError()
-    se = make_to_file_mock('spam', max_n_err=2, exc=exc)
+    se = make_to_file_mock("spam", max_n_err=2, exc=exc)
     mock_civis.io.civis_to_file.side_effect = se
-    fut = ContainerFuture(1, 2, client=mock.MagicMock())
-    fut.set_result(Response({'state': 'success'}))
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="success", run_outputs=mock.MagicMock()
+    )
+    fut = ContainerFuture(1, 2, client=mock_client)
     res = civis.parallel._CivisBackendResult(fut, callback)
 
-    assert res.get() == 'spam'
+    assert res.get() == "spam"
     assert callback.call_count == 1
 
 
-@mock.patch.object(civis.parallel, 'civis')
-def test_result_eventual_failure(mock_civis):
+@mock.patch.object(civis.parallel, "civis")
+@mock.patch("civis.futures.time.sleep", side_effect=lambda x: None)
+def test_result_eventual_failure(m_sleep, mock_civis):
     # We will retry a connection error up to 5 times. Make sure
     # that we will get an error if it persists forever.
     callback = mock.MagicMock()
     exc = requests.ConnectionError()
-    se = make_to_file_mock('spam', max_n_err=10, exc=exc)
+    se = make_to_file_mock("spam", max_n_err=10, exc=exc)
     mock_civis.io.civis_to_file.side_effect = se
-    fut = ContainerFuture(1, 2, client=mock.MagicMock())
-    fut.set_result(Response({'state': 'success'}))
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="success", run_outputs=mock.MagicMock()
+    )
+    fut = ContainerFuture(1, 2, client=mock_client)
     res = civis.parallel._CivisBackendResult(fut, callback)
-
     with pytest.raises(requests.ConnectionError):
         res.get()
     assert callback.call_count == 0
 
 
-@mock.patch.object(civis.parallel, 'civis')
-@mock.patch.object(civis.parallel, '_sklearn_reg_para_backend')
-@mock.patch.object(civis.parallel, '_joblib_reg_para_backend')
+@mock.patch.object(civis.parallel, "civis")
+def test_result_running_and_cancel_requested(mock_civis):
+    # When scripts request cancellation, they remain in a running
+    # state. Make sure these are treated as cancelled runs.
+    response = Response({"is_cancel_requested": True, "state": "running"})
+    mock_client = create_client_mock_for_container_tests(
+        1, 2, state="running", run_outputs=mock.MagicMock()
+    )
+    mock_client.scripts.post_cancel.return_value = response
+    fut = ContainerFuture(1, 2, client=mock_client)
+    callback = mock.MagicMock()
+    # When a _CivisBackendResult created by the Civis joblib backend completes
+    # successfully, a callback is executed. When cancelled, this callback
+    # shouldn't  be run
+    civis.parallel._CivisBackendResult(fut, callback)
+    fut.cancel()
+
+    assert callback.call_count == 0
+
+
+@mock.patch.object(civis.parallel, "civis")
+@mock.patch.object(civis.parallel, "_sklearn_reg_para_backend")
+@mock.patch.object(civis.parallel, "_joblib_reg_para_backend")
 def test_setup_remote_backend(mock_jl, mock_sk, mock_civis):
     # Test that the civis backend is properly registered w/ joblib and sklearn.
     for no_sk in [True, False]:
-        with mock.patch.object(civis.parallel, 'NO_SKLEARN', no_sk):
+        with mock.patch.object(civis.parallel, "NO_SKLEARN", no_sk):
             backend = civis.parallel._CivisBackend()
             backend_name = civis.parallel._setup_remote_backend(backend)
-            assert backend_name == 'civis'
+            assert backend_name == "civis"
             assert mock_jl.call_count == 1
             if no_sk:
                 assert mock_sk.call_count == 0
             else:
                 assert mock_sk.call_count == 1
             mock_jl.reset_mock()
             mock_sk.reset_mock()
 
 
 def test_civis_backend_from_existing():
     # Test to make sure that making a new backend from an existing one makes
     # an exact copy.
     backend = civis.parallel._CivisBackend(
-        setup_cmd='blah',
+        setup_cmd="blah",
         from_template_id=-1,
         max_submit_retries=10,
-        client='ha',
-        remote_backend='cool',
-        hidden=False)
+        client="ha",
+        remote_backend="cool",
+        hidden=False,
+    )
 
     new_backend = civis.parallel._CivisBackend.from_existing(backend)
 
-    assert new_backend.setup_cmd == 'blah'
+    assert new_backend.setup_cmd == "blah"
     assert new_backend.from_template_id == -1
     assert new_backend.max_submit_retries == 10
-    assert new_backend.client == 'ha'
-    assert new_backend.remote_backend == 'cool'
-    assert new_backend.executor_kwargs == {'hidden': False}
+    assert new_backend.client == "ha"
+    assert new_backend.remote_backend == "cool"
+    assert new_backend.executor_kwargs == {"hidden": False}
 
 
-@mock.patch.object(civis.parallel, 'civis')
+@mock.patch.object(civis.parallel, "civis")
 def test_civis_backend_pickles(mock_civis):
     # Test to make sure the backend will pickle.
     backend = civis.parallel._CivisBackend(
-        setup_cmd='blah',
+        setup_cmd="blah",
         from_template_id=-1,
         max_submit_retries=10,
-        client='ha',
-        remote_backend='cool',
-        hidden=False)
+        client="ha",
+        remote_backend="cool",
+        hidden=False,
+    )
 
     with parallel_backend(backend):
         Parallel(n_jobs=-1)([])
 
     buff = io.BytesIO()
     pickle.dump(backend, buff)
     buff.seek(0)
```

### Comparing `civis-1.9.4/civis/tests/test_deprecate.py` & `civis-2.0.0/tests/test_deprecate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,111 @@
+import warnings
+
 from civis import _deprecation
 
 import pytest
 
 
 def adder(param1, param2=0, param3=0):
     return param1 + param2 + param3
 
 
 def test_deprecate_kwarg():
     # Verify that we get a warning if the deprecated parameter is
     # used as a keyword argument.
-    decorated_func = _deprecation.deprecate_param('v2.0.0', 'param2')(adder)
+    decorated_func = _deprecation.deprecate_param("v2.0.0", "param2")(adder)
+
+    with pytest.warns(FutureWarning) as record:
+        output = decorated_func(1, param2=3, param3=5)
+
+    assert output == 9, "The function should still give the expected output."
+    assert len(record) == 1, "Only one warning should be raised."
+    assert (
+        "v2.0.0" in record[0].message.args[0]
+    ), "The warning should mention the removal version."
+    assert (
+        "param2" in record[0].message.args[0]
+    ), "The warning should mention the deprecated parameter."
+    assert (
+        __name__ + ".adder" in record[0].message.args[0]
+    ), "The warning should mention the function name."
+
+
+def test_deprecate_multiple_kwarg():
+    # Verify that we get a warning if the deprecated parameter is
+    # used as a keyword argument.
+    decorated_func = _deprecation.deprecate_param("v2.0.0", "param2", "param3")(adder)
 
     with pytest.warns(FutureWarning) as record:
         output = decorated_func(1, param2=3, param3=5)
 
     assert output == 9, "The function should still give the expected output."
     assert len(record) == 1, "Only one warning should be raised."
-    assert "v2.0.0" in record[0].message.args[0], \
-        "The warning should mention the removal version."
-    assert "param2" in record[0].message.args[0], \
-        "The warning should mention the deprecated parameter."
-    assert __name__ + ".adder" in record[0].message.args[0], \
-        "The warning should mention the function name."
+    assert (
+        "v2.0.0" in record[0].message.args[0]
+    ), "The warning should mention the removal version."
+    assert (
+        "param2" in record[0].message.args[0]
+    ), "The warning should mention the first deprecated parameter."
+    assert (
+        "param3" in record[0].message.args[0]
+    ), "The warning should mention the second deprecated parameter."
+    assert (
+        __name__ + ".adder" in record[0].message.args[0]
+    ), "The warning should mention the function name."
 
 
 def test_deprecate_pos_arg():
     # Verify that we get a warning if the deprecated parameter is
     # used as a positional argument.
-    decorated_func = _deprecation.deprecate_param('v2.0.0', 'param2')(adder)
+    decorated_func = _deprecation.deprecate_param("v2.0.0", "param2")(adder)
+
+    with pytest.warns(FutureWarning) as record:
+        output = decorated_func(1, 3, 5)
+
+    assert output == 9, "The function should still give the expected output."
+    assert len(record) == 1, "Only one warning should be raised."
+    assert (
+        "v2.0.0" in record[0].message.args[0]
+    ), "The warning should mention the removal version."
+    assert (
+        "param2" in record[0].message.args[0]
+    ), "The warning should mention the deprecated parameter."
+    assert (
+        __name__ + ".adder" in record[0].message.args[0]
+    ), "The warning should mention the function name."
+
+
+def test_deprecate_multiple_pos_arg():
+    # Verify that we get a warning if the deprecated parameter is
+    # used as a positional argument.
+    decorated_func = _deprecation.deprecate_param("v2.0.0", "param2", "param3")(adder)
 
     with pytest.warns(FutureWarning) as record:
         output = decorated_func(1, 3, 5)
 
     assert output == 9, "The function should still give the expected output."
     assert len(record) == 1, "Only one warning should be raised."
-    assert "v2.0.0" in record[0].message.args[0], \
-        "The warning should mention the removal version."
-    assert "param2" in record[0].message.args[0], \
-        "The warning should mention the deprecated parameter."
-    assert __name__ + ".adder" in record[0].message.args[0], \
-        "The warning should mention the function name."
+    assert (
+        "v2.0.0" in record[0].message.args[0]
+    ), "The warning should mention the removal version."
+    assert (
+        "param2" in record[0].message.args[0]
+    ), "The warning should mention the first deprecated parameter."
+    assert (
+        "param3" in record[0].message.args[0]
+    ), "The warning should mention the second deprecated parameter."
+    assert (
+        __name__ + ".adder" in record[0].message.args[0]
+    ), "The warning should mention the function name."
 
 
 def test_deprecate_no_warning():
     # Verify that we don't see a warning if we don't use the
     # deprecated parameter.
-    decorated_func = _deprecation.deprecate_param('v2.0.0', 'param2')(adder)
+    decorated_func = _deprecation.deprecate_param("v2.0.0", "param2")(adder)
 
-    with pytest.warns(None) as record:
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
         output = decorated_func(1, param3=5)
 
     assert output == 6, "The function should still give the expected output."
-    assert len(record) == 0, "No warnings should be raised."
```

### Comparing `civis-1.9.4/civis/tests/test_polling.py` & `civis-2.0.0/tests/test_polling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,98 +1,104 @@
 """Test the `civis.polling` module"""
+
 import time
 from concurrent import futures
 import unittest
+from unittest import mock
 
-from civis.compat import mock
 from civis.response import Response
-from civis.polling import PollableResult
+from civis.polling import PollableResult, _ResultPollingThread
 
 import pytest
 
 
 class State:
     def __init__(self, state):
         self.state = state
 
 
 def create_pollable_result(state, exception=None, result=None):
-    f = PollableResult(State, (state, ), polling_interval=0.001)
+    f = PollableResult(State, (state,), polling_interval=0.001)
     f._exception = exception
     f._result = result
     return f
 
 
-CANCELLED_RESULT = create_pollable_result(state='cancelled')
-FINISHED_RESULT = create_pollable_result(state='success')
-QUEUED_RESULT = create_pollable_result(state='queued')
+CANCELLED_RESULT = create_pollable_result(state="cancelled")
+FINISHED_RESULT = create_pollable_result(state="success")
+QUEUED_RESULT = create_pollable_result(state="queued")
 
 
 class TestPolling(unittest.TestCase):
     def test_as_completed(self):
         my_futures = [QUEUED_RESULT, CANCELLED_RESULT, FINISHED_RESULT]
         fs = futures.as_completed(my_futures)
         f1 = next(fs)
         f2 = next(fs)
         finished_futures = set([f1, f2])
 
-        self.assertEqual(finished_futures,
-                         set([FINISHED_RESULT, CANCELLED_RESULT]))
+        self.assertEqual(finished_futures, set([FINISHED_RESULT, CANCELLED_RESULT]))
 
     def test_wait(self):
-        done, not_done = futures.wait([QUEUED_RESULT, FINISHED_RESULT],
-                                      return_when=futures.FIRST_COMPLETED)
+        done, not_done = futures.wait(
+            [QUEUED_RESULT, FINISHED_RESULT], return_when=futures.FIRST_COMPLETED
+        )
         self.assertEqual(set([FINISHED_RESULT]), done)
         self.assertEqual(set([QUEUED_RESULT]), not_done)
 
     def test_error_passthrough(self):
-        pollable = PollableResult(mock.Mock(side_effect=[ZeroDivisionError()]),
-                                  (),
-                                  polling_interval=0.1)
+        pollable = PollableResult(
+            mock.Mock(side_effect=[ZeroDivisionError()]), (), polling_interval=0.1
+        )
         pytest.raises(ZeroDivisionError, pollable.result)
 
     def test_error_setting(self):
-        pollable = PollableResult(mock.Mock(side_effect=[ZeroDivisionError()]),
-                                  (),
-                                  polling_interval=0.1)
+        pollable = PollableResult(
+            mock.Mock(side_effect=[ZeroDivisionError()]), (), polling_interval=0.1
+        )
         assert isinstance(pollable.exception(), ZeroDivisionError)
 
     def test_timeout(self):
         pollable = PollableResult(
             mock.Mock(return_value=Response({"state": "running"})),
             poller_args=(),
-            polling_interval=0.1)
+            polling_interval=0.1,
+        )
         pytest.raises(futures.TimeoutError, pollable.result, timeout=0.05)
 
     def test_poll_on_creation(self):
         poller = mock.Mock(return_value=Response({"state": "running"}))
-        pollable = PollableResult(poller,
-                                  (),
-                                  polling_interval=0.01,
-                                  poll_on_creation=False)
+        pollable = PollableResult(
+            poller, (), polling_interval=0.01, poll_on_creation=False
+        )
         pollable.done()  # Check status once to start the polling thread
         assert poller.call_count == 0
-        time.sleep(0.02)
+        time.sleep(0.05)
         assert poller.call_count > 0
 
+    def test_poller_returns_none(self):
+        poller = mock.Mock(side_effect=[None, None, Response({"state": "success"})])
+        polling_thread = _ResultPollingThread(poller, (), polling_interval=0.01)
+        polling_thread.run()
+        assert poller.call_count == 3
+
     def test_reset_polling_thread(self):
         pollable = PollableResult(
             mock.Mock(return_value=Response({"state": "running"})),
             poller_args=(),
-            polling_interval=0.1
+            polling_interval=0.1,
         )
         initial_polling_thread = pollable._polling_thread
         assert pollable.polling_interval == 0.1
         assert pollable._polling_thread.polling_interval == 0.1
         pollable._reset_polling_thread(0.2)
         # Check that the polling interval was updated
         assert pollable.polling_interval == 0.2
         assert pollable._polling_thread.polling_interval == 0.2
         # Check that the _polling_thread is a new thread
         assert pollable._polling_thread != initial_polling_thread
         # Check that the old thread was stopped
-        time.sleep(0.001)  # Needs extra time to shut down in Python 2.7
         assert not initial_polling_thread.is_alive()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `civis-1.9.4/civis/response.py` & `civis-2.0.0/src/civis/response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-from __future__ import absolute_import
 import requests
 
 from civis._utils import camel_to_snake
 
 
+_RETURN_TYPES = frozenset({"snake", "raw"})
+
+
 class CivisClientError(Exception):
     def __init__(self, message, response):
         self.status_code = response.status_code
         self.error_message = message
 
     def __str__(self):
         return self.error_message
 
 
+class CivisImmutableResponseError(Exception):
+    pass
+
+
 def _response_to_json(response):
     """Parse a raw response to a dict.
 
     Parameters
     ----------
     response: requests.Response
         A raw response returned by an API call.
@@ -28,116 +34,169 @@
         content.
 
     Raises
     ------
     CivisClientError
         If the data in the raw response cannot be parsed.
     """
-    if response.content == b'':
+    if response.content == b"":
         return None
     else:
         try:
             return response.json()
         except ValueError:
-            raise CivisClientError("Unable to parse JSON from response",
-                                   response)
+            raise CivisClientError("Unable to parse JSON from response", response)
 
 
-def convert_response_data_type(response, headers=None, return_type='snake'):
+def convert_response_data_type(response, headers=None, return_type="snake"):
     """Convert a raw response into a given type.
 
     Parameters
     ----------
     response : list, dict, or `requests.Response`
         Convert this object into a different response object.
     headers : dict, optional
         If given and the return type supports it, attach these headers to the
         converted response. If `response` is a `requests.Response`, the headers
         will be inferred from it.
-    return_type : string, {'snake', 'raw', 'pandas'}
+    return_type : string, {'snake', 'raw'}
         Convert the response to this type. See documentation on
         `civis.APIClient` for details of the return types.
 
     Returns
     -------
-    list, dict, `civis.response.Response`, `requests.Response`,
-    `pandas.DataFrame`, or `pandas.Series`
+    list, dict, `civis.response.Response`, or `requests.Response`
         Depending on the value of `return_type`.
     """
-    assert return_type in ['snake', 'raw', 'pandas'], 'Invalid return type'
-
-    if return_type == 'raw':
+    if return_type == "raw":
         return response
 
-    if isinstance(response, requests.Response):
-        headers = response.headers
-        data = _response_to_json(response)
-    else:
-        data = response
+    elif return_type == "snake":
+        if isinstance(response, requests.Response):
+            headers = response.headers
+            data = _response_to_json(response)
+        else:
+            data = response
 
-    if return_type == 'pandas':
-        import pandas as pd
         if isinstance(data, list):
-            return pd.DataFrame.from_records(data)
+            return [Response(d, headers=headers) for d in data]
+        else:
+            return Response(data, headers=headers)
 
-        # there may be nested objects or arrays in this series
-        return pd.Series(data)
+    else:
+        raise ValueError(f"Return type not one of {set(_RETURN_TYPES)}: {return_type}")
 
-    elif return_type == 'snake':
-        if isinstance(data, list):
-            return [Response(d, headers=headers) for d in data]
 
-        return Response(data, headers=headers)
+def _raise_response_immutable_error():
+    raise CivisImmutableResponseError("Response object is not mutable")
 
 
-class Response(dict):
+class Response:
     """Custom Civis response object.
 
     Attributes
     ----------
     json_data : dict | None
         This is `json_data` as it is originally returned to the user without
         the key names being changed. See Notes. None is used if the original
         response returned a 204 No Content response.
     headers : dict
         This is the header for the API call without changing the key names.
     calls_remaining : int
         Number of API calls remaining before rate limit is reached.
     rate_limit : int
         Total number of calls per API rate limit period.
-
-    Notes
-    -----
-    The main features of this class are that it maps camelCase to snake_case
-    at the top level of the json object and attaches keys as attributes.
-    Nested object keys are not changed.
     """
-    def __init__(self, json_data, snake_case=True, headers=None):
+
+    def __init__(self, json_data, *, headers=None):
         self.json_data = json_data
-        if headers is not None:
-            # this circumvents recursive calls
-            self.headers = headers
-            self.calls_remaining = headers.get('X-RateLimit-Remaining')
-            self.rate_limit = headers.get('X-RateLimit-Limit')
+        self.headers = headers
+        self.calls_remaining = (
+            int(x) if (x := (headers or {}).get("X-RateLimit-Remaining")) else x
+        )
+        self.rate_limit = (
+            int(x) if (x := (headers or {}).get("X-RateLimit-Limit")) else x
+        )
+
+        self._data_camel = {}
+        self._data_snake = {}
 
         if json_data is not None:
             for key, v in json_data.items():
-                if snake_case:
-                    key = camel_to_snake(key)
 
                 if isinstance(v, dict):
-                    val = Response(v, False)
+                    val = Response(v)
                 elif isinstance(v, list):
-                    val = [Response(o) if isinstance(o, dict) else o
-                           for o in v]
+                    val = [Response(o) if isinstance(o, dict) else o for o in v]
                 else:
                     val = v
 
-                self.update({key: val})
-                self.__dict__.update({key: val})
+                self._data_camel[key] = val
+                self._data_snake[camel_to_snake(key)] = val
+
+    def __setattr__(self, key, value):
+        if key == "__dict__":
+            self.__dict__.update(value)
+        elif key in (
+            "json_data",
+            "headers",
+            "calls_remaining",
+            "rate_limit",
+            "_data_camel",
+            "_data_snake",
+        ):
+            self.__dict__[key] = value
+        else:
+            _raise_response_immutable_error()
+
+    def __setitem__(self, key, value):
+        _raise_response_immutable_error()
+
+    def __getitem__(self, item):
+        try:
+            return self._data_snake[item]
+        except KeyError:
+            return self._data_camel[item]
+
+    def __getattr__(self, item):
+        try:
+            return self.__getitem__(item)
+        except KeyError as e:
+            raise AttributeError(f"Response object has no attribute {str(e)}")
+
+    def __len__(self):
+        return len(self._data_snake)
+
+    def __repr__(self):
+        return repr(self._data_snake)
+
+    def get(self, key, default=None):
+        try:
+            return self.__getitem__(key)
+        except KeyError:
+            return default
+
+    def items(self):
+        return self._data_snake.items()
+
+    def __eq__(self, other):
+        if isinstance(other, dict):
+            return self._data_snake == other
+        elif isinstance(other, Response):
+            return self._data_snake == other._data_snake
+        else:
+            raise TypeError(f"Response and {type(other)} can't be compared")
+
+    def __setstate__(self, state):
+        """Set the state when unpickling, to avoid RecursionError."""
+        self.__dict__ = state
+
+    def _replace(self, key, value):
+        """Only used within this repo; `key` assumed to be in snake_case."""
+        self._data_snake[key] = value
 
 
 class PaginatedResponse:
     """A response object which is an iterator
 
     Parameters
     ----------
@@ -153,52 +212,137 @@
     Notes
     -----
     This response is returned automatically by endpoints which support
     pagination when the `iterator` kwarg is specified.
 
     Examples
     --------
+    >>> import civis
     >>> client = civis.APIClient()
     >>> queries = client.queries.list(iterator=True)
     >>> for query in queries:
     ...    print(query['id'])
     """
+
     def __init__(self, path, initial_params, endpoint):
         self._path = path
         self._params = initial_params.copy()
         self._endpoint = endpoint
 
         # We are paginating through all items, so start at the beginning and
         # let the API determine the limit.
-        self._params['page_num'] = 1
-        self._params.pop('limit', None)
+        self._params["page_num"] = 1
+        self._params.pop("limit", None)
 
         self._iter = None
 
     def __iter__(self):
         return self
 
     def _get_iter(self):
         while True:
-            response = self._endpoint._make_request('GET',
-                                                    self._path,
-                                                    self._params)
+            response = self._endpoint._make_request("GET", self._path, self._params)
             page_data = _response_to_json(response)
             if len(page_data) == 0:
                 return
 
             for data in page_data:
                 converted_data = convert_response_data_type(
                     data,
                     headers=response.headers,
-                    return_type=self._endpoint._return_type
+                    return_type=self._endpoint._return_type,
                 )
                 yield converted_data
 
-            self._params['page_num'] += 1
+            self._params["page_num"] += 1
 
     def __next__(self):
         if self._iter is None:
             self._iter = self._get_iter()
         return next(self._iter)
 
-    next = __next__  # Python 2 compatibility
+
+def find(object_list, filter_func=None, **kwargs):
+    """Filter :class:`civis.response.Response` objects.
+
+    Parameters
+    ----------
+    object_list : iterable
+        An iterable of arbitrary objects, particularly those with attributes
+        that can be targeted by the filters in `kwargs`. A major use case is
+        an iterable of :class:`civis.response.Response` objects.
+    filter_func : callable, optional
+        A one-argument function. If specified, `kwargs` are ignored.
+        An `object` from the input iterable is kept in the returned list
+        if and only if ``bool(filter_func(object))`` is ``True``.
+    **kwargs
+        Key-value pairs for more fine-grained filtering; they cannot be used
+        in conjunction with ``filter_func``. All keys must be strings.
+        For an object ``obj`` from the input iterable to be included in the
+        returned list, all the keys must be attributes of ``obj``, plus
+        any one of the following conditions for a given key:
+
+        - ``value`` is a one-argument function and
+          ``bool(value(getattr(obj, key)))`` is equal to ``True``
+        - ``value`` is either ``True`` or ``False``, and
+          ``getattr(obj, key) is value`` is ``True``
+        - ``getattr(obj, key) == value`` is ``True``
+
+    Returns
+    -------
+    list
+
+    Examples
+    --------
+    >>> import civis
+    >>> client = civis.APIClient()
+    >>> # creds is a list of civis.response.Response objects
+    >>> creds = client.credentials.list()
+    >>> # target_creds contains civis.response.Response objects
+    >>> # with the attribute 'name' == 'username'
+    >>> target_creds = find(creds, name='username')
+
+    See Also
+    --------
+    civis.find_one
+    """
+    _func = filter_func
+    if not filter_func:
+
+        def default_filter(o):
+            for k, v in kwargs.items():
+                if not hasattr(o, k):
+                    return False
+                elif callable(v):
+                    if not v(getattr(o, k, None)):
+                        return False
+                elif isinstance(v, bool):
+                    if getattr(o, k) is not v:
+                        return False
+                elif v != getattr(o, k, None):
+                    return False
+            return True
+
+        _func = default_filter
+
+    return [o for o in object_list if _func(o)]
+
+
+def find_one(object_list, filter_func=None, **kwargs):
+    """Return one satisfying :class:`civis.response.Response` object.
+
+    The arguments are the same as those for :func:`civis.find`.
+    If more than one object satisfies the filtering criteria,
+    the first one is returned.
+    If no satisfying objects are found, ``None`` is returned.
+
+    Returns
+    -------
+    object or None
+
+    See Also
+    --------
+    civis.find
+    """
+    results = find(object_list, filter_func, **kwargs)
+
+    return results[0] if results else None
```

### Comparing `civis-1.9.4/civis/cli/__main__.py` & `civis-2.0.0/src/civis/cli/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,60 +3,69 @@
 """
 Civis Command Line Interface
 
 This is based on https://github.com/zalando/openapi-cli-client,
 which has an Apache 2.0 License:
 https://github.com/zalando/openapi-cli-client/blob/master/LICENSE
 """
-from __future__ import print_function
-
 
 import calendar
 from collections import OrderedDict
 from functools import partial
 import json
+import logging
 import os
 import re
 import sys
 import time
 from warnings import warn
 
 import click
 from jsonref import JsonRef
 import yaml
+from requests import Request
 from civis.cli._cli_commands import (
-    civis_ascii_art, files_download_cmd, files_upload_cmd,
-    notebooks_download_cmd, notebooks_new_cmd,
-    notebooks_up, notebooks_down, notebooks_open)
+    civis_ascii_art,
+    files_download_cmd,
+    files_upload_cmd,
+    jobs_follow_log,
+    jobs_follow_run_log,
+    notebooks_download_cmd,
+    notebooks_new_cmd,
+    notebooks_up,
+    notebooks_down,
+    notebooks_open,
+    sql_cmd,
+)
+from civis.base import open_session
 from civis.resources import get_api_spec, CACHED_SPEC_PATH
-from civis._utils import open_session
-from civis.compat import FileNotFoundError
+from civis.resources._resources import parse_method_name
+from civis._utils import retry_request, MAX_RETRIES
 
 
-_REPLACEABLE_COMMAND_CHARS = re.compile(r'[^A-Za-z0-9]+')
-_API_URL = "https://api.civisanalytics.com"
-_OPENAPI_SPEC_URL = "https://api.civisanalytics.com/endpoints"
-CLI_USER_AGENT = 'civis-cli'
+_REPLACEABLE_COMMAND_CHARS = re.compile(r"[^A-Za-z0-9]+")
+_BASE_API_URL = "https://api.civisanalytics.com"
+CLI_USER_AGENT = "civis-cli"
 
 
 class YAMLParamType(click.ParamType):
     """
     A click parameter type for YAML/JSON files.
     See http://click.pocoo.org/5/parameters/#implementing-custom-types.
     """
 
-    name = 'yamlpath'
+    name = "yamlpath"
 
     def convert(self, value, param, ctx):
         if value is None:
             return value
 
         try:
             with open(value) as f:
-                result = yaml.load(f)
+                result = yaml.safe_load(f)
                 return result
         except Exception:
             self.fail("Could not load YAML from path: %s" % value, param, ctx)
 
 
 YAML = YAMLParamType()
 
@@ -65,61 +74,56 @@
 # See https://github.com/OAI/OpenAPI-Specification/blob/master/versions/2.0.md#data-types.  # noqa: E501
 _TYPE_MAP = {
     "integer": int,
     "number": float,
     "boolean": bool,
     "string": str,
     "object": YAML,
-    "array": YAML
+    "array": YAML,
 }
 
 
 def get_api_key():
     try:
         return os.environ["CIVIS_API_KEY"]
     except KeyError:
-        print("You must set the CIVIS_API_KEY environment variable.",
-              file=sys.stderr)
+        print("You must set the CIVIS_API_KEY environment variable.", file=sys.stderr)
         sys.exit(1)
 
 
+def get_base_api_url():
+    return os.getenv("CIVIS_API_ENDPOINT") or _BASE_API_URL
+
+
 def camel_to_snake(s):
-    return re.sub(r'([A-Z]+)', r'_\1', s).lower()
+    return re.sub(r"([A-Z]+)", r"_\1", s).lower()
 
 
 def munge_name(s):
     """Replace non-alphanumeric characters with dashes."""
-    result = _REPLACEABLE_COMMAND_CHARS.sub('-', s.lower()).strip('-')
+    result = _REPLACEABLE_COMMAND_CHARS.sub("-", s.lower()).strip("-")
     return result
 
 
 def make_operation_name(path, method, resource_name):
     """Create an appropriate CLI command for an operation.
 
-    E.g., '/imports/files/{id}/runs/{run_id}' -> 'get_imports_files_runs'
+    Examples
+    --------
+    >>> make_operation_name('/scripts/r/{id}/runs/{run_id}', 'get', 'scripts')
+    get-r-runs
     """
-
-    name = path.lower()
-    name = re.sub(r'{[^}]+}', '', name)
-    name = munge_name(name)
+    path = path.lower().lstrip("/")
 
     # Remove resource prefix. Note that the path name for some operations is
     # just the resource name (e.g., /databases).
-    # Munge the resource name for consistency (e.g.,
-    # remote_hosts -> remote-hosts).
-    if name.startswith(munge_name(resource_name)):
-        name = name[len(resource_name):].strip("-")
-
-    # If there's no ID argument at the end, then it'll be a listing operation.
-    if method == 'get' and not path.endswith('}'):
-        method = 'list'
-
-    # Add HTTP method prefix. For operations whose path name is the resource,
-    # make the command just be the HTTP method.
-    name = '{}-{}'.format(method, name) if name else method
+    if path.startswith(resource_name):
+        path = path[len(resource_name) :].strip("-")
+
+    name = parse_method_name(method, path).replace("_", "-")
     return name
 
 
 def param_case_map(param_names):
     # Return a map from snake_case parameter names (for click) to camelCase
     # versions for the API. We need this mapping because the API
     # expects/prefers camelCase but click prefers snake_case.
@@ -132,67 +136,73 @@
 
 def invoke(method, path, op, *args, **kwargs):
     """
     If json_output is in `kwargs` then the output is json. Otherwise, it is
     yaml.
     """
     # Remove None b/c click passes everything in as None if it's not set.
-    kwargs = {k: v for k, v in kwargs.items()
-              if v is not None}
-    json_output = kwargs.pop('json_output', False)
+    kwargs = {k: v for k, v in kwargs.items() if v is not None}
+    json_output = kwargs.pop("json_output", False)
 
     # Construct the body of the request.
     body = {}
-    body_params = [p for p in op['parameters'] if p['in'] == 'body']
+    body_params = [p for p in op["parameters"] if p["in"] == "body"]
     if body_params:
-        assert len(body_params) == 1  # There can be only one body parameter.
-        props = body_params[0]['schema']['properties']
+        if len(body_params) != 1:
+            raise ValueError(
+                "There can be only one body parameter, "
+                f"but {len(body_params)} are found: {body_params}"
+            )
+        props = body_params[0]["schema"]["properties"]
         param_map = param_case_map(props.keys())
-        body = {param_map[k]: v for k, v in kwargs.items()
-                if k in param_map}
+        body = {param_map[k]: v for k, v in kwargs.items() if k in param_map}
 
     # Construct the query part of the request.
-    query_names = {p['name'] for p in op['parameters'] if p['in'] == 'query'}
+    query_names = {p["name"] for p in op["parameters"] if p["in"] == "query"}
     param_map = param_case_map(query_names)
-    query = {param_map[k]: v for k, v in kwargs.items()
-             if k in param_map}
+    query = {param_map[k]: v for k, v in kwargs.items() if k in param_map}
 
     # Make the request.
     request_info = dict(
         params=query,
         json=body,
-        url=_API_URL + path.format(**kwargs),
-        method=method
+        url=get_base_api_url() + path.format(**kwargs),
+        method=method,
     )
     with open_session(get_api_key(), user_agent=CLI_USER_AGENT) as sess:
-        response = sess.request(**request_info)
+        request = Request(**request_info)
+        pre_request = sess.prepare_request(request)
+        response = retry_request(method, pre_request, sess, MAX_RETRIES)
 
-    # Print the response to stderr if there was an error.
+    # Print the response to stderr and set exit code to 1 if there was an error
     output_file = sys.stdout
-    if response.status_code != 200:
+    exit_code = 0
+    if not (200 <= response.status_code < 300):
         output_file = sys.stderr
+        exit_code = 1
 
     # Print the output, if there is any.
     # For commands such as DELETE /scripts/containers/{script_id}/runs/{id},
     # response ends up being " " here.
     try:
         if json_output:
             json.dump(response.json(), output_file)
         else:
-            yaml.safe_dump(response.json(), output_file,
-                           default_flow_style=False)
+            yaml.safe_dump(response.json(), output_file, default_flow_style=False)
         output_file.flush()
 
     # json throws a ValueError if it is passed a blank string to load.
     except ValueError as e:
         # If the message was not blank, print an error message.
         # Otherwise, do nothing.
         if response.text.strip():
             print("Error parsing response: {}".format(e), file=sys.stderr)
 
+    sys.exit(exit_code)
+
 
 def retrieve_spec_dict(api_version="1.0"):
     """Retrieve the API specification from a cached version or from Civis."""
 
     refresh_spec = True
     now_timestamp = calendar.timegm(time.gmtime())
 
@@ -205,53 +215,65 @@
                 spec_dict = json.load(f, object_pairs_hook=OrderedDict)
     except (FileNotFoundError, ValueError):
         # If the file doesn't exist or we can't parse it, just keep going.
         refresh_spec = True
 
     # Download the spec and cache it in the user's home directory.
     if refresh_spec:
-        spec_dict = get_api_spec(get_api_key(), api_version=api_version,
-                                 user_agent=CLI_USER_AGENT)
+        spec_dict = get_api_spec(
+            get_api_key(), api_version=api_version, user_agent=CLI_USER_AGENT
+        )
         with open(CACHED_SPEC_PATH, "w") as f:
             json.dump(spec_dict, f)
     return spec_dict
 
 
 def add_extra_commands(cli):
     """Add useful commands that are not in the OpenAPI spec."""
-    files_cmd = cli.commands['files']
+    files_cmd = cli.commands["files"]
     files_cmd.add_command(files_download_cmd)
     files_cmd.add_command(files_upload_cmd)
-    notebooks_cmd = cli.commands['notebooks']
+    notebooks_cmd = cli.commands["notebooks"]
     notebooks_cmd.add_command(notebooks_download_cmd)
     notebooks_cmd.add_command(notebooks_new_cmd)
     notebooks_cmd.add_command(notebooks_up)
     notebooks_cmd.add_command(notebooks_down)
     notebooks_cmd.add_command(notebooks_open)
+    jobs_cmd = cli.commands["jobs"]
+    jobs_cmd.add_command(jobs_follow_log)
+    jobs_cmd.add_command(jobs_follow_run_log)
     cli.add_command(civis_ascii_art)
 
+    cli.add_command(sql_cmd)
 
-def generate_cli():
 
+def configure_log_level():
+    if os.getenv("CIVIS_LOG_LEVEL"):
+        logging.basicConfig(level=os.getenv("CIVIS_LOG_LEVEL"))
+
+
+def generate_cli():
+    configure_log_level()
     spec = retrieve_spec_dict()
 
     # Replace references in the spec so that we don't have to worry about them
     # when making the CLI.
     spec = JsonRef.replace_refs(spec)
 
     cli = click.Group()
 
     # Iterate through top-level resources (e.g., Scripts, Files, Models).
     groups = {}
-    for path, path_dict in spec['paths'].items():
-        resource = path.strip('/').split('/')[0]
+    for path, path_dict in spec["paths"].items():
+        resource = path.strip("/").split("/")[0]
         grp = groups.get(resource)
         if grp is None:
-            grp = click.Group(munge_name(resource),
-                              short_help='Manage {}'.format(resource))
+            grp = click.Group(
+                munge_name(resource), short_help="Manage {}".format(resource)
+            )
             cli.add_command(grp)
             groups[resource] = grp
 
         add_path_commands(path, path_dict, grp, resource)
 
     add_extra_commands(cli)
 
@@ -261,85 +283,87 @@
 def add_path_commands(path, path_dict, grp, resource):
     """Add commands for the given resource."""
 
     for method, op_dict in path_dict.items():
 
         # Set up a command with the appropriate name and help info.
         name = make_operation_name(path, method, resource)
-        summary = op_dict.get('summary', '')
+        summary = op_dict.get("summary", "")
         op_help = summary
-        description = op_dict.get('description', '')
+        description = op_dict.get("description", "")
         if description:
-            op_help += '\n\n' + description
-        op_help += '\n\n' + path
+            op_help += "\n\n" + description
+        op_help += "\n\n" + path
         callback = partial(invoke, method=method, path=path, op=op_dict)
-        cmd = click.Command(name,
-                            callback=callback,
-                            short_help=summary,
-                            help=op_help)
+        cmd = click.Command(name, callback=callback, short_help=summary, help=op_help)
 
         add_command_params(cmd, op_dict)
 
         # Add an option for JSON output.
-        cmd.params.append(click.Option(['--json-output'], is_flag=True,
-                                       help="output in JSON instead of YAML"))
+        cmd.params.append(
+            click.Option(
+                ["--json-output"], is_flag=True, help="output in JSON instead of YAML"
+            )
+        )
 
         if cmd.name in grp.commands:
-            warn("conflicting command name: %s" % cmd.name)
+            warn('conflicting command name "%s" for path "%s"' % (cmd.name, path))
 
         grp.add_command(cmd)
 
 
 def add_command_params(cmd, op_dict):
     """Add parameters to the click command for an API operation."""
 
     # Extract properties of objects in body to make click params for them.
-    parameters_orig = op_dict.get('parameters', [])
+    parameters_orig = op_dict.get("parameters", [])
     parameters = []
     for p in parameters_orig:
-        if p['in'] == 'body':
+        if p["in"] == "body":
             body_params = []
-            req = p['schema'].get('required', [])
-            for prop_name, prop_info in p['schema']['properties'].items():
+            req = p["schema"].get("required", [])
+            for prop_name, prop_info in p["schema"]["properties"].items():
                 p_new = dict(
                     name=camel_to_snake(prop_name),
-                    type=prop_info['type'],
-                    description=prop_info.get('description', ''),
-                    required=req == 'all' or prop_name in req,
+                    type=prop_info["type"],
+                    description=prop_info.get("description", ""),
+                    required=req == "all" or prop_name in req,
                 )
                 body_params.append(p_new)
 
             # Sort the parameters since they don't have an order as properties.
-            body_params = sorted(body_params, key=lambda x: x['name'])
+            body_params = sorted(body_params, key=lambda x: x["name"])
 
             parameters.extend(body_params)
         else:
             parameters.append(p)
 
     # Specify the parameters for this command.
     for p in parameters:
-        param_type_spec = p.get('type', 'string')
+        param_type_spec = p.get("type", "string")
         param_type = _TYPE_MAP[param_type_spec]
-        description = p.get('description', '')
+        description = p.get("description", "")
 
-        if p['required']:
+        if p["required"]:
             cmd.help += "\n\n{} ({}) - {}".format(
-                p['name'].upper(), param_type_spec, description)
-            arg = click.Argument([p['name'].lower()],
-                                 type=param_type)
+                p["name"].upper(), param_type_spec, description
+            )
+            arg = click.Argument([p["name"].lower()], type=param_type)
             cmd.params.append(arg)
         else:
-            arg = click.Option(['--' + munge_name(p['name'].lower())],
-                               help=description,
-                               type=param_type)
+            arg = click.Option(
+                ["--" + munge_name(p["name"].lower())],
+                help=description,
+                type=param_type,
+            )
             cmd.params.append(arg)
 
 
 def main():
-    # Note: this needs to be its own function so that setup.py can make it an
-    # entry point.
+    # Note: this needs to be its own function
+    # so that pyproject.toml can make it an entry point.
     cli = generate_cli()
     cli()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `civis-1.9.4/civis/futures.py` & `civis-2.0.0/src/civis/futures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,210 +1,222 @@
-from __future__ import absolute_import
-
 from abc import ABCMeta, abstractmethod
-from builtins import super
 from concurrent.futures import Executor
 from concurrent import futures
 import copy
 import datetime
 import logging
 import os
 import time
 import threading
 import warnings
 
-import six
-
 from civis import APIClient
-from civis.base import CivisAPIError, DONE
+from civis.base import CivisAPIError, CivisJobFailure, DONE, _err_msg_with_job_run_ids
 from civis.polling import PollableResult
 
-from pubnub.pubnub import PubNub
-from pubnub.pnconfiguration import PNConfiguration, PNReconnectionPolicy
-from pubnub.enums import PNStatusCategory
-from pubnub.callbacks import SubscribeCallback
 
 log = logging.getLogger(__name__)
 
-# Pubnub connections can recover missed messages upon reconnecting for up to 10
-# minutes from the disconnect. Polling on a 9.5 minute interval is used as a
-# fallback in case the job complete message is missed in an outage.
-_LONG_POLLING_INTERVAL = 9.5 * 60
-
-
-class JobCompleteListener(SubscribeCallback):
-    _disconnect_categories = [
-        PNStatusCategory.PNTimeoutCategory,
-        PNStatusCategory.PNNetworkIssuesCategory,
-        PNStatusCategory.PNUnexpectedDisconnectCategory,
-    ]
-
-    def __init__(self, match_function, callback_function,
-                 disconnect_function=None):
-        self.match_function = match_function
-        self.callback_function = callback_function
-        self.disconnect_function = disconnect_function
-
-    def message(self, pubnub, message):
-        if self.match_function(message.message):
-            self.callback_function()
-
-    def status(self, pubnub, status):
-        if status.category in self._disconnect_categories:
-            if self.disconnect_function:
-                self.disconnect_function()
-
-    def presence(self, pubnub, presence):
-        pass
-
 
 class CivisFuture(PollableResult):
-    """
-    A class for tracking future results.
-
-    This class will attempt to subscribe to a Pubnub channel to listen for
-    job completion events. If you don't have access to Pubnub channels, then
-    it will fallback to polling.
+    """A class for tracking future results.
 
     This is a subclass of :class:`python:concurrent.futures.Future` from the
     Python standard library. See:
     https://docs.python.org/3/library/concurrent.futures.html
 
     Parameters
     ----------
     poller : func
         A function which returns an object that has a ``state`` attribute.
     poller_args : tuple
         The arguments with which to call the poller function.
     polling_interval : int or float, optional
         The number of seconds between API requests to check whether a result
         is ready.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
     poll_on_creation : bool, optional
         If ``True`` (the default), it will poll upon calling ``result()`` the
         first time. If ``False``, it will wait the number of seconds specified
         in `polling_interval` from object creation before polling.
 
     Examples
     --------
     This example is provided as a function at :func:`~civis.io.query_civis`.
 
+    >>> import civis
     >>> client = civis.APIClient()
     >>> database_id = client.get_database_id("my_database")
     >>> cred_id = client.default_credential
     >>> sql = "SELECT 1"
     >>> preview_rows = 10
     >>> response = client.queries.post(database_id, sql, preview_rows,
     >>>                                credential=cred_id)
-    >>> job_id = response.id
     >>>
-    >>> poller = client.queries.get
-    >>> poller_args = (job_id, ) # (job_id, run_id) if poller requires run_id
+    >>> poller = client.queries.get_runs
+    >>> poller_args = response.id, response.last_run_id
     >>> polling_interval = 10
     >>> future = CivisFuture(poller, poller_args, polling_interval)
+    >>> future.job_id == response.id
+    True
+    >>> future.run_id == response.last_run_id
+    True
     """
-    def __init__(self, poller, poller_args,
-                 polling_interval=None, api_key=None, client=None,
-                 poll_on_creation=True):
+
+    def __init__(
+        self,
+        poller,
+        poller_args,
+        polling_interval=None,
+        client=None,
+        poll_on_creation=True,
+    ):
         if client is None:
-            client = APIClient(api_key=api_key)
+            client = APIClient()
 
-        if polling_interval is None and hasattr(client, 'channels'):
-            polling_interval = _LONG_POLLING_INTERVAL
+        super().__init__(
+            poller=poller,
+            poller_args=poller_args,
+            polling_interval=polling_interval,
+            client=client,
+            poll_on_creation=poll_on_creation,
+        )
 
-        super().__init__(poller=poller,
-                         poller_args=poller_args,
-                         polling_interval=polling_interval,
-                         api_key=api_key,
-                         client=client,
-                         poll_on_creation=poll_on_creation)
-
-    def _begin_tracking(self, start_thread=False):
-        # Be sure to subscribe to the PubNub channel before polling.
-        # Otherwise the job might complete after polling and before
-        # we subscribe, causing us to miss the notification.
-        with self._condition:
-            if hasattr(self.client, 'channels') and not self.subscribed:
-                config, channels = self._pubnub_config()
-                self._pubnub = self._subscribe(config, channels)
-            super()._begin_tracking(start_thread)  # superclass does polling
+        self._exception_handled = False
+        self.add_done_callback(self._set_job_exception)
+
+    @staticmethod
+    def _set_job_exception(fut):
+        """Callback: On job completion, check the status.
+        If the job has failed, and has no pre-existing error message,
+        populate the error message with recent logs.
+        """
+        # Prevent infinite recursion: this function calls `set_exception`,
+        # which triggers callbacks (i.e. re-calls this function).
+        if fut._exception_handled:
+            return
+        else:
+            fut._exception_handled = True
+
+        if fut.failed():
+            # Some platform script types do not return the error message,
+            # so we override with an exception we can pull from the
+            # logs
+            if isinstance(
+                fut._exception, CivisJobFailure
+            ) and fut._exception._original_err_msg in ("None", "", None):
+                fut._exception.error_message = ""
+                exc = fut._exception_from_logs(fut._exception)
+                fut.set_exception(exc)
+
+    def _exception_from_logs(self, exc, nlog=15):
+        """Create an exception if the log has a recognizable error
+
+        Search "error" emits in the last ``n_log`` lines.
+        This function presently recognizes the following errors:
+
+        - MemoryError
+        """
+        # Traceback in platform logs may be delayed for a few seconds.
+        time.sleep(15)
+        logs = self.client.jobs.list_runs_logs(self.job_id, self.run_id, limit=nlog)
+        # Reverse order as logs come back in reverse chronological order.
+        logs = logs[::-1]
+
+        # Check for memory errors
+        msgs = [x["message"] for x in logs if x["level"] == "error"]
+        mem_err = [m for m in msgs if m.startswith("Process ran out of its")]
+        if mem_err:
+            err_msg = _err_msg_with_job_run_ids(mem_err[0], self.job_id, self.run_id)
+            exc = MemoryError(err_msg)
+        else:
+            # Unknown error; return logs to the user as a sort of traceback
+            all_logs = "\n".join([x["message"] for x in logs])
+            if isinstance(exc, CivisJobFailure):
+                err_msg = _err_msg_with_job_run_ids(
+                    all_logs + "\n" + exc.error_message, self.job_id, self.run_id
+                )
+                exc.error_message = err_msg
+            else:
+                err_msg = _err_msg_with_job_run_ids(all_logs, self.job_id, self.run_id)
+                exc = CivisJobFailure("", job_id=self.job_id, run_id=self.run_id)
+                exc.error_message = err_msg
+        return exc
 
     @property
-    def subscribed(self):
-        return (hasattr(self, '_pubnub') and
-                len(self._pubnub.get_subscribed_channels()) > 0)
+    def job_id(self):
+        """The job ID for the Civis Platform job that this future is tracking.
 
-    def cleanup(self):
-        with self._condition:
-            super().cleanup()
-            if hasattr(self, '_pubnub'):
-                self._pubnub.unsubscribe_all()
-
-                # Pubnub doesn't close its open session, so do that ourselves
-                # to free up sockets. We have to access a private attribute,
-                # but this exists at least in (4.0.0 <= versions <= 4.0.11).
-                # After closing the Session, remove it so that PubNub
-                # can't reopen it.
-                self._pubnub._request_handler.session.close()
-                del self._pubnub._request_handler.session
-
-                # The PubNub object is no longer usable.
-                # Note that it can't be garbage collected because of circular
-                # references, so this represents a (small) memory leak.
-                del self._pubnub
-
-    def _subscribe(self, pnconfig, channels):
-        listener = JobCompleteListener(self._check_message,
-                                       self._poll_and_set_api_result,
-                                       self._reset_polling_thread)
-        pubnub = PubNub(pnconfig)
-        pubnub.add_listener(listener)
-
-        # Start our subscription 30 seconds in the past to catch any
-        # missed messages.
-        # https://www.pubnub.com/docs/python/api-reference-misc#time
-        token = int((time.time() - 30) * 10**7)
-        pubnub.subscribe().channels(channels).with_timetoken(token).execute()
-        return pubnub
-
-    def _pubnub_config(self):
-        channel_config = self.client.channels.list()
-        channels = [channel['name'] for channel in channel_config['channels']]
-        pnconfig = PNConfiguration()
-        pnconfig.subscribe_key = channel_config['subscribe_key']
-        pnconfig.cipher_key = channel_config['cipher_key']
-        pnconfig.auth_key = channel_config['auth_key']
-        pnconfig.ssl = True
-        pnconfig.reconnect_policy = PNReconnectionPolicy.EXPONENTIAL
-        return pnconfig, channels
+        Returns
+        -------
+        int
+        """
+        return self.poller_args[0]
+
+    @property
+    def run_id(self):
+        """The run ID for the Civis Platform job that this future is tracking.
+
+        Returns
+        -------
+        int | None
+        """
+        try:
+            return self.poller_args[1]
+        except IndexError:
+            # when poller function has job_id only but not run_id
+            return None
+
+    @property
+    def job_url(self):
+        """The URL for the Civis Platform job that this future is tracking.
+
+        Returns
+        -------
+        str
+        """
+        return f"https://platform.civisanalytics.com/spa/#/jobs/{self.job_id}"
 
     def _check_message(self, message):
         try:
             # poller_args can be (job_id,) or (job_id, run_id)
             if len(self.poller_args) == 1:
-                match = (message['object']['id'] == self.poller_args[0] and
-                         message['run']['state'] in DONE)
+                match = (
+                    message["object"]["id"] == self.poller_args[0]
+                    and message["run"]["state"] in DONE
+                )
             else:
-                match = (message['object']['id'] == self.poller_args[0] and
-                         message['run']['id'] == self.poller_args[1] and
-                         message['run']['state'] in DONE)
+                match = (
+                    message["object"]["id"] == self.poller_args[0]
+                    and message["run"]["id"] == self.poller_args[1]
+                    and message["run"]["state"] in DONE
+                )
         except KeyError:
             return False
         return match
 
-    def _poll_and_set_api_result(self):
-        with self._condition:
-            try:
-                result = self.poller(*self.poller_args)
-                self._set_api_result(result)
-            except Exception as e:
-                self._set_api_exception(exc=e)
+    def outputs(self):
+        """Block on job completion and return a list of run outputs.
+
+        The method will only return run outputs for successful jobs.
+        Failed jobs will raise an exception.
+
+        Returns
+        -------
+        list[dict]
+            List of run outputs from a successfully completed job.
+
+        Raises
+        ------
+        civis.base.CivisJobFailure
+            If the job fails.
+        """
+        self.result()
+        outputs = self.client.jobs.list_runs_outputs(self.job_id, self.run_id)
+        return outputs
 
 
 class ContainerFuture(CivisFuture):
     """Encapsulates asynchronous execution of a Civis Container Script
 
     This object includes the ability to cancel a run in progress,
     as well as the option to automatically retry failed runs.
@@ -217,49 +229,49 @@
         The ID for the container/script/job.
     run_id : int
         The ID for the run to monitor
     max_n_retries : int, optional
         If the job generates an exception, retry up to this many times
     polling_interval: int or float, optional
         The number of seconds between API requests to check whether a result
-        is ready. You should not set this if you're using ``pubnub``
-        (the default if ``pubnub`` is installed).
+        is ready.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     poll_on_creation : bool, optional
         If ``True`` (the default), it will poll upon calling ``result()`` the
         first time. If ``False``, it will wait the number of seconds specified
         in `polling_interval` from object creation before polling.
 
     See Also
     --------
     civis.futures.CivisFuture
     """
-    def __init__(self, job_id, run_id,
-                 max_n_retries=0,
-                 polling_interval=None,
-                 client=None,
-                 poll_on_creation=True):
+
+    def __init__(
+        self,
+        job_id,
+        run_id,
+        max_n_retries=0,
+        polling_interval=None,
+        client=None,
+        poll_on_creation=True,
+    ):
         if client is None:
             client = APIClient()
-        super().__init__(client.scripts.get_containers_runs,
-                         [int(job_id), int(run_id)],
-                         polling_interval=polling_interval,
-                         client=client,
-                         poll_on_creation=poll_on_creation)
-        self._max_n_retries = max_n_retries
 
-    @property
-    def job_id(self):
-        return self.poller_args[0]
+        self._max_n_retries = max_n_retries
 
-    @property
-    def run_id(self):
-        return self.poller_args[1]
+        super().__init__(
+            client.scripts.get_containers_runs,
+            [int(job_id), int(run_id)],
+            polling_interval=polling_interval,
+            client=client,
+            poll_on_creation=poll_on_creation,
+        )
 
     def _set_api_exception(self, exc, result=None):
         # Catch attempts to set an exception. If there's retries
         # remaining, retry the run instead of erroring.
         with self._condition:
             if self._max_n_retries > 0:
                 # Start a new run of the script and update
@@ -275,18 +287,22 @@
                 # stopped in cleanup. Start a new polling thread.
                 # Note that it's possible to have a race condition if
                 # you shut down the old thread too soon after starting it.
                 # In practice this only happens when testing retries
                 # with extremely short polling intervals.
                 self._begin_tracking(start_thread=True)
 
-                log.debug('Job ID %d / Run ID %d failed. Retrying '
-                          'with run %d. %d retries remaining.',
-                          self.job_id, orig_run_id,
-                          run_id, self._max_n_retries)
+                log.debug(
+                    "Job ID %d / Run ID %d failed. Retrying "
+                    "with run %d. %d retries remaining.",
+                    self.job_id,
+                    orig_run_id,
+                    run_id,
+                    self._max_n_retries,
+                )
             else:
                 super()._set_api_exception(exc=exc, result=result)
 
     def cancel(self):
         """Submit a request to cancel the container/script/run.
 
         Returns
@@ -304,17 +320,19 @@
                     self._result = self.client.scripts.post_cancel(self.job_id)
                 except CivisAPIError as exc:
                     if exc.status_code == 404:
                         # The most likely way to get this error
                         # is for the job to already be completed.
                         return False
                     else:
-                        warnings.warn("Unexpected error when attempting to "
-                                      "cancel job ID %d / run ID %d:\n%s" %
-                                      (self.job_id, self.run_id, str(exc)))
+                        warnings.warn(
+                            "Unexpected error when attempting to "
+                            "cancel job ID %d / run ID %d:\n%s"
+                            % (self.job_id, self.run_id, str(exc))
+                        )
                         return False
                 for waiter in self._waiters:
                     waiter.add_cancelled(self)
                 self._condition.notify_all()
                 self.cleanup()
                 self._invoke_callbacks()
                 return self.cancelled()
@@ -327,28 +345,30 @@
     followed by the keyword arguments kwargs (in sorted order, for
     consistency), separated by spaces.
 
     For example,
     ``_create_docker_command('./myprogram', 5, 6, wibble=7, wobble=8)``
     returns ``"./myprogram 5 6 --wibble 7 --wobble 8"``.
     """
-    return " ".join([str(x) for x in args] +
-                    ["--{} {}".format(k, v)
-                     for k, v in sorted(kwargs.items())])
-
-
-@six.add_metaclass(ABCMeta)
-class _CivisExecutor(Executor):
-    def __init__(self,
-                 name=None,
-                 hidden=True,
-                 max_n_retries=0,
-                 client=None,
-                 polling_interval=None,
-                 inc_script_names=False):
+    return " ".join(
+        [str(x) for x in args]
+        + ["--{} {}".format(k, v) for k, v in sorted(kwargs.items())]
+    )
+
+
+class _CivisExecutor(Executor, metaclass=ABCMeta):
+    def __init__(
+        self,
+        name=None,
+        hidden=True,
+        max_n_retries=0,
+        client=None,
+        polling_interval=None,
+        inc_script_names=False,
+    ):
         self.max_n_retries = max_n_retries
         self.hidden = hidden
         self.name = name
         self.polling_interval = polling_interval
         self.inc_script_names = inc_script_names
         self._script_name_counter = 0
 
@@ -363,19 +383,22 @@
         self._futures = []
 
     def _make_future(self, job_id, run_id):
         """Instantiates a :class:`~civis.futures.ContainerFuture`,
         adds it to the internal list of futures, and returns it.
         This is a helper method for :func:`submit`.
         """
-        future = ContainerFuture(job_id, run_id,
-                                 polling_interval=self.polling_interval,
-                                 max_n_retries=self.max_n_retries,
-                                 client=self.client,
-                                 poll_on_creation=False)
+        future = ContainerFuture(
+            job_id,
+            run_id,
+            polling_interval=self.polling_interval,
+            max_n_retries=self.max_n_retries,
+            client=self.client,
+            poll_on_creation=False,
+        )
 
         self._futures.append(future)
 
         # Return a ContainerFuture object with the job ID.
         return future
 
     def submit(self, fn, *args, **kwargs):
@@ -403,41 +426,44 @@
         -------
         :class:`~civis.futures.ContainerFuture`
             Note that the ``Future`` returned by ``submit`` will
             provide the final status of your Container Script as
             its ``.result()``. The user is responsible for downloading
             outputs produced by the script, if any.
         """
-        arguments = kwargs.pop('arguments', {})
-        arguments.update({'CIVIS_PARENT_JOB_ID': os.getenv('CIVIS_JOB_ID'),
-                          'CIVIS_PARENT_RUN_ID': os.getenv('CIVIS_RUN_ID')})
+        arguments = kwargs.pop("arguments", {})
+        arguments.update(
+            {
+                "CIVIS_PARENT_JOB_ID": os.getenv("CIVIS_JOB_ID"),
+                "CIVIS_PARENT_RUN_ID": os.getenv("CIVIS_RUN_ID"),
+            }
+        )
 
         with self._shutdown_lock:
             if self._shutdown_thread:
-                raise RuntimeError('cannot schedule new '
-                                   'futures after shutdown')
+                raise RuntimeError("cannot schedule new " "futures after shutdown")
 
-            if isinstance(fn, six.string_types):
+            if isinstance(fn, str):
                 cmd = fn
             else:
                 if fn is None:
                     fn = _create_docker_command
                 cmd = fn(*args, **kwargs)
 
             name = self.name
             if self.inc_script_names:
                 name = "{} {}".format(name, self._script_name_counter)
                 self._script_name_counter += 1
 
-            job = self._create_job(name=name,
-                                   arguments=arguments,
-                                   cmd=cmd)
+            job = self._create_job(name=name, arguments=arguments, cmd=cmd)
             run = self.client.jobs.post_runs(job.id)
-            log.debug('Container "{}" created with script ID {} and '
-                      'run ID {}'.format(name, job.id, run.id))
+            log.debug(
+                'Container "{}" created with script ID {} and '
+                "run ID {}".format(name, job.id, run.id)
+            )
 
             return self._make_future(job.id, run.id)
 
     @abstractmethod
     def _create_job(self, name, arguments=None, cmd=None):
         raise NotImplementedError("Implement in the child class")
 
@@ -515,78 +541,99 @@
         e.g. network problems.
     client: APIClient, optional
         The :class:`~civis.APIClient` object to use for interacting with the
         API. If not specified, a new one will be instantiated.
     polling_interval: int or float, optional
         The number of seconds between API requests to check whether a result
         is ready.  This will be passed to the
-        :class:`~ContainerFuture` objects that are created. You should
-        only set this if you aren't using ``pubnub`` notifications.
+        :class:`~ContainerFuture` objects that are created.
     inc_script_names: bool, optional
         If ``True``, a counter will be added to the ``name`` to create
         the script names for each submission.
     **kwargs:
         Additional keyword arguments will be passed
         directly to :func:`~civis.APIClient.scripts.post_containers`.
 
     See Also
     --------
     civis.APIClient.scripts.post_containers
     """
-    def __init__(self, docker_image_name="civisanalytics/datascience-python",
-                 name=None,
-                 required_resources=None,
-                 hidden=True,
-                 max_n_retries=0,
-                 client=None,
-                 polling_interval=None,
-                 inc_script_names=False,
-                 **kwargs):
+
+    def __init__(
+        self,
+        docker_image_name="civisanalytics/datascience-python",
+        name=None,
+        required_resources=None,
+        hidden=True,
+        max_n_retries=0,
+        client=None,
+        polling_interval=None,
+        inc_script_names=False,
+        **kwargs,
+    ):
         self.docker_image_name = docker_image_name
         self.container_kwargs = kwargs
 
-        params = [{'name': 'CIVIS_PARENT_JOB_ID',
-                   'type': 'integer',
-                   'value': os.getenv('CIVIS_JOB_ID')},
-                  {'name': 'CIVIS_PARENT_RUN_ID',
-                   'type': 'integer',
-                   'value': os.getenv('CIVIS_RUN_ID')}]
-        self.container_kwargs.setdefault('params', []).extend(params)
+        # Add params for parent job info.
+        # Overwrite them if they already exist to avoid duplicates, which would
+        # lead to job failure.
+        params = [
+            p
+            for p in self.container_kwargs.get("params", [])
+            if p["name"].upper() not in ("CIVIS_PARENT_JOB_ID", "CIVIS_PARENT_RUN_ID")
+        ]
+        params.extend(
+            [
+                {
+                    "name": "CIVIS_PARENT_JOB_ID",
+                    "type": "integer",
+                    "value": os.getenv("CIVIS_JOB_ID"),
+                },
+                {
+                    "name": "CIVIS_PARENT_RUN_ID",
+                    "type": "integer",
+                    "value": os.getenv("CIVIS_RUN_ID"),
+                },
+            ]
+        )
+        self.container_kwargs["params"] = params
 
         if required_resources is None:
-            required_resources = {'cpu': 1024, 'memory': 1024}
+            required_resources = {"cpu": 1024, "memory": 1024}
         self.required_resources = required_resources
 
         if name is None:
             date_str = datetime.datetime.today().strftime("%Y-%m-%d")
             name = "ContainerShellExecutorScript {}".format(date_str)
 
-        super().__init__(name=name,
-                         hidden=hidden,
-                         client=client,
-                         max_n_retries=max_n_retries,
-                         polling_interval=polling_interval,
-                         inc_script_names=inc_script_names)
+        super().__init__(
+            name=name,
+            hidden=hidden,
+            client=client,
+            max_n_retries=max_n_retries,
+            polling_interval=polling_interval,
+            inc_script_names=inc_script_names,
+        )
 
     def _create_job(self, name, arguments=None, cmd=None):
         # Combine instance and input arguments into one dictionary.
         # Use `None` instead of an empty dictionary.
         kwargs = copy.deepcopy(self.container_kwargs)
-        kwargs.setdefault('arguments', {}).update(arguments or {})
-        if not kwargs['arguments']:
-            del kwargs['arguments']
+        kwargs.setdefault("arguments", {}).update(arguments or {})
+        if not kwargs["arguments"]:
+            del kwargs["arguments"]
 
         # Submit a request to Civis to make the container script object.
         job = self.client.scripts.post_containers(
             name=name,
             required_resources=self.required_resources,
             docker_command=cmd,
             docker_image_name=self.docker_image_name,
             hidden=self.hidden,
-            **self.container_kwargs
+            **self.container_kwargs,
         )
 
         return job
 
 
 class CustomScriptExecutor(_CivisExecutor):
     """Manage a pool of Custom Scripts in the Civis Platform
@@ -630,45 +677,50 @@
         e.g. network problems.
     client: APIClient, optional
         The :class:`~civis.APIClient` object to use for interacting with the
         API. If not specified, a new one will be instantiated.
     polling_interval: int or float, optional
         The number of seconds between API requests to check whether a result
         is ready.  This will be passed to the
-        :class:`~ContainerFuture` objects that are created. You should
-        only set this if you aren't using ``pubnub`` notifications.
+        :class:`~ContainerFuture` objects that are created.
     inc_script_names: bool, optional
         If ``True``, a counter will be added to the ``name`` to create
         the script names for each submission.
 
     See Also
     --------
     civis.APIClient.scripts.post_custom
     """
-    def __init__(self, from_template_id,
-                 name=None,
-                 hidden=True,
-                 arguments=None,
-                 max_n_retries=0,
-                 client=None,
-                 polling_interval=None,
-                 inc_script_names=False):
+
+    def __init__(
+        self,
+        from_template_id,
+        name=None,
+        hidden=True,
+        arguments=None,
+        max_n_retries=0,
+        client=None,
+        polling_interval=None,
+        inc_script_names=False,
+    ):
         self.from_template_id = from_template_id
         self.arguments = arguments
 
         if name is None:
             date_str = datetime.datetime.today().strftime("%Y-%m-%d")
             name = "CustomScriptExecutorScript {}".format(date_str)
 
-        super().__init__(name=name,
-                         hidden=hidden,
-                         client=client,
-                         max_n_retries=max_n_retries,
-                         polling_interval=polling_interval,
-                         inc_script_names=inc_script_names)
+        super().__init__(
+            name=name,
+            hidden=hidden,
+            client=client,
+            max_n_retries=max_n_retries,
+            polling_interval=polling_interval,
+            inc_script_names=inc_script_names,
+        )
 
     def submit(self, **arguments):
         """Submit a Custom Script with the given arguments
 
         Parameters
         ----------
         arguments: dict, optional
@@ -690,9 +742,10 @@
         if not combined_args:
             combined_args = None
 
         job = self.client.scripts.post_custom(
             self.from_template_id,
             name=name,
             arguments=combined_args,
-            hidden=self.hidden)
+            hidden=self.hidden,
+        )
         return job
```

### Comparing `civis-1.9.4/civis/ml/_model.py` & `civis-2.0.0/src/civis/ml/_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,251 +1,223 @@
-"""Run CivisML jobs and retrieve the results
-"""
+"""Run CivisML jobs and retrieve the results"""
+
 import builtins
 from builtins import super
-from collections import namedtuple
+import collections
+from functools import lru_cache
+import io
 import json
 import logging
 import os
+import re
 import shutil
-import six
 import tempfile
 import threading
 import warnings
 from concurrent import futures
 from functools import wraps
 
 import joblib
+
 try:
     from sklearn.base import BaseEstimator
+
     HAS_SKLEARN = True
 except ImportError:
     HAS_SKLEARN = False
 
-from civis import APIClient, find, find_one, __version__
+from civis import APIClient, find, find_one
 from civis._utils import camel_to_snake
 from civis.base import CivisAPIError, CivisJobFailure
-from civis.compat import FileNotFoundError, TemporaryDirectory
 import civis.io as cio
 from civis.futures import ContainerFuture
+from civis.response import Response
+
 
-__all__ = ['ModelFuture', 'ModelError', 'ModelPipeline']
+__all__ = ["ModelFuture", "ModelError", "ModelPipeline"]
 log = logging.getLogger(__name__)
 
 # sentinel value for default primary key value
-SENTINEL = namedtuple('Sentinel', [])()
-
-# Map training template to prediction template so that we
-# always use a compatible version for predictions.
-_PRED_TEMPLATES = {11219: 11220,  # v2.2
-                   11221: 11220,  # v2.2 registration
-                   10582: 10583,  # v2.1
-                   9968: 9969,    # v2.0
-                   9112: 9113,    # v1.1
-                   8387: 8388,    # v1.0
-                   7020: 7021,    # v0.5
-                   }
-_CIVISML_TEMPLATE = None  # CivisML training template to use
-REGISTRATION_TEMPLATES = [11221,  # v2.2
-                          ]
+SENTINEL = collections.namedtuple("Sentinel", [])()
 
 
 class ModelError(RuntimeError):
     def __init__(self, msg, estimator=None, metadata=None):
         self.metadata = metadata
         self.estimator = estimator
         super().__init__(msg)
 
 
 def _check_fit_initiated(method):
     """Makes sure that the ModelPipeline's been trained"""
+
     @wraps(method)
     def wrapper(*args, **kwargs):
         self = args[0]
         if not self.train_result_:
             raise ValueError("This model hasn't been trained yet.")
         return method(*args, **kwargs)
+
     return wrapper
 
 
 def _block_and_handle_missing(method):
     """For ModelFuture file-retrieving property methods.
     Block until completion and attempt to retrieve result.
     Raise exception only if the result isn't found.
     """
+
     @wraps(method)
     def wrapper(self):
         futures.wait((self,))  # Block until done
         try:
             return method(self)
         except FileNotFoundError:
             # We get here if the modeling job failed to produce
             # any output and we don't have metadata.
             if self.exception():
-                six.raise_from(self.exception(), None)
+                raise self.exception() from None
             else:
                 raise
+
     return wrapper
 
 
 def _stash_local_dataframe(df, template_id, client=None):
     """Store data in a temporary Civis File and return the file ID"""
     # Standard dataframe indexes do not have a "levels" attribute,
     # but multiindexes do. Checking for this attribute means we don't
     # need to import pandas to do error handling here.
     if getattr(getattr(df, "index", None), "levels", None) is not None:
-        raise TypeError("CivisML does not support multi-indexed data frames. "
-                        "Try calling `.reset_index` on your data to convert "
-                        "it into a CivisML-friendly format.")
+        raise TypeError(
+            "CivisML does not support multi-indexed data frames. "
+            "Try calling `.reset_index` on your data to convert "
+            "it into a CivisML-friendly format."
+        )
     try:
         if template_id > 9969:
             return _stash_dataframe_as_feather(df, client)
         else:
             return _stash_dataframe_as_csv(df, client)
     except (ImportError, AttributeError) as exc:
-        if (df.dtypes == 'category').any():
+        if (df.dtypes == "category").any():
             # The original exception should tell users if they need
             # to upgrade pandas (an AttributeError)
             # # or if they need to install "feather-format" (ImportError).
-            six.raise_from(ValueError(
-                'Categorical columns can only be handled with pandas '
-                'version >= 0.20 and `feather-format` installed.'),
-                exc)
+            raise ValueError(
+                "Categorical columns can only be handled with pandas "
+                "version >= 0.20 and `feather-format` installed."
+            ) from exc
         return _stash_dataframe_as_csv(df, client)
 
 
 def _stash_dataframe_as_feather(df, client):
-    civis_fname = 'modelpipeline_data.feather'
-    with TemporaryDirectory() as tdir:
+    civis_fname = "modelpipeline_data.feather"
+    with tempfile.TemporaryDirectory() as tdir:
         path = os.path.join(tdir, civis_fname)
         df.to_feather(path)
         file_id = cio.file_to_civis(path, name=civis_fname, client=client)
     return file_id
 
 
 def _stash_dataframe_as_csv(df, client):
-    civis_fname = 'modelpipeline_data.csv'
-    if six.PY3:
-        txt = six.StringIO()
-    else:
-        txt = six.BytesIO()
-    df.to_csv(txt, encoding='utf-8', index=False)
+    civis_fname = "modelpipeline_data.csv"
+    txt = io.StringIO()
+    df.to_csv(txt, encoding="utf-8", index=False)
     txt.flush()
     txt.seek(0)
     file_id = cio.file_to_civis(txt, name=civis_fname, client=client)
 
     return file_id
 
 
 def _stash_local_file(csv_path, client=None):
     """Store data in a temporary Civis File and return the file ID"""
-    civis_fname = 'modelpipeline_data.csv'
+    civis_fname = "modelpipeline_data.csv"
     with open(csv_path) as _fin:
         file_id = cio.file_to_civis(_fin, name=civis_fname, client=client)
 
     return file_id
 
 
 def _decode_train_run(train_job_id, train_run_id, client):
     """Determine correct run ID for use for a given training job ID"""
     try:
         return int(train_run_id)
     except ValueError:
         container = client.scripts.get_containers(int(train_job_id))
-        if train_run_id == 'active':
-            train_run_id = container.arguments.get('ACTIVE_BUILD', find_one(
-                container.params, name='ACTIVE_BUILD'))['default']
+        if train_run_id == "active":
+            train_run_id = container.arguments.get(
+                "ACTIVE_BUILD", find_one(container.params, name="ACTIVE_BUILD")
+            )["default"]
 
-        if train_run_id == 'latest':
+        if train_run_id == "latest":
             return container.last_run.id
 
         try:
             return int(train_run_id)
         except Exception as exc:
-            msg = ('Please provide valid train_run_id! Needs to be '
-                   'integer corresponding to a training run ID '
-                   'or one of "active" or "latest".')
-            six.raise_from(ValueError(msg), exc)
+            msg = (
+                "Please provide valid train_run_id! Needs to be "
+                "integer corresponding to a training run ID "
+                'or one of "active" or "latest".'
+            )
+            raise ValueError(msg) from exc
 
 
 def _retrieve_file(fname, job_id, run_id, local_dir, client=None):
     """Download a Civis file using a reference on a previous run"""
     file_id = cio.file_id_from_run_output(fname, job_id, run_id, client=client)
     fpath = os.path.join(local_dir, fname)
     # fname may contain a path
     output_dir = os.path.dirname(fpath)
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
-    with open(fpath, 'wb') as down_file:
+    with open(fpath, "wb") as down_file:
         cio.civis_to_file(file_id, down_file, client=client)
     return fpath
 
 
-def _load_table_from_outputs(job_id, run_id, filename, client=None,
-                             **table_kwargs):
+def _load_table_from_outputs(job_id, run_id, filename, client=None, **table_kwargs):
     """Load a table from a run output directly into a ``DataFrame``"""
     client = APIClient() if client is None else client
-    file_id = cio.file_id_from_run_output(filename, job_id, run_id,
-                                          client=client, regex=True)
+    file_id = cio.file_id_from_run_output(
+        filename, job_id, run_id, client=client, regex=True
+    )
     return cio.file_to_dataframe(file_id, client=client, **table_kwargs)
 
 
-def _load_estimator(job_id, run_id, filename='estimator.pkl', client=None):
+def _load_estimator(job_id, run_id, filename="estimator.pkl", client=None):
     """Load a joblib-serialized Estimator from run outputs"""
     try:
         tempdir = tempfile.mkdtemp()
         path = _retrieve_file(filename, job_id, run_id, tempdir, client=client)
         obj = joblib.load(path)
     finally:
         shutil.rmtree(tempdir)
     return obj
 
 
-def _exception_from_logs(exc, job_id, run_id, client, nlog=15):
-    """Create an exception if the log has a recognizable error
-
-    Search "error" emits in the last ``n_log`` lines.
-    This function presently recognizes the following errors:
-
-    - MemoryError
-    """
-    logs = client.scripts.list_containers_runs_logs(job_id, run_id, limit=nlog)
-
-    # Check for memory errors
-    msgs = [l['message'] for l in logs if l['level'] == 'error']
-    mem_err = [m for m in msgs if m.startswith('Process ran out of its')]
-    if mem_err:
-        exc = MemoryError(mem_err[0])
-    else:
-        # Unknown error; return logs to the user as a sort of traceback
-        all_logs = '\n'.join([l['message'] for l in logs])
-        if isinstance(exc, CivisJobFailure):
-            exc.error_message = all_logs + '\n' + exc.error_message
-        else:
-            exc = CivisJobFailure(all_logs)
-    return exc
-
-
 def _parse_warning(warn_str):
     """Reverse-engineer a warning string
 
     Parameters
     ----------
     warn_str : string
 
     Returns
     -------
     (str, Warning, str, int)
         message, category, filename, lineno
     """
-    tokens = warn_str.rstrip('\n').split(" ")
+    tokens = warn_str.rstrip("\n").split(" ")
 
     # The first token is
     # "[filename]:[lineno]:"
-    filename, lineno, _ = tokens[0].split(':')
+    filename, lineno, _ = tokens[0].split(":")
 
     # The second token is
     # "[category name]:"
     category = getattr(builtins, tokens[1][:-1], RuntimeWarning)
 
     message = " ".join(tokens[2:])
 
@@ -264,14 +236,143 @@
         try:
             warnings.warn_explicit(*_parse_warning(warn_str))
         except Exception:  # NOQA
             warn_str = "Remote warning from CivisML:\n" + warn_str
             warnings.warn(warn_str, RuntimeWarning)
 
 
+def _get_job_type_version(alias):
+    """Derive the job type and version from the given alias.
+
+    Parameters
+    ----------
+    alias : str
+        CivisML alias
+
+    Returns
+    -------
+    str
+        Job type, one of {training, prediction, registration}.
+    str
+        CivisML version, e.g., "v2.2".
+    """
+    # A version-less alias for production, e.g., "civis-civisml-training"
+    match_production = re.search(r"\Acivis-civisml-(\w+)\Z", alias)
+    # A versioned alias, e.g., "civis-civisml-training-v2-3"
+    match_v = re.search(r"\Acivis-civisml-(\w+)-v(\d+)-(\d+)\Z", alias)
+    # A special-version alias, e.g., "civis-civisml-training-dev"
+    match_special = re.search(r"\Acivis-civisml-(\w+)-(\S+[^-])\Z", alias)
+
+    if match_production:
+        job_type = match_production.group(1)
+        version = None
+    elif match_v:
+        job_type = match_v.group(1)
+        version = "v%s.%s" % match_v.group(2, 3)
+    elif match_special:
+        job_type = match_special.group(1)
+        version = match_special.group(2)
+    else:
+        msg = 'Unable to parse the job type and version from the CivisML alias "%r"'
+        raise ValueError(msg % alias)
+
+    return job_type, version
+
+
+@lru_cache()
+def _get_template_ids_all_versions(client):
+    """Get templates IDs for all accessible CivisML versions.
+
+    Parameters
+    ----------
+    client : APIClient
+        Civis API client object
+
+    Returns
+    -------
+    Dict[str, Dict[str, int]]
+        Mapping between versions (e.g., "v2.2") and template IDs for the given
+        version (e.g., {'training': 1, 'prediction': 2, 'registration': 3}).
+    """
+    template_alias_objects = client.aliases.list(
+        object_type="template_script", iterator=True
+    )
+    civisml_template_alias_objects = find(
+        template_alias_objects, alias=lambda alias: alias.startswith("civis-civisml-")
+    )
+    ids = collections.defaultdict(
+        lambda: {"training": None, "prediction": None, "registration": None}
+    )
+    for alias_obj in civisml_template_alias_objects:
+        try:
+            job_type, version = _get_job_type_version(alias_obj.alias)
+        except ValueError:
+            msg = (
+                '%r looks like a CivisML alias for the prefix "civis-civisml-"'
+                ", but it is impossible to parse its job type and version"
+            )
+            log.debug(msg % alias_obj)
+            continue
+        ids[version][job_type] = alias_obj.object_id
+    if not ids:
+        r = Response(
+            {
+                "status_code": 404,
+                "reason": "No CivisML template IDs are accessible.",
+                "content": None,
+            }
+        )
+        raise CivisAPIError(r)
+    # Disallow a defaultdict in the output, so that a non-existent CivisML
+    # version as key should trigger a KeyError.
+    ids = dict(ids)
+    return ids
+
+
+def _get_template_ids(civisml_version, client):
+    """Get template IDs for the specified CivisML version.
+
+    Parameters
+    ----------
+    civisml_version : str
+        CivisML version
+    client : APIClient
+        Civis API client object
+
+    Returns
+    -------
+    int
+        Template ID for training
+    int
+        Template ID for prediction
+    int
+        Template ID for pre-trained model registration
+    """
+    template_ids_all_versions = _get_template_ids_all_versions(client)
+    try:
+        ids = template_ids_all_versions[civisml_version]
+    except KeyError:
+        msg = (
+            '"{civisml_version}" is an invalid CivisML version. '
+            "Either this version does not exist, or you do not have access "
+            "to this version. "
+            "Versions accessible to you are {{{accessible_versions}}}, "
+            "as well as `None` for the latest production version."
+        ).format(
+            civisml_version=civisml_version,
+            accessible_versions=", ".join(
+                '"%s"' % v
+                # Don't include None, or else it would crash sorted()
+                for v in sorted(v for v in template_ids_all_versions.keys() if v)
+            ),
+        )
+        raise ValueError(msg)
+    return ids["training"], ids["prediction"], ids["registration"]
+
+
 class ModelFuture(ContainerFuture):
     """Encapsulates asynchronous execution of a CivisML job
 
     This object knows where to find modeling outputs
     from CivisML jobs. All data attributes are
     lazily retrieved and block on job completion.
 
@@ -289,17 +390,15 @@
         If not provided, this object is assumed to encapsulate a training
         job, and ``train_job_id`` will equal ``job_id``.
     train_run_id : int, optional
         If not provided, this object is assumed to encapsulate a training
         run, and ``train_run_id`` will equal ``run_id``.
     polling_interval : int or float, optional
         The number of seconds between API requests to check whether a result
-        is ready. The default intelligently switches between a short
-        interval if ``pubnub`` is not available and a long interval
-        for ``pubnub`` backup if that library is installed.
+        is ready.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     poll_on_creation : bool, optional
         If ``True`` (the default), it will poll upon calling ``result()`` the
         first time. If ``False``, it will wait the number of seconds specified
         in `polling_interval` from object creation before polling.
@@ -356,152 +455,167 @@
     See Also
     --------
     civis.futures.CivisFuture
     civis.futures.ContainerFuture
     concurrent.futures.Future
     """
 
-    def __init__(self, job_id, run_id, train_job_id=None, train_run_id=None,
-                 polling_interval=None, client=None, poll_on_creation=True):
-        super().__init__(job_id, run_id,
-                         polling_interval=polling_interval,
-                         client=client,
-                         poll_on_creation=poll_on_creation)
+    def __init__(
+        self,
+        job_id,
+        run_id,
+        train_job_id=None,
+        train_run_id=None,
+        polling_interval=None,
+        client=None,
+        poll_on_creation=True,
+    ):
         if train_job_id and train_run_id:
             self.is_training = False
             self.train_job_id = train_job_id
             self.train_run_id = train_run_id
         else:
             self.is_training = True
-            self.train_job_id = self.job_id
-            self.train_run_id = self.run_id
+            self.train_job_id = job_id
+            self.train_run_id = run_id
         self._metadata, self._val_metadata = None, None
         self._train_data, self._train_data_fname = None, None
         self._train_metadata = None
         self._table, self._estimator = None, None
-        self._exception_handled = False
-        self.add_done_callback(self._set_model_exception)
+        super().__init__(
+            job_id,
+            run_id,
+            polling_interval=polling_interval,
+            client=client,
+            poll_on_creation=poll_on_creation,
+        )
 
     @staticmethod
-    def _set_model_exception(fut):
+    def _set_job_exception(fut):
         """Callback: On job completion, check the metadata.
         If it indicates an exception, replace the generic
         ``CivisJobFailure`` by a more informative ``ModelError``.
         """
         # Prevent infinite recursion: this function calls `set_exception`,
         # which triggers callbacks (i.e. re-calls this function).
         if fut._exception_handled:
             return
         else:
             fut._exception_handled = True
 
         try:
             meta = fut.metadata
-            if fut.is_training and meta['run']['status'] == 'succeeded':
+            if fut.is_training and meta["run"]["status"] == "succeeded":
                 # if training job and job succeeded, check validation job
                 meta = fut.validation_metadata
-            if meta is not None and meta['run']['status'] == 'exception':
+            if meta is not None and meta["run"]["status"] == "exception":
                 try:
                     # This will fail if the user doesn't have joblib installed
                     est = fut.estimator
                 except Exception:  # NOQA
                     est = None
                 fut.set_exception(
-                    ModelError('Model run failed with stack trace:\n'
-                               '{}'.format(meta['run']['stack_trace']),
-                               est, meta))
+                    ModelError(
+                        "Model run failed with stack trace:\n"
+                        "{}".format(meta["run"]["stack_trace"]),
+                        est,
+                        meta,
+                    )
+                )
         except (FileNotFoundError, CivisJobFailure) as exc:
             # If there's no metadata file
             # (we get FileNotFound or CivisJobFailure),
             # check the tail of the log for a clearer exception.
-            exc = _exception_from_logs(exc, fut.job_id, fut.run_id, fut.client)
+            exc = fut._exception_from_logs(exc)
             fut.set_exception(exc)
         except futures.CancelledError:
             # We don't need to change the exception if the run was cancelled
             pass
         except KeyError:
             # KeyErrors always represent a bug in the modeling code,
             # but showing the resulting KeyError can be confusing and
             # mask the real error.
-            warnings.warn("Received malformed metadata from Civis Platform. "
-                          "Something went wrong with job execution.")
+            warnings.warn(
+                "Received malformed metadata from Civis Platform. "
+                "Something went wrong with job execution."
+            )
 
     def __getstate__(self):
         state = self.__dict__.copy()
-        del state['_polling_thread']
-        del state['client']
-        del state['poller']
-        del state['_condition']
-        if '_pubnub' in state:
-            state['_pubnub'] = True  # Replace with a boolean flag
-        state['_done_callbacks'] = []
-        state['_self_polling_executor'] = None
+        del state["_polling_thread"]
+        del state["client"]
+        del state["poller"]
+        del state["_condition"]
+        state["_done_callbacks"] = []
+        state["_self_polling_executor"] = None
 
         return state
 
     def __setstate__(self, state):
         self.__dict__ = state
         self._condition = threading.Condition()
         self.client = APIClient()
         self.poller = self.client.scripts.get_containers_runs
         self._begin_tracking()
-        self.add_done_callback(self._set_model_exception)
+        self.add_done_callback(self._set_job_exception)
 
     @property
     def state(self):
         state = self._civis_state
-        if state == 'succeeded':
-            state = self.metadata['run']['status']
+        if state == "succeeded":
+            state = self.metadata["run"]["status"]
         return state
 
     @property
     def table_fname(self):
-        return 'predictions.csv'
+        return "predictions.csv"
 
     @property
     def metadata_fname(self):
-        return 'model_info.json'
+        return "model_info.json"
 
     @property
     def train_data_fname(self):
         if self._train_data_fname is None:
-            self._train_data_fname = os.path.basename(self.training_metadata
-                                                      .get('run')
-                                                      .get('configuration')
-                                                      .get('data')
-                                                      .get('location'))
+            self._train_data_fname = os.path.basename(
+                self.training_metadata.get("run")
+                .get("configuration")
+                .get("data")
+                .get("location")
+            )
         return self._train_data_fname
 
     @property
     def train_data(self):
         if self._train_data is None:
             try:
                 self._train_data = _load_table_from_outputs(
                     self.train_job_id,
                     self.train_run_id,
                     self.train_data_fname,
-                    client=self.client)
+                    client=self.client,
+                )
             except CivisAPIError as err:
                 if err.status_code == 404:
-                    msg = 'There is no training data stored for this job!'
-                    six.raise_from(ValueError(msg), err)
+                    msg = "There is no training data stored for this job!"
+                    raise ValueError(msg) from err
                 else:
                     raise
 
         return self._train_data
 
     def _table_primary_key(self):
         # metadata path to input parameters is different
         # for training and prediction
         if self.is_training:
-            pkey = self.metadata[
-                'run']['configuration']['data']['primary_key']
+            pkey = self.metadata["run"]["configuration"]["data"]["primary_key"]
         else:
-            pkey = self.metadata[
-                'jobs'][0]['run']['configuration']['data']['primary_key']
+            pkey = self.metadata["jobs"][0]["run"]["configuration"]["data"][
+                "primary_key"
+            ]
         return pkey
 
     @property
     def table(self):
         self.result()  # Block and raise errors if any
         if self._table is None:
             # An index column will only be present if primary key is
@@ -509,63 +623,70 @@
                 index_col = False
             else:
                 index_col = 0
 
             if self.is_training:
                 try:
                     # Training jobs only have one output table, the OOS scores
-                    self._table = _load_table_from_outputs(self.job_id,
-                                                           self.run_id,
-                                                           self.table_fname,
-                                                           index_col=index_col,
-                                                           client=self.client)
+                    self._table = _load_table_from_outputs(
+                        self.job_id,
+                        self.run_id,
+                        self.table_fname,
+                        index_col=index_col,
+                        client=self.client,
+                    )
                 except FileNotFoundError:
                     # Just pass here, because we want the table to stay None
                     # if it does not exist
                     pass
             else:
                 # Prediction jobs may have many output tables.
-                output_ids = self.metadata['output_file_ids']
+                output_ids = self.metadata["output_file_ids"]
                 if len(output_ids) > 1:
-                    print('This job output {} files. Retrieving only the '
-                          'first. Find the full list at `metadata'
-                          '["output_file_ids"]`.'.format(len(output_ids)))
-                self._table = cio.file_to_dataframe(output_ids[0],
-                                                    client=self.client,
-                                                    index_col=index_col)
+                    print(
+                        "This job output {} files. Retrieving only the "
+                        "first. Find the full list at `metadata"
+                        '["output_file_ids"]`.'.format(len(output_ids))
+                    )
+                self._table = cio.file_to_dataframe(
+                    output_ids[0], client=self.client, index_col=index_col
+                )
         return self._table
 
     @property
     @_block_and_handle_missing
     def metadata(self):
         if self._metadata is None:
-            fid = cio.file_id_from_run_output('model_info.json', self.job_id,
-                                              self.run_id, client=self.client)
+            fid = cio.file_id_from_run_output(
+                "model_info.json", self.job_id, self.run_id, client=self.client
+            )
             self._metadata = cio.file_to_json(fid, client=self.client)
-            _show_civisml_warnings(self._metadata.get('warnings', []))
+            _show_civisml_warnings(self._metadata.get("warnings", []))
         return self._metadata
 
     @property
     @_block_and_handle_missing
     def estimator(self):
         if self._estimator is None:
-            self._estimator = _load_estimator(self.train_job_id,
-                                              self.train_run_id,
-                                              client=self.client)
+            self._estimator = _load_estimator(
+                self.train_job_id, self.train_run_id, client=self.client
+            )
         return self._estimator
 
     @property
     @_block_and_handle_missing
     def validation_metadata(self):
         if self._val_metadata is None:
             try:
-                fid = cio.file_id_from_run_output('metrics.json',
-                                                  self.train_job_id,
-                                                  self.train_run_id,
-                                                  client=self.client)
+                fid = cio.file_id_from_run_output(
+                    "metrics.json",
+                    self.train_job_id,
+                    self.train_run_id,
+                    client=self.client,
+                )
             except FileNotFoundError:
                 # Use an empty dictionary to indicate that
                 # we've already checked for metadata.
                 self._val_metadata = {}
             else:
                 self._val_metadata = cio.file_to_json(fid, client=self.client)
         if not self._val_metadata:
@@ -573,26 +694,28 @@
             return None
         else:
             return self._val_metadata
 
     @property
     def metrics(self):
         if self.validation_metadata:
-            return self.validation_metadata['metrics']
+            return self.validation_metadata["metrics"]
         else:
             return None
 
     @property
     @_block_and_handle_missing
     def training_metadata(self):
         if self._train_metadata is None:
-            fid = cio.file_id_from_run_output('model_info.json',
-                                              self.train_job_id,
-                                              self.train_run_id,
-                                              client=self.client)
+            fid = cio.file_id_from_run_output(
+                "model_info.json",
+                self.train_job_id,
+                self.train_run_id,
+                client=self.client,
+            )
             self._train_metadata = cio.file_to_json(fid, client=self.client)
         return self._train_metadata
 
 
 class ModelPipeline:
     """Interface for scikit-learn modeling in the Civis Platform
 
@@ -661,14 +784,17 @@
         private git repositories.
     verbose : bool, optional
         If True, supply debug outputs in Platform logs and make
         prediction child jobs visible.
     etl : Estimator, optional
         Custom ETL estimator which overrides the default ETL, and
         is run before training and validation.
+    civisml_version : str, optional
+        CivisML version to use for training and prediction.
+        If not provided, the latest version in production is used.
 
     Methods
     -------
     train()
         Train the model on data in Civis Platform; outputs
         :class:`~civis.ml.ModelFuture`
     predict()
@@ -719,102 +845,99 @@
     ...                       primary_key='voterbase_id',
     ...                       cross_validation_parameters={'C': [0.1, 1, 10]})
 
     See Also
     --------
     civis.ml.ModelFuture
     """
-    def _get_template_ids(self, client):
-        """Determine which version of CivisML to use.
 
-        Select the most recent template to which the user has access.
-        Used for internal or limited releases of new CivisML versions.
-        """
-        global _CIVISML_TEMPLATE
-        if _CIVISML_TEMPLATE is None:
-            for t_id in sorted(_PRED_TEMPLATES)[::-1]:
-                if t_id in REGISTRATION_TEMPLATES:
-                    continue
-                try:
-                    # Check that we can access the template
-                    client.templates.get_scripts(id=t_id)
-                    client.templates.get_scripts(id=_PRED_TEMPLATES[t_id])
-                except CivisAPIError:
-                    continue
-                else:
-                    # Store the template ID so we don't need to repeat
-                    # these API calls in this session.
-                    _CIVISML_TEMPLATE = t_id
-                    break
-            else:
-                raise RuntimeError("Unable to find a CivisML template.")
-        return _CIVISML_TEMPLATE, _PRED_TEMPLATES[_CIVISML_TEMPLATE]
-
-    def __init__(self, model, dependent_variable,
-                 primary_key=None, parameters=None,
-                 cross_validation_parameters=None, model_name=None,
-                 calibration=None, excluded_columns=None, client=None,
-                 cpu_requested=None, memory_requested=None,
-                 disk_requested=None, notifications=None,
-                 dependencies=None, git_token_name=None, verbose=False,
-                 etl=None):
+    def __init__(
+        self,
+        model,
+        dependent_variable,
+        primary_key=None,
+        parameters=None,
+        cross_validation_parameters=None,
+        model_name=None,
+        calibration=None,
+        excluded_columns=None,
+        client=None,
+        cpu_requested=None,
+        memory_requested=None,
+        disk_requested=None,
+        notifications=None,
+        dependencies=None,
+        git_token_name=None,
+        verbose=False,
+        etl=None,
+        civisml_version=None,
+    ):
         self.model = model
         self._input_model = model  # In case we need to modify the input
-        if isinstance(dependent_variable, six.string_types):
+        if isinstance(dependent_variable, str):
             # Standardize the dependent variable as a list.
             dependent_variable = [dependent_variable]
         self.dependent_variable = dependent_variable
 
         # optional but common parameters
         self.primary_key = primary_key
         self.parameters = parameters or {}
         self.cv_params = cross_validation_parameters or {}
         self.model_name = model_name  # None lets Platform use template name
         self.excluded_columns = excluded_columns
         self.calibration = calibration
-        self.job_resources = {'REQUIRED_CPU': cpu_requested,
-                              'REQUIRED_MEMORY': memory_requested,
-                              'REQUIRED_DISK_SPACE': disk_requested}
+        self.job_resources = {
+            "REQUIRED_CPU": cpu_requested,
+            "REQUIRED_MEMORY": memory_requested,
+            "REQUIRED_DISK_SPACE": disk_requested,
+        }
         self.notifications = notifications or {}
         self.dependencies = dependencies
         self.git_token_name = git_token_name
         self.verbose = verbose
 
         if client is None:
             client = APIClient()
         self._client = client
         self.train_result_ = None
 
-        template_ids = self._get_template_ids(self._client)
-        self.train_template_id, self.predict_template_id = template_ids
+        template_ids = _get_template_ids(civisml_version, self._client)
+        self.train_template_id, self.predict_template_id, _ = template_ids
 
         self.etl = etl
         if self.train_template_id < 9968 and self.etl is not None:
             # This is a pre-v2.0 CivisML template
-            raise NotImplementedError("The etl argument is not implemented"
-                                      " in this version of CivisML.")
+            raise NotImplementedError(
+                "The etl argument is not implemented" " in this version of CivisML."
+            )
 
     def __getstate__(self):
         state = self.__dict__.copy()
-        del state['_client']
+        del state["_client"]
         return state
 
     def __setstate__(self, state):
         self.__dict__ = state
         self._client = APIClient()
-        template_ids = self._get_template_ids(self._client)
-        self.train_template_id, self.predict_template_id = template_ids
 
     @classmethod
-    def register_pretrained_model(cls, model, dependent_variable=None,
-                                  features=None, primary_key=None,
-                                  model_name=None, dependencies=None,
-                                  git_token_name=None,
-                                  skip_model_check=False, verbose=False,
-                                  client=None):
+    def register_pretrained_model(
+        cls,
+        model,
+        dependent_variable=None,
+        features=None,
+        primary_key=None,
+        model_name=None,
+        dependencies=None,
+        git_token_name=None,
+        skip_model_check=False,
+        verbose=False,
+        client=None,
+        civisml_version=None,
+    ):
         """Use a fitted scikit-learn model with CivisML scoring
 
         Use this function to set up your own fitted scikit-learn-compatible
         Estimator object for scoring with CivisML. This function will
         upload your model to Civis Platform and store enough metadata
         about it that you can subsequently use it with a CivisML scoring job.
 
@@ -826,14 +949,16 @@
 
         Parameters
         ----------
         model : sklearn.base.BaseEstimator or int
             The model object. This must be a fitted scikit-learn compatible
             Estimator object, or else the integer Civis File ID of a
             pickle or joblib-serialized file which stores such an object.
+            If an Estimator object is provided, it will be uploaded to the
+            Civis Files endpoint and set to be available indefinitely.
         dependent_variable : string or List[str], optional
             The dependent variable of the training dataset.
             For a multi-target problem, this should be a list of
             column names of dependent variables.
         features : string or List[str], optional
             A list of column names of features which were used for training.
             These will be used to ensure that tables input for prediction
@@ -858,99 +983,112 @@
             will fail the comprehensive verification, set this to True.
         verbose : bool, optional
             If True, supply debug outputs in Platform logs and make
             prediction child jobs visible.
         client : :class:`~civis.APIClient`, optional
             If not provided, an :class:`~civis.APIClient` object will be
             created from the :envvar:`CIVIS_API_KEY`.
+        civisml_version : str, optional
+            CivisML version to use.
+            If not provided, the latest version in production is used.
 
         Returns
         -------
         :class:`~civis.ml.ModelPipeline`
 
         Examples
         --------
         This example assumes that you already have training data
         ``X`` and ``y``, where ``X`` is a :class:`~pandas.DataFrame`.
+
         >>> from civis.ml import ModelPipeline
         >>> from sklearn.linear_model import Lasso
         >>> est = Lasso().fit(X, y)
         >>> model = ModelPipeline.register_pretrained_model(
         ...     est, 'concrete', features=X.columns)
         >>> model.predict(table_name='my.table', database_name='my-db')
         """
         client = client or APIClient()
 
-        if isinstance(dependent_variable, six.string_types):
+        if isinstance(dependent_variable, str):
             dependent_variable = [dependent_variable]
-        if isinstance(features, six.string_types):
+        if isinstance(features, str):
             features = [features]
-        if isinstance(dependencies, six.string_types):
+        if isinstance(dependencies, str):
             dependencies = [dependencies]
         if not model_name:
-            model_name = ("Pretrained {} model for "
-                          "CivisML".format(model.__class__.__name__))
+            model_name = "Pretrained {} model for " "CivisML".format(
+                model.__class__.__name__
+            )
             model_name = model_name[:255]  # Max size is 255 characters
 
-        if isinstance(model, (int, float, six.string_types)):
+        if isinstance(model, (int, float, str)):
             model_file_id = int(model)
         else:
             try:
                 tempdir = tempfile.mkdtemp()
-                fout = os.path.join(tempdir, 'model_for_civisml.pkl')
+                fout = os.path.join(tempdir, "model_for_civisml.pkl")
                 joblib.dump(model, fout, compress=3)
-                with open(fout, 'rb') as _fout:
+                with open(fout, "rb") as _fout:
                     # NB: Using the name "estimator.pkl" means that
                     # CivisML doesn't need to copy this input to a file
                     # with a different name.
-                    model_file_id = cio.file_to_civis(_fout, 'estimator.pkl',
-                                                      client=client)
+                    model_file_id = cio.file_to_civis(
+                        _fout, "estimator.pkl", expires_at=None, client=client
+                    )
             finally:
                 shutil.rmtree(tempdir)
 
-        args = {'MODEL_FILE_ID': str(model_file_id),
-                'SKIP_MODEL_CHECK': skip_model_check,
-                'DEBUG': verbose}
+        args = {
+            "MODEL_FILE_ID": str(model_file_id),
+            "SKIP_MODEL_CHECK": skip_model_check,
+            "DEBUG": verbose,
+        }
         if dependent_variable is not None:
-            args['TARGET_COLUMN'] = ' '.join(dependent_variable)
+            args["TARGET_COLUMN"] = " ".join(dependent_variable)
         if features is not None:
-            args['FEATURE_COLUMNS'] = ' '.join(features)
+            args["FEATURE_COLUMNS"] = " ".join(features)
         if dependencies is not None:
-            args['DEPENDENCIES'] = ' '.join(dependencies)
+            args["DEPENDENCIES"] = " ".join(dependencies)
         if git_token_name:
-            creds = find(client.credentials.list(),
-                         name=git_token_name,
-                         type='Custom')
+            creds = find(client.credentials.list(), name=git_token_name, type="Custom")
             if len(creds) > 1:
-                raise ValueError("Unique credential with name '{}' for "
-                                 "remote git hosting service not found!"
-                                 .format(git_token_name))
-            args['GIT_CRED'] = creds[0].id
-
-        template_id = max(REGISTRATION_TEMPLATES)
+                raise ValueError(
+                    "Unique credential with name '{}' for "
+                    "remote git hosting service not found!".format(git_token_name)
+                )
+            args["GIT_CRED"] = creds[0].id
+
+        _, _, template_id = _get_template_ids(civisml_version, client)
+        if template_id is None:
+            msg = (
+                "No registration template ID is available. "
+                "Pre-trained model registration is available for CivisML "
+                'v2.2 (for which `civisml_version` would be "v2.2") or above, '
+                'but you have specified CivisML version "%r"'
+            )
+            raise ValueError(msg % civisml_version)
         container = client.scripts.post_custom(
-            from_template_id=template_id,
-            name=model_name,
-            arguments=args)
-        log.info('Created custom script %s.', container.id)
+            from_template_id=template_id, name=model_name, arguments=args
+        )
+        log.info("Created custom script %s.", container.id)
 
         run = client.scripts.post_custom_runs(container.id)
-        log.debug('Started job %s, run %s.', container.id, run.id)
+        log.debug("Started job %s, run %s.", container.id, run.id)
 
-        fut = ModelFuture(container.id, run.id, client=client,
-                          poll_on_creation=False)
+        fut = ModelFuture(container.id, run.id, client=client, poll_on_creation=False)
         fut.result()
-        log.info('Model registration complete.')
+        log.info("Model registration complete.")
 
         mp = ModelPipeline.from_existing(fut.job_id, fut.run_id, client)
         mp.primary_key = primary_key
         return mp
 
     @classmethod
-    def from_existing(cls, train_job_id, train_run_id='latest', client=None):
+    def from_existing(cls, train_job_id, train_run_id="latest", client=None):
         """Create a :class:`ModelPipeline` object from existing model IDs
 
         Parameters
         ----------
         train_job_id : int
             The ID of the CivisML job in the Civis Platform
         train_run_id : int or string, optional
@@ -982,88 +1120,100 @@
             client = APIClient()
         train_run_id = _decode_train_run(train_job_id, train_run_id, client)
         try:
             fut = ModelFuture(train_job_id, train_run_id, client=client)
             container = client.scripts.get_containers(train_job_id)
         except CivisAPIError as api_err:
             if api_err.status_code == 404:
-                msg = ('There is no Civis Platform job with '
-                       'script ID {} and run ID {}!'.format(train_job_id,
-                                                            train_run_id))
-                six.raise_from(ValueError(msg), api_err)
+                msg = (
+                    "There is no Civis Platform job with "
+                    "script ID {} and run ID {}!".format(train_job_id, train_run_id)
+                )
+                raise ValueError(msg) from api_err
             raise
 
         args = container.arguments
 
         # Older templates used "WORKFLOW" instead of "MODEL"
-        model = args.get('MODEL', args.get('WORKFLOW'))
-        dependent_variable = args['TARGET_COLUMN'].split()
-        primary_key = args.get('PRIMARY_KEY')
-        parameters = json.loads(args.get('PARAMS', "{}"))
-        cross_validation_parameters = json.loads(args.get('CVPARAMS', "{}"))
-        calibration = args.get('CALIBRATION')
-        excluded_columns = args.get('EXCLUDE_COLS', None)
+        model = args.get("MODEL", args.get("WORKFLOW"))
+        dependent_variable = args["TARGET_COLUMN"].split()
+        primary_key = args.get("PRIMARY_KEY")
+        parameters = json.loads(args.get("PARAMS", "{}"))
+        cross_validation_parameters = json.loads(args.get("CVPARAMS", "{}"))
+        calibration = args.get("CALIBRATION")
+        excluded_columns = args.get("EXCLUDE_COLS", None)
         if excluded_columns:
             excluded_columns = excluded_columns.split()
-        cpu_requested = args.get('REQUIRED_CPU')
-        memory_requested = args.get('REQUIRED_MEMORY')
-        disk_requested = args.get('REQUIRED_DISK_SPACE')
+        cpu_requested = args.get("REQUIRED_CPU")
+        memory_requested = args.get("REQUIRED_MEMORY")
+        disk_requested = args.get("REQUIRED_DISK_SPACE")
         name = container.name
-        if name.endswith(' Train'):
+        if name.endswith(" Train"):
             # Strip object-applied suffix
-            name = name[:-len(' Train')]
-        notifications = {camel_to_snake(key): val for key, val
-                         in container.notifications.items()}
-        dependencies = args.get('DEPENDENCIES', None)
+            name = name[: -len(" Train")]
+        notifications = {
+            camel_to_snake(key): val for key, val in container.notifications.items()
+        }
+        dependencies = args.get("DEPENDENCIES", None)
         if dependencies:
             dependencies = dependencies.split()
-        git_token_name = args.get('GIT_CRED', None)
+        git_token_name = args.get("GIT_CRED", None)
         if git_token_name:
             git_token_name = client.credentials.get(git_token_name).name
 
-        klass = cls(model=model,
-                    dependent_variable=dependent_variable,
-                    primary_key=primary_key,
-                    model_name=name,
-                    parameters=parameters,
-                    cross_validation_parameters=cross_validation_parameters,
-                    calibration=calibration,
-                    excluded_columns=excluded_columns,
-                    client=client,
-                    cpu_requested=cpu_requested,
-                    disk_requested=disk_requested,
-                    memory_requested=memory_requested,
-                    notifications=notifications,
-                    dependencies=dependencies,
-                    git_token_name=git_token_name,
-                    verbose=args.get('DEBUG', False))
+        klass = cls(
+            model=model,
+            dependent_variable=dependent_variable,
+            primary_key=primary_key,
+            model_name=name,
+            parameters=parameters,
+            cross_validation_parameters=cross_validation_parameters,
+            calibration=calibration,
+            excluded_columns=excluded_columns,
+            client=client,
+            cpu_requested=cpu_requested,
+            disk_requested=disk_requested,
+            memory_requested=memory_requested,
+            notifications=notifications,
+            dependencies=dependencies,
+            git_token_name=git_token_name,
+            verbose=args.get("DEBUG", False),
+        )
         klass.train_result_ = fut
 
-        # Set prediction template corresponding to training template
-        template_id = int(container['from_template_id'])
-        p_id = _PRED_TEMPLATES.get(template_id)
-        if p_id is None:
-            warnings.warn('Model %s was trained with a newer version of '
-                          'CivisML than is available in the API client '
-                          'version %s. Please update your API client version. '
-                          'Attempting to use an older version of the '
-                          'prediction code. Prediction will either fail '
-                          'immediately or succeed.'
-                          % (train_job_id, __version__), RuntimeWarning)
-            p_id = max([v for k, v in _PRED_TEMPLATES.items()
-                        if k not in REGISTRATION_TEMPLATES])
+        # Set prediction template corresponding to training
+        # or registration template
+        template_id = int(container["from_template_id"])
+        ids = find_one(
+            _get_template_ids_all_versions(client).values(),
+            lambda ids: ids["training"] == template_id
+            or ids["registration"] == template_id,  # noqa
+        )
+        p_id = ids["prediction"]
         klass.predict_template_id = p_id
 
         return klass
 
-    def train(self, df=None, csv_path=None, table_name=None,
-              database_name=None, file_id=None,
-              sql_where=None, sql_limit=None, oos_scores=None,
-              oos_scores_db=None, if_exists='fail', fit_params=None,
-              polling_interval=None, validation_data='train', n_jobs=None):
+    def train(
+        self,
+        df=None,
+        csv_path=None,
+        table_name=None,
+        database_name=None,
+        file_id=None,
+        sql_where=None,
+        sql_limit=None,
+        oos_scores=None,
+        oos_scores_db=None,
+        if_exists="fail",
+        fit_params=None,
+        polling_interval=None,
+        validation_data="train",
+        n_jobs=None,
+    ):
         """Start a Civis Platform job to train your model
 
         Provide input through one of
         a :class:`~pandas.DataFrame` (``df``),
         a local CSV (``csv_path``),
         a Civis Table (``table_name`` and ``database_name``), or
         a Civis File containing a CSV (``file_id``).
@@ -1133,175 +1283,223 @@
             combinations in grid search/hyperband, or decrease to use fewer
             computational resources at once.
 
         Returns
         -------
         :class:`~civis.ml.ModelFuture`
         """
-        if ((table_name is None or database_name is None) and
-                file_id is None and df is None and csv_path is None):
-            raise ValueError('Provide a source of data.')
-        if sum((bool(table_name and database_name),
-                bool(file_id), df is not None, csv_path is not None)) > 1:
-            raise ValueError('Provide a single source of data.')
+        if (
+            (table_name is None or database_name is None)
+            and file_id is None
+            and df is None
+            and csv_path is None
+        ):
+            raise ValueError("Provide a source of data.")
+        if (
+            sum(
+                (
+                    bool(table_name and database_name),
+                    bool(file_id),
+                    df is not None,
+                    csv_path is not None,
+                )
+            )
+            > 1
+        ):
+            raise ValueError("Provide a single source of data.")
 
         if df is not None:
-            file_id = _stash_local_dataframe(df, self.train_template_id,
-                                             client=self._client)
+            file_id = _stash_local_dataframe(
+                df, self.train_template_id, client=self._client
+            )
         elif csv_path:
             file_id = _stash_local_file(csv_path, client=self._client)
 
-        train_args = {'TARGET_COLUMN': ' '.join(self.dependent_variable),
-                      'PRIMARY_KEY': self.primary_key,
-                      'PARAMS': json.dumps(self.parameters),
-                      'CVPARAMS': json.dumps(self.cv_params),
-                      'CALIBRATION': self.calibration,
-                      'IF_EXISTS': if_exists}
+        train_args = {
+            "TARGET_COLUMN": " ".join(self.dependent_variable),
+            "PRIMARY_KEY": self.primary_key,
+            "PARAMS": json.dumps(self.parameters),
+            "CVPARAMS": json.dumps(self.cv_params),
+            "CALIBRATION": self.calibration,
+            "IF_EXISTS": if_exists,
+        }
         if oos_scores:
-            train_args['OOSTABLE'] = oos_scores
+            train_args["OOSTABLE"] = oos_scores
         if oos_scores_db:
             oos_db_id = self._client.get_database_id(oos_scores_db)
-            train_args['OOSDB'] = {'database': oos_db_id}
+            train_args["OOSDB"] = {"database": oos_db_id}
         if sql_where:
-            train_args['WHERESQL'] = sql_where
+            train_args["WHERESQL"] = sql_where
         if sql_limit:
-            train_args['LIMITSQL'] = sql_limit
+            train_args["LIMITSQL"] = sql_limit
         if self.excluded_columns:
-            train_args['EXCLUDE_COLS'] = ' '.join(self.excluded_columns)
+            train_args["EXCLUDE_COLS"] = " ".join(self.excluded_columns)
         if fit_params:
-            train_args['FIT_PARAMS'] = json.dumps(fit_params)
+            train_args["FIT_PARAMS"] = json.dumps(fit_params)
         if self.dependencies:
-            train_args['DEPENDENCIES'] = ' '.join(self.dependencies)
+            train_args["DEPENDENCIES"] = " ".join(self.dependencies)
         if self.train_template_id >= 9968:
             if validation_data:
-                train_args['VALIDATION_DATA'] = validation_data
+                train_args["VALIDATION_DATA"] = validation_data
             if n_jobs:
-                train_args['N_JOBS'] = n_jobs
+                train_args["N_JOBS"] = n_jobs
 
         if HAS_SKLEARN and isinstance(self.model, BaseEstimator):
             try:
                 tempdir = tempfile.mkdtemp()
-                fout = os.path.join(tempdir, 'estimator.pkl')
+                fout = os.path.join(tempdir, "estimator.pkl")
                 joblib.dump(self.model, fout, compress=3)
-                with open(fout, 'rb') as _fout:
+                with open(fout, "rb") as _fout:
                     n = self.model_name if self.model_name else "CivisML"
                     estimator_file_id = cio.file_to_civis(
-                        _fout, 'Estimator for ' + n, client=self._client)
+                        _fout, "Estimator for " + n, client=self._client
+                    )
                 self._input_model = self.model  # Keep the estimator
                 self.model = str(estimator_file_id)
             finally:
                 shutil.rmtree(tempdir)
-        train_args['MODEL'] = self.model
+        train_args["MODEL"] = self.model
 
         if HAS_SKLEARN and self.train_template_id >= 9968:
             if isinstance(self.etl, BaseEstimator):
                 try:
                     tempdir = tempfile.mkdtemp()
-                    fout = os.path.join(tempdir, 'ETL.pkl')
+                    fout = os.path.join(tempdir, "ETL.pkl")
                     joblib.dump(self.etl, fout, compress=3)
-                    with open(fout, 'rb') as _fout:
+                    with open(fout, "rb") as _fout:
                         etl_file_id = cio.file_to_civis(
-                            _fout, 'ETL Estimator', client=self._client)
-                    train_args['ETL'] = str(etl_file_id)
+                            _fout, "ETL Estimator", client=self._client
+                        )
+                    train_args["ETL"] = str(etl_file_id)
                 finally:
                     shutil.rmtree(tempdir)
 
-        name = self.model_name + ' Train' if self.model_name else None
+        name = self.model_name + " Train" if self.model_name else None
         # Clear the existing training result so we can make a new one.
         self.train_result_ = None
 
         result, container, run = self._create_custom_run(
             self.train_template_id,
             job_name=name,
             table_name=table_name,
             database_name=database_name,
             file_id=file_id,
             args=train_args,
             resources=self.job_resources,
-            polling_interval=polling_interval)
+            polling_interval=polling_interval,
+        )
 
         self.train_result_ = result
 
         return result
 
-    def _create_custom_run(self, template_id, job_name=None, table_name=None,
-                           database_name=None, file_id=None, args=None,
-                           resources=None, polling_interval=None):
+    def _create_custom_run(
+        self,
+        template_id,
+        job_name=None,
+        table_name=None,
+        database_name=None,
+        file_id=None,
+        args=None,
+        resources=None,
+        polling_interval=None,
+    ):
         # Handle int-like but non-Python-integer types such as np.int64
         file_id = int(file_id) if file_id is not None else file_id
-        script_arguments = {'TABLE_NAME': table_name,
-                            'CIVIS_FILE_ID': file_id,
-                            'DEBUG': self.verbose}
+        script_arguments = {
+            "TABLE_NAME": table_name,
+            "CIVIS_FILE_ID": file_id,
+            "DEBUG": self.verbose,
+        }
         if database_name:
             if template_id < 8000:
                 # v0 jobs used a different database parameter
-                script_arguments['DB_NAME'] = database_name
+                script_arguments["DB_NAME"] = database_name
             else:
                 db_id = self._client.get_database_id(database_name)
-                script_arguments['DB'] = {'database': db_id}
+                script_arguments["DB"] = {"database": db_id}
         resources = resources or {}
         for key, value in resources.items():
             if value:
                 # Default resources are set on the template. Only
                 # modify via arguments if users give a non-default value.
                 script_arguments[key] = value
         if self.git_token_name:
-            creds = find(self._client.credentials.list(),
-                         name=self.git_token_name,
-                         type='Custom')
+            creds = find(
+                self._client.credentials.list(), name=self.git_token_name, type="Custom"
+            )
             if len(creds) > 1:
-                raise ValueError("Unique credential with name '{}' for "
-                                 "remote git hosting service not found!"
-                                 .format(self.git_token_name))
-            script_arguments['GIT_CRED'] = creds[0].id
+                raise ValueError(
+                    "Unique credential with name '{}' for "
+                    "remote git hosting service not found!".format(self.git_token_name)
+                )
+            script_arguments["GIT_CRED"] = creds[0].id
 
         script_arguments.update(args or {})
 
         container = self._client.scripts.post_custom(
             from_template_id=template_id,
             name=job_name,
             arguments=script_arguments,
-            notifications=self.notifications)
-        log.info('Created custom script %s.', container.id)
+            notifications=self.notifications,
+        )
+        log.info("Created custom script %s.", container.id)
 
         run = self._client.scripts.post_custom_runs(container.id)
-        log.debug('Started job %s, run %s.', container.id, run.id)
+        log.debug("Started job %s, run %s.", container.id, run.id)
 
         train_kwargs = {}
         if self.train_result_ is not None:
-            train_kwargs = {'train_job_id': self.train_result_.job_id,
-                            'train_run_id': self.train_result_.run_id}
+            train_kwargs = {
+                "train_job_id": self.train_result_.job_id,
+                "train_run_id": self.train_result_.run_id,
+            }
         fut = ModelFuture(
             container.id,
             run.id,
             client=self._client,
             polling_interval=polling_interval,
             poll_on_creation=False,
-            **train_kwargs)
+            **train_kwargs,
+        )
 
         return fut, container, run
 
     @property
     @_check_fit_initiated
     def state(self):
         return self.train_result_.state
 
     @property
     @_check_fit_initiated
     def estimator(self):
         return self.train_result_.estimator
 
     @_check_fit_initiated
-    def predict(self, df=None, csv_path=None,
-                table_name=None, database_name=None,
-                manifest=None, file_id=None, sql_where=None, sql_limit=None,
-                primary_key=SENTINEL, output_table=None, output_db=None,
-                if_exists='fail', n_jobs=None, polling_interval=None,
-                cpu=None, memory=None, disk_space=None,
-                dvs_to_predict=None):
+    def predict(
+        self,
+        df=None,
+        csv_path=None,
+        table_name=None,
+        database_name=None,
+        manifest=None,
+        file_id=None,
+        sql_where=None,
+        sql_limit=None,
+        primary_key=SENTINEL,
+        output_table=None,
+        output_db=None,
+        if_exists="fail",
+        n_jobs=None,
+        polling_interval=None,
+        cpu=None,
+        memory=None,
+        disk_space=None,
+        dvs_to_predict=None,
+    ):
         """Make predictions on a trained model
 
         Provide input through one of
         a :class:`~pandas.DataFrame` (``df``),
         a local CSV (``csv_path``),
         a Civis Table (``table_name`` and ``database_name``),
         a Civis File containing a CSV (``file_id``), or
@@ -1395,71 +1593,88 @@
 
         Returns
         -------
         :class:`~civis.ml.ModelFuture`
         """
         self.train_result_.result()  # Blocks and raises training errors
 
-        if ((table_name is None or database_name is None) and
-                file_id is None and df is None and csv_path is None and
-                manifest is None):
-            raise ValueError('Provide a source of data.')
-        if sum((bool(table_name and database_name) or (manifest is not None),
-                bool(file_id), df is not None, csv_path is not None)) > 1:
-            raise ValueError('Provide a single source of data.')
+        if (
+            (table_name is None or database_name is None)
+            and file_id is None
+            and df is None
+            and csv_path is None
+            and manifest is None
+        ):
+            raise ValueError("Provide a source of data.")
+        if (
+            sum(
+                (
+                    bool(table_name and database_name) or (manifest is not None),
+                    bool(file_id),
+                    df is not None,
+                    csv_path is not None,
+                )
+            )
+            > 1
+        ):
+            raise ValueError("Provide a single source of data.")
 
         if df is not None:
-            file_id = _stash_local_dataframe(df, self.predict_template_id,
-                                             client=self._client)
+            file_id = _stash_local_dataframe(
+                df, self.predict_template_id, client=self._client
+            )
         elif csv_path:
             file_id = _stash_local_file(csv_path, client=self._client)
 
         if primary_key is SENTINEL:
             primary_key = self.primary_key
 
-        predict_args = {'TRAIN_JOB': self.train_result_.job_id,
-                        'TRAIN_RUN': self.train_result_.run_id,
-                        'PRIMARY_KEY': primary_key,
-                        'IF_EXISTS': if_exists}
+        predict_args = {
+            "TRAIN_JOB": self.train_result_.job_id,
+            "TRAIN_RUN": self.train_result_.run_id,
+            "PRIMARY_KEY": primary_key,
+            "IF_EXISTS": if_exists,
+        }
         if output_table:
-            predict_args['OUTPUT_TABLE'] = output_table
+            predict_args["OUTPUT_TABLE"] = output_table
         if output_db:
             if self.predict_template_id == 7021:
                 # v0 jobs used a different database parameter
-                predict_args['OUTPUT_DB'] = output_db
+                predict_args["OUTPUT_DB"] = output_db
             else:
                 output_db_id = self._client.get_database_id(output_db)
-                predict_args['OUTPUT_DB'] = {'database': output_db_id}
+                predict_args["OUTPUT_DB"] = {"database": output_db_id}
 
         if manifest:
-            predict_args['MANIFEST'] = manifest
+            predict_args["MANIFEST"] = manifest
         if sql_where:
-            predict_args['WHERESQL'] = sql_where
+            predict_args["WHERESQL"] = sql_where
         if sql_limit:
-            predict_args['LIMITSQL'] = sql_limit
+            predict_args["LIMITSQL"] = sql_limit
         if n_jobs:
-            predict_args['N_JOBS'] = n_jobs
+            predict_args["N_JOBS"] = n_jobs
         if dvs_to_predict:
-            if isinstance(dvs_to_predict, six.string_types):
+            if isinstance(dvs_to_predict, str):
                 dvs_to_predict = [dvs_to_predict]
             if self.predict_template_id > 10583:
                 # This feature was added in v2.2; 10583 is the v2.1 template
-                predict_args['TARGET_COLUMN'] = ' '.join(dvs_to_predict)
+                predict_args["TARGET_COLUMN"] = " ".join(dvs_to_predict)
         if self.predict_template_id >= 9969:
             if cpu:
-                predict_args['CPU'] = cpu
+                predict_args["CPU"] = cpu
             if memory:
-                predict_args['MEMORY'] = memory
+                predict_args["MEMORY"] = memory
             if disk_space:
-                predict_args['DISK_SPACE'] = disk_space
+                predict_args["DISK_SPACE"] = disk_space
 
-        name = self.model_name + ' Predict' if self.model_name else None
+        name = self.model_name + " Predict" if self.model_name else None
         result, container, run = self._create_custom_run(
             self.predict_template_id,
             job_name=name,
             table_name=table_name,
             database_name=database_name,
             file_id=file_id,
             args=predict_args,
-            polling_interval=polling_interval)
+            polling_interval=polling_interval,
+        )
 
         return result
```

### Comparing `civis-1.9.4/civis/run_joblib_func.py` & `civis-2.0.0/src/civis/run_joblib_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,55 +3,76 @@
 for the Civis platform. It takes a Civis File ID representing
 a callable serialized by either ``pickle`` or ``cloudpickle``
 as an argument, downloads the file,
 deserializes it, calls the callable, serializes the result,
 and uploads the result to another Civis File. The output file's ID
 will be set as an output on this run.
 """
-from __future__ import absolute_import, print_function
 
 from datetime import datetime, timedelta
 from io import BytesIO
 import os
-import pickle
+import pickle  # nosec
 import sys
+import warnings
 
 import civis
 import cloudpickle
-from joblib.my_exceptions import TransportableException
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore", DeprecationWarning)
+    from joblib.my_exceptions import TransportableException
+
 from joblib.format_stack import format_exc
 from joblib import parallel_backend as _joblib_para_backend
 
 try:
-    from sklearn.externals.joblib import (
-        parallel_backend as _sklearn_para_backend)
-    NO_SKLEARN = False
+    with warnings.catch_warnings():
+        # Ignore the warning: "DeprecationWarning: sklearn.externals.joblib is
+        # deprecated in 0.21 and will be removed in 0.23. Please import this
+        # functionality directly from joblib, which can be installed with:
+        # pip install joblib. If this warning is raised when loading pickled
+        # models, you may need to re-serialize those models with
+        # scikit-learn 0.21+."
+        warnings.simplefilter("ignore", DeprecationWarning)
+        # sklearn 0.22 has switched from DeprecationWarning to FutureWarning
+        warnings.simplefilter("ignore", FutureWarning)
+        from sklearn.externals.joblib import parallel_backend as _sklearn_para_backend
+
+        # NO_SKLEARN_BACKEND would be a better name here since it'll be true
+        # for future scikit-learn versions that won't include the joblib
+        # module as well as when scikit-learn isn't installed, but changing
+        # the name would technically be a breaking change.
+        NO_SKLEARN = False
 except ImportError:
     NO_SKLEARN = True
 
 from civis.parallel import (
-    _robust_pickle_download, _robust_file_to_civis, _setup_remote_backend)
+    _robust_pickle_download,
+    _robust_file_to_civis,
+    _setup_remote_backend,
+)
 
 
 def worker_func(func_file_id):
     # Have the output File expire in 7 days.
     expires_at = (datetime.now() + timedelta(days=7)).isoformat()
 
     client = civis.APIClient()
-    job_id = os.environ.get('CIVIS_JOB_ID')
-    run_id = os.environ.get('CIVIS_RUN_ID')
+    job_id = os.environ.get("CIVIS_JOB_ID")
+    run_id = os.environ.get("CIVIS_RUN_ID")
     if not job_id or not run_id:
-        raise RuntimeError("This function must be run inside a "
-                           "Civis container job.")
+        raise RuntimeError("This function must be run inside a " "Civis container job.")
 
     # Run the function.
     result = None
     try:
         func, remote_backend = _robust_pickle_download(
-            func_file_id, client=client, n_retries=5, delay=0.5)
+            func_file_id, client=client, n_retries=5, delay=0.5
+        )
 
         _backend = _setup_remote_backend(remote_backend)
 
         # graceful nested context managers are ~hard across python versions,
         # this just works...
         if NO_SKLEARN:
             with _joblib_para_backend(_backend):
@@ -78,31 +99,34 @@
     finally:
         # Serialize the result and upload it to the Files API.
         if result is not None:
             # If the function exits without erroring, we may not have a result.
             result_buffer = BytesIO()
             cloudpickle.dump(result, result_buffer, pickle.HIGHEST_PROTOCOL)
             result_buffer.seek(0)
-            output_name = "Results from Joblib job {} / run {}".format(job_id,
-                                                                       run_id)
-            output_file_id = _robust_file_to_civis(result_buffer, output_name,
-                                                   n_retries=5, delay=0.5,
-                                                   expires_at=expires_at,
-                                                   client=client)
-            client.scripts.post_containers_runs_outputs(job_id, run_id,
-                                                        'File', output_file_id)
-            print("Results output to file ID: {}".format(output_name,
-                                                         output_file_id))
+            output_name = "Results from Joblib job {} / run {}".format(job_id, run_id)
+            output_file_id = _robust_file_to_civis(
+                result_buffer,
+                output_name,
+                n_retries=5,
+                delay=0.5,
+                expires_at=expires_at,
+                client=client,
+            )
+            client.scripts.post_containers_runs_outputs(
+                job_id, run_id, "File", output_file_id
+            )
+            print("Results output to file ID: {}".format(output_file_id))
 
 
 def main():
     if len(sys.argv) > 1:
         func_file_id = sys.argv[1]
     else:
         # If the file ID to download isn't given as a command-line
         # argument, assume that it's in an environment variable.
-        func_file_id = os.environ['JOBLIB_FUNC_FILE_ID']
+        func_file_id = os.environ["JOBLIB_FUNC_FILE_ID"]
     worker_func(func_file_id=func_file_id)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `civis-1.9.4/civis/polling.py` & `civis-2.0.0/src/civis/polling.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-from __future__ import absolute_import
-from builtins import super
-
 import time
 import threading
 
 from civis.base import CivisJobFailure, CivisAsyncResultBase, FAILED, DONE
 from civis.response import Response
 
 
 _DEFAULT_POLLING_INTERVAL = 15
 
 
 class _ResultPollingThread(threading.Thread):
-    """Poll a function until it returns a Response with a DONE state
-    """
+    """Poll a function until it returns a Response with a DONE state"""
+
     # Inspired by `threading.Timer`
 
     def __init__(self, poller, poller_args, polling_interval):
-        super().__init__()
+        super().__init__(daemon=True)
         self.polling_interval = polling_interval
         self.poller = poller
         self.poller_args = poller_args
         self.finished = threading.Event()
 
     def cancel(self):
-        """Stop the poller if it hasn't finished yet.
-        """
+        """Stop the poller if it hasn't finished yet."""
         self.finished.set()
 
     def join(self, timeout=None):
-        """Shut down the polling when the thread is terminated.
-        """
+        """Shut down the polling when the thread is terminated."""
         self.cancel()
         super().join(timeout=timeout)
 
     def run(self):
-        """Poll until done.
-        """
+        """Poll until done."""
         while not self.finished.wait(self.polling_interval):
-            if self.poller(*self.poller_args).state in DONE:
+            # Spotty internet connectivity can result in polling functions
+            # returning None. This treats None responses like responses which
+            # have a non-DONE state.
+            poller_result = self.poller(*self.poller_args)
+            if poller_result is not None and poller_result.state in DONE:
                 self.finished.set()
 
 
 class PollableResult(CivisAsyncResultBase):
     """A class for tracking pollable results.
 
     This class will begin polling immediately upon creation, and poll for
@@ -54,17 +52,14 @@
     poller : func
         A function which returns an object that has a ``state`` attribute.
     poller_args : tuple
         The arguments with which to call the poller function.
     polling_interval : int or float
         The number of seconds between API requests to check whether a result
         is ready.
-    api_key : DEPRECATED str, optional
-        This is not used by PollableResult, but is required to match the
-        interface from CivisAsyncResultBase.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     poll_on_creation : bool, optional
         If ``True`` (the default), it will poll upon calling ``result()`` the
         first time. If ``False``, it will wait the number of seconds specified
         in `polling_interval` from object creation before polling.
@@ -81,39 +76,46 @@
     >>> job_id = response.id
     >>>
     >>> poller = client.queries.get
     >>> poller_args = (job_id, ) # (job_id, run_id) if poller requires run_id
     >>> polling_interval = 10
     >>> poll = PollableResult(poller, poller_args, polling_interval)
     """
+
     # this may not be friendly to a rate-limited api
     # Implementation notes: The `PollableResult` depends on some private
     # features of the `concurrent.futures.Future` class, so it's possible
     # that future versions of Python could break something here.
-    # (It works under at least 3.4, 3.5, and 3.6)
+    # (It works under at least 3.6)
     # We use the following `Future` implementation details
     # - The `Future` checks its state against predefined strings. We use
     #   `STATE_TRANS` to translate from the Civis platform states to `Future`
     #    states.
     # - `Future` uses a `_state` attribute to check its current condition
     # - `Future` handles event notification through `set_result` and
     #   `set_exception`, which we call from `_check_result`.
     # - We use the `Future` thread lock called `_condition`
     # - We assume that results of the Future are stored in `_result`.
-    def __init__(self, poller, poller_args,
-                 polling_interval=None, api_key=None, client=None,
-                 poll_on_creation=True):
+    def __init__(
+        self,
+        poller,
+        poller_args,
+        polling_interval=None,
+        client=None,
+        poll_on_creation=True,
+    ):
         if polling_interval is None:
             polling_interval = _DEFAULT_POLLING_INTERVAL
-        super().__init__(poller=poller,
-                         poller_args=poller_args,
-                         polling_interval=polling_interval,
-                         api_key=api_key,
-                         client=client,
-                         poll_on_creation=poll_on_creation)
+        super().__init__(
+            poller=poller,
+            poller_args=poller_args,
+            polling_interval=polling_interval,
+            client=client,
+            poll_on_creation=poll_on_creation,
+        )
         if self.polling_interval <= 0:
             raise ValueError("The polling interval must be positive.")
 
         # Polling arguments. Never poll more often than the requested interval.
         if poll_on_creation:
             self._last_polled = None
         else:
@@ -121,17 +123,19 @@
         self._last_result = None
 
         self._begin_tracking()
 
     def _begin_tracking(self, start_thread=False):
         """Start monitoring the Civis Platform job"""
         with self._condition:
-            if getattr(self, 'poller', None) is None:
-                raise RuntimeError('Internal error: Must set polling '
-                                   'function before initializing thread.')
+            if getattr(self, "poller", None) is None:
+                raise RuntimeError(
+                    "Internal error: Must set polling "
+                    "function before initializing thread."
+                )
             self._reset_polling_thread(self.polling_interval, start_thread)
 
     def _check_result(self):
         """Return the job result from Civis. Once the job completes, store the
         result and never poll again."""
         with self._condition:
             # Start a single thread continuously polling.
@@ -143,16 +147,18 @@
                 # If the job is already completed, just return the stored
                 # result.
                 return self._result
 
             # Check to see if the job has finished, but don't poll more
             # frequently than the requested polling frequency.
             now = time.time()
-            if (not self._last_polled or
-                    (now - self._last_polled) >= self.polling_interval):
+            if (
+                not self._last_polled
+                or (now - self._last_polled) >= self.polling_interval
+            ):
                 # Poll for a new result
                 self._last_polled = now
                 try:
                     self._last_result = self.poller(*self.poller_args)
                 except Exception as e:
                     # The _poller can raise API exceptions
                     # Set those directly as this Future's exception
@@ -165,19 +171,23 @@
 
             return self._last_result
 
     def _set_api_result(self, result):
         with self._condition:
             if result.state in FAILED:
                 try:
-                    err_msg = str(result['error'])
+                    err_msg = str(result["error"])
                 except:  # NOQA
                     err_msg = str(result)
-                self._set_api_exception(exc=CivisJobFailure(err_msg, result),
-                                        result=result)
+                job_id = getattr(self, "job_id", None)
+                run_id = getattr(self, "run_id", None)
+                self._set_api_exception(
+                    exc=CivisJobFailure(err_msg, result, job_id, run_id),
+                    result=result,
+                )
             elif result.state in DONE:
                 self.set_result(result)
                 self.cleanup()
 
     def _set_api_exception(self, exc, result=None):
         with self._condition:
             if result is None:
@@ -190,19 +200,22 @@
     def cleanup(self):
         # This gets called after the result is set.
         # Ensure that the polling thread shuts down when it's no longer needed.
         with self._condition:
             if self._polling_thread.is_alive():
                 self._polling_thread.cancel()
 
-    def _reset_polling_thread(self,
-                              polling_interval=_DEFAULT_POLLING_INTERVAL,
-                              start_thread=False):
-        with self._condition:
-            if (getattr(self, '_polling_thread', None) is not None and
-                    self._polling_thread.is_alive()):
+    def _reset_polling_thread(
+        self, polling_interval=_DEFAULT_POLLING_INTERVAL, start_thread=False
+    ):
+        with self._condition:
+            if (
+                getattr(self, "_polling_thread", None) is not None
+                and self._polling_thread.is_alive()
+            ):
                 self._polling_thread.cancel()
             self.polling_interval = polling_interval
-            self._polling_thread = _ResultPollingThread(self._check_result, (),
-                                                        polling_interval)
+            self._polling_thread = _ResultPollingThread(
+                self._check_result, (), polling_interval
+            )
             if start_thread:
                 self._polling_thread.start()
```

### Comparing `civis-1.9.4/civis/parallel.py` & `civis-2.0.0/src/civis/parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,90 @@
-"""Parallel computations using the Civis Platform infrastructure
-"""
-from __future__ import absolute_import
+"""Parallel computations using the Civis Platform infrastructure"""
 
 from concurrent.futures import wait
 from datetime import datetime, timedelta
 from io import BytesIO
 import logging
 import os
-import pickle
+import pickle  # nosec
+from tempfile import TemporaryDirectory
 import time
+import warnings
 
 import cloudpickle
 from joblib._parallel_backends import ParallelBackendBase
-from joblib.my_exceptions import TransportableException
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore", DeprecationWarning)
+    from joblib.my_exceptions import TransportableException
+
 from joblib import register_parallel_backend as _joblib_reg_para_backend
 import requests
 
 import civis
 from civis.base import CivisAPIError
-
-from civis.compat import TemporaryDirectory
 from civis.futures import _ContainerShellExecutor, CustomScriptExecutor
 
 try:
-    from sklearn.externals.joblib import (
-        register_parallel_backend as _sklearn_reg_para_backend)
-    NO_SKLEARN = False
+    with warnings.catch_warnings():
+        # Ignore the warning: "DeprecationWarning: sklearn.externals.joblib is
+        # deprecated in 0.21 and will be removed in 0.23. Please import this
+        # functionality directly from joblib, which can be installed with:
+        # pip install joblib. If this warning is raised when loading pickled
+        # models, you may need to re-serialize those models with
+        # scikit-learn 0.21+."
+        warnings.simplefilter("ignore", DeprecationWarning)
+        # sklearn 0.22 has switched from DeprecationWarning to FutureWarning
+        warnings.simplefilter("ignore", FutureWarning)
+        from sklearn.externals.joblib import (
+            register_parallel_backend as _sklearn_reg_para_backend,
+        )
+
+        # NO_SKLEARN_BACKEND would be a better name here since it'll be true
+        # for future scikit-learn versions that won't include the joblib
+        # module as well as when scikit-learn isn't installed, but changing
+        # the name would technically be a breaking change.
+        NO_SKLEARN = False
 except ImportError:
     NO_SKLEARN = True
+    _sklearn_reg_para_backend = None
 
 log = logging.getLogger(__name__)
 _THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 _DEFAULT_SETUP_CMD = ":"  # An sh command that does nothing.
-_DEFAULT_REPO_SETUP_CMD = "cd /app; python setup.py install; cd /"
+_DEFAULT_REPO_SETUP_CMD = "cd /app; pip install .; cd /"
 _ALL_JOBS = 50  # Give the user this many jobs if they request "all of them"
 
 # When creating a remote execution environment from an existing
 # Container Script, read these keys.
-KEYS_TO_INFER = ['docker_image_name', 'docker_image_tag', 'repo_http_uri',
-                 'repo_ref', 'remote_host_credential_id', 'git_credential_id',
-                 'cancel_timeout', 'time_zone']
-
-
-def infer_backend_factory(required_resources=None,
-                          params=None,
-                          arguments=None,
-                          client=None,
-                          polling_interval=None,
-                          setup_cmd=None,
-                          max_submit_retries=0,
-                          max_job_retries=0,
-                          hidden=True,
-                          remote_backend='sequential',
-                          **kwargs):
+KEYS_TO_INFER = [
+    "docker_image_name",
+    "docker_image_tag",
+    "repo_http_uri",
+    "repo_ref",
+    "remote_host_credential_id",
+    "git_credential_id",
+    "cancel_timeout",
+    "time_zone",
+]
+
+
+def infer_backend_factory(
+    required_resources=None,
+    params=None,
+    arguments=None,
+    client=None,
+    polling_interval=None,
+    setup_cmd=None,
+    max_submit_retries=0,
+    max_job_retries=0,
+    hidden=True,
+    remote_backend="sequential",
+    **kwargs,
+):
     """Infer the container environment and return a backend factory.
 
     This function helps you run additional jobs from code which executes
     inside a Civis container job. The function reads settings for
     relevant parameters (e.g. the Docker image) of the container
     it's running inside of.
 
@@ -105,26 +133,25 @@
         arguments.
     client : `civis.APIClient` instance or None, optional
         An API Client object to use.
     polling_interval : int, optional
         The polling interval, in seconds, for checking container script status.
         If you have many jobs, you may want to set this higher (e.g., 300) to
         avoid `rate-limiting <https://platform.civisanalytics.com/api#basics>`.
-        You should only set this if you aren't using ``pubnub`` notifications.
     setup_cmd : str, optional
         A shell command or sequence of commands for setting up the environment.
         These will precede the commands used to run functions in joblib.
         This is primarily for installing dependencies that are not available
-        in the dockerhub repo (e.g., "cd /app && python setup.py install"
+        in the dockerhub repo (e.g., "cd /app && pip install ."
         or "pip install gensim").
 
         With no GitHub repo input, the setup command will
         default to a command that does nothing. If a ``repo_http_uri``
         is provided, the default setup command will attempt to run
-        "python setup.py install". If this command fails, execution
+        "pip install .". If this command fails, execution
         will still continue.
     max_submit_retries : int, optional
         The maximum number of retries for submitting each job. This is to help
         avoid a large set of jobs failing because of a single 5xx error. A
         value higher than zero should only be used for jobs that are idempotent
         (i.e., jobs whose result and side effects are the same regardless of
         whether they are run once or many times).
@@ -160,83 +187,96 @@
     See Also
     --------
     civis.parallel.make_backend_factory
     """
     if client is None:
         client = civis.APIClient()
 
-    if not os.environ.get('CIVIS_JOB_ID'):
-        raise RuntimeError('This function must be run '
-                           'inside a container job.')
-    state = client.scripts.get_containers(os.environ['CIVIS_JOB_ID'])
+    if not os.environ.get("CIVIS_JOB_ID"):
+        raise RuntimeError("This function must be run " "inside a container job.")
+    state = client.scripts.get_containers(os.environ["CIVIS_JOB_ID"])
     if state.from_template_id:
         # If this is a Custom Script from a template, we need the
         # backing script. Make sure to save the arguments from
         # the Custom Script: those are the only user-settable parts.
         template = client.templates.get_scripts(state.from_template_id)
         try:
             custom_args = state.arguments
             state = client.scripts.get_containers(template.script_id)
-            state.arguments = custom_args
+            state._replace("arguments", custom_args)
         except civis.base.CivisAPIError as err:
             if err.status_code == 404:
-                raise RuntimeError('Unable to introspect environment from '
-                                   'your template\'s backing script. '
-                                   'You may not have permission to view '
-                                   'script ID {}.'.format(template.script_id))
+                raise RuntimeError(
+                    "Unable to introspect environment from "
+                    "your template's backing script. "
+                    "You may not have permission to view "
+                    "script ID {}.".format(template.script_id)
+                )
             else:
                 raise
 
     # Default to this container's resource requests, but
     # allow users to override it.
-    state.required_resources.update(required_resources or {})
+    state.required_resources._data_snake.update(required_resources or {})
 
     # Update parameters with user input
     params = params or []
     for input_param in params:
-        for param in state.params:
-            if param['name'] == input_param['name']:
-                param.update(input_param)
+        for i, param in enumerate(list(state.params)):
+            if param["name"] == input_param["name"]:
+                param._data_snake.update(input_param)
                 break
         else:
-            state.params.append(input_param)
+            state._data_snake["params"].append(input_param)
 
     # Update arguments with input
-    state.arguments.update(arguments or {})
+    state.arguments._data_snake.update(arguments or {})
 
     # Set defaults on other keyword arguments with
     # values from the current script
     for key in KEYS_TO_INFER:
         kwargs.setdefault(key, state[key])
 
-    return make_backend_factory(required_resources=state.required_resources,
-                                params=state.params,
-                                arguments=state.arguments,
-                                client=client,
-                                polling_interval=polling_interval,
-                                setup_cmd=setup_cmd,
-                                max_submit_retries=max_submit_retries,
-                                max_job_retries=max_job_retries,
-                                hidden=hidden,
-                                remote_backend=remote_backend,
-                                **kwargs)
+    # Don't include parent job params since they're added automatically
+    # in _ContainerShellExecutor.__init__.
+    filtered_params = [
+        p
+        for p in state.params
+        if p["name"].upper() not in ("CIVIS_PARENT_JOB_ID", "CIVIS_PARENT_RUN_ID")
+    ]
+
+    return make_backend_factory(
+        required_resources=state.required_resources,
+        params=filtered_params,
+        arguments=state.arguments,
+        client=client,
+        polling_interval=polling_interval,
+        setup_cmd=setup_cmd,
+        max_submit_retries=max_submit_retries,
+        max_job_retries=max_job_retries,
+        hidden=hidden,
+        remote_backend=remote_backend,
+        **kwargs,
+    )
 
 
 infer_backend_factory.__doc__ = infer_backend_factory.__doc__ % KEYS_TO_INFER
 
 
-def make_backend_factory(docker_image_name="civisanalytics/datascience-python",
-                         client=None,
-                         polling_interval=None,
-                         setup_cmd=None,
-                         max_submit_retries=0,
-                         max_job_retries=0,
-                         hidden=True,
-                         remote_backend='sequential',
-                         **kwargs):
+def make_backend_factory(
+    docker_image_name="civisanalytics/datascience-python",
+    client=None,
+    polling_interval=None,
+    setup_cmd=None,
+    max_submit_retries=0,
+    max_job_retries=0,
+    hidden=True,
+    remote_backend="sequential",
+    **kwargs,
+):
     """Create a joblib backend factory that uses Civis Container Scripts
 
     Jobs created through this backend will have environment variables
     "CIVIS_PARENT_JOB_ID" and "CIVIS_PARENT_RUN_ID" with the contents
     of the "CIVIS_JOB_ID" and "CIVIS_RUN_ID" of the environment which
     created them. If the code doesn't have "CIVIS_JOB_ID" and "CIVIS_RUN_ID"
     environment variables available, the child will not have
@@ -260,26 +300,25 @@
         a ``docker_image_tag`` in the keyword arguments.
     client : `civis.APIClient` instance or None, optional
         An API Client object to use.
     polling_interval : int, optional
         The polling interval, in seconds, for checking container script status.
         If you have many jobs, you may want to set this higher (e.g., 300) to
         avoid `rate-limiting <https://platform.civisanalytics.com/api#basics>`.
-        You should only set this if you aren't using ``pubnub`` notifications.
     setup_cmd : str, optional
         A shell command or sequence of commands for setting up the environment.
         These will precede the commands used to run functions in joblib.
         This is primarily for installing dependencies that are not available
-        in the dockerhub repo (e.g., "cd /app && python setup.py install"
+        in the dockerhub repo (e.g., "cd /app && pip install ."
         or "pip install gensim").
 
         With no GitHub repo input, the setup command will
         default to a command that does nothing. If a `repo_http_uri`
         is provided, the default setup command will attempt to run
-        "python setup.py install". If this command fails, execution
+        "pip install .". If this command fails, execution
         will still continue.
     max_submit_retries : int, optional
         The maximum number of retries for submitting each job. This is to help
         avoid a large set of jobs failing because of a single 5xx error. A
         value higher than zero should only be used for jobs that are idempotent
         (i.e., jobs whose result and side effects are the same regardless of
         whether they are run once or many times).
@@ -305,15 +344,14 @@
     **kwargs:
         Additional keyword arguments will be passed
         directly to :func:`~civis.APIClient.scripts.post_containers`.
 
     Examples
     --------
     >>> # Without joblib:
-    >>> from __future__ import print_function
     >>> from math import sqrt
     >>> print([sqrt(i ** 2) for i in range(10)])
     [0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0]
 
     >>> # Using the default joblib backend:
     >>> from joblib import delayed, Parallel
     >>> parallel = Parallel(n_jobs=5)
@@ -374,40 +412,44 @@
     module, that module must be installed in the remote environment.
 
     See Also
     --------
     civis.APIClient.scripts.post_containers
     """
     if setup_cmd is None:
-        if kwargs.get('repo_http_uri'):
+        if kwargs.get("repo_http_uri"):
             setup_cmd = _DEFAULT_REPO_SETUP_CMD
         else:
             setup_cmd = _DEFAULT_SETUP_CMD
 
     def backend_factory():
-        return _CivisBackend(docker_image_name=docker_image_name,
-                             client=client,
-                             polling_interval=polling_interval,
-                             setup_cmd=setup_cmd,
-                             max_submit_retries=max_submit_retries,
-                             max_n_retries=max_job_retries,
-                             hidden=hidden,
-                             remote_backend=remote_backend,
-                             **kwargs)
+        return _CivisBackend(
+            docker_image_name=docker_image_name,
+            client=client,
+            polling_interval=polling_interval,
+            setup_cmd=setup_cmd,
+            max_submit_retries=max_submit_retries,
+            max_n_retries=max_job_retries,
+            hidden=hidden,
+            remote_backend=remote_backend,
+            **kwargs,
+        )
 
     return backend_factory
 
 
-def make_backend_template_factory(from_template_id,
-                                  arguments=None,
-                                  client=None,
-                                  polling_interval=None,
-                                  max_submit_retries=0,
-                                  max_job_retries=0,
-                                  hidden=True):
+def make_backend_template_factory(
+    from_template_id,
+    arguments=None,
+    client=None,
+    polling_interval=None,
+    max_submit_retries=0,
+    max_job_retries=0,
+    hidden=True,
+):
     """Create a joblib backend factory that uses Civis Custom Scripts.
 
     If your template has settable parameters "CIVIS_PARENT_JOB_ID" and
     "CIVIS_PARENT_RUN_ID", then this executor will fill them with the contents
     of the "CIVIS_JOB_ID" and "CIVIS_RUN_ID" of the environment which
     created them. If the code doesn't have "CIVIS_JOB_ID" and "CIVIS_RUN_ID"
     environment variables available, the child will not have
@@ -428,15 +470,14 @@
         for details.
     client : `civis.APIClient` instance or None, optional
         An API Client object to use.
     polling_interval : int, optional
         The polling interval, in seconds, for checking container script status.
         If you have many jobs, you may want to set this higher (e.g., 300) to
         avoid `rate-limiting <https://platform.civisanalytics.com/api#basics>`.
-        You should only set this if you aren't using ``pubnub`` notifications.
     max_submit_retries : int, optional
         The maximum number of retries for submitting each job. This is to help
         avoid a large set of jobs failing because of a single 5xx error. A
         value higher than zero should only be used for jobs that are idempotent
         (i.e., jobs whose result and side effects are the same regardless of
         whether they are run once or many times).
     max_job_retries : int, optional
@@ -447,32 +488,34 @@
         These retries assist with jobs which may have failed because
         of network or worker failures.
     hidden: bool, optional
         The hidden status of the object. Setting this to true
         hides it from most API endpoints. The object can still
         be queried directly by ID. Defaults to True.
     """
+
     def backend_factory():
-        return _CivisBackend(from_template_id=from_template_id,
-                             arguments=arguments,
-                             client=client,
-                             polling_interval=polling_interval,
-                             max_submit_retries=max_submit_retries,
-                             max_n_retries=max_job_retries,
-                             hidden=hidden)
+        return _CivisBackend(
+            from_template_id=from_template_id,
+            arguments=arguments,
+            client=client,
+            polling_interval=polling_interval,
+            max_submit_retries=max_submit_retries,
+            max_n_retries=max_job_retries,
+            hidden=hidden,
+        )
 
     return backend_factory
 
 
 class JobSubmissionError(Exception):
     pass
 
 
-def _robust_pickle_download(output_file_id, client=None,
-                            n_retries=5, delay=0.0):
+def _robust_pickle_download(output_file_id, client=None, n_retries=5, delay=0.0):
     """Download and deserialize the result from output_file_id
 
     Retry network errors `n_retries` times with `delay` seconds between calls
 
     Parameters
     ----------
     output_file_id : int
@@ -490,38 +533,36 @@
         downloaded file
 
     See Also
     --------
     cloudpickle.load
     """
     client = client or civis.APIClient()
-    retry_exc = (requests.HTTPError,
-                 requests.ConnectionError,
-                 requests.ConnectTimeout)
+    retry_exc = (requests.HTTPError, requests.ConnectionError, requests.ConnectTimeout)
     n_failed = 0
     while True:
         buffer = BytesIO()
         try:
             civis.io.civis_to_file(output_file_id, buffer, client=client)
         except retry_exc as exc:
             buffer.close()
             if n_failed < n_retries:
                 n_failed += 1
-                log.debug("Download failure %s due to %s; retrying.",
-                          n_failed, str(exc))
+                log.debug(
+                    "Download failure %s due to %s; retrying.", n_failed, str(exc)
+                )
                 time.sleep(delay)
             else:
                 raise
         else:
             buffer.seek(0)
             return cloudpickle.load(buffer)
 
 
-def _robust_file_to_civis(buf, name, client=None, n_retries=5,
-                          delay=0.0, **kwargs):
+def _robust_file_to_civis(buf, name, client=None, n_retries=5, delay=0.0, **kwargs):
     """Upload the contents of an input file-like buffer
 
     Call :func:`~civis.io.file_to_civis`, and retry a specified
     number of times before giving up. This will abandon
     Civis files created for failed uploads. Thoase files may
     be partially filled; it's necessary to create new files
     to ensure that the contents are exactly as requested.
@@ -549,28 +590,24 @@
         ID of the new Civis File
 
     See Also
     --------
     civis.io.file_to_civis
     """
     client = client or civis.APIClient()
-    retry_exc = (requests.HTTPError,
-                 requests.ConnectionError,
-                 requests.ConnectTimeout)
+    retry_exc = (requests.HTTPError, requests.ConnectionError, requests.ConnectTimeout)
     n_failed = 0
     while True:
         buf.seek(0)
         try:
-            file_id = civis.io.file_to_civis(buf, name=name,
-                                             client=client, **kwargs)
+            file_id = civis.io.file_to_civis(buf, name=name, client=client, **kwargs)
         except retry_exc as exc:
             if n_failed < n_retries:
                 n_failed += 1
-                log.debug("Upload failure %s due to %s; retrying.",
-                          n_failed, str(exc))
+                log.debug("Upload failure %s due to %s; retrying.", n_failed, str(exc))
                 time.sleep(delay)
             else:
                 raise
         else:
             return file_id
 
 
@@ -585,32 +622,34 @@
 
     Returns
     -------
     backend : str
         The name of the backend to use.
     """
     if isinstance(remote_backend, _CivisBackend):
+
         def backend_factory():
             return _CivisBackend.from_existing(remote_backend)
+
         # joblib and global state: fun!
         #
         # joblib internally maintains a global list of backends and
         # specifically tracks which backend is currently in use. Further,
         # sklearn ships its own COPY of the entire joblib package at
         # `sklearn.externals.joblib`. Thus there are TWO copies of joblib
         # in use (the joblib package and the one in sklearn) and thus different
         # global states that need to be handeled. Whew.
         #
         # Therefore, we have to register our backend with both copies in order
         # to allow our containers to run `Parallel` objects from both copies
         # of joblib. Yay!
-        _joblib_reg_para_backend('civis', backend_factory)
+        _joblib_reg_para_backend("civis", backend_factory)
         if not NO_SKLEARN:
-            _sklearn_reg_para_backend('civis', backend_factory)
-        return 'civis'
+            _sklearn_reg_para_backend("civis", backend_factory)
+        return "civis"
     else:
         return remote_backend
 
 
 class _CivisBackendResult:
     """A wrapper for results of joblib tasks
 
@@ -635,36 +674,39 @@
     * This is similar to a Future object except with ``get`` instead of
       ``result``, and with a callback specified.
     * This is only intended to work within joblib and with the Civis backend.
     * Joblib calls ``get`` on one result at a time, in order of submission.
     * Exceptions should only be raised inside ``get`` so that joblib can
         handle them properly.
     """
+
     def __init__(self, future, callback):
         self._future = future
         self._callback = callback
         self.result = None
-        if hasattr(future, 'client'):
+        if hasattr(future, "client"):
             self._client = future.client
         else:
             self._client = civis.APIClient()
 
         # Download results and trigger the next job as a callback
         # so that we don't have to wait for `get` to be called.
         # Note that the callback of a `concurrent.futures.Future`
         # (which self._future is a subclass of) is called with a
         # single argument, the Future itself.
         self._future.remote_func_output = None  # `get` reads results from here
         self._future.result_fetched = False  # Did we get the result?
         self._future.add_done_callback(
-            self._make_fetch_callback(self._callback, self._client))
+            self._make_fetch_callback(self._callback, self._client)
+        )
 
     @staticmethod
     def _make_fetch_callback(joblib_callback, client):
         """Create a closure for use as a callback on the ContainerFuture"""
+
         def _fetch_result(fut):
             """Retrieve outputs from the remote function.
             Run the joblib callback only if there were no errors.
 
             Parameters
             ----------
             fut : :class:`~civis.futures.ContainerFuture`
@@ -675,54 +717,76 @@
             ----
             We can't return data from a callback, so the remote
             function output is attached to the Future object
             as a new attribute ``remote_func_output``.
             """
             if fut.succeeded():
                 log.debug(
-                    "Ran job through Civis. Job ID: %d, run ID: %d;"
-                    " job succeeded!", fut.job_id, fut.run_id)
+                    "Ran job through Civis. Job ID: %d, run ID: %d;" " job succeeded!",
+                    fut.job_id,
+                    fut.run_id,
+                )
             elif fut.cancelled():
                 log.debug(
-                    "Ran job through Civis. Job ID: %d, run ID: %d;"
-                    " job cancelled!", fut.job_id, fut.run_id)
+                    "Ran job through Civis. Job ID: %d, run ID: %d;" " job cancelled!",
+                    fut.job_id,
+                    fut.run_id,
+                )
             else:
                 log.error(
-                    "Ran job through Civis. Job ID: %d, run ID: %d;"
-                    " job failure!", fut.job_id, fut.run_id)
+                    "Ran job through Civis. Job ID: %d, run ID: %d;" " job failure!",
+                    fut.job_id,
+                    fut.run_id,
+                )
 
             try:
                 # Find the output file ID from the run outputs.
                 run_outputs = client.scripts.list_containers_runs_outputs(
-                    fut.job_id, fut.run_id)
+                    fut.job_id, fut.run_id
+                )
                 if run_outputs:
-                    output_file_id = run_outputs[0]['object_id']
-                    res = _robust_pickle_download(output_file_id, client,
-                                                  n_retries=5, delay=1.0)
+                    output_file_id = run_outputs[0]["object_id"]
+                    res = _robust_pickle_download(
+                        output_file_id, client, n_retries=5, delay=1.0
+                    )
                     fut.remote_func_output = res
                     log.debug("Downloaded and deserialized the result.")
             except BaseException as exc:
                 # If something went wrong when fetching outputs, record the
                 # exception so we can re-raise it in the parent process.
                 # Catch BaseException so we can also re-raise a
                 # KeyboardInterrupt where it can be properly handled.
-                log.debug('Exception during result download: %s', str(exc))
+                log.debug("Exception during result download: %s", str(exc))
                 fut.remote_func_output = exc
             else:
                 fut.result_fetched = True
-                if not fut.cancelled() and not fut.exception():
+                cancelled = fut.cancelled()
+                try:
+                    # After requesting cancellation, a script stays in a
+                    # running state and sets _result.is_cancel_requested
+                    # to True to allow for clean up logic. Here, we make sure
+                    # to treat these runs the same as cancelled runs.
+                    cancelled |= fut._result.is_cancel_requested
+                except AttributeError:
+                    pass
+                if not cancelled and not fut.exception():
                     # The next job will start when this callback is called.
                     # Only run it if the job was a success.
                     joblib_callback(fut.remote_func_output)
 
         return _fetch_result
 
-    def get(self):
+    def get(self, timeout=None):
         """Block and return the result of the job
 
+        Parameters
+        ----------
+        timeout: float, optional
+            If provided, wait this many seconds before issuing a TimeoutError
+
         Returns
         -------
         The output of the function which ``joblib`` ran via Civis
             NB: ``joblib`` expects that ``get`` will always return an iterable.
         The remote function(s) should always be wrapped in
         ``joblib.parallel.BatchedCalls``, which does always return a list.
 
@@ -732,15 +796,15 @@
             Any error in the remote job will result in a
             ``TransportableException``, to be handled by ``Parallel.retrieve``.
         futures.CancelledError
             If the remote job was cancelled before completion
         """
         if self.result is None:
             # Wait for the script to complete.
-            wait([self._future])
+            wait([self._future], timeout=timeout)
             self.result = self._future.remote_func_output
 
         if self._future.exception() or not self._future.result_fetched:
             # If the job errored, we may have been able to return
             # an exception via the run outputs. If not, fall back
             # to the API exception.
             # Note that a successful job may still have an exception
@@ -757,144 +821,170 @@
 
 
 class _CivisBackend(ParallelBackendBase):
     """The backend class that tells joblib how to use Civis to run jobs
 
     Users should interact with this through ``make_backend_factory``.
     """
-    def __init__(self, setup_cmd=_DEFAULT_SETUP_CMD,
-                 from_template_id=None,
-                 max_submit_retries=0,
-                 client=None,
-                 remote_backend='sequential',
-                 **executor_kwargs):
+
+    uses_threads = False
+    supports_sharedmem = False
+    supports_timeout = True
+
+    def __init__(
+        self,
+        setup_cmd=_DEFAULT_SETUP_CMD,
+        from_template_id=None,
+        max_submit_retries=0,
+        client=None,
+        remote_backend="sequential",
+        nesting_level=0,
+        **executor_kwargs,
+    ):
         self.setup_cmd = setup_cmd
         self.from_template_id = from_template_id
         self.max_submit_retries = max_submit_retries
         self.client = client
         self.remote_backend = remote_backend
         self.executor_kwargs = executor_kwargs
+        self.nesting_level = nesting_level
         self._init_civis_backend()
 
     @classmethod
     def from_existing(cls, klass):
         """Build a new `_CivisBackend` from an existing one."""
         return cls(
             setup_cmd=klass.setup_cmd,
             from_template_id=klass.from_template_id,
             max_submit_retries=klass.max_submit_retries,
             client=klass.client,
             remote_backend=klass.remote_backend,
-            **klass.executor_kwargs)
+            **klass.executor_kwargs,
+        )
 
     def _init_civis_backend(self):
         """init the Civis API client and the executors"""
-        self.using_template = (self.from_template_id is not None)
+        self.using_template = self.from_template_id is not None
 
         if self.max_submit_retries < 0:
             raise ValueError(
-                "max_submit_retries cannot be negative (value = %d)" %
-                self.max_submit_retries)
+                "max_submit_retries cannot be negative (value = %d)"
+                % self.max_submit_retries
+            )
 
         self.client = self.client or civis.APIClient()
         if self.from_template_id:
-            self.executor = CustomScriptExecutor(self.from_template_id,
-                                                 client=self.client,
-                                                 **self.executor_kwargs)
+            self.executor = CustomScriptExecutor(
+                self.from_template_id, client=self.client, **self.executor_kwargs
+            )
         else:
-            self.executor = _ContainerShellExecutor(client=self.client,
-                                                    **self.executor_kwargs)
+            self.executor = _ContainerShellExecutor(
+                client=self.client, **self.executor_kwargs
+            )
 
     def effective_n_jobs(self, n_jobs):
+        if n_jobs is None:
+            n_jobs = 1
         if n_jobs == -1:
             n_jobs = _ALL_JOBS
         if n_jobs <= 0:
-            raise ValueError("Please request a positive number of jobs, "
-                             "or use \"-1\" to request a default "
-                             "of {} jobs.".format(_ALL_JOBS))
+            raise ValueError(
+                "Please request a positive number of jobs, "
+                'or use "-1" to request a default '
+                "of {} jobs.".format(_ALL_JOBS)
+            )
         return n_jobs
 
     def abort_everything(self, ensure_ready=True):
         # This method is called when a job has raised an exception.
         # In that case, we're not going to finish computations, so
         # we should free up Platform resources in any remaining jobs.
         self.executor.cancel_all()
         if not ensure_ready:
             self.executor.shutdown(wait=False)
 
+    def terminate(self):
+        """Shutdown the workers and free the shared memory."""
+        return self.abort_everything(ensure_ready=True)
+
     def apply_async(self, func, callback=None):
-        """Schedule func to be run
-        """
+        """Schedule func to be run"""
         # Serialize func to a temporary file and upload it to a Civis File.
         # Make the temporary files expire in a week.
         expires_at = (datetime.now() + timedelta(days=7)).isoformat()
         with TemporaryDirectory() as tempdir:
             temppath = os.path.join(tempdir, "civis_joblib_backend_func")
             with open(temppath, "wb") as tmpfile:
                 cloudpickle.dump(
-                    (func,
-                     self if self.remote_backend == 'civis'
-                     else self.remote_backend),
+                    (
+                        func,
+                        self if self.remote_backend == "civis" else self.remote_backend,
+                    ),
                     tmpfile,
-                    pickle.HIGHEST_PROTOCOL)
+                    pickle.HIGHEST_PROTOCOL,
+                )
             with open(temppath, "rb") as tmpfile:
-                func_file_id = \
-                    _robust_file_to_civis(tmpfile,
-                                          "civis_joblib_backend_func",
-                                          n_retries=5,
-                                          delay=0.5,
-                                          expires_at=expires_at,
-                                          client=self.client)
-                log.debug("uploaded serialized function to File: %d",
-                          func_file_id)
+                func_file_id = _robust_file_to_civis(
+                    tmpfile,
+                    "civis_joblib_backend_func",
+                    n_retries=5,
+                    delay=0.5,
+                    expires_at=expires_at,
+                    client=self.client,
+                )
+                log.debug("uploaded serialized function to File: %d", func_file_id)
 
             # Use the Civis CLI client to download the job runner script into
             # the container, and then run it on the uploaded job.
             # Only download the runner script if it doesn't already
             # exist in the destination environment.
             runner_remote_path = "civis_joblib_worker"
-            cmd = ("{setup_cmd} && "
-                   "if command -v {runner_remote_path} >/dev/null; "
-                   "then exec {runner_remote_path} {func_file_id}; "
-                   "else pip install civis=={civis_version} && "
-                   "exec {runner_remote_path} {func_file_id}; fi "
-                   .format(civis_version=civis.__version__,
-                           runner_remote_path=runner_remote_path,
-                           func_file_id=func_file_id,
-                           setup_cmd=self.setup_cmd))
+            cmd = (
+                "{setup_cmd} && "
+                "if command -v {runner_remote_path} >/dev/null; "
+                "then exec {runner_remote_path} {func_file_id}; "
+                "else pip install civis=={civis_version} && "
+                "exec {runner_remote_path} {func_file_id}; fi ".format(
+                    civis_version=civis.__version__,
+                    runner_remote_path=runner_remote_path,
+                    func_file_id=func_file_id,
+                    setup_cmd=self.setup_cmd,
+                )
+            )
 
             # Try to submit the command, with optional retrying for certain
             # error types.
             for n_retries in range(1 + self.max_submit_retries):
                 try:
                     if self.using_template:
-                        args = {'JOBLIB_FUNC_FILE_ID': func_file_id}
+                        args = {"JOBLIB_FUNC_FILE_ID": func_file_id}
                         future = self.executor.submit(**args)
-                        log.debug("Started custom script from template "
-                                  "%s with arguments %s",
-                                  self.executor.from_template_id, args)
+                        log.debug(
+                            "Started custom script from template "
+                            "%s with arguments %s",
+                            self.executor.from_template_id,
+                            args,
+                        )
                     else:
                         future = self.executor.submit(fn=cmd)
-                        log.debug("started container script with "
-                                  "command: %s", cmd)
+                        log.debug("started container script with " "command: %s", cmd)
                     # Stop retrying if submission was successful.
                     break
                 except CivisAPIError as e:
                     # If we've retried the maximum number of times already,
                     # then raise an exception.
                     retries_left = self.max_submit_retries - n_retries - 1
                     if retries_left < 1:
                         raise JobSubmissionError(e)
 
-                    log.debug("Retrying submission. %d retries left",
-                              retries_left)
+                    log.debug("Retrying submission. %d retries left", retries_left)
 
                     # Sleep with exponentially increasing intervals in case
                     # the issue persists for a while.
-                    time.sleep(2 ** n_retries)
+                    time.sleep(2**n_retries)
 
             if self.executor.max_n_retries:
                 # Start the ContainerFuture polling.
                 # This will use more API calls, but will
                 # allow the ContainerFuture to launch
                 # retries if necessary.
                 # (This is only relevant if we're not using the
@@ -904,21 +994,21 @@
             result = _CivisBackendResult(future, callback)
 
         return result
 
     def __getstate__(self):
         """override pickle to remove threading and civis APIClient objects"""
         state = self.__dict__.copy()
-        if 'client' in state:
-            state['client'] = None
-        if 'executor' in state:
-            del state['executor']
+        if "client" in state:
+            state["client"] = None
+        if "executor" in state:
+            del state["executor"]
         # the parallel attribute gets added by the parent class when the
         # backend is in use.
-        if 'parallel' in state:
-            state['parallel'] = None
+        if "parallel" in state:
+            state["parallel"] = None
         return state
 
     def __setstate__(self, state):
         """re-init the backend when unpickling"""
         self.__dict__.update(state)
         self._init_civis_backend()
```

### Comparing `civis-1.9.4/civis/base.py` & `civis-2.0.0/src/civis/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,81 @@
-from __future__ import absolute_import
-from builtins import super
 import os
-from posixpath import join
+import sys
 import threading
-from concurrent import futures
-import six
 import warnings
+from concurrent import futures
+from json.decoder import JSONDecodeError
+from posixpath import join
+
+import requests
 
+import civis
 from civis.response import PaginatedResponse, convert_response_data_type
-from civis._utils import open_session
+from civis._utils import retry_request, MAX_RETRIES
 
-FINISHED = ['success', 'succeeded']
-FAILED = ['failed']
-NOT_FINISHED = ['queued', 'running']
-CANCELLED = ['cancelled']
+FINISHED = ["success", "succeeded"]
+FAILED = ["failed"]
+NOT_FINISHED = ["queued", "running"]
+CANCELLED = ["cancelled"]
 DONE = FINISHED + FAILED + CANCELLED
 
 # Translate Civis state strings into `future` state strings
 STATE_TRANS = {}
 for name in FINISHED + FAILED:
     STATE_TRANS[name] = futures._base.FINISHED
 for name in NOT_FINISHED:
     STATE_TRANS[name] = futures._base.RUNNING
 for name in CANCELLED:
     STATE_TRANS[name] = futures._base.CANCELLED_AND_NOTIFIED
 
 
-DEFAULT_API_ENDPOINT = 'https://api.civisanalytics.com/'
+DEFAULT_API_ENDPOINT = "https://api.civisanalytics.com/"
 
 
 def tostr_urljoin(*x):
     return join(*map(str, x))
 
 
 class CivisJobFailure(Exception):
-    def __init__(self, err_msg, response=None):
-        self.error_message = err_msg
+    def __init__(self, err_msg, response=None, job_id=None, run_id=None):
+        self.job_id = job_id
+        self.run_id = run_id
+        self._original_err_msg = err_msg
+        self.error_message = _err_msg_with_job_run_ids(err_msg, job_id, run_id)
         self.response = response
 
     def __str__(self):
         return self.error_message
 
 
+def _err_msg_with_job_run_ids(err_msg, job_id, run_id) -> str:
+    if job_id is None and run_id is None:
+        return err_msg
+    elif run_id is None:
+        return f"(From job {job_id}) {err_msg}"
+    else:
+        return f"(From job {job_id} / run {run_id}) {err_msg}"
+
+
 class CivisAPIError(Exception):
     def __init__(self, response):
         if response.content:  # the API itself gave an error response
-            json = response.json()
-            self.error_message = json["errorDescription"]
+            try:
+                json = response.json()
+            except JSONDecodeError as e:
+                if "Expecting value: line 1 column 1 (char 0)" in str(e):
+                    self.error_message = "No Response Content from Civis API"
+                else:
+                    self.error_message = (
+                        f"Response Content: " f"{(response.content or b'').decode()}"
+                    )
+            else:
+                self.error_message = (
+                    json.get("errorDescription") or "No Error Message Available"
+                )
         else:  # this was something like a 502
             self.error_message = response.reason
 
         self.status_code = response.status_code
         self._response = response
 
     def __str__(self):
@@ -64,64 +89,82 @@
     pass
 
 
 class CivisAPIKeyError(Exception):
     pass
 
 
+class CivisImportError(Exception):
+    pass
+
+
 def get_base_url():
-    base_url = os.environ.get('CIVIS_API_ENDPOINT', DEFAULT_API_ENDPOINT)
-    if not base_url.endswith('/'):
-        base_url += '/'
+    base_url = os.environ.get("CIVIS_API_ENDPOINT", DEFAULT_API_ENDPOINT)
+    if not base_url.endswith("/"):
+        base_url += "/"
     return base_url
 
 
-class Endpoint(object):
+class Endpoint:
 
     _lock = threading.Lock()
 
-    def __init__(self, session_kwargs, return_type='civis'):
+    def __init__(self, session_kwargs, client, return_type="raw"):
         self._session_kwargs = session_kwargs
         self._return_type = return_type
         self._base_url = get_base_url()
+        self._client = client
 
     def _build_path(self, path):
         if not path:
             return self._base_url
         return tostr_urljoin(self._base_url, path.strip("/"))
 
-    def _make_request(self, method, path=None, params=None, data=None,
-                      **kwargs):
+    def _make_request(self, method, path=None, params=None, data=None, **kwargs):
         url = self._build_path(path)
 
         with self._lock:
             with open_session(**self._session_kwargs) as sess:
-                response = sess.request(method, url, json=data,
-                                        params=params, **kwargs)
+                request = requests.Request(
+                    method, url, json=data, params=params, **kwargs
+                )
+                pre_request = sess.prepare_request(request)
+                response = retry_request(method, pre_request, sess, MAX_RETRIES)
 
         if response.status_code == 401:
             auth_error = response.headers["www-authenticate"]
-            six.raise_from(CivisAPIKeyError(auth_error),
-                           CivisAPIError(response))
+            raise CivisAPIKeyError(auth_error) from CivisAPIError(response)
 
         if not response.ok:
             raise CivisAPIError(response)
 
         return response
 
-    def _call_api(self, method, path=None, params=None, data=None, **kwargs):
-        iterator = kwargs.pop('iterator', False)
+    def _call_api(
+        self,
+        method,
+        path=None,
+        params=None,
+        data=None,
+        deprecation_warning=None,
+        **kwargs,
+    ):
+        if deprecation_warning:
+            # stacklevel=3 to point to the call just outside civis-python
+            warnings.warn(deprecation_warning, FutureWarning, stacklevel=3)
+
+        iterator = kwargs.pop("iterator", False)
 
         if iterator:
-            return PaginatedResponse(path, params, self)
+            resp = PaginatedResponse(path, params, self)
         else:
             resp = self._make_request(method, path, params, data, **kwargs)
-            resp = convert_response_data_type(resp,
-                                              return_type=self._return_type)
-            return resp
+            resp = convert_response_data_type(resp, return_type=self._return_type)
+        self._client.last_response = resp
+        return resp
 
 
 class CivisAsyncResultBase(futures.Future):
     """A base class for tracking asynchronous results.
 
     Sub-classes needs to call either the `set_result` method to set a result
     when it finishes or call `set_exception` if there is an error.
@@ -136,59 +179,62 @@
     poller : func
         A function which returns an object that has a ``state`` attribute.
     poller_args : tuple
         The arguments with which to call the poller function.
     polling_interval : int or float
         The number of seconds between API requests to check whether a result
         is ready.
-    api_key : DEPRECATED str, optional
-        Your Civis API key. If not given, the :envvar:`CIVIS_API_KEY`
-        environment variable will be used.
     client : :class:`civis.APIClient`, optional
         If not provided, an :class:`civis.APIClient` object will be
         created from the :envvar:`CIVIS_API_KEY`.
     poll_on_creation : bool, optional
         If ``True`` (the default), it will poll upon calling ``result()`` the
         first time. If ``False``, it will wait the number of seconds specified
         in `polling_interval` from object creation before polling.
     """
-    def __init__(self, poller, poller_args,
-                 polling_interval=None, api_key=None, client=None,
-                 poll_on_creation=True):
+
+    def __init__(
+        self,
+        poller,
+        poller_args,
+        polling_interval=None,
+        client=None,
+        poll_on_creation=True,
+    ):
         super().__init__()
         self.poller = poller
         self.poller_args = poller_args
         self.polling_interval = polling_interval
-        if api_key is not None:
-            warnings.warn('The "api_key" parameter is deprecated and will be '
-                          'removed in v2. Please use the `client` parameter '
-                          'instead.', FutureWarning)
         self.client = client
         self.poll_on_creation = poll_on_creation
 
     def __repr__(self):
         # Almost the same as the superclass's __repr__, except we use
         # the `_civis_state` rather than the `_state`.
         with self._condition:
             if self._civis_state in FINISHED + FAILED:
                 if self.exception():
-                    return '<%s at %#x state=%s raised %s>' % (
+                    return "<%s at %#x state=%s raised %s>" % (
                         self.__class__.__name__,
                         id(self),
                         self._civis_state,
-                        self._exception.__class__.__name__)
+                        self._exception.__class__.__name__,
+                    )
                 else:
-                    return '<%s at %#x state=%s returned %s>' % (
+                    return "<%s at %#x state=%s returned %s>" % (
                         self.__class__.__name__,
                         id(self),
                         self._civis_state,
-                        self.result().__class__.__name__)
-            out = '<%s at %#x state=%s>' % (self.__class__.__name__,
-                                            id(self),
-                                            self._civis_state)
+                        self.result().__class__.__name__,
+                    )
+            out = "<%s at %#x state=%s>" % (
+                self.__class__.__name__,
+                id(self),
+                self._civis_state,
+            )
             return out
 
     def cancel(self):
         """Not currently implemented."""
         raise NotImplementedError("Running jobs cannot currently be cancelled")
 
     def succeeded(self):
@@ -208,19 +254,72 @@
 
     @property
     def _civis_state(self):
         """State as returned from Civis."""
         with self._condition:
             if self._check_result():
                 return self._check_result().state
-            return 'running'
+            return "running"
 
     @property
     def _state(self):
         """State of the CivisAsyncResultBase in `future` language."""
         with self._condition:
             return STATE_TRANS[self._civis_state]
 
     @_state.setter
     def _state(self, value):
         # Ignore attempts to set the _state from the `Future` superclass
         pass
+
+    def set_result(self, result):
+        """Sets the return value of work associated with the future.
+
+        This is adapted from
+        https://github.com/python/cpython/blob/3.8/Lib/concurrent/futures/_base.py#L517-L530
+        This version does not try to change the _state or check that the
+        initial _state is running since the Civis implementation has _state
+        depend on the Platform job state.
+        """
+        with self._condition:
+            self._result = result
+            for waiter in self._waiters:
+                waiter.add_result(self)
+            self._condition.notify_all()
+        self._invoke_callbacks()
+
+    def set_exception(self, exception):
+        """Sets the result of the future as being the given exception.
+
+        This is adapted from
+        https://github.com/python/cpython/blob/3.8/Lib/concurrent/futures/_base.py#L532-L545
+        This version does not try to change the _state or check that the
+        initial _state is running since the Civis implementation has _state
+        depend on the Platform job state.
+        """
+        with self._condition:
+            self._exception = exception
+            for waiter in self._waiters:
+                waiter.add_exception(self)
+            self._condition.notify_all()
+        self._invoke_callbacks()
+
+
+def open_session(api_key, user_agent="civis-python"):
+    """Create a new Session which can connect with the Civis API"""
+    civis_version = civis.__version__
+    session = requests.Session()
+    session.auth = (api_key, "")
+    session_agent = session.headers.get("User-Agent", "")
+    ver_string = "{}.{}.{}".format(
+        sys.version_info.major, sys.version_info.minor, sys.version_info.micro
+    )
+    user_agent = "{}/Python v{} Civis v{} {}".format(
+        user_agent, ver_string, civis_version, session_agent
+    )
+    headers = {"User-Agent": user_agent.strip()}
+    job_id, run_id = os.getenv("CIVIS_JOB_ID"), os.getenv("CIVIS_RUN_ID")
+    if job_id:
+        headers.update({"X-Civis-Job-ID": job_id, "X-Civis-Run-ID": run_id})
+    session.headers.update(headers)
+
+    return session
```

### Comparing `civis-1.9.4/civis/_utils.py` & `civis-2.0.0/src/civis/_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,99 @@
-from __future__ import absolute_import
-from builtins import super
 import logging
 import os
 import re
 import time
 import uuid
+from random import random
 
-import requests
-from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util import Retry
-
-import civis
+from tenacity import (
+    Retrying,
+    retry_if_result,
+    stop_after_attempt,
+    stop_after_delay,
+    wait_random_exponential,
+)
+from tenacity.wait import wait_base
 
 
 log = logging.getLogger(__name__)
-UNDERSCORER1 = re.compile(r'(.)([A-Z][a-z]+)')
-UNDERSCORER2 = re.compile('([a-z0-9])([A-Z])')
+UNDERSCORER1 = re.compile(r"(.)([A-Z][a-z]+)")
+UNDERSCORER2 = re.compile("([a-z0-9])([A-Z])")
+MAX_RETRIES = 10
+
+_RETRY_CODES = [429, 502, 503, 504]
+_RETRY_VERBS = ["HEAD", "TRACE", "GET", "PUT", "OPTIONS", "DELETE"]
+_POST_RETRY_CODES = [429, 503]
 
 
 def maybe_get_random_name(name):
     if not name:
         name = uuid.uuid4().hex
     return name
 
 
 def camel_to_snake(word):
     # https://gist.github.com/jaytaylor/3660565
-    word = UNDERSCORER1.sub(r'\1_\2', word)
-    return UNDERSCORER2.sub(r'\1_\2', word).lower()
+    word = UNDERSCORER1.sub(r"\1_\2", word)
+    return UNDERSCORER2.sub(r"\1_\2", word).lower()
 
 
 def to_camelcase(s):
-    return re.sub(r'(^|_)([a-zA-Z])', lambda m: m.group(2).upper(), s)
+    return re.sub(r"(^|_)([a-zA-Z])", lambda m: m.group(2).upper(), s)
 
 
 def get_api_key(api_key):
     """Pass-through if `api_key` is not None otherwise tries the CIVIS_API_KEY
     environmental variable.
     """
     if api_key is not None:  # always prefer user given one
         return api_key
     api_key = os.environ.get("CIVIS_API_KEY", None)
     if api_key is None:
-        raise EnvironmentError("No Civis API key found. Please store in "
-                               "CIVIS_API_KEY environment variable")
+        raise EnvironmentError(
+            "No Civis API key found. Please store in "
+            "CIVIS_API_KEY environment variable"
+        )
     return api_key
 
 
-def open_session(api_key, max_retries=5, user_agent="civis-python"):
-    """Create a new Session which can connect with the Civis API"""
-    civis_version = civis.__version__
-    session = requests.Session()
-    session.auth = (api_key, '')
-    session_agent = session.headers.get('User-Agent', '')
-    user_agent = "{}/{} {}".format(user_agent, civis_version, session_agent)
-    session.headers.update({"User-Agent": user_agent.strip()})
-    max_retries = AggressiveRetry(max_retries, backoff_factor=.75,
-                                  status_forcelist=civis.civis.RETRY_CODES)
-    adapter = HTTPAdapter(max_retries=max_retries)
-    session.mount("https://", adapter)
-
-    return session
-
-
-class AggressiveRetry(Retry):
-    # Subclass Retry so that it retries more things. In particular,
-    # always retry API requests with a Retry-After header, regardless
-    # of the verb.
-    def is_retry(self, method, status_code, has_retry_after=False):
-        """ Is this method/status code retryable? (Based on whitelists and control
-        variables such as the number of total retries to allow, whether to
-        respect the Retry-After header, whether this header is present, and
-        whether the returned status code is on the list of status codes to
-        be retried upon on the presence of the aforementioned header)
-        """
-        if (self.total and
-                self.respect_retry_after_header and
-                has_retry_after and
-                (status_code in self.RETRY_AFTER_STATUS_CODES)):
-            return True
+def retry_request(method, prepared_req, session, max_retries=10):
+    retry_conditions = None
 
-        else:
-            return super().is_retry(method=method, status_code=status_code,
-                                    has_retry_after=has_retry_after)
+    def _make_request(req, sess):
+        """send the prepared session request"""
+        response = sess.send(req)
+        return response
+
+    def _return_last_value(retry_state):
+        """return the result of the last call attempt
+        and let code pick up the error"""
+        return retry_state.outcome.result()
+
+    if method.upper() == "POST":
+        retry_conditions = retry_if_result(
+            lambda res: res.status_code in _POST_RETRY_CODES
+        )
+    elif method.upper() in _RETRY_VERBS:
+        retry_conditions = retry_if_result(lambda res: res.status_code in _RETRY_CODES)
+
+    if retry_conditions:
+        retry_config = Retrying(
+            retry=retry_conditions,
+            wait=wait_for_retry_after_header(
+                fallback=wait_random_exponential(multiplier=2, max=60)
+            ),
+            stop=(stop_after_delay(600) | stop_after_attempt(max_retries)),
+            retry_error_callback=_return_last_value,
+        )
+        response = retry_config(_make_request, prepared_req, session)
+        return response
+
+    response = _make_request(prepared_req, session)
+    return response
 
 
 def retry(exceptions, retries=5, delay=0.5, backoff=2):
     """
     Retry decorator
 
     Parameters
@@ -94,39 +101,43 @@
     exceptions: Exception
         exceptions to trigger retry
     retries: int, optional
         number of retries to perform
     delay: float, optional
         delay before next retry
     backoff: int, optional
-        factor used to increase delay after each retry
+        factor used to calculate the exponential increase
+        delay after each retry
 
     Returns
     -------
     retry decorator
 
     Raises
     ------
     exception raised by decorator function
     """
+
     def deco_retry(f):
         def f_retry(*args, **kwargs):
             n_failed = 0
             new_delay = delay
             while True:
                 try:
                     return f(*args, **kwargs)
                 except exceptions as exc:
                     if n_failed < retries:
                         n_failed += 1
-                        msg = "%s, Retrying in %d seconds..." % \
-                              (str(exc), new_delay)
+                        msg = "%s, Retrying in %d seconds..." % (str(exc), new_delay)
                         log.debug(msg)
                         time.sleep(new_delay)
-                        new_delay *= backoff
+                        new_delay = min(
+                            (pow(2, n_failed) / 4) * (random() + backoff),  # nosec
+                            50 + 10 * random(),  # nosec
+                        )
                     else:
                         raise exc
 
         return f_retry
 
     return deco_retry
 
@@ -136,16 +147,40 @@
         self.buf = buf
         self.max_bytes = max_bytes
         self.bytes_read = 0
         self.len = max_bytes
 
     def read(self, size=-1):
         if self.bytes_read >= self.max_bytes:
-            return b''
+            return b""
         bytes_left = self.max_bytes - self.bytes_read
         if size < 0:
             bytes_to_read = bytes_left
         else:
             bytes_to_read = min(size, bytes_left)
         data = self.buf.read(bytes_to_read)
         self.bytes_read += len(data)
         return data
+
+
+class wait_for_retry_after_header(wait_base):
+    """Wait strategy that first looks for Retry-After header. If not
+    present it uses the fallback strategy as the wait param"""
+
+    def __init__(self, fallback):
+        self.fallback = fallback
+
+    def __call__(self, retry_state):
+        # retry_state is an instance of tenacity.RetryCallState.
+        # The .outcome property contains the result/exception
+        # that came from the underlying function.
+        result_headers = retry_state.outcome._result.headers
+        retry_after = result_headers.get("Retry-After") or result_headers.get(
+            "retry-after"
+        )
+
+        try:
+            log.info("Retrying after {} seconds".format(retry_after))
+            return int(retry_after)
+        except (TypeError, ValueError):
+            pass
+        return self.fallback(retry_state)
```

### Comparing `civis-1.9.4/civis/civis.py` & `civis-2.0.0/src/civis/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,80 @@
-from __future__ import absolute_import
+from functools import lru_cache
 import logging
-import warnings
 
 import civis
-from civis.compat import lru_cache
 from civis.resources import generate_classes_maybe_cached
 from civis._utils import get_api_key
-from civis._deprecation import deprecate_param
+from civis.response import _RETURN_TYPES, find, find_one
 
 
-log = logging.getLogger(__name__)
+_log = logging.getLogger(__name__)
 
-RETRY_CODES = [429, 502, 503, 504]
 
-
-def find(object_list, filter_func=None, **kwargs):
-    """Filter :class:`civis.response.Response` objects.
+class APIClient:
+    """The Civis API client.
 
     Parameters
     ----------
-    object_list : iterable
-        An iterable of arbitrary objects, particularly those with attributes
-        that can be targeted by the filters in `kwargs`. A major use case is
-        an iterable of :class:`civis.response.Response` objects.
-    filter_func : callable, optional
-        A one-argument function. If specified, `kwargs` are ignored.
-        An `object` from the input iterable is kept in the returned list
-        if and only if ``bool(filter_func(object))`` is ``True``.
-    **kwargs
-        Key-value pairs for more fine-grained filtering; they cannot be used
-        in conjunction with `filter_func`. All keys must be strings.
-        For an `object` from the input iterable to be included in the
-        returned list, all the `key`s must be attributes of `object`, plus
-        any one of the following conditions for a given `key`:
-
-        - `value` is a one-argument function and
-          ``bool(value(getattr(object, key)))`` is ``True``
-        - `value` is ``True``
-        - ``getattr(object, key)`` is equal to ``value``
-
-    Returns
-    -------
-    list
-
-    Examples
-    --------
-    >>> import civis
-    >>> client = civis.APIClient()
-    >>> # creds is a list of civis.response.Response objects
-    >>> creds = client.credentials.list()
-    >>> # target_creds contains civis.response.Response objects
-    >>> # with the attribute 'name' == 'username'
-    >>> target_creds = find(creds, name='username')
-
-    See Also
-    --------
-    civis.find_one
-    """
-    _func = filter_func
-    if not filter_func:
-        def default_filter(o):
-            for k, v in kwargs.items():
-                if not hasattr(o, k):
-                    return False
-                elif callable(v):
-                    if not v(getattr(o, k, None)):
-                        return False
-                elif isinstance(v, bool):
-                    if hasattr(o, k) != v:
-                        return False
-                elif v != getattr(o, k, None):
-                    return False
-            return True
-
-        _func = default_filter
-
-    return [o for o in object_list if _func(o)]
-
-
-def find_one(object_list, filter_func=None, **kwargs):
-    """Return one satisfying :class:`civis.response.Response` object.
-
-    The arguments are the same as those for :func:`civis.find`.
-    If more than one object satisfies the filtering criteria,
-    the first one is returned.
-    If no satisfying objects are found, ``None`` is returned.
-
-    Returns
-    -------
-    object or None
-
-    See Also
-    --------
-    civis.find
+    api_key : str, optional
+        Your API key obtained from the Civis Platform. If not given, the
+        client will use the :envvar:`CIVIS_API_KEY` environment variable.
+    return_type : str, optional
+        The following types are implemented:
+
+        - ``'raw'`` Returns the raw :class:`requests:requests.Response` object.
+        - ``'snake'`` Returns a :class:`civis.response.Response` object for the
+          json-encoded content of a response. This maps the top-level json
+          keys to snake_case.
+    api_version : string, optional
+        The version of endpoints to call. May instantiate multiple client
+        objects with different versions. Currently only "1.0" is supported.
+    local_api_spec : collections.OrderedDict or string, optional
+        The methods on this class are dynamically built from the Civis API
+        specification, which can be retrieved from the /endpoints endpoint.
+        When local_api_spec is None, the default, this specification is
+        downloaded the first time APIClient is instantiated. Alternatively,
+        a local cache of the specification may be passed as either an
+        OrderedDict or a filename which points to a json file.
     """
-    results = find(object_list, filter_func, **kwargs)
 
-    return results[0] if results else None
+    def __init__(
+        self, api_key=None, return_type="snake", api_version="1.0", local_api_spec=None
+    ):
+        if return_type not in _RETURN_TYPES:
+            raise ValueError(
+                f"Return type must be one of {set(_RETURN_TYPES)}: " f"{return_type}"
+            )
+        self._feature_flags = ()
+        session_auth_key = get_api_key(api_key)
+        self._session_kwargs = {"api_key": session_auth_key}
+        self.last_response = None
+
+        classes = generate_classes_maybe_cached(
+            local_api_spec, session_auth_key, api_version
+        )
+        for class_name, cls in classes.items():
+            setattr(
+                self,
+                class_name,
+                cls(self._session_kwargs, client=self, return_type=return_type),
+            )
 
+    @property
+    def feature_flags(self):
+        if self._feature_flags:
+            return self._feature_flags
+        me = self.users.list_me()
+        self._feature_flags = tuple(
+            flag for flag, value in me["feature_flags"].items() if value
+        )
+        return self._feature_flags
 
-class MetaMixin():
+    def __getstate__(self):
+        raise RuntimeError("The APIClient object can't be pickled.")
 
     @lru_cache(maxsize=128)
     def get_database_id(self, database):
         """Return the database ID for a given database name.
 
         Parameters
         ----------
@@ -163,23 +134,25 @@
         >>> client.get_database_credential_id(1111, 'redshift-general')
         1111
         """
         if isinstance(username, int):
             return username
         else:
             creds = self.credentials.list(type="Database")
-            filter_kwargs = {'username': username}
+            filter_kwargs = {"username": username}
             if isinstance(database_name, int):
-                filter_kwargs['remote_host_id'] = database_name
+                filter_kwargs["remote_host_id"] = database_name
             else:
-                filter_kwargs['remote_host_name'] = database_name
+                filter_kwargs["remote_host_name"] = database_name
             my_creds = find_one(creds, **filter_kwargs)
             if my_creds is None:
-                raise ValueError("Credential ID for {} on {} not "
-                                 "found.".format(username, database_name))
+                raise ValueError(
+                    "Credential ID for {} on {} not "
+                    "found.".format(username, database_name)
+                )
 
         return my_creds["id"]
 
     @lru_cache(maxsize=128)
     def get_aws_credential_id(self, cred_name, owner=None):
         """Find an AWS credential ID.
 
@@ -234,17 +207,21 @@
             elif len(my_creds) > 1:
                 if owner is None:
                     # If the user didn't specify an owner, see if we can
                     # narrow down to just credentials owned by this user.
                     owner = self.username
                     my_creds = find(my_creds, owner=owner)
                 if len(my_creds) > 1:
-                    log.warning("Found %d AWS credentials with name %s and "
-                                "owner %s. Returning the first.",
-                                len(my_creds), cred_name, owner)
+                    _log.warning(
+                        "Found %d AWS credentials with name %s and "
+                        "owner %s. Returning the first.",
+                        len(my_creds),
+                        cred_name,
+                        owner,
+                    )
             my_creds = my_creds[0]
 
         return my_creds["id"]
 
     @lru_cache(maxsize=128)
     def get_table_id(self, table, database):
         """Return the table ID for a given database and table name.
@@ -275,105 +252,65 @@
         >>> client.get_table_id('foo.bar', 'redshift-general')
         123
         >>> client.get_table_id('"schema.has.periods".bar', 'redshift-general')
         456
         """
         database_id = self.get_database_id(database)
         schema, name = civis.io.split_schema_tablename(table)
-        tables = self.tables.list(database_id=database_id, schema=schema,
-                                  name=name)
+        tables = self.tables.list(database_id=database_id, schema=schema, name=name)
         if not tables:
             msg = "No tables found for {} in database {}"
             raise ValueError(msg.format(table, database))
 
         return tables[0].id
 
+    @lru_cache(maxsize=128)
+    def get_storage_host_id(self, storage_host):
+        """Return the storage host ID for a given storage host name.
+
+        Parameters
+        ----------
+        storage_host : str or int
+            If an integer ID is given, passes through. If a str is given
+            the storage host ID corresponding to that storage host is returned.
+
+        Returns
+        -------
+        storage_host_id : int
+            The ID of the storage host.
+
+        Raises
+        ------
+        ValueError
+            If the storage host can't be found.
+
+        Examples
+        --------
+        >>> import civis
+        >>> client = civis.APIClient()
+        >>> client.get_storage_host_id('test host')
+        1234
+
+        >>> client.get_storage_host_id(1111)
+        1111
+        """
+        if isinstance(storage_host, int):
+            return storage_host
+        sh = find_one(self.storage_hosts.list(), name=storage_host)
+        if not sh:
+            raise ValueError("Storage Host {} not found.".format(storage_host))
+
+        return sh["id"]
+
     @property
     @lru_cache(maxsize=128)
     def default_credential(self):
         """The current user's default credential."""
         # NOTE: this should be optional to endpoints...so this could go away
         creds = self.credentials.list(default=True)
-        return creds[0]['id'] if len(creds) > 0 else None
+        return creds[0]["id"] if len(creds) > 0 else None
 
     @property
     @lru_cache(maxsize=128)
     def username(self):
         """The current user's username."""
         return self.users.list_me().username
-
-
-class APIClient(MetaMixin):
-    """The Civis API client.
-
-    Parameters
-    ----------
-    api_key : str, optional
-        Your API key obtained from the Civis Platform. If not given, the
-        client will use the :envvar:`CIVIS_API_KEY` environment variable.
-    return_type : str, optional
-        The following types are implemented:
-
-        - ``'raw'`` Returns the raw :class:`requests:requests.Response` object.
-        - ``'snake'`` Returns a :class:`civis.response.Response` object for the
-          json-encoded content of a response. This maps the top-level json
-          keys to snake_case.
-        - ``'pandas'`` Returns a :class:`pandas:pandas.DataFrame` for
-          list-like responses and a :class:`pandas:pandas.Series` for single a
-          json response.
-    retry_total : int, optional
-        A number indicating the maximum number of retries for 429, 502, 503, or
-        504 errors.
-    api_version : string, optional
-        The version of endpoints to call. May instantiate multiple client
-        objects with different versions. Currently only "1.0" is supported.
-    resources : string, optional
-        When set to "base", only the default endpoints will be exposed in the
-        client object. Set to "all" to include all endpoints available for
-        a given user, including those that may be in development and subject
-        to breaking changes at a later date. This will be removed in a future
-        version of the API client.
-    local_api_spec : collections.OrderedDict or string, optional
-        The methods on this class are dynamically built from the Civis API
-        specification, which can be retrieved from the /endpoints endpoint.
-        When local_api_spec is None, the default, this specification is
-        downloaded the first time APIClient is instantiated. Alternatively,
-        a local cache of the specification may be passed as either an
-        OrderedDict or a filename which points to a json file.
-    """
-    @deprecate_param('v2.0.0', 'resources')
-    def __init__(self, api_key=None, return_type='snake',
-                 retry_total=6, api_version="1.0", resources="all",
-                 local_api_spec=None):
-        if return_type not in ['snake', 'raw', 'pandas']:
-            raise ValueError("Return type must be one of 'snake', 'raw', "
-                             "'pandas'")
-        self._feature_flags = ()
-        session_auth_key = get_api_key(api_key)
-        self._session_kwargs = {'api_key': session_auth_key,
-                                'max_retries': retry_total}
-
-        # Catch deprecation warnings from generate_classes_maybe_cached and
-        # the functions it calls until the `resources` argument is removed.
-        with warnings.catch_warnings():
-            warnings.filterwarnings(
-                "ignore",
-                category=FutureWarning,
-                module='civis')
-            classes = generate_classes_maybe_cached(local_api_spec,
-                                                    session_auth_key,
-                                                    api_version,
-                                                    resources)
-        for class_name, cls in classes.items():
-            setattr(self, class_name, cls(self._session_kwargs, return_type))
-
-    @property
-    def feature_flags(self):
-        if self._feature_flags:
-            return self._feature_flags
-        me = self.users.list_me()
-        self._feature_flags = tuple(flag for flag, value
-                                    in me['feature_flags'].items() if value)
-        return self._feature_flags
-
-    def __getstate__(self):
-        raise RuntimeError("The APIClient object can't be pickled.")
```

### Comparing `civis-1.9.4/README.rst` & `civis-2.0.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Civis API Python Client
 =======================
 
-|Travis| |PyPI| |PyVersions|
+.. start-include-marker-introductory-paragraph
+
+|PyPI| |PyVersions| |CircleCI| |Documentation|
 
-.. |Travis| image:: https://img.shields.io/travis/civisanalytics/civis-python/master.svg
-   :alt: Build status
-   :target: https://travis-ci.org/civisanalytics/civis-python
+.. |CircleCI| image:: https://circleci.com/gh/civisanalytics/civis-python.svg?style=shield
+   :target: https://circleci.com/gh/civisanalytics/civis-python
+   :alt: CircleCI build status
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/civis.svg
    :target: https://pypi.org/project/civis/
    :alt: Latest version on PyPI
 
 .. |PyVersions| image:: https://img.shields.io/pypi/pyversions/civis.svg
    :target: https://pypi.org/project/civis/
    :alt: Supported python versions for civis-python
 
+.. |Documentation| image:: https://readthedocs.org/projects/civis-python/badge/?version=latest
+    :target: https://civis-python.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
 
-Introduction
-------------
-
-.. start-include-marker-introductory-paragraph
-
-The Civis API Python client is a Python package that helps analysts and
-developers interact with the Civis Platform. The package includes a set of
+The Civis API Python client is a Python package that helps analysts
+and developers interact with Civis Platform programmatically. The package includes a set of
 tools around common workflows as well as a convenient interface to make
 requests directly to the Civis API.
 
 .. end-include-marker-introductory-paragraph
 
 Please see the
 `full documentation <https://civis-python.readthedocs.io>`_ for more details.
@@ -44,22 +44,22 @@
 least every 30 days. The API client will look for a ``CIVIS_API_KEY``
 environmental variable to access your API key, so after creating a new API key,
 follow the steps below for your operating system to set up your environment.
 
 Linux / MacOS
 ~~~~~~~~~~~~~
 
-1. Add the following to ``.bash_profile`` (or ``.bashrc`` for Linux) for bash::
+1. Add the following to your shell configuration file (``~/.zshrc`` for MacOS or ``~/.bashrc`` for Linux, by default)::
 
     export CIVIS_API_KEY="alphaNumericApiK3y"
 
-2. Source your ``.bash_profile`` (or restart your terminal).
+2. Source your shell configuration file (or restart your terminal).
 
-Windows 10
-~~~~~~~~~~
+Windows
+~~~~~~~
 
 1. Navigate to "Settings" -> type "environment" in search bar ->
    "Edit environment variables for your account". This can also be found
    in "System Properties" -> "Advanced" -> "Environment Variables...".
 2. In the user variables section, if ``CIVIS_API_KEY`` already exists in
    the list of environment variables, click on it and press "Edit...".
    Otherwise, click "New..".
@@ -76,21 +76,19 @@
 
 After creating an API key and setting the ``CIVIS_API_KEY`` environmental
 variable, install the Python package ``civis`` with the recommended method via ``pip``::
 
     pip install civis
 
 Alternatively, if you are interested in the latest functionality not yet released through ``pip``,
-you may clone the code from GitHub and build from source:
+you may clone the code from GitHub and build from source (``git`` assumed to be available):
 
 .. code-block:: bash
 
-   git clone https://github.com/civisanalytics/civis-python.git
-   cd civis-python
-   python setup.py install
+   pip install git+https://github.com/civisanalytics/civis-python.git
 
 You can test your installation by running
 
 .. code-block:: python
 
     import civis
     client = civis.APIClient()
@@ -135,23 +133,14 @@
 
    pip install civisml-extensions
    pip install glmnet
    pip install muffnn
 
 .. end-include-marker-installation-section
 
-.. start-include-marker-python-version-support-section
-
-Python version support
-----------------------
-
-Python 2.7, 3.4, 3.5, 3.6, and 3.7
-
-.. end-include-marker-python-version-support-section
-
 Usage
 -----
 
 ``civis`` includes a number of wrappers around the Civis API for
 common workflows.
 
 .. code-block:: python
@@ -165,15 +154,15 @@
 
 .. code-block:: python
 
     import civis
     client = civis.APIClient()
     database = client.databases.list()
 
-See the `full documentation <https://civis-python.readthedocs.io>`_ for a more
+See the `documentation <https://civis-python.readthedocs.io>`_ for a more
 complete user guide.
 
 
 .. start-include-marker-retries-section
 
 Retries
 -------
@@ -182,44 +171,55 @@
 
 If the error is one of [413, 429, 503] and the API client is told how long it needs
 to wait before it's safe to retry (this is always the case with 429s, which are
 rate limit errors), then the client will wait the specified amount of time
 before retrying the request.
 
 If the error is one of [429, 502, 503, 504] and the request is not a ``patch*`` or ``post*``
-method, then the API client will retry the request several times, with a delay,
-to see if it will succeed.
+method, then the API client will retry the request several times, with an exponential delay,
+to see if it will succeed. If the request is of type ``post*`` it will retry with the same parameters
+for error codes [429, 503].
 
 .. end-include-marker-retires-section
 
 
 Build Documentation Locally
 ---------------------------
 
 To install dependencies for building the documentation::
 
-    pip install Sphinx
-    pip install sphinx_rtd_theme
-    pip install numpydoc
+    pip install -r docs/requirements.txt
 
 To build the API documentation locally::
 
-    cd docs
-    make html
+    sphinx-build -b html docs/source docs/build/html  # or prepend this command with `FETCH_REMOTE_RESOURCES=true ` for the API resources available to the given CIVIS_API_KEY
 
 Then open ``docs/build/html/index.html``.
 
-Note that this will use your API key in the ``CIVIS_API_KEY`` environment
-variable so it will generate documentation for all the endpoints that you have access to.
+Command-line Interface (CLI)
+----------------------------
+
+After installing the Python package, you'll also have a ``civis`` command accessible from your shell. It surfaces a commandline interface to all of the regular Civis API endpoints, plus a few helpers. To get started, run ``civis --help``.
+Please see the `CLI documentation <https://civis-python.readthedocs.io/en/stable/cli.html>`_ for more details.
+
 
 Contributing
 ------------
 
-See ``CONTRIBUTING.md`` for information about contributing to this project.
+See `CONTRIBUTING.md <CONTRIBUTING.md>`_ for information about contributing to this project.
 
 
 License
 -------
 
 BSD-3
 
-See ``LICENSE.md`` for details.
+See `LICENSE.md <LICENSE.md>`_ for details.
+
+
+For Maintainers
+---------------
+
+The `tools <tools/>`_ directory contains scripts that civis-python maintainers can
+use (and maintain...). Please see their docstrings for usage.
+Non-public information can be found by searching the internal documentation system
+or consulting the current maintainers.
```

