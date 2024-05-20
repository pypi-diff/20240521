# Comparing `tmp/tsperf-1.1.0.tar.gz` & `tmp/tsperf-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsperf-1.1.0.tar", last modified: Tue Jun  1 14:17:59 2021, max compression
+gzip compressed data, was "tsperf-1.2.0.tar", last modified: Mon May 20 22:45:47 2024, max compression
```

## Comparing `tsperf-1.1.0.tar` & `tsperf-1.2.0.tar`

### file list

```diff
@@ -1,62 +1,105 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.764998 tsperf-1.1.0/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-01 14:16:53.000000 tsperf-1.1.0/CHANGES.md
--rw-r--r--   0 amo        (501) staff       (20)    10174 2021-06-01 14:16:53.000000 tsperf-1.1.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)     2116 2021-06-01 14:17:59.764738 tsperf-1.1.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      682 2021-06-01 14:16:53.000000 tsperf-1.1.0/README.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.722669 tsperf-1.1.0/batch_size_automator/
--rw-r--r--   0 amo        (501) staff       (20)    10293 2021-06-01 14:16:53.000000 tsperf-1.1.0/batch_size_automator/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.754855 tsperf-1.1.0/data_generator/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)    16467 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/__main__.py
--rw-r--r--   0 amo        (501) staff       (20)     8143 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/argument_parser.py
--rw-r--r--   0 amo        (501) staff       (20)     5778 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/config.py
--rw-r--r--   0 amo        (501) staff       (20)     2894 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/crate_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     2035 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     3946 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/edge.py
--rw-r--r--   0 amo        (501) staff       (20)     3885 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/influx_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     3562 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/mongo_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     4662 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/mssql_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     3577 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/postgres_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     5234 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/timescale_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     6681 2021-06-01 14:16:53.000000 tsperf-1.1.0/data_generator/timestream_db_writer.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.755090 tsperf-1.1.0/float_simulator/
--rw-r--r--   0 amo        (501) staff       (20)     7141 2021-06-01 14:16:53.000000 tsperf-1.1.0/float_simulator/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      587 2021-06-01 14:16:53.000000 tsperf-1.1.0/pyproject.toml
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.755946 tsperf-1.1.0/query_timer/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-01 14:16:53.000000 tsperf-1.1.0/query_timer/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     7380 2021-06-01 14:16:53.000000 tsperf-1.1.0/query_timer/__main__.py
--rw-r--r--   0 amo        (501) staff       (20)     3792 2021-06-01 14:16:53.000000 tsperf-1.1.0/query_timer/argument_parser.py
--rw-r--r--   0 amo        (501) staff       (20)     2690 2021-06-01 14:16:53.000000 tsperf-1.1.0/query_timer/config.py
--rw-r--r--   0 amo        (501) staff       (20)       38 2021-06-01 14:17:59.765108 tsperf-1.1.0/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     2238 2021-06-01 14:17:57.000000 tsperf-1.1.0/setup.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.760716 tsperf-1.1.0/tests/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     6920 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_crate_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)      354 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_dg_argument_parser.py
--rw-r--r--   0 amo        (501) staff       (20)    12107 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_dg_config.py
--rw-r--r--   0 amo        (501) staff       (20)     9144 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_dg_main.py
--rw-r--r--   0 amo        (501) staff       (20)     4396 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_edge.py
--rw-r--r--   0 amo        (501) staff       (20)     6223 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_influx_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     4792 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_models.py
--rw-r--r--   0 amo        (501) staff       (20)     3475 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_mongo_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     6128 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_mssql_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     7745 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_postgres_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)      342 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_qt_argument_parser.py
--rw-r--r--   0 amo        (501) staff       (20)     5287 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_qt_config.py
--rw-r--r--   0 amo        (501) staff       (20)     2067 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_qt_main.py
--rw-r--r--   0 amo        (501) staff       (20)    11250 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_timescale_db_writer.py
--rw-r--r--   0 amo        (501) staff       (20)     6801 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/test_timestream_db_writer.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.762034 tsperf-1.1.0/tests/util/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/util/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)    12715 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/util/test_batch_size_automator.py
--rw-r--r--   0 amo        (501) staff       (20)     2831 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/util/test_float_simulator.py
--rw-r--r--   0 amo        (501) staff       (20)    12866 2021-06-01 14:16:53.000000 tsperf-1.1.0/tests/util/test_ticktrack.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.762397 tsperf-1.1.0/tictrack/
--rw-r--r--   0 amo        (501) staff       (20)     8010 2021-06-01 14:16:53.000000 tsperf-1.1.0/tictrack/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-06-01 14:17:59.764365 tsperf-1.1.0/tsperf.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     2116 2021-06-01 14:17:59.000000 tsperf-1.1.0/tsperf.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     1398 2021-06-01 14:17:59.000000 tsperf-1.1.0/tsperf.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2021-06-01 14:17:59.000000 tsperf-1.1.0/tsperf.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       88 2021-06-01 14:17:59.000000 tsperf-1.1.0/tsperf.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      366 2021-06-01 14:17:59.000000 tsperf-1.1.0/tsperf.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       79 2021-06-01 14:17:59.000000 tsperf-1.1.0/tsperf.egg-info/top_level.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.478148 tsperf-1.2.0/
+-rw-r--r--   0 amo        (501) staff       (20)     1010 2024-05-20 22:40:26.000000 tsperf-1.2.0/CHANGES.md
+-rw-r--r--   0 amo        (501) staff       (20)    10174 2024-05-18 15:01:58.000000 tsperf-1.2.0/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)     8109 2024-05-20 22:45:47.477762 tsperf-1.2.0/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     5238 2024-05-20 17:46:28.000000 tsperf-1.2.0/README.md
+-rw-r--r--   0 amo        (501) staff       (20)     2575 2024-05-20 17:46:28.000000 tsperf-1.2.0/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-05-20 22:45:47.478220 tsperf-1.2.0/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     2951 2024-05-20 22:44:51.000000 tsperf-1.2.0/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.447431 tsperf-1.2.0/tests/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.451980 tsperf-1.2.0/tests/adapter/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     7599 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/test_cratedb.py
+-rw-r--r--   0 amo        (501) staff       (20)     7797 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/test_cratedbpg.py
+-rw-r--r--   0 amo        (501) staff       (20)     6544 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/test_influxdb.py
+-rw-r--r--   0 amo        (501) staff       (20)     3882 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/test_mongodb.py
+-rw-r--r--   0 amo        (501) staff       (20)     6678 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/test_mssql.py
+-rw-r--r--   0 amo        (501) staff       (20)     8257 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/test_postgresql.py
+-rw-r--r--   0 amo        (501) staff       (20)    11563 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/test_timescaledb.py
+-rw-r--r--   0 amo        (501) staff       (20)     7376 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/adapter/test_timestream.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.453564 tsperf-1.2.0/tests/read/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/read/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      723 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/read/test_tsqt_cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     5520 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/read/test_tsqt_config.py
+-rw-r--r--   0 amo        (501) staff       (20)     1818 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/read/test_tsqt_core.py
+-rw-r--r--   0 amo        (501) staff       (20)      328 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/test_cli.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.454843 tsperf-1.2.0/tests/util/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/util/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)    12453 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/util/test_batch_size_automator.py
+-rw-r--r--   0 amo        (501) staff       (20)     2845 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/util/test_float_simulator.py
+-rw-r--r--   0 amo        (501) staff       (20)    12871 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/util/test_ticktrack.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.457193 tsperf-1.2.0/tests/write/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/write/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     4798 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/write/schema.py
+-rw-r--r--   0 amo        (501) staff       (20)     4527 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/write/test_channel.py
+-rw-r--r--   0 amo        (501) staff       (20)     1053 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/write/test_tsdg_cli.py
+-rw-r--r--   0 amo        (501) staff       (20)    12167 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/write/test_tsdg_config.py
+-rw-r--r--   0 amo        (501) staff       (20)    11083 2024-05-18 15:01:58.000000 tsperf-1.2.0/tests/write/test_tsdg_core.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.458067 tsperf-1.2.0/tsperf/
+-rw-r--r--   0 amo        (501) staff       (20)       93 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.463990 tsperf-1.2.0/tsperf/adapter/
+-rw-r--r--   0 amo        (501) staff       (20)     3120 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/adapter/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     3726 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/adapter/cratedb.py
+-rw-r--r--   0 amo        (501) staff       (20)     2491 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/adapter/cratedbpg.py
+-rw-r--r--   0 amo        (501) staff       (20)     2153 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/adapter/dummy.py
+-rw-r--r--   0 amo        (501) staff       (20)     5463 2024-05-18 21:18:54.000000 tsperf-1.2.0/tsperf/adapter/influxdb.py
+-rw-r--r--   0 amo        (501) staff       (20)     5336 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/adapter/mongodb.py
+-rw-r--r--   0 amo        (501) staff       (20)     5800 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/adapter/mssql.py
+-rw-r--r--   0 amo        (501) staff       (20)     4464 2024-05-18 21:18:54.000000 tsperf-1.2.0/tsperf/adapter/postgresql.py
+-rw-r--r--   0 amo        (501) staff       (20)     6447 2024-05-18 21:18:54.000000 tsperf-1.2.0/tsperf/adapter/timescaledb.py
+-rw-r--r--   0 amo        (501) staff       (20)     7614 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/adapter/timestream.py
+-rw-r--r--   0 amo        (501) staff       (20)    11434 2024-05-20 22:18:22.000000 tsperf-1.2.0/tsperf/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     3220 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/engine.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.464872 tsperf-1.2.0/tsperf/model/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/model/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1955 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/model/configuration.py
+-rw-r--r--   0 amo        (501) staff       (20)     2670 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/model/interface.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.465849 tsperf-1.2.0/tsperf/read/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/read/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     3456 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/read/config.py
+-rw-r--r--   0 amo        (501) staff       (20)     9188 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/read/core.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.466284 tsperf-1.2.0/tsperf/schema/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.467352 tsperf-1.2.0/tsperf/schema/basic/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/basic/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1743 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/basic/demo.json
+-rw-r--r--   0 amo        (501) staff       (20)     3457 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/basic/environment.json
+-rw-r--r--   0 amo        (501) staff       (20)     8210 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/basic/motor.json
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.467848 tsperf-1.2.0/tsperf/schema/factory/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/factory/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.469445 tsperf-1.2.0/tsperf/schema/factory/complex/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/factory/complex/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1340 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/factory/complex/base1.json
+-rw-r--r--   0 amo        (501) staff       (20)     1798 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/factory/complex/base2.json
+-rw-r--r--   0 amo        (501) staff       (20)     1030 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/factory/complex/lower.json
+-rw-r--r--   0 amo        (501) staff       (20)     1032 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/factory/complex/upper.json
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.469943 tsperf-1.2.0/tsperf/schema/factory/simple/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/factory/simple/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1999 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/schema/factory/simple/machine.json
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.470439 tsperf-1.2.0/tsperf/util/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/util/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.470790 tsperf-1.2.0/tsperf/util/batch_size_automator/
+-rw-r--r--   0 amo        (501) staff       (20)    10045 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/util/batch_size_automator/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1534 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/util/common.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.471114 tsperf-1.2.0/tsperf/util/float_simulator/
+-rw-r--r--   0 amo        (501) staff       (20)     7023 2024-05-18 21:16:44.000000 tsperf-1.2.0/tsperf/util/float_simulator/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.471588 tsperf-1.2.0/tsperf/util/tictrack/
+-rw-r--r--   0 amo        (501) staff       (20)     7920 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/util/tictrack/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.472609 tsperf-1.2.0/tsperf/write/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/write/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     4554 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/write/config.py
+-rw-r--r--   0 amo        (501) staff       (20)    16642 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/write/core.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.474171 tsperf-1.2.0/tsperf/write/model/
+-rw-r--r--   0 amo        (501) staff       (20)       98 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/write/model/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     2922 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/write/model/channel.py
+-rw-r--r--   0 amo        (501) staff       (20)     2606 2024-05-18 15:01:58.000000 tsperf-1.2.0/tsperf/write/model/metrics.py
+-rw-r--r--   0 amo        (501) staff       (20)     1028 2024-05-18 21:16:44.000000 tsperf-1.2.0/tsperf/write/model/sensor.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-20 22:45:47.474914 tsperf-1.2.0/tsperf.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     8109 2024-05-20 22:45:47.000000 tsperf-1.2.0/tsperf.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     2278 2024-05-20 22:45:47.000000 tsperf-1.2.0/tsperf.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-05-20 22:45:47.000000 tsperf-1.2.0/tsperf.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       43 2024-05-20 22:45:47.000000 tsperf-1.2.0/tsperf.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2021-06-02 23:40:52.000000 tsperf-1.2.0/tsperf.egg-info/not-zip-safe
+-rw-r--r--   0 amo        (501) staff       (20)      532 2024-05-20 22:45:47.000000 tsperf-1.2.0/tsperf.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       13 2024-05-20 22:45:47.000000 tsperf-1.2.0/tsperf.egg-info/top_level.txt
```

### Comparing `tsperf-1.1.0/LICENSE` & `tsperf-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsperf-1.1.0/batch_size_automator/__init__.py` & `tsperf-1.2.0/tsperf/util/batch_size_automator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,15 @@
                 "times": [],
                 "avg_time": -1,
                 "batch_per_second": 0.0,
             },
         }
         self.alpha = 1.0
         # smaller steps than data_batch_size make no sense at this is the smallest batch_size
-        self.step_size = (
-            step_size if step_size > self.data_batch_size else self.data_batch_size
-        )
+        self.step_size = step_size if step_size > self.data_batch_size else self.data_batch_size
         self.test_size = test_size
         self.default_test_size = test_size
         self.surveillance_mode = False
 
     def get_next_batch_size(self) -> int:
         """
         this function returns the batch_size that should be used for the next insert
@@ -149,67 +147,55 @@
             # if batch_size goes down to a number smaller than data_batch_size
             # it is set to data_batch_size and the direction flipped
             self.bigger_batch_size = not self.bigger_batch_size
             self.batch_size = self.data_batch_size
         else:
             # the batch_size must always be a multitude of self.data_batch_size
             if batch_size % self.data_batch_size != 0:
-                batch_size = self.data_batch_size * round(
-                    batch_size / self.data_batch_size
-                )
+                batch_size = self.data_batch_size * round(batch_size / self.data_batch_size)
             self.batch_size = batch_size
 
     def _calc_better_batch_time(self):
         if self._is_current_batch_size_better():
             # if during surveillance_mode the performance changes quit surveillance
             # and calculate better batch_size faster
             self._adjust_batch_size(True)
         else:
             # if we were in surveillance mode and the performance got worse we want to readjust the batch_size,
             # this means we stop surveillance mode and do a retest over 10 batches with slightly adjusted batch_size.
             if self.surveillance_mode:
                 self._stop_surveillance_mode()
                 self._adjust_batch_size(True)
             else:
-                self.alpha -= (
-                    self.alpha / 10
-                )  # reduce step_size by 10% each calculation
+                self.alpha -= self.alpha / 10  # reduce step_size by 10% each calculation
                 # if step_size is smaller than 100 no more adjustment necessary. batch_size_automator will go into
                 # surveillance mode and only check periodically if batch_performance has gotten worse
                 if self.step_size * self.alpha < 100:
                     self._start_surveillance_mode()
                 else:
                     # if we didn't change into surveillance mode we change the direction of the batch_size adjustment
                     # and let the automator run with a new batch_size
-                    self.bigger_batch_size = (
-                        not self.bigger_batch_size
-                    )  # change direction of batch_size adjustment
+                    self.bigger_batch_size = not self.bigger_batch_size  # change direction of batch_size adjustment
                     self._adjust_batch_size(False)
         # reset current batch_times for next batch_size
         self.batch_times["current"] = {
             "size": self.batch_size,
             "times": [],
             "avg_time": -1,
         }
 
     def _adjust_batch_size(self, take_current: bool):
         if take_current:
             self.batch_times["best"] = self.batch_times["current"]
-        batch_size_change = (
-            self.factors[self.bigger_batch_size] * self.alpha * self.step_size
-        )
+        batch_size_change = self.factors[self.bigger_batch_size] * self.alpha * self.step_size
         # there would be no change in real batch size if the change was less than data_batch_size
         if abs(batch_size_change) < self.data_batch_size:
             # we got to preserve the direction
-            batch_size_change = self.data_batch_size * (
-                batch_size_change / abs(batch_size_change)
-            )
-        self._set_batch_size(
-            round(self.batch_times["best"]["size"] + batch_size_change)
-        )
+            batch_size_change = self.data_batch_size * (batch_size_change / abs(batch_size_change))
+        self._set_batch_size(round(self.batch_times["best"]["size"] + batch_size_change))
 
     def _start_surveillance_mode(self):
         self.test_size = 1000
         self._set_batch_size(self.batch_times["best"]["size"])
         self.surveillance_mode = True
 
     def _stop_surveillance_mode(self):
@@ -219,14 +205,12 @@
 
     def _is_current_batch_size_better(self):
         current_avg = statistics.mean(self.batch_times["current"]["times"])
         self.batch_times["current"]["avg_time"] = current_avg
         best_avg = self.batch_times["best"]["avg_time"]
         best_per_second = self.batch_times["best"]["size"] / best_avg
         current_per_second = self.batch_times["current"]["size"] / current_avg
-        self.batch_times["best"][
-            "batch_per_second"
-        ] = best_per_second  # this is not really necessary
+        self.batch_times["best"]["batch_per_second"] = best_per_second  # this is not really necessary
         self.batch_times["current"]["batch_per_second"] = current_per_second
         current_was_better = current_per_second > best_per_second
         # if best_avg is -1 no best batch_size has been calculated yet
         return best_avg == -1 or current_was_better
```

### Comparing `tsperf-1.1.0/data_generator/__main__.py` & `tsperf-1.2.0/tsperf/write/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,238 +14,202 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
-
-import json
-import urllib3
-import time
 import logging
-import tictrack
-from batch_size_automator import BatchSizeAutomator
-from queue import Queue, Empty
+import time
+from queue import Empty, Queue
 from threading import Thread, current_thread
-from typing import Tuple
-from data_generator.edge import Edge
-from data_generator.db_writer import DbWriter
-from data_generator.crate_db_writer import CrateDbWriter
-from data_generator.timescale_db_writer import TimescaleDbWriter
-from data_generator.influx_db_writer import InfluxDbWriter
-from data_generator.mongo_db_writer import MongoDbWriter
-from data_generator.postgres_db_writer import PostgresDbWriter
-from data_generator.timestream_db_writer import TimeStreamWriter
-from data_generator.mssql_db_writer import MsSQLDbWriter
-from data_generator.config import DataGeneratorConfig
-from data_generator.argument_parser import parse_arguments
-from prometheus_client import start_http_server, Gauge, Counter
-
-
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-logging.basicConfig(
-    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s", level=logging.INFO
-)
+from typing import Optional, Tuple
+
+from prometheus_client import start_http_server
+from tqdm import tqdm
 
-# global variables shared accross threads
-config = DataGeneratorConfig()
-model = {}
+from tsperf.engine import TsPerfEngine, load_schema
+from tsperf.model.interface import AbstractDatabaseInterface
+from tsperf.util import tictrack
+from tsperf.util.batch_size_automator import BatchSizeAutomator
+from tsperf.write.config import DataGeneratorConfig
+from tsperf.write.model import IngestMode
+from tsperf.write.model.channel import Channel
+from tsperf.write.model.metrics import (
+    c_generated_values,
+    c_inserted_values,
+    c_inserts_failed,
+    c_inserts_performed_success,
+    c_values_queue_was_empty,
+    g_batch_size,
+    g_best_batch_rps,
+    g_best_batch_size,
+    g_insert_percentage,
+    g_insert_time,
+    g_rows_per_second,
+)
+
+logger = logging.getLogger(__name__)
+
+
+# Global variables shared across threads
+# TODO: Get rid of global variables.
+engine: TsPerfEngine = None
+config: DataGeneratorConfig = None
+schema = {}
 last_ts = 0
 current_values_queue = Queue(10000)
 inserted_values_queue = Queue(10000)
 stop_queue = Queue(1)
 insert_finished_queue = Queue(1)
-
-# prometheus metrics published to port config.prometheus_port
-c_values_queue_was_empty = Counter(
-    "data_gen_values_queue_empty",
-    "How many times the values_queue was empty when "
-    "insert_routine needed more values",
-)
-c_inserts_performed_success = Counter(
-    "data_gen_inserts_performed_success",
-    "How many times the an insert into the " "database was performed successfully",
-)
-c_inserts_failed = Counter(
-    "data_gen_inserts_failed",
-    "How many times an insert operation failed due to an error",
-)
-c_generated_values = Counter(
-    "data_gen_generated_values", "How many values have been generated"
-)
-c_inserted_values = Counter(
-    "data_gen_inserted_values", "How many values have been inserted"
-)
-g_insert_percentage = Gauge(
-    "data_gen_insert_percentage", "Percentage of values that have been inserted"
-)
-g_batch_size = Gauge(
-    "data_gen_batch_size", "The currently used batch size", labelnames=("thread",)
-)
-g_insert_time = Gauge(
-    "data_gen_insert_time",
-    "The average time it took to insert the current batch into the " "database",
-    labelnames=("thread",),
-)
-g_rows_per_second = Gauge(
-    "data_gen_rows_per_second",
-    "The average number of rows per second with the latest " "batch_size",
-    labelnames=("thread",),
-)
-g_best_batch_size = Gauge(
-    "data_gen_best_batch_size",
-    "The up to now best batch size found by the " "batch_size_automator",
-    labelnames=("thread",),
-)
-g_best_batch_rps = Gauge(
-    "data_gen_best_batch_rps",
-    "The rows per second for the up to now best batch size",
-    labelnames=("thread",),
-)
+insert_exceptions = Queue()
 
 
-def get_db_writer() -> DbWriter:  # noqa
+def get_database_adapter_old() -> AbstractDatabaseInterface:  # pragma: no cover
+    """
     if config.database == 0:  # crate
-        db_writer = CrateDbWriter(
-            config.host,
-            config.username,
-            config.password,
-            model,
-            config.table_name,
-            config.shards,
-            config.replicas,
-            config.partition,
-        )
+        adapter = CrateDbAdapter(config=config, schema=schema)
+        # adapter = AdapterManager.create(
+        #    interface=DatabaseInterfaceType.CrateDB, config=config, schema=schema
+        # )
     elif config.database == 1:  # timescale
-        db_writer = TimescaleDbWriter(
-            config.host,
+        adapter = TimescaleDbAdapter(
+            config.address,
             config.port,
             config.username,
             config.password,
-            config.db_name,
-            model,
-            config.table_name,
+            config.database,
+            schema,
+            config.table,
             config.partition,
             config.copy,
             config.distributed,
         )
     elif config.database == 2:  # influx
-        db_writer = InfluxDbWriter(
-            config.host, config.token, config.organization, model, config.db_name
+        adapter = InfluxDbAdapter(
+            config.address, config.token, config.organization, schema, config.database
         )
     elif config.database == 3:  # mongo
-        db_writer = MongoDbWriter(
-            config.host, config.username, config.password, config.db_name, model
+        adapter = MongoDbAdapter(
+            config.address, config.username, config.password, config.database, schema
         )
     elif config.database == 4:  # postgres
-        db_writer = PostgresDbWriter(
-            config.host,
+        adapter = PostgreSQLAdapter(
+            config.address,
             config.port,
             config.username,
             config.password,
-            config.db_name,
-            model,
-            config.table_name,
+            config.database,
+            schema,
+            config.table,
             config.partition,
         )
     elif config.database == 5:  # timestream
-        db_writer = TimeStreamWriter(
+        adapter = AmazonTimestreamAdapter(
             config.aws_access_key_id,
             config.aws_secret_access_key,
             config.aws_region_name,
-            config.db_name,
-            model,
+            config.database,
+            schema,
         )
     elif config.database == 6:  # ms_sql
-        db_writer = MsSQLDbWriter(
-            config.host,
+        adapter = MsSQLDbAdapter(
+            config.address,
             config.username,
             config.password,
-            config.db_name,
-            model,
+            config.database,
+            schema,
             port=config.port,
-            table_name=config.table_name,
+            table=config.table,
         )
     else:
-        db_writer = None
-    return db_writer
+        adapter = None
+    return adapter
+    """
 
 
 @tictrack.timed_function()
-def create_edges() -> dict:
-    # this function creates metric objects in the given range [id_start, id_end]
-    edges = {}
-    for i in range(config.id_start, config.id_end + 1):
-        edges[i] = Edge(i, get_sub_element("tags"), get_sub_element("metrics"))
-    return edges
+def create_channels() -> dict:
+    """
+    Create channel objects in the given range [id_start, id_end]
+    """
+    id_start = config.id_start
+    id_end = config.id_end + 1
+    count = id_end - id_start
+    logger.info(f"Creating {count} channels [{id_start}, {id_end}]")
+    channels = {}
+    for i in tqdm(range(config.id_start, config.id_end + 1)):
+        channels[i] = Channel(i, get_sub_element("tags"), get_sub_element("fields"))
+    return channels
 
 
 def get_sub_element(sub: str) -> dict:
     element = {}
-    for key in model.keys():
-        if key != "description" and sub in model[key]:
-            element = model[key][sub]
+    for key in schema.keys():
+        if key != "description" and sub in schema[key]:
+            element = schema[key][sub]
     if "description" in element:
         element.pop("description")
     return element
 
 
 @tictrack.timed_function()
-def get_next_value(edges: dict):
+def get_next_value(channels: dict):
     global last_ts
-    # for each edge in the edges list all next values are calculated and saved to the edge_value list
-    # this list is then added to the FIFO queue, so each entry of the FIFO queue contains all next values for each edge
-    # in the edge list
-    edge_values = []
-    for edge in edges.values():
-        edge_values.append(edge.calculate_next_value())
-    if len(edge_values) > 0:
-        c_generated_values.inc(len(edge_values))
-        if config.ingest_mode == 1:
-            ts = last_ts + config.ingest_delta
-            ingest_ts_factor = 1 / config.ingest_delta
-            last_ts = round(ts * ingest_ts_factor) / ingest_ts_factor
-            timestamps = [int(last_ts * 1000)] * len(edge_values)
-            current_values_queue.put({"timestamps": timestamps, "batch": edge_values})
+    # for each channel in the channels list all next values are calculated and
+    # saved to the `channel_values` list. This list is then added to the FIFO
+    # queue, so each entry of the FIFO queue contains all next values for each
+    # channel in the channel list.
+    channel_values = []
+    for channel in channels.values():
+        channel_values.append(channel.calculate_next_value())
+    if len(channel_values) > 0:
+        c_generated_values.inc(len(channel_values))
+        if config.ingest_mode == IngestMode.FAST:
+            ts = last_ts + config.timestamp_delta
+            timestamp_factor = 1 / config.timestamp_delta
+            last_ts = round(ts * timestamp_factor) / timestamp_factor
+            timestamps = [int(last_ts * 1000)] * len(channel_values)
+            current_values_queue.put({"timestamps": timestamps, "batch": channel_values})
         else:
-            current_values_queue.put(edge_values)
+            current_values_queue.put(channel_values)
 
 
-def log_stat_delta(last_stat_ts_local: float) -> float:
-    if time.time() - last_stat_ts_local >= config.stat_delta:
+def statistics_logger(last_stat_ts_local: float) -> float:
+    if time.time() - last_stat_ts_local >= config.statistics_interval:
         for key, value in tictrack.tic_toc_delta.items():
-            logging.info(f"average time for {key}: {(sum(value) / len(value))}")
+            logger.info(f"Average time for {key}: {(sum(value) / len(value))}")
         tictrack.tic_toc_delta = {}
     return time.time()
 
 
-def stat_delta_thread_function():  # pragma: no cover
+def statistics_thread():
+    logger.info("Starting statistics thread")
     last_stat_ts_local = time.time()
     while not stop_process():
-        if time.time() - last_stat_ts_local >= config.stat_delta:
-            last_stat_ts_local = log_stat_delta(last_stat_ts_local)
+        if time.time() - last_stat_ts_local >= config.statistics_interval:
+            last_stat_ts_local = statistics_logger(last_stat_ts_local)
         else:
             # we could calculate the exact time to sleep until next output but this would block the
             # the thread until it happens, this would mean at the end the whole data generator could
-            # sleep for another `config.stat_delta` seconds before finishing
+            # sleep for another `config.statistics_interval` seconds before finishing
             time.sleep(1)
 
 
-def do_insert(db_writer, timestamps, batch):
+def do_insert(adapter, timestamps, batch):
     try:
-        db_writer.insert_stmt(timestamps, batch)
+        adapter.insert_stmt(timestamps, batch)
         c_inserts_performed_success.inc()
         inserted_values_queue.put_nowait(len(batch))
     except Exception as e:
-        # if an exception is thrown while inserting we don't want the whole data_generator to crash
-        # as the values have not been inserted we remove them from our runtime_metrics
-        # TODO: more sophistic error handling on db_writer level
+        # if an exception is thrown while inserting we don't want the whole write to crash
+        # as the values have not been inserted we remove them from our runtime metrics
+        # TODO: more sophistic error handling on adapter level
         c_inserts_failed.inc()
-        logging.error(e)
+        logger.error(e)
 
 
 def get_insert_values(batch_size: int) -> Tuple[list, list]:
     batch = []
     timestamps = []
     while len(batch) < batch_size:
         try:
@@ -256,199 +220,238 @@
             # if there are no more values in the queue the insert is done
             # without proper batch_size
             c_values_queue_was_empty.inc()
             break
     return batch, timestamps
 
 
+def probe_insert():
+    logger.info("Probing insert")
+    try:
+        engine.create_adapter().prepare_database()
+        return True
+    except Exception:
+        logger.exception("Failure communicating with or preparing database")
+        return False
+
+
 def insert_routine():
     name = current_thread().name
-    db_writer = get_db_writer()
-    db_writer.prepare_database()
     data_batch_size = config.id_end - config.id_start + 1
     insert_bsa = BatchSizeAutomator(
         batch_size=config.batch_size,
         active=bool(config.ingest_mode),
         data_batch_size=data_batch_size,
     )
 
+    adapter = engine.create_adapter()
     while not current_values_queue.empty() or not stop_process():
         local_batch_size = insert_bsa.get_next_batch_size()
         if insert_bsa.auto_batch_mode:
             g_batch_size.labels(thread=name).set(local_batch_size)
 
         batch, timestamps = get_insert_values(local_batch_size)
 
         if len(batch) > 0:
             start = time.time()
-            do_insert(db_writer, timestamps, batch)
+            do_insert(adapter, timestamps, batch)
 
             if insert_bsa.auto_batch_mode and len(batch) == local_batch_size:
                 duration = time.time() - start
                 g_insert_time.labels(thread=name).set(duration)
                 g_rows_per_second.labels(thread=name).set(len(batch) / duration)
-                g_best_batch_size.labels(thread=name).set(
-                    insert_bsa.batch_times["best"]["size"]
-                )
-                g_best_batch_rps.labels(thread=name).set(
-                    insert_bsa.batch_times["best"]["batch_per_second"]
-                )
+                g_best_batch_size.labels(thread=name).set(insert_bsa.batch_times["best"]["size"])
+                g_best_batch_rps.labels(thread=name).set(insert_bsa.batch_times["best"]["batch_per_second"])
                 insert_bsa.insert_batch_time(duration)
 
-    db_writer.close_connection()
+    adapter.close_connection()
+
+    return True
 
 
-def spawn_insert_threads():  # pragma: no cover
+def spawn_insert_threads():
+    logger.info(f"Starting {config.concurrency} database writer thread(s)")
     insert_threads = []
-    for i in range(config.num_threads):
-        insert_threads.append(Thread(target=insert_routine, name=f"insert_thread_{i}"))
+    for i in range(config.concurrency):
+        insert_threads.append(Thread(target=insert_routine, name=f"InsertThread-{i}"))
     for thread in insert_threads:
         thread.start()
     for thread in insert_threads:
         thread.join()
-    # signal the prometheus thread that insert is finished
+
+    # Signal the Prometheus thread that insert is finished.
     insert_finished_queue.put_nowait(True)
 
 
-def fast_insert():  # pragma: no cover
+def fast_insert():
     fast_insert_threads = [
-        Thread(target=spawn_insert_threads, name="spawn_insert_threads"),
-        Thread(target=stat_delta_thread_function, name="stat_delta_thread"),
+        Thread(target=spawn_insert_threads, name="InsertThreadSpawner"),
+        Thread(target=statistics_thread, name="StatisticsThread"),
     ]
     for thread in fast_insert_threads:
         thread.start()
     for thread in fast_insert_threads:
         thread.join()
 
 
 def consecutive_insert():
     global last_ts
-    db_writer = get_db_writer()
-    db_writer.prepare_database()
-    last_insert = config.ingest_ts
+    logger.info("Starting single database writer thread")
+    adapter = engine.create_adapter()
+
+    adapter.prepare_database()
+    last_insert = config.timestamp_start
     last_stat_ts_local = time.time()
     while not current_values_queue.empty() or not stop_process():
         # we calculate the time delta from the last insert to the current timestamp
         insert_delta = time.time() - last_insert
-        # delta needs to be bigger than ingest_delta
-        # if delta is smaller than ingest_delta the time difference is waited (as we want an insert
-        # every `config.ingest_delta` second
-        if insert_delta > config.ingest_delta:
-            last_stat_ts_local = log_stat_delta(last_stat_ts_local)
+        # delta needs to be bigger than timestamp_delta
+        # if delta is smaller than timestamp_delta the time difference is waited (as we want an insert
+        # every `config.timestamp_delta` second
+        if insert_delta > config.timestamp_delta:
+            last_stat_ts_local = statistics_logger(last_stat_ts_local)
             c_inserted_values.inc(config.id_end - config.id_start + 1)
             try:
                 batch = current_values_queue.get_nowait()
                 ts = time.time()
                 # we want the same timestamp for each value this timestamp should be the same
-                # even if the data_generator runs in multiple containers therefore we round the
-                # timestamp to match ingest_delta this is done by multiplying
-                # by ingest_delta and then dividing the result by ingest_delta
-                ingest_ts_factor = 1 / config.ingest_delta
-                last_insert = round(ts * ingest_ts_factor) / ingest_ts_factor
+                # even if the write runs in multiple containers therefore we round the
+                # timestamp to match timestamp_delta this is done by multiplying
+                # by timestamp_delta and then dividing the result by timestamp_delta
+                timestamp_factor = 1 / config.timestamp_delta
+                last_insert = round(ts * timestamp_factor) / timestamp_factor
                 timestamps = [int(last_insert * 1000)] * len(batch)
-                do_insert(db_writer, timestamps, batch)
+                do_insert(adapter, timestamps, batch)
             except Empty:
                 c_values_queue_was_empty.inc()
 
         else:
-            time.sleep(config.ingest_delta - insert_delta)
-    db_writer.close_connection()
-    # signal the prometheus thread that insert is finished
+            time.sleep(config.timestamp_delta - insert_delta)
+    adapter.close_connection()
+
+    # Signal the Prometheus thread that insert is finished.
     insert_finished_queue.put_nowait(True)
 
 
 def stop_process() -> bool:
     return not stop_queue.empty()
 
 
-def prometheus_insert_percentage():  # pragma: no cover
+def prometheus_insert_percentage():
     while not inserted_values_queue.empty() or insert_finished_queue.empty():
         try:
             inserted_values = inserted_values_queue.get_nowait()
             c_inserted_values.inc(inserted_values)
             g_insert_percentage.set(
-                (
-                    c_inserted_values._value.get()
-                    / (config.ingest_size * (config.id_end - config.id_start + 1))
-                )
-                * 100
+                (c_inserted_values._value.get() / (config.ingest_size * (config.id_end - config.id_start + 1))) * 100
             )
         except Empty:
             # get_nowait throws Empty exception which might happen if the inserted_values_queue
             # is empty and the insert_finished_queue is as well
             pass
 
 
 @tictrack.timed_function()
-def run_dg():  # pragma: no cover
-    # start the thread that writes to the db
-    if config.ingest_mode == 0:
-        db_writer_thread = Thread(
-            target=consecutive_insert, name="consecutive_insert_thread"
-        )
+def run_dg():
+    logger.info(f"Starting data generator with config »{config}« and schema »{config.schema}«")
+
+    logger.info("Starting database writer subsystem")
+    if config.ingest_mode == IngestMode.CONSECUTIVE:
+        logger.info("Using insert mode »consecutive«")
+        adapter_thread = Thread(target=consecutive_insert, name="ConsecutiveInsert")
     else:
-        db_writer_thread = Thread(target=fast_insert, name="fast_insert_thread")
-    db_writer_thread.start()
+        logger.info("Using insert mode »fast«")
+        adapter_thread = Thread(target=fast_insert, name="ParallelInsert")
+    adapter_thread.start()
 
-    # start the thread that collects the insert metrics from the db_writer threads
-    prometheus_insert_percentage_thread = Thread(
-        target=prometheus_insert_percentage, name="prometheus_insert_percentage_thread"
-    )
+    logger.info("Starting metrics collector thread")
+    prometheus_insert_percentage_thread = Thread(target=prometheus_insert_percentage, name="PrometheusThread")
     prometheus_insert_percentage_thread.start()
 
     try:
-        edges = create_edges()
+        channels = create_channels()
 
-        # TODO: this should not have an endless loop for now stop with ctrl+C
-        # we are either in endless mode or have a certain amount of values to create
+        # We are either in endless mode or have a certain amount of values to create.
+        # TODO: This should not have an endless loop. For now, stop with CTRL+C.
+        logger.info(f"Starting insert operation with ingest size {config.ingest_size}")
         while_count = 0
+        progress = tqdm(total=config.ingest_size)
         while config.ingest_size == 0 or while_count < config.ingest_size:
             while_count += 1
-            get_next_value(edges)
+            get_next_value(channels)
+            progress.update()
+        progress.close()
     except Exception as e:
-        logging.exception(e)
+        logger.exception(e)
     finally:
-        # once value creation is finished we signal the other threads to stop and wait for them to join
+        # Once value creation is finished, signal the worker threads to stop.
+        logger.info("Shutting down")
         stop_queue.put(True)
-        db_writer_thread.join()
-        prometheus_insert_percentage_thread.join()
-
-
-def main():  # pragma: no cover
-    global last_ts, model, config
+        logger.info("Waiting for database writer thread(s)")
+        wait_for_thread(adapter_thread, insert_exceptions)
 
-    # load configuration an set everything up
-    config = parse_arguments(config)
-    valid_config = config.validate_config()
-    if not valid_config:
-        logging.error(f"invalid configuration: {config.invalid_configs}")
-        exit(-1)
-
-    f = open(config.model_path, "r")
-    model = json.load(f)
+        if config.prometheus_enable:
+            logger.info("Waiting for metrics collector thread")
+            prometheus_insert_percentage_thread.join()
+
+
+def wait_for_thread(thread: Thread, error_channel: Optional[Queue] = None):
+    """
+    Wait for thread to finish and, on failure, catch the thread's exception in
+    the caller thread.
+
+    - https://stackoverflow.com/a/2830127
+    """
+    while True:
+        if error_channel:
+            try:
+                exc = error_channel.get(block=False)
+            except Empty:
+                pass
+            else:
+                exc_type, exc_obj, exc_trace = exc
+                # Re-raise the exception.
+                raise exc_obj
+
+        thread.join(0.1)
+        if thread.is_alive():
+            continue
+        break
+
+
+def start(configuration: DataGeneratorConfig):
+    # TODO: Get rid of global variables.
+    global engine, config
+    global schema, last_ts
+
+    # TODO: Move schema loading to engine.
+    schema = load_schema(configuration.schema)
+    engine = TsPerfEngine(config=configuration, schema=schema)
+    engine.bootstrap()
+
+    # TODO: Get rid of global variables.
+    config = engine.config
+
+    if not probe_insert():
+        raise Exception(f"Failure communicating with or preparing database at {config.address}")
+
+    if config.prometheus_enable:
+        logger.info(f"Starting Prometheus HTTP server on {config.prometheus_host}:{config.prometheus_port}")
+        start_http_server(config.prometheus_port, addr=config.prometheus_host)
 
-    start_http_server(config.prometheus_port)
     data_batch_size = config.id_end - config.id_start + 1
-    last_ts = config.ingest_ts
+    last_ts = config.timestamp_start
 
-    # start the data_generator logic
+    # start the write logic
     run_dg()
 
     # we analyze the runtime of the different function
     run = 0
     for k, v in tictrack.tic_toc.items():
         if k == "run_dg":
             run = sum(v) / len(v)
-        logging.info(f"average time for {k}: {(sum(v) / len(v))}")
+        logger.info(f"Average time for {k}: {(sum(v) / len(v))}")
 
-    logging.info(
-        f"""rows per second:    {data_batch_size * config.ingest_size / run}"""
-    )
-    logging.info(
-        f"""metrics per second: {data_batch_size * config.ingest_size * len(get_sub_element("metrics").keys()) / run}"""
+    logger.info(
+        f"Values per second: {data_batch_size * config.ingest_size * len(get_sub_element('fields').keys()) / run}"
     )
-
-    # finished
-
-
-if __name__ == "__main__":  # pragma: no cover
-    main()
+    logger.info(f"Records per second: {data_batch_size * config.ingest_size / run}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tsperf-1.1.0/data_generator/crate_db_writer.py` & `tsperf-1.2.0/tsperf/adapter/cratedb.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,63 +14,83 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
+import logging
+from typing import Dict, Optional, Union
 
-from data_generator.db_writer import DbWriter
 from crate import client
-from tictrack import timed_function
 
+from tsperf.adapter import AdapterManager
+from tsperf.model.interface import AbstractDatabaseInterface, DatabaseInterfaceType
+from tsperf.read.config import QueryTimerConfig
+from tsperf.util.tictrack import timed_function
+from tsperf.write.config import DataGeneratorConfig
+
+logger = logging.getLogger(__name__)
+
+
+class CrateDbAdapter(AbstractDatabaseInterface):
+    default_address = "localhost:4200"
+    default_username = "crate"
+    default_query = "SELECT 1;"
 
-class CrateDbWriter(DbWriter):
     def __init__(
         self,
-        host: str,
-        username: str,
-        password: str,
-        model: dict,
-        table_name: str = None,
-        shards: int = None,
-        replicas: int = None,
-        partition: str = "week",
+        config: Union[DataGeneratorConfig, QueryTimerConfig],
+        schema: Optional[Dict] = None,
     ):
         super().__init__()
-        self.conn = client.connect(host, username=username, password=password)
+
+        self.conn = client.connect(config.address, username=config.username, password=config.password)
         self.cursor = self.conn.cursor()
-        self.model = model
-        self.table_name = (table_name, self._get_model_table_name())[
-            table_name is None or table_name == ""
-        ]
-        self.shards = (shards, 21)[shards is None]
-        self.replicas = (replicas, 1)[replicas is None]
-        self.partition = partition
+        self.schema = schema
+        self.table_name = (config.table, self._get_schema_table_name())[config.table is None or config.table == ""]
+        self.partition = config.partition
+
+        logger.info(f"Configuring CrateDB with {config.shards} shards and {config.replicas} replicas")
+        self.shards = config.shards
+        self.replicas = config.replicas
 
     def close_connection(self):
         self.cursor.close()
         self.conn.close()
 
     def prepare_database(self):
-        stmt = f"""CREATE TABLE IF NOT EXISTS {self.table_name} ("ts" TIMESTAMP WITH TIME ZONE,
+        # Drop table.
+        stmt = f"DROP TABLE IF EXISTS {self.table_name}"
+        self.cursor.execute(stmt)
+
+        # Create table.
+        stmt = f"""CREATE TABLE {self.table_name} ("ts" TIMESTAMP WITH TIME ZONE,
  "g_ts_{self.partition}" TIMESTAMP WITH TIME ZONE GENERATED ALWAYS AS date_trunc('{self.partition}', "ts"),
  "payload" OBJECT(DYNAMIC))
  CLUSTERED INTO {self.shards} SHARDS
  PARTITIONED BY ("g_ts_{self.partition}")
  WITH (number_of_replicas = {self.replicas})"""
+        logger.info(f"Preparing database with statement:\n{stmt}")
         self.cursor.execute(stmt)
 
     @timed_function()
     def insert_stmt(self, timestamps: list, batch: list):
-        stmt = f"""INSERT INTO {self.table_name} (ts, payload) (SELECT col1, col2 FROM UNNEST(?,?))"""
+        stmt = f"""INSERT INTO {self.table_name} (ts, payload) (SELECT col1, col2 FROM UNNEST(?,?))"""  # noqa: S608
         self.cursor.execute(stmt, (timestamps, batch))
 
     @timed_function()
     def execute_query(self, query: str) -> list:
+        return self.run_query(query)
+
+    def run_query(self, query: str) -> list:
         self.cursor.execute(query)
         return self.cursor.fetchall()
 
-    def _get_model_table_name(self) -> str:
-        for key in self.model.keys():
+    def _get_schema_table_name(self) -> str:
+        for key in self.schema.keys():
             if key != "description":
                 return key
+        raise ValueError("Unable to determine table name")
+
+
+AdapterManager.register(interface=DatabaseInterfaceType.CrateDB, factory=CrateDbAdapter)
```

### Comparing `tsperf-1.1.0/data_generator/db_writer.py` & `tsperf-1.2.0/tsperf/model/interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,43 +14,71 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
+from abc import abstractmethod
+from enum import Enum
 
 
-class DbWriter:
+class DatabaseInterfaceType(Enum):
+    CrateDB = "cratedb"
+    CrateDBpg = "cratedbpg"
+    Dummy = "dummy"
+    InfluxDB = "influxdb"
+    MicrosoftSQL = "mssql"
+    MongoDB = "mongodb"
+    PostgreSQL = "postgresql"
+    TimescaleDB = "timescaledb"
+    Timestream = "timestream"
+
+
+class AbstractDatabaseInterface:
+    default_address = None
+    default_username = None
+    default_database = None
+    default_query = None
+
+    @abstractmethod
     def __init__(self):
         pass
 
+    @abstractmethod
     def connect_to_database(self):  # pragma: no cover
         pass
 
-    def close_connection(self):  # pragma: no cover
+    @abstractmethod
+    def prepare_database(self):  # pragma: no cover
         pass
 
-    def prepare_database(self):  # pragma: no cover
+    @abstractmethod
+    def close_connection(self):  # pragma: no cover
         pass
 
+    @abstractmethod
     def insert_stmt(self, timestamps: list, batch: list):  # pragma: no cover
         pass
 
+    @abstractmethod
     def execute_query(self, query: str):  # pragma: no cover
         pass
 
-    def _get_tags_and_metrics(self):
-        key = self._get_model_table_name()
-        tags = self.model[key]["tags"]
-        metrics = self.model[key]["metrics"]
+    def _get_schema_table_name(self) -> str:
+        pass
+
+    def _get_tags_and_fields(self):
+        key = self._get_schema_table_name()
+        tags = self.schema[key]["tags"]
+        fields = self.schema[key]["fields"]
         columns = {}
         for key, value in tags.items():
             if key != "description":
                 if type(value).__name__ == "list":
                     columns[key] = "TEXT"
                 else:
                     columns[key] = "INTEGER"
-        for key, value in metrics.items():
+        for key, value in fields.items():
             if key != "description":
                 columns[value["key"]["value"]] = value["type"]["value"]
         return columns
```

### Comparing `tsperf-1.1.0/data_generator/influx_db_writer.py` & `tsperf-1.2.0/tsperf/adapter/influxdb.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,89 +14,131 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
+import logging
+from datetime import datetime
+from typing import Dict, Optional, Tuple, Union
 
-from typing import Tuple
-
-from tictrack import timed_function
-from data_generator.db_writer import DbWriter
-from influxdb_client import InfluxDBClient, Bucket
+from influxdb_client import Bucket, InfluxDBClient
 from influxdb_client.client.write_api import SYNCHRONOUS, Point
-from datetime import datetime
 
+from tsperf.adapter import AdapterManager
+from tsperf.model.interface import AbstractDatabaseInterface, DatabaseInterfaceType
+from tsperf.read.config import QueryTimerConfig
+from tsperf.util.tictrack import timed_function
+from tsperf.write.config import DataGeneratorConfig
+
+logger = logging.getLogger(__name__)
+
+
+class InfluxDbAdapter(AbstractDatabaseInterface):
+    default_address = "http://localhost:8086/"
 
-class InfluxDbWriter(DbWriter):
     def __init__(
-        self, host: str, token: str, org: str, model: dict, database_name: str = None
+        self,
+        config: Union[DataGeneratorConfig, QueryTimerConfig],
+        schema: Optional[Dict] = None,
     ):
         super().__init__()
-        self.client = InfluxDBClient(url=host, token=token)
+
+        logger.info(
+            f"Connecting to InfluxDB at {config.address} with organization "
+            f"{config.influxdb_organization} and token {config.influxdb_token}"
+        )
+        self.client = InfluxDBClient(
+            url=config.address,
+            token=config.influxdb_token,
+            org=config.influxdb_organization,
+        )
         self.write_api = self.client.write_api(write_options=SYNCHRONOUS)
         self.query_api = self.client.query_api()
-        self.org = org
-        self.model = model
+        self.organization = config.influxdb_organization
+        self.schema = schema or {}
         self.bucket = None
-        self.database_name = (database_name, self._get_model_database_name())[
+
+        database_name = config.database
+        self.database_name = (database_name, self._get_schema_database_name())[
             database_name is None or database_name == ""
         ]
+        logger.info(f"Using InfluxDB bucket »{self.database_name}«")
 
     def close_connection(self):
         self.client.close()
 
     def prepare_database(self):
         buckets = self.client.buckets_api().find_buckets()
         for bucket in buckets.buckets:
             if bucket.name == self.database_name:
                 self.bucket = bucket
 
         if self.bucket is None:
-            bucket = Bucket(
-                name=self.database_name, org_id=self.org, retention_rules=[]
-            )
+            if self.client.__class__.__name__ == "Mock":
+                org_id = "Mock12345"
+            else:
+                org = self._get_first_organization()
+                org_id = org.id
+            logger.info(f"Creating InfluxDB bucket {bucket.name} in organization {org_id}")
+            bucket = Bucket(name=self.database_name, org_id=org_id, retention_rules=[])
             self.bucket = self.client.buckets_api().create_bucket(bucket)
 
+    def _get_first_organization(self):
+        org = list(
+            filter(
+                lambda it: it.name == self.organization,
+                self.client.organizations_api().find_organizations(),
+            )
+        )[0]
+        return org
+
     @timed_function()
     def insert_stmt(self, timestamps: list, batch: list):
         data = self._prepare_influx_stmt(timestamps, batch)
-        self.write_api.write(bucket=self.database_name, org=self.org, record=data)
+        self.write_api.write(bucket=self.database_name, org=self.organization, record=data)
 
     @timed_function()
     def _prepare_influx_stmt(self, timestamps: list, batch: list) -> list:
         data = []
-        tags, metrics = self._get_tags_and_metrics()
+        tags, fields = self._get_tags_and_fields()
         for i in range(0, len(batch)):
             t = datetime.fromtimestamp(timestamps[i] / 1000)
             point = Point(self.database_name).time(t)
             for tag in tags:
                 point.tag(tag, batch[i][tag])
-            for metric in metrics:
-                point.field(metric, batch[i][metric])
+            for field in fields:
+                point.field(field, batch[i][field])
             data.append(point)
 
         return data
 
     @timed_function()
     def execute_query(self, query: str) -> list:
-        return self.query_api.query(query)
+        return self.run_query(query)
 
-    def _get_tags_and_metrics(self) -> Tuple[dict, dict]:
-        key = self._get_model_database_name()
-        tags_ = self.model[key]["tags"]
-        metrics_ = self.model[key]["metrics"]
+    def run_query(self, query: str) -> list:
+        return self.query_api.query(query, org=self.organization)
+
+    def _get_tags_and_fields(self) -> Tuple[dict, dict]:
+        key = self._get_schema_database_name()
+        tags_ = self.schema[key]["tags"]
+        fields_ = self.schema[key]["fields"]
         tags = []
-        metrics = []
-        for key, value in tags_.items():
+        fields = []
+        for key in tags_.keys():
             if key != "description":
                 tags.append(key)
-        for key, value in metrics_.items():
+        for key, value in fields_.items():
             if key != "description":
-                metrics.append(value["key"]["value"])
-        return tags, metrics
+                fields.append(value["key"]["value"])
+        return tags, fields
 
-    def _get_model_database_name(self) -> str:
-        for key in self.model.keys():
+    def _get_schema_database_name(self) -> str:
+        for key in self.schema.keys():
             if key != "description":
                 return key
+        raise ValueError("Unable to determine database name")
+
+
+AdapterManager.register(interface=DatabaseInterfaceType.InfluxDB, factory=InfluxDbAdapter)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tsperf-1.1.0/data_generator/mssql_db_writer.py` & `tsperf-1.2.0/tsperf/adapter/mongodb.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,118 +14,135 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
+import json
+import logging
+from datetime import datetime
+from typing import Dict, Optional, Tuple, Union
 
-from typing import Tuple
+from pymongo import MongoClient
+
+from tsperf.adapter import AdapterManager, DatabaseInterfaceMixin
+from tsperf.model.interface import AbstractDatabaseInterface, DatabaseInterfaceType
+from tsperf.read.config import QueryTimerConfig
+from tsperf.util.tictrack import timed_function
+from tsperf.write.config import DataGeneratorConfig
+
+logger = logging.getLogger(__name__)
 
-import pyodbc
-from tictrack import timed_function
-from data_generator.db_writer import DbWriter
-from datetime import datetime
 
+class MongoDbAdapter(AbstractDatabaseInterface, DatabaseInterfaceMixin):
+    default_address = "localhost:27017"
+    default_database = "tsperf"
 
-class MsSQLDbWriter(DbWriter):
     def __init__(
         self,
-        host: str,
-        username: str,
-        password: str,
-        db_name: str,
-        model: dict,
-        port: int = 1433,
-        table_name: str = None,
+        config: Union[DataGeneratorConfig, QueryTimerConfig],
+        schema: Optional[Dict] = None,
     ):
+        DatabaseInterfaceMixin.__init__(self, config=config)
         super().__init__()
-        driver = "{ODBC Driver 17 for SQL Server}"
-        connection_string = (
-            f"DRIVER={driver};SERVER={host},{port};DATABASE={db_name};"
-            f"UID={username};PWD={password};CONNECTION TIMEOUT=170000;"
+        self.schema = schema
+
+        if "://" in self.config.address:
+            connection_string = self.config.address
+
+        else:
+            # Compute credentials.
+            credentials = ""
+            if self.username:
+                credentials += self.username
+                if config.password:
+                    credentials += ":" + config.password
+                credentials += "@"
+
+            if self.host == "localhost":
+                connection_string = f"""mongodb://{credentials}{self.host}"""
+            else:
+                connection_string = f"""mongodb+srv://{credentials}{self.host}"""
+
+        self.collection_name = self._get_schema_collection_name()
+
+        logger.info(
+            f"Connecting to MongoDB at »{connection_string}« "
+            f"with database »{self.database}« and collection »{self.collection_name}«"
         )
-        self.conn = pyodbc.connect(connection_string)
-        self.cursor = self.conn.cursor()
-        self.cursor.fast_executemany = True
-        self.model = model
-        self.table_name = (table_name, self._get_model_table_name())[
-            table_name is None or table_name == ""
-        ]
+        self.client = MongoClient(connection_string)
+        self.db = self.client[self.database]
+        self.collection = self.db[self.collection_name]
+
+    def close_connection(self):
+        self.client.close()
 
     def prepare_database(self):
-        columns = self._get_tags_and_metrics()
-        stmt = f"""
-IF NOT EXISTS (SELECT * FROM sysobjects WHERE id = object_id(N'{self.table_name}')
-AND OBJECTPROPERTY(id, N'IsUserTable') = 1) CREATE TABLE {self.table_name} (
-ts DATETIME NOT NULL,
-"""
-        for key, value in columns.items():
-            stmt += f"""{key} {value},"""
-
-        stmt += f" CONSTRAINT PK_{self.table_name} PRIMARY KEY (ts, "
-        tags = list(self.model[self._get_model_table_name()]["tags"].keys())
-        for tag in tags:
-            if tag != "description":
-                stmt += f"{tag}, "
-        stmt = stmt.rstrip(", ") + "));"
+        """
+        Communicate with database server.
 
-        self.cursor.execute(stmt)
-        self.conn.commit()
+        https://stackoverflow.com/a/12014215
+        """
+        logger.info("dbstats:   %s", self.db.command("dbstats"))
+        # TODO: logger.info("collstats: %s", self.db.command("collstats", self.collection_name))
 
     @timed_function()
     def insert_stmt(self, timestamps: list, batch: list):
-        stmt, params = self._prepare_mssql_stmt(timestamps, batch)
-        self.cursor.executemany(stmt, params)
-        self.conn.commit()
+        data = self._prepare_mongo_stmt(timestamps, batch)
+        self.collection.insert_many(data)
 
     @timed_function()
-    def _prepare_mssql_stmt(self, timestamps: list, batch: list) -> Tuple[str, list]:
-        columns = self._get_tags_and_metrics().keys()
-        stmt = f"""INSERT INTO {self.table_name} (ts ,"""
-        for column in columns:
-            stmt += f"""{column}, """
-
-        stmt = stmt.rstrip(", ") + ") VALUES (?, "
-
-        for column in columns:
-            stmt += "?, "
-
-        stmt = stmt.rstrip(", ") + ")"
-
-        params = []
+    def _prepare_mongo_stmt(self, timestamps: list, batch: list) -> list:
+        data = []
+        tags, fields = self._get_tags_and_fields()
         for i in range(0, len(batch)):
             t = datetime.fromtimestamp(timestamps[i] / 1000)
-            row = [t]
-            for column in columns:
-                row.append(batch[i][column])
-            params.append(row)
-        return stmt, params
+            document = {
+                "measurement": self._get_schema_collection_name(),
+                "date": t,
+                "tags": {},
+                "fields": {},
+            }
+            for tag in tags:
+                document["tags"][tag] = batch[i][tag]
+            for field in fields:
+                document["fields"][field] = batch[i][field]
+            data.append(document)
+        return data
 
     @timed_function()
-    def execute_query(self, query: str) -> list:
-        self.cursor.execute(query)
-        return self.cursor.fetchall()
-
-    def _get_tags_and_metrics(self) -> dict:
-        key = self._get_model_table_name()
-        tags = self.model[key]["tags"]
-        metrics = self.model[key]["metrics"]
-        columns = {}
-        for key, value in tags.items():
+    def execute_query(self, query: Dict) -> list:
+        return self.run_query(query)
+
+    def run_query(self, query: Dict) -> list:
+        if query is None:
+            query = {}
+        elif isinstance(query, Dict):
+            pass
+        else:
+            query = json.loads(query)
+        cursor = self.collection.find(query).limit(10)
+        return list(cursor)
+
+    def _get_tags_and_fields(self) -> Tuple[dict, dict]:
+        key = self._get_schema_collection_name()
+        tags_ = self.schema[key]["tags"]
+        fields_ = self.schema[key]["fields"]
+        tags = []
+        fields = []
+        for key in tags_.keys():
             if key != "description":
-                if type(value).__name__ == "list":
-                    columns[key] = "TEXT"
-                else:
-                    columns[key] = "INTEGER"
-        for key, value in metrics.items():
+                tags.append(key)
+        for key, value in fields_.items():
             if key != "description":
-                if value["type"]["value"] == "BOOL":
-                    columns[value["key"]["value"]] = "BIT"
-                else:
-                    columns[value["key"]["value"]] = value["type"]["value"]
-        return columns
+                fields.append(value["key"]["value"])
+        return tags, fields
 
-    def _get_model_table_name(self) -> str:
-        for key in self.model.keys():
+    def _get_schema_collection_name(self) -> str:
+        for key in self.schema.keys():
             if key != "description":
                 return key
+        raise ValueError("Unable to determine collection name")
+
+
+AdapterManager.register(interface=DatabaseInterfaceType.MongoDB, factory=MongoDbAdapter)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tsperf-1.1.0/data_generator/postgres_db_writer.py` & `tsperf-1.2.0/tsperf/adapter/postgresql.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,55 +15,70 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 
+from datetime import datetime
+from typing import Dict, Optional, Union
+
 import psycopg2
 import psycopg2.extras
-from tictrack import timed_function
-from data_generator.db_writer import DbWriter
-from datetime import datetime
 from datetime_truncate import truncate
 
+from tsperf.adapter import AdapterManager, DatabaseInterfaceMixin
+from tsperf.model.interface import AbstractDatabaseInterface, DatabaseInterfaceType
+from tsperf.read.config import QueryTimerConfig
+from tsperf.util.tictrack import timed_function
+from tsperf.write.config import DataGeneratorConfig
+
+
+class PostgreSQLAdapter(AbstractDatabaseInterface, DatabaseInterfaceMixin):
+    default_address = "localhost:5432"
+    default_username = "postgres"
+    default_query = "SELECT 1;"
 
-class PostgresDbWriter(DbWriter):
     def __init__(
         self,
-        host: str,
-        port: int,
-        username: str,
-        password: str,
-        db_name: str,
-        model: dict,
-        table_name: str = None,
-        partition: str = "week",
+        config: Union[DataGeneratorConfig, QueryTimerConfig],
+        schema: Optional[Dict] = None,
     ):
+        DatabaseInterfaceMixin.__init__(self, config=config)
         super().__init__()
+
         self.conn = psycopg2.connect(
-            dbname=db_name, user=username, password=password, host=host, port=port
+            dbname=config.database,
+            user=self.username,
+            password=config.password,
+            host=self.host,
+            port=self.port,
         )
         self.cursor = self.conn.cursor()
-        self.model = model
-        self.table_name = (table_name, self._get_model_table_name())[
-            table_name is None or table_name == ""
-        ]
-        self.partition = partition
+        self.schema = schema
+        self.table_name = (config.table, self._get_schema_table_name())[config.table is None or config.table == ""]
+        self.partition = config.partition
 
     def close_connection(self):
         self.cursor.close()
         self.conn.close()
 
     def prepare_database(self):
-        columns = self._get_tags_and_metrics()
-        stmt = f"""CREATE TABLE IF NOT EXISTS {self.table_name} (
+        # Drop table.
+        stmt = f"DROP TABLE IF EXISTS {self.table_name}"
+        self.cursor.execute(stmt)
+        self.conn.commit()
+
+        # Create table.
+        stmt = f"""CREATE TABLE {self.table_name} (
 ts TIMESTAMP NOT NULL,
 ts_{self.partition} TIMESTAMP NOT NULL,
 """
+
+        columns = self._get_tags_and_fields()
         for key, value in columns.items():
             stmt += f"""{key} {value},"""
         stmt = stmt.rstrip(",") + ");"
 
         self.cursor.execute(stmt)
         self.conn.commit()
 
@@ -71,15 +86,15 @@
     def insert_stmt(self, timestamps: list, batch: list):
         stmt = self._prepare_postgres_stmt(timestamps, batch)
         self.cursor.execute(stmt)
         self.conn.commit()
 
     @timed_function()
     def _prepare_postgres_stmt(self, timestamps: list, batch: list) -> str:
-        columns = self._get_tags_and_metrics().keys()
+        columns = self._get_tags_and_fields().keys()
         stmt = f"""INSERT INTO {self.table_name} (ts, ts_{self.partition},"""
         for column in columns:
             stmt += f"""{column}, """
 
         stmt = stmt.rstrip(", ") + ") VALUES"
         for i in range(0, len(batch)):
             t = datetime.fromtimestamp(timestamps[i] / 1000)
@@ -89,14 +104,22 @@
                 stmt += f"""'{batch[i][column]}',"""
             stmt = stmt.rstrip(",") + "),"
         stmt = stmt.rstrip(",")
         return stmt
 
     @timed_function()
     def execute_query(self, query: str) -> list:
+        return self.run_query(query)
+
+    def run_query(self, query: str) -> list:
         self.cursor.execute(query)
+        # self.conn.commit()  # noqa: ERA001
         return self.cursor.fetchall()
 
-    def _get_model_table_name(self) -> str:
-        for key in self.model.keys():
+    def _get_schema_table_name(self) -> str:
+        for key in self.schema.keys():
             if key != "description":
                 return key
+        raise ValueError("Unable to determine table name")
+
+
+AdapterManager.register(interface=DatabaseInterfaceType.PostgreSQL, factory=PostgreSQLAdapter)
```

### Comparing `tsperf-1.1.0/data_generator/timescale_db_writer.py` & `tsperf-1.2.0/tsperf/adapter/timescaledb.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,90 +14,113 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
+import logging
+from datetime import datetime
+from typing import Dict, Optional, Union
 
 import psycopg2
 import psycopg2.extras
-from pgcopy import CopyManager
-from tictrack import timed_function
-from data_generator.db_writer import DbWriter
-from datetime import datetime
 from datetime_truncate import truncate
+from pgcopy import CopyManager
+
+from tsperf.adapter import AdapterManager, DatabaseInterfaceMixin
+from tsperf.model.interface import AbstractDatabaseInterface, DatabaseInterfaceType
+from tsperf.read.config import QueryTimerConfig
+from tsperf.util.tictrack import timed_function
+from tsperf.write.config import DataGeneratorConfig
+
+logger = logging.getLogger(__name__)
 
 
-class TimescaleDbWriter(DbWriter):
+class TimescaleDbAdapter(AbstractDatabaseInterface, DatabaseInterfaceMixin):
+    default_address = "localhost:5432"
+    default_username = "postgres"
+    default_query = "SELECT 1;"
+
     def __init__(
         self,
-        host: str,
-        port: int,
-        username: str,
-        password: str,
-        ts_db_name: str,
-        model: dict,
-        table_name: str = None,
-        partition: str = "week",
-        copy: bool = False,
-        distributed: bool = False,
+        config: Union[DataGeneratorConfig, QueryTimerConfig],
+        schema: Optional[Dict] = None,
     ):
+        DatabaseInterfaceMixin.__init__(self, config=config)
         super().__init__()
+
         self.conn = psycopg2.connect(
-            dbname=ts_db_name, user=username, password=password, host=host, port=port
+            dbname=config.database,
+            user=self.username,
+            password=config.password,
+            host=self.host,
+            port=self.port,
         )
         self.cursor = self.conn.cursor()
-        self.model = model
-        self.table_name = (table_name, self._get_model_table_name())[
-            table_name is None or table_name == ""
-        ]
-        self.partition = partition
-        self.copy = copy
-        self.distributed = distributed
+        self.schema = schema
+        self.table_name = (config.table, self._get_schema_table_name())[config.table is None or config.table == ""]
+        self.partition = config.partition
+
+        self.distributed = config.timescaledb_distributed
+        self.use_pgcopy = config.timescaledb_pgcopy is not None and config.timescaledb_pgcopy or False
+
+        if self.use_pgcopy:
+            logger.info("Using strategy »pgcopy«")
+        else:
+            logger.info("Using strategy »INSERT«")
 
     def close_connection(self):
         self.cursor.close()
         self.conn.close()
 
     def prepare_database(self):
-        columns = self._get_tags_and_metrics()
-        stmt = f"""CREATE TABLE IF NOT EXISTS {self.table_name} (
+        # Drop table.
+        stmt = f"DROP TABLE IF EXISTS {self.table_name}"
+        self.cursor.execute(stmt)
+        self.conn.commit()
+
+        # Create table.
+        stmt = f"""CREATE TABLE {self.table_name} (
 ts TIMESTAMP NOT NULL,
 ts_{self.partition} TIMESTAMP NOT NULL,
 """
+
+        columns = self._get_tags_and_fields()
         for key, value in columns.items():
             stmt += f"""{key} {value},"""
         stmt = stmt.rstrip(",") + ");"
 
         self.cursor.execute(stmt)
         self.conn.commit()
         if self.distributed:
+            logger.info("Using variant »distributed hypertable«")
             tag = self._get_partition_tag()
             stmt = f"SELECT create_distributed_hypertable('{self.table_name}', 'ts', '{tag}', if_not_exists => true);"
         else:
+            logger.info("Using variant »regular hypertable«")
             stmt = (
                 f"SELECT create_hypertable('{self.table_name}', 'ts', 'ts_{self.partition}', 10, "
                 f"if_not_exists => true);"
             )
         self.cursor.execute(stmt)
         self.conn.commit()
 
     @timed_function()
     def insert_stmt(self, timestamps: list, batch: list):
-        if self.copy:
+        if self.use_pgcopy:
             self._prepare_copy(timestamps, batch)
         else:
             stmt = self._prepare_timescale_stmt(timestamps, batch)
             self.cursor.execute(stmt)
         self.conn.commit()
 
     @timed_function()
     def _prepare_copy(self, timestamps: list, batch: list):
-        columns = self._get_tags_and_metrics().keys()
+        columns = self._get_tags_and_fields().keys()
         values = []
 
         for i in range(0, len(timestamps)):
             t = datetime.fromtimestamp(timestamps[i] / 1000)
             trunc = truncate(t, self.partition)
             data = [t, trunc]
             for column in columns:
@@ -108,15 +131,15 @@
         for column in columns:
             cols.append(column)
         copy_manager = CopyManager(self.conn, self.table_name, cols)
         copy_manager.copy(values)
 
     @timed_function()
     def _prepare_timescale_stmt(self, timestamps: list, batch: list) -> str:
-        columns = self._get_tags_and_metrics().keys()
+        columns = self._get_tags_and_fields().keys()
         stmt = f"""INSERT INTO {self.table_name} (ts, ts_{self.partition},"""
         for column in columns:
             stmt += f"""{column}, """
 
         stmt = stmt.rstrip(", ") + ") VALUES"
         for i in range(0, len(batch)):
             t = datetime.fromtimestamp(timestamps[i] / 1000)
@@ -126,21 +149,28 @@
                 stmt += f"""'{batch[i][column]}',"""
             stmt = stmt.rstrip(",") + "),"
         stmt = stmt.rstrip(",")
         return stmt
 
     @timed_function()
     def execute_query(self, query: str) -> list:
+        return self.run_query(query)
+
+    def run_query(self, query: str) -> list:
         self.cursor.execute(query)
         return self.cursor.fetchall()
 
-    def _get_model_table_name(self) -> str:
-        for key in self.model.keys():
+    def _get_schema_table_name(self) -> str:
+        for key in self.schema.keys():
             if key != "description":
                 return key
+        raise ValueError("Unable to determine table name")
 
     def _get_partition_tag(self, top_level: bool = False) -> str:
-        key = self._get_model_table_name()
-        tags = list(self.model[key]["tags"].keys())
+        key = self._get_schema_table_name()
+        tags = list(self.schema[key]["tags"].keys())
         if "description" in tags:
             tags.remove("description")
         return tags[0] if top_level else tags[-1]
+
+
+AdapterManager.register(interface=DatabaseInterfaceType.TimescaleDB, factory=TimescaleDbAdapter)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tsperf-1.1.0/data_generator/timestream_db_writer.py` & `tsperf-1.2.0/tsperf/adapter/mssql.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,166 +14,143 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
-
-from typing import Tuple
-
-import boto3
 import logging
-import math
-import numpy
-from tictrack import timed_function
-from botocore.config import Config
-from data_generator.db_writer import DbWriter
+from datetime import datetime
+from typing import Dict, Optional, Tuple, Union
 
+from tsperf.adapter import AdapterManager, DatabaseInterfaceMixin
+from tsperf.model.interface import AbstractDatabaseInterface, DatabaseInterfaceType
+from tsperf.read.config import QueryTimerConfig
+from tsperf.util.tictrack import timed_function
+from tsperf.write.config import DataGeneratorConfig
+
+logger = logging.getLogger(__name__)
+
+
+class MsSQLDbAdapter(AbstractDatabaseInterface, DatabaseInterfaceMixin):
+    default_address = "127.0.0.1:1433"  # "localhost" does not work here
+    default_username = "sa"
+    default_password = "yayRirr3"  # noqa: S105
+    default_query = "SELECT 1;"
 
-class TimeStreamWriter(DbWriter):
     def __init__(
         self,
-        aws_access_key_id: str,
-        aws_secret_access_key: str,
-        region_name: str,
-        database_name: str,
-        model: dict,
+        config: Union[DataGeneratorConfig, QueryTimerConfig],
+        schema: Optional[Dict] = None,
     ):
+        import pyodbc
+
+        DatabaseInterfaceMixin.__init__(self, config=config)
         super().__init__()
-        self.model = model
-        self.database_name = database_name
-        self.table_name = self._get_model_collection_name()
-        self.session = boto3.session.Session(
-            aws_access_key_id,
-            aws_secret_access_key=aws_secret_access_key,
-            region_name=region_name,
+
+        driver = "{ODBC Driver 17 for SQL Server}"
+        connection_string = (
+            f"DRIVER={driver};SERVER={self.host},{self.port};DATABASE={config.database};"
+            f"UID={self.username};PWD={self.password};CONNECTION TIMEOUT=10;"
         )
-        self.write_client = self.session.client(
-            "timestream-write",
-            config=Config(
-                read_timeout=20, max_pool_connections=5000, retries={"max_attempts": 10}
-            ),
+        logger.info(f"Connecting with »{connection_string}«")
+        self.conn = pyodbc.connect(connection_string, timeout=15)
+        self.cursor = self.conn.cursor()
+        self.cursor.fast_executemany = True
+        self.schema = schema
+        self.table_name = (config.table, self._get_schema_table_name())[config.table is None or config.table == ""]
+
+    def prepare_database(self):
+        # Drop table.
+        stmt = (
+            f"IF EXISTS "  # noqa: S608
+            f"   (SELECT * FROM sysobjects "
+            f"   WHERE id = object_id(N'{self.table_name}') AND OBJECTPROPERTY(id, N'IsUserTable') = 1) "
+            f"DROP TABLE {self.table_name}"
         )
-        self.query_client = self.session.client("timestream-query")
+        self.cursor.execute(stmt)
+        self.conn.commit()
+
+        # Create table.
+        stmt = f"CREATE TABLE {self.table_name} (ts DATETIME NOT NULL,"
+
+        columns = self._get_tags_and_fields()
+        for key, value in columns.items():
+            stmt += f"""{key} {value},"""
+
+        stmt += f" CONSTRAINT PK_{self.table_name} PRIMARY KEY (ts, "
+        tags = list(self.schema[self._get_schema_table_name()]["tags"].keys())
+        for tag in tags:
+            if tag != "description":
+                stmt += f"{tag}, "
+        stmt = stmt.rstrip(", ") + "));"
+
+        self.cursor.execute(stmt)
+        self.conn.commit()
 
     @timed_function()
     def insert_stmt(self, timestamps: list, batch: list):
-        data = self._prepare_timestream_stmt(timestamps, batch)
-        for key, values in data.items():
-            common_attributes = values["common_attributes"]
-            records = numpy.array_split(
-                values["records"], math.ceil(len(values["records"]) / 100)
-            )
-            for record in records:
-                record_list = list(record)
-                try:
-                    self.write_client.write_records(
-                        DatabaseName=self.database_name,
-                        TableName=self.table_name,
-                        Records=record_list,
-                        CommonAttributes=common_attributes,
-                    )
-                except Exception as e:
-                    logging.warning(e)
+        stmt, params = self._prepare_mssql_stmt(timestamps, batch)
+        self.cursor.executemany(stmt, params)
+        self.conn.commit()
 
     @timed_function()
-    def _prepare_timestream_stmt(self, timestamps: list, batch: list) -> dict:
-        data = {}
-        tags, metrics = self._get_tags_and_metrics()
+    def _prepare_mssql_stmt(self, timestamps: list, batch: list) -> Tuple[str, list]:
+        columns = self._get_tags_and_fields().keys()
+        stmt = f"""INSERT INTO {self.table_name} (ts ,"""
+        for column in columns:
+            stmt += f"""{column}, """
+
+        stmt = stmt.rstrip(", ") + ") VALUES (?, "
+
+        for _ in columns:
+            stmt += "?, "
+
+        stmt = stmt.rstrip(", ") + ")"
+
+        params = []
         for i in range(0, len(batch)):
-            record = {"Time": str(timestamps[i])}
-            common_attributes = {"Dimensions": []}
-            for tag in tags:
-                common_attributes["Dimensions"].append(
-                    {"Name": tag, "Value": str(batch[i][tag])}
-                )
-            if str(common_attributes) not in data:
-                data[str(common_attributes)] = {
-                    "common_attributes": common_attributes,
-                    "records": [],
-                }
-            for metric in metrics:
-                record_metric = dict(record)
-                record_metric.update(
-                    {
-                        "MeasureName": metric["name"],
-                        "MeasureValue": str(batch[i][metric["name"]]),
-                        "MeasureValueType": metric["type"],
-                    }
-                )
-                data[str(common_attributes)]["records"].append(record_metric)
-        return data
+            t = datetime.fromtimestamp(timestamps[i] / 1000)
+            row = [t]
+            for column in columns:
+                row.append(batch[i][column])
+            params.append(row)
+        return stmt, params
 
     @timed_function()
-    def execute_query(self, query: str, retry: bool = True) -> list:
-        result = []
-        try:
-            paginator = self.query_client.get_paginator("query")
-            page_iterator = paginator.paginate(QueryString=query)
-            for page in page_iterator:
-                result.append(page)
-        except Exception as e:
-            if retry:
-                result = self.execute_query(query, False)
-            else:
-                raise RuntimeError(e)
-        return result
-
-    def _get_tags_and_metrics(self) -> Tuple[dict, dict]:
-        key = self._get_model_collection_name()
-        tags_ = self.model[key]["tags"]
-        metrics_ = self.model[key]["metrics"]
-        tags = []
-        metrics = []
-        for key, value in tags_.items():
+    def execute_query(self, query: str) -> list:
+        return self.run_query(query)
+
+    def run_query(self, query: str) -> list:
+        self.cursor.execute(query)
+        return self.cursor.fetchall()
+
+    def _get_tags_and_fields(self) -> dict:
+        key = self._get_schema_table_name()
+        tags = self.schema[key]["tags"]
+        fields = self.schema[key]["fields"]
+        columns = {}
+        for key, value in tags.items():
             if key != "description":
-                tags.append(key)
-        for key, value in metrics_.items():
+                if type(value).__name__ == "list":
+                    columns[key] = "TEXT"
+                else:
+                    columns[key] = "INTEGER"
+        for key, value in fields.items():
             if key != "description":
-                metrics.append(
-                    {
-                        "name": value["key"]["value"],
-                        "type": self._convert_to_timestream_type(
-                            value["type"]["value"]
-                        ),
-                    }
-                )
-        return tags, metrics
-
-    @staticmethod
-    def _convert_to_timestream_type(metric_type: str) -> str:
-        metric_type = metric_type.lower()
-        if metric_type in ["float", "double"]:
-            return "DOUBLE"
-        elif metric_type in ["bool", "boolean"]:
-            return "BOOLEAN"
-        elif metric_type in ["int", "long", "uint"]:
-            return "BIGINT"
-        else:
-            return "VARCHAR"
+                if value["type"]["value"] == "BOOL":
+                    columns[value["key"]["value"]] = "BIT"
+                else:
+                    columns[value["key"]["value"]] = value["type"]["value"]
+        return columns
 
-    def _get_model_collection_name(self) -> str:
-        for key in self.model.keys():
+    def _get_schema_table_name(self) -> str:
+        for key in self.schema.keys():
             if key != "description":
                 return key
+        raise ValueError("Unable to determine table name")
 
-    def prepare_database(self):
-        try:
-            self.write_client.create_database(DatabaseName=self.database_name)
-            print("Database [%s] created successfully." % self.database_name)
-        except Exception as err:
-            print("Create database failed:", err)
-
-        retention_properties = {
-            "MemoryStoreRetentionPeriodInHours": 24,
-            "MagneticStoreRetentionPeriodInDays": 7,
-        }
-        try:
-            self.write_client.create_table(
-                DatabaseName=self.database_name,
-                TableName=self.table_name,
-                RetentionProperties=retention_properties,
-            )
-            print("Table [%s] successfully created." % self.table_name)
-        except Exception as err:
-            print("Create table failed:", err)
+    def close_connection(self):
+        self.conn.close()
+
+
+AdapterManager.register(interface=DatabaseInterfaceType.MicrosoftSQL, factory=MsSQLDbAdapter)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tsperf-1.1.0/float_simulator/__init__.py` & `tsperf-1.2.0/tsperf/util/float_simulator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # software solely pursuant to the terms of the relevant commercial agreement.
 
 import random
 
 
 class FloatSimulator:
     """
-    The FloatSimulator produces consecutive float values based on a statistical model and the normal
+    The FloatSimulator produces consecutive float values based on a statistical schema and the normal
     distribution. It can be used to simulate sensor data with more than 100.000 simulated values per second.
 
     To use the FloatSimulator instantiate an object and call the `calculate_next_value()` function
     """
 
     def __init__(
         self,
@@ -65,17 +65,15 @@
         self.standard_deviation = stdev
         self.default_error_rate = error_rate
         self.default_error_length = error_length
         self.current_error_rate = error_rate
         self.current_error_length = error_length
         self.variance = variance
         self.current_error = False
-        self.value = round(
-            random.uniform(self.mean - self.variance, self.mean + self.variance), 2
-        )
+        self.value = round(random.uniform(self.mean - self.variance, self.mean + self.variance), 2)
         self.factors = [-1, 1]
 
     def calculate_next_value(self) -> float:
         """
         This function return the next value for a float_simulator instance
         :return: float
         """
@@ -133,31 +131,25 @@
         else:
             distance = self.mean - self.value
             continue_direction = 0
             change_direction = 1
         chance = (50 * self.standard_deviation) - distance
 
         return (
-            continue_direction
-            if random.randint(0, (100 * self.standard_deviation)) < chance
-            else change_direction
+            continue_direction if random.randint(0, int(100 * self.standard_deviation)) < chance else change_direction
         )
 
     def _new_error_value(self):
         self.error_count += 1
 
         # if the next value is a consecutive error it is basically calculated in a similar way to a new value but
         # within the bounds of the respective error margin (upper or lower error)
         # otherwise a new error is calculated and chosen randomly from the upper or lower values
         if not self.current_error:
             if self.value < self.mean:
-                self.value = round(
-                    random.uniform(self.minimum, self.mean - self.standard_deviation), 2
-                )
+                self.value = round(random.uniform(self.minimum, self.mean - self.standard_deviation), 2)
             else:
-                self.value = round(
-                    random.uniform(self.mean + self.standard_deviation, self.maximum), 2
-                )
+                self.value = round(random.uniform(self.mean + self.standard_deviation, self.maximum), 2)
             self.current_error = True
         else:
             value_change = round(random.uniform(0, self.variance), 2)
             self.value += value_change * self.factors[random.randint(0, 1)]
```

### Comparing `tsperf-1.1.0/query_timer/__main__.py` & `tsperf-1.2.0/tsperf/read/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,217 +1,268 @@
+# -*- coding: utf-8; -*-
+#
+# Licensed to Crate.io GmbH ("Crate") under one or more contributor
+# license agreements.  See the NOTICE file distributed with this work for
+# additional information regarding copyright ownership.  Crate licenses
+# this file to you under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.  You may
+# obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+# However, if you have executed another commercial license agreement
+# with Crate these terms will supersede the license and you may use the
+# software solely pursuant to the terms of the relevant commercial agreement.
+import io
 import logging
-import numpy
-import urllib3
+import shutil
 import statistics
+import sys
 import time
-import shutil
-from blessed import Terminal
+from contextlib import redirect_stdout
 from queue import Queue
-from tictrack import tic_toc, timed_function
 from threading import Thread
-from data_generator.crate_db_writer import CrateDbWriter
-from data_generator.postgres_db_writer import PostgresDbWriter
-from data_generator.timescale_db_writer import TimescaleDbWriter
-from data_generator.influx_db_writer import InfluxDbWriter
-
-# from data_generator.mongo_db_writer import MongoDbWriter
-from data_generator.mssql_db_writer import MsSQLDbWriter
-from data_generator.timestream_db_writer import TimeStreamWriter
-from data_generator.db_writer import DbWriter
-from query_timer.config import QueryTimerConfig
-from query_timer.argument_parser import parse_arguments
+
+import numpy
+from blessed import Terminal
+
+from tsperf.engine import TsPerfEngine, load_schema
+from tsperf.model.interface import AbstractDatabaseInterface
+from tsperf.read.config import QueryTimerConfig
+from tsperf.util.tictrack import tic_toc, timed_function
 
 terminal = Terminal()
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-logging.basicConfig(
-    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s", level=logging.INFO
-)
+logger = logging.getLogger(__name__)
 
-model = {"value": "none"}
+
+# TODO: Get rid of global variables.
+engine: TsPerfEngine = None
+config: QueryTimerConfig = None
+schema = {"value": "none"}
 start_time = time.time()
 success = 0
 failure = 0
 queries_done = Queue(1)
 
-config = QueryTimerConfig()
-
 
-def get_db_writer() -> DbWriter:  # noqa
-    if config.database == 0:  # crate
-        db_writer = CrateDbWriter(config.host, config.username, config.password, model)
-    elif config.database == 1:  # timescale
-        db_writer = TimescaleDbWriter(
-            config.host,
+def get_database_adapter_old() -> AbstractDatabaseInterface:  # pragma: no cover
+    """
+    if config.database == 0:
+        adapter = CrateDbAdapter(config=config, schema=schema)
+    elif config.database == 1:
+        adapter = TimescaleDbAdapter(
+            config.address,
             config.port,
             config.username,
             config.password,
-            config.db_name,
-            model,
+            config.database,
+            schema,
         )
-    elif config.database == 2:  # influx
-        db_writer = InfluxDbWriter(
-            config.host, config.token, config.organization, model
+    elif config.database == 2:
+        adapter = InfluxDbAdapter(
+            config.address, config.token, config.organization, schema
         )
-    elif config.database == 3:  # mongo
+    elif config.database == 3:
         raise ValueError(
             "MongoDB queries are not supported (but can be manually added to the script - see "
-            "query_timer documentation)"
+            "read documentation)"
         )
-        # db_writer = MongoDbWriter(config.host, config.username, config.password, config.db_name, model)
-    elif config.database == 4:  # postgres
-        db_writer = PostgresDbWriter(
-            config.host,
+        # adapter = MongoDbAdapter(config.address, config.username, config.password, config.database, schema)
+    elif config.database == 4:
+        adapter = PostgreSQLAdapter(
+            config.address,
             config.port,
             config.username,
             config.password,
-            config.db_name,
-            model,
+            config.database,
+            schema,
         )
-    elif config.database == 5:  # timestream
-        db_writer = TimeStreamWriter(
+    elif config.database == 5:
+        adapter = AmazonTimestreamAdapter(
             config.aws_access_key_id,
             config.aws_secret_access_key,
             config.aws_region_name,
-            config.db_name,
-            model,
+            config.database,
+            schema,
         )
-    elif config.database == 6:  # ms_sql
-        db_writer = MsSQLDbWriter(
-            config.host,
+    elif config.database == 6:
+        adapter = MsSQLDbAdapter(
+            config.address,
             config.username,
             config.password,
-            config.db_name,
-            model,
+            config.database,
+            schema,
             port=config.port,
         )
     else:
-        db_writer = None
-    return db_writer
+        raise ValueError("Unknown database adapter")
+
+    return adapter
+    """
 
 
 def percentage_to_rgb(percentage):
     red = (percentage - 50) / 100.0 if percentage > 50 else 1.0
     green = 1.0 if percentage > 50 else 2 * percentage / 100.0
     blue = 0.0
     return red * 255, green * 255, blue * 255
 
 
 @timed_function()
-def print_progressbar(
-    iteration, total, prefix="", suffix="", decimals=1, length=100, fill="█"
-):  # pragma: no cover
+def print_progressbar(iteration, total, prefix="", suffix="", decimals=1, length=100, fill="█"):
     """
     Call in a loop to create terminal progress bar
     @params:
         iteration   - Required  : current iteration (Int)
         total       - Required  : total iterations (Int)
         prefix      - Optional  : prefix string (Str)
         suffix      - Optional  : suffix string (Str)
         decimals    - Optional  : positive number of decimals in percent complete (Int)
         length      - Optional  : character length of bar (Int)
         fill        - Optional  : bar fill character (Str)
     """
+
+    screen_position_y = 30
+
     duration = time.time() - start_time
-    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
-    r, g, b = percentage_to_rgb(float(percent))
+    percentage = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
+    # Prevent "division by zero" errors.
+    percent = max(float(percentage), 0.1)
+
+    r, g, b = percentage_to_rgb(percent)
     filled_length = int(length * iteration // total)
     bar = fill * filled_length + "-" * (length - filled_length)
 
     if "execute_query" in tic_toc:
         values = tic_toc["execute_query"]
-        print(
-            terminal.move_y(3)
-            + f"{prefix} |{terminal.color_rgb(r, g, b)}{bar}{terminal.normal}| {percent}% "
-            f"{suffix} {round(duration, 2)}s"
-        )
-        print(
-            f"time left: {round(((duration / float(percent)) * 100) - duration, 2)}s                                "
-        )
-        if len(values) > 1:
-            pass
+
+        f = io.StringIO()
+        # ruff: noqa: T201
+        with redirect_stdout(f):
             print(
-                terminal.move_y(6)
-                + f"rate   : {round((1 / numpy.mean(values)) * config.concurrency, 3)}qs/s       "
+                terminal.move_y(screen_position_y)
+                + f"{prefix} |{terminal.color_rgb(r, g, b)}{bar}{terminal.normal}| {percentage}% "
+                f"{suffix} {round(duration, 2)}s"
             )
-            print(f"mean   : {round(numpy.mean(values) * 1000, 3)}ms       ")
-            print(f"stdev  : {round(numpy.std(values) * 1000, 3)}ms      ")
-            print(f"min    : {round(min(values) * 1000, 3)}ms       ")
-            print(f"max    : {round(max(values) * 1000, 3)}ms       ")
-            print(f"success: {terminal.green}{success}{terminal.normal}      ")
-            print(f"failure: {terminal.red}{failure}{terminal.normal}        ")
+            print(f"time left: {round(((duration / percent) * 100) - duration, 2)}s                              ")
+            if len(values) > 1:
+                print(
+                    terminal.move_y(screen_position_y + 3)
+                    + f"rate   : {round((1 / numpy.mean(values)) * config.concurrency, 3)}qps       "
+                )
+                print(f"mean   : {round(numpy.mean(values) * 1000, 3)}ms       ")
+                print(f"stdev  : {round(numpy.std(values) * 1000, 3)}ms      ")
+                print(f"min    : {round(min(values) * 1000, 3)}ms       ")
+                print(f"max    : {round(max(values) * 1000, 3)}ms       ")
+                print(f"success: {terminal.green}{success}{terminal.normal}      ")
+                print(f"failure: {terminal.red}{failure}{terminal.normal}        ")
+        report = f.getvalue()
+        sys.stderr.write(f"\n{report}\n")
+        sys.stderr.flush()
+
+
+def probe_query():
+    try:
+        engine.create_adapter().run_query(config.query)
+        return True
+    except Exception:
+        logger.exception(f"Failure executing query '{config.query}'")
+        return False
 
 
 def start_query_run():
     global success, failure
-    db_writer = get_db_writer()
-    for x in range(0, config.iterations):
+    adapter = engine.create_adapter()
+    for _ in range(0, config.iterations):
         try:
-            db_writer.execute_query(config.query)
+            adapter.execute_query(config.query)
             success += 1
         except Exception:
             failure += 1
+            logger.exception(f"Failure executing query '{config.query}'")
 
 
-def print_progress_thread():  # pragma: no cover
+def print_progress_thread():
     while queries_done.empty():
-        time.sleep(config.refresh_rate)
+        time.sleep(config.refresh_interval)
         total_queries = success + failure
         terminal_size = shutil.get_terminal_size()
         print_progressbar(
             total_queries,
             config.concurrency * config.iterations,
             prefix="Progress:",
             suffix="Complete",
             length=(terminal_size.columns - 40),
         )
 
 
-def run_qt():  # pragma: no cover
+def run_qt():
+    logger.info(f"Starting query timer with {config} and schema {config.schema}")
     global start_time
     start_time = time.time()
-    progress_thread = Thread(target=print_progress_thread)
+
+    logger.info("Starting progress monitor thread")
+    progress_thread = Thread(target=print_progress_thread, name="ProgressMonitor")
     progress_thread.start()
+
+    logger.info("Starting worker threads")
     threads = []
-    for y in range(0, config.concurrency):
-        thread = Thread(target=start_query_run)
+    logger.info(f"Invoking query »{config.query}«")
+    for i in range(0, config.concurrency):
+        thread = Thread(target=start_query_run, name=f"WorkerThread-{i}")
         threads.append(thread)
     for thread in threads:
         thread.start()
+
+    logger.info("Waiting for worker threads")
     for thread in threads:
         thread.join()
     queries_done.put_nowait(True)
+
+    logger.info("Waiting for progress monitor thread")
     progress_thread.join()
 
 
-def main():  # pragma: no cover
-    global config
-    with terminal.hidden_cursor():
-        # load configuration an set everything up
-        config = parse_arguments(config)
-        valid_config = config.validate_config()
-        if not valid_config:
-            logging.error(f"invalid configuration: {config.invalid_configs}")
-            exit(-1)
+def start(configuration: QueryTimerConfig):
+    global engine, schema, config
+
+    # TODO: Move schema loading to engine.
+    schema = load_schema(configuration.schema)
+    engine = TsPerfEngine(config=configuration, schema=schema)
+    engine.bootstrap()
+    config = engine.config
+
+    logger.info(f"Probing query »{config.query}«")
+    if not probe_query():
+        raise RuntimeError("Error probing database. Not starting machinery.")
+
+    logger.info(f"Running {config.iterations} iterations with concurrency {config.concurrency}")
 
-        print(f"concurrency: {config.concurrency}\niterations : {config.iterations}")
+    with terminal.hidden_cursor():
         terminal_size = shutil.get_terminal_size()
         print_progressbar(
             0,
             config.concurrency * config.iterations,
             prefix="Progress:",
             suffix="Complete",
             length=(terminal_size.columns - 40),
         )
 
         run_qt()
 
         if "execute_query" in tic_toc:
             values = tic_toc["execute_query"]
             qus = statistics.quantiles(values, n=100, method="inclusive")
-            print("")
-            for i in range(0, len(qus)):
-                if str(i + 1) in config.quantiles:
-                    print(f"p{i+1}  : {round(qus[i]*1000, 3)}ms")
-
-
-if __name__ == "__main__":  # pragma: no cover
-    main()
+            f = io.StringIO()
+            with redirect_stdout(f):
+                for i in range(0, len(qus)):
+                    if str(i + 1) in config.quantiles:
+                        print(f"p{i+1}  : {round(qus[i]*1000, 3)}ms")
+            report = f.getvalue()
+            logger.info("\n")
+            logger.info(f"Statistics:\n{report}")
```

### Comparing `tsperf-1.1.0/tests/test_crate_db_writer.py` & `tsperf-1.2.0/tests/adapter/test_cratedbpg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,229 @@
-import mock
-from crate import client
-from data_generator.crate_db_writer import CrateDbWriter
-from tests.test_models import test_model, test_model2
+from unittest import mock
 
+import psycopg2
+import pytest
 
-@mock.patch.object(client, "connect", autospec=True)
+from tests.write.schema import test_schema1, test_schema2
+from tsperf.adapter.cratedbpg import CrateDbPgWireAdapter
+from tsperf.model.configuration import DatabaseConnectionConfiguration
+from tsperf.model.interface import DatabaseInterfaceType
+
+
+@pytest.fixture
+def config():
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.CrateDBpg,
+        address="localhost:5432",
+    )
+    return config
+
+
+@mock.patch.object(psycopg2, "connect", autospec=True)
 def test_close_connection(mock_connect):
     """
     This function tests if the .close() functions of the self.conn and self.cursor objects is called
 
     Pre Condition: crate.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        CrateDbWriter is called.
-    -> mock_connect is called by CrateDbWriter with values given the constructor
+        CrateDbAdapter is called.
+    -> mock_connect is called by CrateDbAdapter with values given the constructor
 
     Test Case 1:
-    when calling CrateDbWriter.close_connection() conn.close() and cursor.close() are called
+    when calling CrateDbAdapter.close_connection() conn.close() and cursor.close() are called
 
     :param mock_connect: mocked function call from crate.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = CrateDbWriter("localhost:4200", "crate", "password", test_model)
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.CrateDBpg,
+        address="localhost:5432",
+        username="foobar",
+        password=None,
+        database="mydb",
+    )
+    db_writer = CrateDbPgWireAdapter(config=config, schema=test_schema1)
     mock_connect.assert_called_with(
-        "localhost:4200", username="crate", password="password"
+        host="localhost",
+        port=5432,
+        user="foobar",
+        password=None,
+        dbname="mydb",
     )
+
     # Test Case 1:
     db_writer.close_connection()
     conn.close.assert_called()
     cursor.close.assert_called()
 
 
-@mock.patch.object(client, "connect", autospec=True)
+@mock.patch.object(psycopg2, "connect", autospec=True)
 def test_prepare_database1(mock_connect):
     """
-    This function tests if the .prepare_database() functions of the db_writer uses the correct values when
+    This function tests if the .prepare_database() functions of the adapter uses the correct values when
         creating the the database tables
 
     Pre Condition: crate.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        CrateDbWriter is called.
-    -> mock_connect is called by CrateDbWriter with values given the constructor
+        CrateDbAdapter is called.
+    -> mock_connect is called by CrateDbAdapter with values given the constructor
 
     Test Case 1:
-    when calling CrateDbWriter.prepare_database() the statement given to cursor.execute() contains the correct values:
+    when calling CrateDbAdapter.prepare_database() the statement given to cursor.execute() contains the correct values:
     -> "temperature" is used in stmt as table name
     -> "g_ts_week" is used as partitioning column
-    -> "21 SHARDS" are configured for table
+    -> "4 SHARDS" are configured for table
     -> "number_of_replicas = 1" is set for table
 
     :param mock_connect: mocked function call from crate.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = CrateDbWriter("localhost:4200", "crate2", "password2", test_model)
+
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.CrateDBpg,
+        address="localhost:8200",
+        username="crate2",
+        password="password2",
+    )
+    db_writer = CrateDbPgWireAdapter(config=config, schema=test_schema1)
+
     mock_connect.assert_called_with(
-        "localhost:4200", username="crate2", password="password2"
+        host="localhost",
+        port=8200,
+        user="crate2",
+        password="password2",
+        dbname=None,
     )
+
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     # table name is in stmt
     assert "temperature" in stmt
     # partition is default
     assert "g_ts_week" in stmt
     # shards is default
-    assert "21 SHARDS" in stmt
+    assert "4 SHARDS" in stmt
     # replicas is default
     assert "number_of_replicas = 1" in stmt
 
 
-@mock.patch.object(client, "connect", autospec=True)
-def test_prepare_database2(mock_connect):
+@mock.patch.object(psycopg2, "connect", autospec=True)
+def test_prepare_database2(mock_connect, config):
     """
-    This function tests if the .prepare_database() functions of the db_writer uses the correct values when
+    This function tests if the .prepare_database() functions of the adapter uses the correct values when
         creating the the database tables
 
     Pre Condition: crate.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        CrateDbWriter is called.
-    -> mock_connect is called by CrateDbWriter with values given the constructor
+        CrateDbAdapter is called.
+    -> mock_connect is called by CrateDbAdapter with values given the constructor
 
     Test Case 1:
-    A new CrateDbWriter is initialized that overwrites default values used in prepare_database()
-    -> "table_name" is used in stmt as table name
+    A new CrateDbAdapter is initialized that overwrites default values used in prepare_database()
+    -> "table" is used in stmt as table name
     -> "g_ts_day" is used as partitioning column
     -> "3 SHARDS" are configured for table
     -> "number_of_replicas = 0" is set for table
 
     :param mock_connect: mocked function call from crate.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = CrateDbWriter(
-        "localhost:4200", "crate3", "password3", test_model2, "table_name", 3, 0, "day"
-    )
+
+    config.table = "foobar"
+    config.shards = 3
+    config.replicas = 0
+    config.partition = "day"
+    db_writer = CrateDbPgWireAdapter(config=config, schema=test_schema2)
+
     db_writer.prepare_database()
     # Test Case 1:
     stmt = cursor.execute.call_args.args[0]
     # table name is in stmt
-    assert "table_name" in stmt
+    assert "foobar" in stmt
     # partition is default
     assert "g_ts_day" in stmt
     # shards is default
     assert "3 SHARDS" in stmt
     # replicas is default
     assert "number_of_replicas = 0" in stmt
 
 
-@mock.patch.object(client, "connect", autospec=True)
-def test_insert_stmt(mock_connect):
+@mock.patch.object(psycopg2, "connect", autospec=True)
+def test_insert_stmt(mock_connect, config):
     """
-    This function tests if the .insert_stmt() functions of CrateDbWriter uses the correct table name and arguments
+    This function tests if the .insert_stmt() functions of CrateDbAdapter uses the correct table name and arguments
 
     Pre Condition: crate.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        CrateDbWriter is called.
+        CrateDbAdapter is called.
 
     Test Case 1:
-    when calling CrateDbWriter.insert_stmt() the correct values are used for cursor.execute()
+    when calling CrateDbAdapter.insert_stmt() the correct values are used for cursor.execute()
     -> stmt contains the correct table name
     -> values are equal to the insert_stmt arguments
 
     :param mock_connect: mocked function call from crate.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = CrateDbWriter("localhost:4200", "crate2", "password2", test_model)
+
+    db_writer = CrateDbPgWireAdapter(config=config, schema=test_schema1)
+
     # Test Case 1:
     db_writer.insert_stmt(
         [1586327807000],
         [{"plant": 1, "line": 1, "sensor_id": 1, "value": 6.7, "button_press": False}],
     )
     call_arguments = cursor.execute.call_args.args
     stmt = call_arguments[0]
     values = call_arguments[1]
-    assert (
-        stmt
-        == "INSERT INTO temperature (ts, payload) (SELECT col1, col2 FROM UNNEST(?,?))"
-    )
+    assert stmt == "INSERT INTO temperature (ts, payload) (SELECT col1, col2 FROM UNNEST(?,?))"
     assert values == (
         [1586327807000],
         [{"plant": 1, "line": 1, "sensor_id": 1, "value": 6.7, "button_press": False}],
     )
 
 
-@mock.patch.object(client, "connect", autospec=True)
-def test_execute_query(mock_connect):
+@mock.patch.object(psycopg2, "connect", autospec=True)
+def test_execute_query(mock_connect, config):
     """
-    This function tests if the .execute_query() functions of CrateDbWriter uses the correct query
+    This function tests if the .execute_query() functions of CrateDbAdapter uses the correct query
 
     Pre Condition: crate.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        CrateDbWriter is called.
+        CrateDbAdapter is called.
 
     Test Case 1:
-    when calling CrateDbWriter.execute_query() the correct values are used for cursor.execute()
+    when calling CrateDbAdapter.execute_query() the correct values are used for cursor.execute()
     -> cursor.execute is called with argument from execute_query
     -> fetchall is called
 
     :param mock_connect: mocked function call from crate.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = CrateDbWriter("localhost:4200", "crate2", "password2", test_model)
+
+    db_writer = CrateDbPgWireAdapter(config=config, schema=test_schema1)
+
     # Test Case 1:
     db_writer.execute_query("SELECT * FROM temperature;")
     cursor.execute.assert_called_with("SELECT * FROM temperature;")
     cursor.fetchall.assert_called()
```

### Comparing `tsperf-1.1.0/tests/test_edge.py` & `tsperf-1.2.0/tests/write/test_channel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,125 @@
-import pytest
 import numpy
-from data_generator.edge import Edge, BoolSensor
-from tests.test_models import (
-    metrics_model_float1_bool1,
-    metrics_model_string,
-    tag_model_plant100_line5_sensorId,
-    bool_model,
-    tag_model_list,
+import pytest
+
+from tests.write.schema import (
+    bool_schema,
+    channel_schema_float1_bool1,
+    channel_schema_string,
+    tag_schema_list,
+    tag_schema_plant100_line5_sensorId,
 )
+from tsperf.write.model.channel import Channel
+from tsperf.write.model.sensor import BoolSensor
 
 
 def test_init_sensors():
     """
-    This function tests if the Edge Object is correctly initialized
+    This function tests if the Channel Object is correctly initialized
 
     Test Case 1:
-    Edge is initialized with:
+    Channel is initialized with:
     id: 1
-    tags: valid tag model
-    metrics: metrics model containing one float and one bool sensor
+    tags: valid tag schema
+    fields: fields schema containing one float and one bool sensor
     -> FloatSensor must be in sensor_types
     -> BoolSensor must be in sensor_types
 
     Test Case 2:
-    Edge is initialized with:
+    Channel is initialized with:
     id: 1
-    tags: valid tag model
-    metrics: metrics model containing one string sensor
+    tags: valid tag schema
+    fields: fields schema containing one string sensor
     -> Constructor raises NotImplementedError
     """
     # Test Case 1:
-    edge = Edge(1, tag_model_plant100_line5_sensorId, metrics_model_float1_bool1)
+    channel = Channel(1, tag_schema_plant100_line5_sensorId, channel_schema_float1_bool1)
     sensor_types = []
-    for sensor in edge.sensors:
+    for sensor in channel.sensors:
         sensor_types.append(sensor.__class__.__name__)
     assert "FloatSensor" in sensor_types
     assert "BoolSensor" in sensor_types
 
     # Test Case 2:
     with pytest.raises(NotImplementedError):
-        Edge(1, tag_model_plant100_line5_sensorId, metrics_model_string)
+        Channel(1, tag_schema_plant100_line5_sensorId, channel_schema_string)
 
 
-def test_calculate_next_value_edge():
+def test_calculate_next_value_channel():
     """
-    This function tests if the Edge Object correctly calculates the next value of it's sensors
+    This function tests if the Channel Object correctly calculates the next value of it's sensors
 
-    Pre Condition: Edge Object created with id 1, a valid tag model and a the metrics_model_float1_bool1 model
+    Pre Condition: Channel Object created with id 1, a valid tag schema and a the `channel_schema_float1_bool1` schema
 
-    Test Case 1: the first value of the edge object is calculated
+    Test Case 1: the first value of the channel object is calculated
     -> "plant" tag is in batch
     -> "plant" values is 1
     -> "line" tag is in batch
     -> "line" value is 1
     -> "sensor_id" tag is in batch
     -> "sensor_id" value is 1
     -> "value" metric is in batch
     -> "value" value is not None
     -> "button_press" is in batch
     -> "button_press" is not None
 
-    Test Case 2: another 1000 values for the edge object are calculated to see if button_press is at least True once
+    Test Case 2: another 1000 values for the channel object are calculated to see if button_press is at least True once
         and value is not the same value each time
     -> True is contained in button_press array
     -> length of unique values in values array is bigger than 1
     """
     # Pre Condition
-    edge = Edge(1, tag_model_plant100_line5_sensorId, metrics_model_float1_bool1)
+    channel = Channel(1, tag_schema_plant100_line5_sensorId, channel_schema_float1_bool1)
     results = []
     # Test Case 1.
-    batch = edge.calculate_next_value()
+    batch = channel.calculate_next_value()
     assert "plant" in batch
     assert batch["plant"] == 0
     assert "line" in batch
     assert batch["line"] == 0
     assert "sensor_id" in batch
     assert batch["sensor_id"] == 1
     assert "value" in batch
     assert batch["value"] is not None
     assert "button_press" in batch
     assert batch["button_press"] is not None
     results.append(batch)
 
     # Test Case 2:
     # because button_press has a probability of 1:100 to be True, we do a thousand operations to get True for sure
-    for i in range(0, 1000):
-        results.append(edge.calculate_next_value())
+    for _ in range(0, 1000):
+        results.append(channel.calculate_next_value())
 
     button_press = []
     values = []
     for result in results:
         button_press.append(result["button_press"])
         values.append(result["value"])
     assert True in button_press
     assert len(numpy.unique(values)) > 1
 
 
 def test_calculate_next_value_bool():
     """
-    This function tests if the BoolSensor produces values that match the model
+    This function tests if the BoolSensor produces values that match the schema
 
-    Pre Condition: BoolSensor initialized with bool_model
+    Pre Condition: BoolSensor initialized with `bool_schema`
 
     Test Case 1: 10000 values for BoolSensor are created
-    -> true_ratio of generated values == true_ratio of model +- 0.001
+    -> true_ratio of generated values == true_ratio of schema +- 0.001
     """
     # Pre Condition:
-    bool_sensor = BoolSensor(bool_model)
+    bool_sensor = BoolSensor(bool_schema)
     results = []
     # Test Case 1:
-    for i in range(0, 10000):
+    for _ in range(0, 10000):
         results.append(bool_sensor.calculate_next_value())
     sum_true = sum(results)
     true_ratio = sum_true / len(results)
-    assert true_ratio == pytest.approx(bool_model["true_ratio"]["value"], abs=0.001)
+    assert true_ratio == pytest.approx(bool_schema["true_ratio"]["value"], abs=0.001)
 
 
 def test_calculate_next_value_tag_list():
     results = [
         ["A", "L1"],
         ["A", "L2"],
         ["A", "L3"],
@@ -131,11 +133,11 @@
         ["D", "L2"],
         ["D", "L3"],
         ["E", "L1"],
         ["E", "L2"],
         ["E", "L3"],
     ]
     for i in range(1, 16):
-        edge = Edge(i, tag_model_list, metrics_model_float1_bool1)
-        payload = edge.calculate_next_value()
+        channel = Channel(i, tag_schema_list, channel_schema_float1_bool1)
+        payload = channel.calculate_next_value()
         assert payload["plant"] == results[i - 1][0]
         assert payload["line"] == results[i - 1][1]
```

### Comparing `tsperf-1.1.0/tests/test_influx_db_writer.py` & `tsperf-1.2.0/tests/adapter/test_influxdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,163 +1,177 @@
-import mock
+from unittest import mock
+
+import pytest
 from dotmap import DotMap
 from influxdb_client import Bucket
 from influxdb_client.client.write_api import Point
-from data_generator.influx_db_writer import InfluxDbWriter
-from tests.test_models import test_model
+
+from tests.write.schema import test_schema1
+from tsperf.adapter.influxdb import InfluxDbAdapter
+from tsperf.model.configuration import DatabaseConnectionConfiguration
+from tsperf.model.interface import DatabaseInterfaceType
+
+
+@pytest.fixture
+def config():
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.InfluxDB,
+        address="http://localhost:8086/",
+        influxdb_organization="acme",
+        influxdb_token="token",
+    )
+    return config
 
 
-@mock.patch("data_generator.influx_db_writer.InfluxDBClient", autospec=True)
-def test_close_connection(mock_client):
+@mock.patch("tsperf.adapter.influxdb.InfluxDBClient", autospec=True)
+def test_close_connection(mock_client, config):
     """
-    This function tests if the .close_connection() function of InfluxDbWriter calls the close() function of self.client
+    This function tests if the .close_connection() function of InfluxDbAdapter calls the close() function of self.client
 
     Pre Condition: InfluxDBClient() returns a Mock Object client
-        InfluxDbWriter is called.
-    -> Parameters of InfluxDbWriter match constructor parameters
+        InfluxDbAdapter is called.
+    -> Parameters of InfluxDbAdapter match constructor parameters
 
     Test Case 1:
-    when calling InfluxDbWriter.close_connection() self.client.close() is called
+    when calling InfluxDbAdapter.close_connection() self.client.close() is called
     -> client.close() is called
 
     :param mock_client: mocked InfluxDBClient class
     """
     # Pre Condition:
     client = mock.Mock()
     mock_client.return_value = client
-    db_writer = InfluxDbWriter("localhost", "token", "org", test_model)
-    mock_client.assert_called_with("localhost", token="token")
+    db_writer = InfluxDbAdapter(config=config, schema=test_schema1)
+    mock_client.assert_called_with("http://localhost:8086/", token="token", org="acme")
     # Test Case 1
     db_writer.close_connection()
     client.close.assert_called()
 
 
-@mock.patch("data_generator.influx_db_writer.InfluxDBClient", autospec=True)
-def test_prepare_database_bucket_exists(mock_client):
+@mock.patch("tsperf.adapter.influxdb.InfluxDBClient", autospec=True)
+def test_prepare_database_bucket_exists(mock_client, config):
     """
-    This function tests if the .prepare_database() function of InfluxDbWriter loads the correct bucket
+    This function tests if the .prepare_database() function of InfluxDbAdapter loads the correct bucket
 
     Pre Condition: InfluxDBClient() returns a Mock Object client
         client.buckets_api() returns a Mock Object buckets_api
         buckets_api.find_buckets() returns a DotMap Object where .buckets returns a list of influx Buckets
-        InfluxDbWriter is called.
-    -> Parameters of InfluxDbWriter match constructor parameters
+        InfluxDbAdapter is called.
+    -> Parameters of InfluxDbAdapter match constructor parameters
 
     Test Case 1:
-    calling InfluxDbWriter.prepare_database() with a already existing Bucket in the Influx DB
+    calling InfluxDbAdapter.prepare_database() with a already existing Bucket in the Influx DB
     -> buckets_api.create_bucket() is not called
 
     :param mock_client: mocked InfluxDBClient class
     """
     # Pre Condition:
     client = mock.Mock()
     buckets_api = mock.Mock()
     client.buckets_api.return_value = buckets_api
     mock_client.return_value = client
-    db_writer = InfluxDbWriter("localhost", "token1", "org1", test_model)
-    mock_client.assert_called_with("localhost", token="token1")
+    db_writer = InfluxDbAdapter(config=config, schema=test_schema1)
     bucket_list = DotMap()
     bucket_list.buckets = [
         Bucket(name="", retention_rules=[]),
         Bucket(name="temperature", retention_rules=[]),
     ]
     buckets_api.find_buckets.return_value = bucket_list
     # Test Case 1:
     db_writer.prepare_database()
     buckets_api.create_bucket.assert_not_called()
 
 
-@mock.patch("data_generator.influx_db_writer.InfluxDBClient", autospec=True)
-def test_prepare_database_bucket_not_exists(mock_client):
+@mock.patch("tsperf.adapter.influxdb.InfluxDBClient", autospec=True)
+def test_prepare_database_bucket_not_exists(mock_client, config):
     """
-    This function tests if the .prepare_database() function of InfluxDbWriter loads the correct bucket
+    This function tests if the .prepare_database() function of InfluxDbAdapter loads the correct bucket
 
     Pre Condition: InfluxDBClient() returns a Mock Object client
         client.buckets_api() returns a Mock Object buckets_api
         buckets_api.find_buckets() returns a DotMap Object where .buckets returns a list of influx Buckets
-        InfluxDbWriter is called.
-    -> Parameters of InfluxDbWriter match constructor parameters
+        InfluxDbAdapter is called.
+    -> Parameters of InfluxDbAdapter match constructor parameters
 
     Test Case 1:
-    calling InfluxDbWriter.prepare_database() with the matching Bucket not in bucket_list
+    calling InfluxDbAdapter.prepare_database() with the matching Bucket not in bucket_list
     -> buckets_api.create_bucket() is called
 
     :param mock_client: mocked InfluxDBClient class
     """
     # Pre Condition:
     client = mock.Mock()
     buckets_api = mock.Mock()
     client.buckets_api.return_value = buckets_api
     mock_client.return_value = client
-    db_writer = InfluxDbWriter("localhost", "token2", "org2", test_model)
-    mock_client.assert_called_with("localhost", token="token2")
+    db_writer = InfluxDbAdapter(config=config, schema=test_schema1)
     bucket_list = DotMap()
     bucket_list.buckets = [
         Bucket(name="x", retention_rules=[]),
         Bucket(name="y", retention_rules=[]),
     ]
     buckets_api.find_buckets.return_value = bucket_list
     # Test Case 1:
     db_writer.prepare_database()
     buckets_api.create_bucket.assert_called()
 
 
-@mock.patch("data_generator.influx_db_writer.InfluxDBClient", autospec=True)
-def test_insert_stmt(mock_client):
+@mock.patch("tsperf.adapter.influxdb.InfluxDBClient", autospec=True)
+def test_insert_stmt(mock_client, config):
     """
-    This function tests if the .insert_stmt() function of InfluxDbWriter uses the correct arguments for write_api.write
+    This function tests if the .insert_stmt() function of InfluxDbAdapter uses the correct arguments for write_api.write
 
     Pre Condition: InfluxDBClient() returns a Mock Object client
         client.write_api() returns a Mock Object write_api
-        InfluxDbWriter is called.
+        InfluxDbAdapter is called.
 
     Test Case 1:
-    calling InfluxDbWriter.insert_stmt() with one timestamp and one batch and check write parameters
-    -> org is "org"
+    calling InfluxDbAdapter.insert_stmt() with one timestamp and one batch and check write parameters
+    -> org is "acme"
     -> data is of type list
     -> data is of length 1
     -> element in data is of type influxdb_client.Point
 
     :param mock_client: mocked InfluxDBClient class
     """
     # Pre Condition:
     client = mock.Mock()
     write_api = mock.Mock()
     mock_client.return_value = client
     client.write_api.return_value = write_api
-    db_writer = InfluxDbWriter("localhost", "token", "org", test_model)
+    db_writer = InfluxDbAdapter(config=config, schema=test_schema1)
     # Test Case 1:
     db_writer.insert_stmt(
         [1586327807000],
         [{"plant": 2, "line": 2, "sensor_id": 2, "value": 6.7, "button_press": False}],
     )
     call_arguments = write_api.write.call_args[1]
     org = call_arguments["org"]
     data = call_arguments["record"]
-    assert org == "org"
+    assert org == "acme"
     assert isinstance(data, list)
     assert len(data) == 1
     assert isinstance(data[0], Point)
 
 
-@mock.patch("data_generator.influx_db_writer.InfluxDBClient", autospec=True)
-def test_execute_query(mock_client):
+@mock.patch("tsperf.adapter.influxdb.InfluxDBClient", autospec=True)
+def test_execute_query(mock_client, config):
     """
-    This function tests if the .execute_query() function of InfluxDbWriter uses the correct arguments
+    This function tests if the .execute_query() function of InfluxDbAdapter uses the correct arguments
 
     Pre Condition: InfluxDBClient() returns a Mock Object client
         client.query_api() returns a Mock Object query_api
-        InfluxDbWriter is called.
+        InfluxDbAdapter is called.
 
     Test Case 1:
-    calling InfluxDbWriter.execute_query()
+    calling InfluxDbAdapter.execute_query()
     -> query_api.query is called with the same query given execute_query
 
     :param mock_client: mocked InfluxDBClient class
     """
     client = mock.Mock()
     query_api = mock.Mock()
     mock_client.return_value = client
     client.query_api.return_value = query_api
-    db_writer = InfluxDbWriter("localhost", "token", "org", test_model)
+    db_writer = InfluxDbAdapter(config=config, schema=test_schema1)
     db_writer.execute_query("SELECT * FROM temperature;")
-    query_api.query.assert_called_with("SELECT * FROM temperature;")
+    query_api.query.assert_called_with("SELECT * FROM temperature;", org="acme")
```

### Comparing `tsperf-1.1.0/tests/test_models.py` & `tsperf-1.2.0/tests/write/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-test_model = {
+test_schema1 = {
     "description": "test",
     "temperature": {
         "tags": {"description": "test", "plant": 100, "line": 5, "sensor_id": "id"},
-        "metrics": {
+        "fields": {
             "description": "test",
             "temperature": {
                 "description": "test",
                 "key": {"description": "test", "value": "value"},
                 "type": {"description": "test", "value": "FLOAT"},
                 "min": {
                     "description": "test",
@@ -51,19 +51,19 @@
                 "type": {"description": "test", "value": "BOOL"},
                 "true_ratio": {"description": "test", "value": 0.001},
             },
         },
     },
 }
 
-test_model2 = {
+test_schema2 = {
     "booleans": {
         "description": "test",
         "tags": {"description": "test", "plant": 100, "line": 5, "sensor_id": "id"},
-        "metrics": {
+        "fields": {
             "description": "test",
             "switch": {
                 "description": "test",
                 "key": {"description": "test", "value": "switch_on"},
                 "type": {"description": "test", "value": "BOOL"},
                 "true_ratio": {"description": "test", "value": 0.9},
             },
@@ -73,24 +73,24 @@
                 "type": {"description": "test", "value": "BOOL"},
                 "true_ratio": {"description": "test", "value": 0.001},
             },
         },
     }
 }
 
-test_model3 = {
+test_schema3 = {
     "booleans": {
         "description": "test",
         "tags": {
             "description": "test",
             "plant": ["A", "B", "C", "D", "E"],
             "line": ["L1", "L2", "L3"],
             "sensor_id": "id",
         },
-        "metrics": {
+        "fields": {
             "description": "test",
             "switch": {
                 "description": "test",
                 "key": {"description": "test", "value": "switch_on"},
                 "type": {"description": "test", "value": "BOOL"},
                 "true_ratio": {"description": "test", "value": 0.9},
             },
@@ -100,15 +100,15 @@
                 "type": {"description": "test", "value": "BOOL"},
                 "true_ratio": {"description": "test", "value": 0.001},
             },
         },
     }
 }
 
-metrics_model_float1_bool1 = {
+channel_schema_float1_bool1 = {
     "temperature": {
         "key": {"value": "value"},
         "type": {"value": "FLOAT"},
         "min": {
             "value": 6.0,
         },
         "max": {
@@ -135,27 +135,27 @@
     },
     "button": {
         "key": {"value": "button_press"},
         "type": {"value": "BOOL"},
         "true_ratio": {"value": 0.01},
     },
 }
-metrics_model_string = {
+channel_schema_string = {
     "string": {
         "key": {"value": "not_implemented_sensor_type"},
         "type": {"value": "STRING"},
         "true_ratio": {"value": "not_implemented"},
     }
 }
-tag_model_plant100_line5_sensorId = {"plant": 100, "line": 5, "sensor_id": "id"}
+tag_schema_plant100_line5_sensorId = {"plant": 100, "line": 5, "sensor_id": "id"}
 
-tag_model_list = {
+tag_schema_list = {
     "plant": ["A", "B", "C", "D", "E"],
     "line": ["L1", "L2", "L3"],
     "sensor_id": "id",
 }
 
-bool_model = {
+bool_schema = {
     "key": {"value": "button_press"},
     "type": {"value": "BOOL"},
     "true_ratio": {"value": 0.001},
 }
```

### Comparing `tsperf-1.1.0/tests/test_mssql_db_writer.py` & `tsperf-1.2.0/tests/adapter/test_mssql.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,133 +1,161 @@
-import mock
-import pyodbc
-from data_generator.mssql_db_writer import MsSQLDbWriter
-from tests.test_models import test_model, test_model2, test_model3
+from unittest import mock
+
+import pytest
+
+from tests.write.schema import test_schema1, test_schema3
+from tsperf.adapter.mssql import MsSQLDbAdapter
+from tsperf.model.configuration import DatabaseConnectionConfiguration
+from tsperf.model.interface import DatabaseInterfaceType
+
+pyodbc = pytest.importorskip("pyodbc")
+
+
+@pytest.fixture
+def config():
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.MicrosoftSQL,
+        address="localhost:1433",
+    )
+    return config
 
 
 @mock.patch.object(pyodbc, "connect", autospec=True)
-def test_prepare_database1(mock_connect):
+def test_prepare_database1(mock_connect, config):
     """
     This function tests if the .prepare_database() function uses the correct statement to create the database table
 
     Pre Condition: pyodbc.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        MsSQLDbWriter is called.
-    -> mock_connect is called by MsSQLDbWriter with values given the constructor
+        MsSQLDbAdapter is called.
+    -> mock_connect is called by MsSQLDbAdapter with values given the constructor
 
-    Test Case 1: calling MsSQLDbWriter.prepare_database()
+    Test Case 1: calling MsSQLDbAdapter.prepare_database()
     -> "temperature" is in stmt (table name)
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = MsSQLDbWriter("localhost", "mssql", "password", "test", test_model)
+
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.MicrosoftSQL,
+        address="localhost:1433",
+        username="foobar",
+        password="bazqux",
+        database="testdrive",
+        schema=test_schema1,
+    )
+    db_writer = MsSQLDbAdapter(config=config, schema=test_schema1)
+
     connection_string = (
         "DRIVER={ODBC Driver 17 for SQL Server};SERVER=localhost,1433;"
-        "DATABASE=test;UID=mssql;PWD=password;CONNECTION TIMEOUT=170000;"
+        "DATABASE=testdrive;UID=foobar;PWD=bazqux;CONNECTION TIMEOUT=10;"
     )
-    mock_connect.assert_called_with(connection_string)
+    mock_connect.assert_called_with(connection_string, timeout=15)
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     # table name is in stmt
     assert "temperature" in stmt
 
 
 @mock.patch.object(pyodbc, "connect", autospec=True)
-def test_prepare_database2(mock_connect):
+def test_prepare_database2(mock_connect, config):
     """
     This function tests if the .prepare_database() function uses the correct statment to create the database table
 
     Pre Condition: pyodbc.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        MsSQLDbWriter is called.
+        MsSQLDbAdapter is called.
 
-    Test Case 1: calling MsSQLDbWriter.prepare_database() with default values overwritten by constructor arguments
-    -> "table_name" is in stmt (table name)
+    Test Case 1: calling MsSQLDbAdapter.prepare_database() with default values overwritten by constructor arguments
+    -> "table" is in stmt (table name)
     -> conn.commit function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = MsSQLDbWriter(
-        "localhost", "timescale2", "password2", "test", test_model2, 1444, "table_name"
-    )
+
+    config.table = "foobar"
+    db_writer = MsSQLDbAdapter(config=config, schema=test_schema1)
+
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     # table name is in stmt
-    assert "table_name" in stmt
+    assert "foobar" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(pyodbc, "connect", autospec=True)
-def test_prepare_database3(mock_connect):
+def test_prepare_database3(mock_connect, config):
     """
     This function tests if the .prepare_database() function uses the correct statement to create the database table
 
     Pre Condition: pyodbc.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        MsSQLDbWriter is called.
+        MsSQLDbAdapter is called.
 
-    Test Case 1: calling MsSQLDbWriter.prepare_database() with default values overwritten by constructor arguments
+    Test Case 1: calling MsSQLDbAdapter.prepare_database() with default values overwritten by constructor arguments
     -> tags are of type STRING
     -> conn.commit function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = MsSQLDbWriter(
-        "localhost", "timescale2", "password2", "test", test_model3
-    )
+
+    db_writer = MsSQLDbAdapter(config=config, schema=test_schema3)
+
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     assert "plant TEXT" in stmt
     assert "line TEXT" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(pyodbc, "connect", autospec=True)
-def test_insert_stmt(mock_connect):
+def test_insert_stmt(mock_connect, config):
     """
     This function tests if the .insert_stmt() function uses the correct statement to insert values
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.insert_stmt()
+    Test Case 1: calling TimescaleDbAdapter.insert_stmt()
     -> "plant" is in stmt
     -> "line" is in stmt
     -> "sensor_id" is in stmt
     -> "value" is in stmt
     -> "button_press" is in stmt
     -> conn.commit() function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = MsSQLDbWriter("localhost", "mssql", "password", "test", test_model)
+
+    db_writer = MsSQLDbAdapter(config=config, schema=test_schema1)
+
     # Test Case 1:
     db_writer.insert_stmt(
         [1586327807000],
         [{"plant": 1, "line": 1, "sensor_id": 1, "value": 6.7, "button_press": False}],
     )
     call_arguments = cursor.executemany.call_args.args
     stmt = call_arguments[0]
@@ -137,30 +165,32 @@
     assert "sensor_id" in stmt
     assert "value" in stmt
     assert "button_press" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(pyodbc, "connect", autospec=True)
-def test_execute_query(mock_connect):
+def test_execute_query(mock_connect, config):
     """
     This function tests if the .execute_query() function uses the given query
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.execute_query()
+    Test Case 1: calling TimescaleDbAdapter.execute_query()
     -> cursor.execute function is called with given argument
     -> cursor.fetchall function is called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = MsSQLDbWriter("localhost", "mssql", "password", "test", test_model)
+
+    db_writer = MsSQLDbAdapter(config=config, schema=test_schema1)
+
     db_writer.execute_query("SELECT * FROM temperature;")
     cursor.execute.assert_called_with("SELECT * FROM temperature;")
     cursor.fetchall.assert_called()
```

### Comparing `tsperf-1.1.0/tests/test_postgres_db_writer.py` & `tsperf-1.2.0/tests/adapter/test_postgresql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,188 +1,211 @@
-import mock
+from unittest import mock
+
 import psycopg2.extras
-from data_generator.postgres_db_writer import PostgresDbWriter
-from tests.test_models import test_model, test_model2, test_model3
+import pytest
+
+from tests.write.schema import test_schema1, test_schema3
+from tsperf.adapter.postgresql import PostgreSQLAdapter
+from tsperf.model.configuration import DatabaseConnectionConfiguration
+from tsperf.model.interface import DatabaseInterfaceType
+
+
+@pytest.fixture
+def config():
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.PostgreSQL,
+        address="localhost:5432",
+    )
+    return config
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
 def test_close_connection(mock_connect):
     """
     This function tests if the .close() functions of the self.conn and self.cursor objects is called
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
-    -> mock_connect is called by TimescaleDbWriter with values given the constructor
+        TimescaleDbAdapter is called.
+    -> mock_connect is called by TimescaleDbAdapter with values given the constructor
 
     Test Case 1:
-    when calling TimescaleDbWriter.close_connection() conn.close() and cursor.close() are called
+    when calling TimescaleDbAdapter.close_connection() conn.close() and cursor.close() are called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = PostgresDbWriter(
-        "localhost", 4200, "timescale", "password", "test", test_model
+
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.PostgreSQL,
+        address="localhost:5432",
+        username="foobar",
+        password=None,
+        database="test",
     )
+    db_writer = PostgreSQLAdapter(config=config, schema=test_schema1)
+
     mock_connect.assert_called_with(
-        dbname="test",
-        user="timescale",
-        password="password",
         host="localhost",
-        port=4200,
+        port=5432,
+        user="foobar",
+        password=None,
+        dbname="test",
     )
     # Test Case 1:
     db_writer.close_connection()
     conn.close.assert_called()
     cursor.close.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
 def test_prepare_database1(mock_connect):
     """
     This function tests if the .prepare_database() function uses the correct statment to create the database table
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
-    -> mock_connect is called by TimescaleDbWriter with values given the constructor
+        TimescaleDbAdapter is called.
+    -> mock_connect is called by TimescaleDbAdapter with values given the constructor
 
-    Test Case 1: calling TimescaleDbWriter.prepare_database()
+    Test Case 1: calling TimescaleDbAdapter.prepare_database()
     -> "temperature" is in stmt (table name)
     -> "ts_week" is in stmt (partitioning of hyper_table)
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = PostgresDbWriter(
-        "localhost", 4200, "timescale", "password2", "test", test_model
+
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.PostgreSQL,
+        address="localhost:5432",
+        username="foobar",
+        password="bazqux",
+        database="test",
     )
+    db_writer = PostgreSQLAdapter(config=config, schema=test_schema1)
+
     mock_connect.assert_called_with(
-        dbname="test",
-        user="timescale",
-        password="password2",
         host="localhost",
-        port=4200,
+        port=5432,
+        user="foobar",
+        password="bazqux",
+        dbname="test",
     )
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     # table name is in stmt
     assert "temperature" in stmt
     # partition is default
     assert "ts_week" in stmt
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_prepare_database2(mock_connect):
+def test_prepare_database2(mock_connect, config):
     """
     This function tests if the .prepare_database() function uses the correct statment to create the database table
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.prepare_database() with default values overwritten by constructor arguments
-    -> "table_name" is in stmt (table name)
+    Test Case 1: calling TimescaleDbAdapter.prepare_database() with default values overwritten by constructor arguments
+    -> "table" is in stmt (table name)
     -> "ts_day is in stmt (partitioning of hyper_table)
     -> conn.commit function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = PostgresDbWriter(
-        "localhost",
-        4200,
-        "timescale3",
-        "password3",
-        "test",
-        test_model2,
-        "table_name",
-        "day",
-    )
+
+    config.table = "table"
+    config.partition = "day"
+    db_writer = PostgreSQLAdapter(config=config, schema=test_schema1)
+
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     # table name is in stmt
-    assert "table_name" in stmt
+    assert "table" in stmt
     # partition is correctly set
     assert "ts_day" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_prepare_database3(mock_connect):
+def test_prepare_database3(mock_connect, config):
     """
     This function tests if the .prepare_database() function uses the correct statment to create the database table
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.prepare_database() with default values overwritten by constructor arguments
+    Test Case 1: calling TimescaleDbAdapter.prepare_database() with default values overwritten by constructor arguments
     -> tags are of type TEXT
     -> conn.commit function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = PostgresDbWriter(
-        "localhost", 4200, "timescale3", "password3", "test", test_model3
-    )
+
+    db_writer = PostgreSQLAdapter(config=config, schema=test_schema3)
+
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     assert "plant TEXT" in stmt
     assert "line TEXT" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_insert_stmt(mock_connect):
+def test_insert_stmt(mock_connect, config):
     """
     This function tests if the .insert_stmt() function uses the correct statement to insert values
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.insert_stmt()
+    Test Case 1: calling TimescaleDbAdapter.insert_stmt()
     -> "plant" is in stmt
     -> "line" is in stmt
     -> "sensor_id" is in stmt
     -> "value" is in stmt
     -> "button_press" is in stmt
     -> conn.commit() function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = PostgresDbWriter(
-        "localhost", 4200, "timescale", "password", "test", test_model
-    )
+
+    db_writer = PostgreSQLAdapter(config=config, schema=test_schema1)
+
     # Test Case 1:
     db_writer.insert_stmt(
         [1586327807000],
         [{"plant": 1, "line": 1, "sensor_id": 1, "value": 6.7, "button_press": False}],
     )
     call_arguments = cursor.execute.call_args.args
     stmt = call_arguments[0]
@@ -192,32 +215,32 @@
     assert "sensor_id" in stmt
     assert "value" in stmt
     assert "button_press" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_execute_query(mock_connect):
+def test_execute_query(mock_connect, config):
     """
     This function tests if the .execute_query() function uses the given query
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.execute_query()
+    Test Case 1: calling TimescaleDbAdapter.execute_query()
     -> cursor.execute function is called with given argument
     -> cursor.fetchall function is called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = PostgresDbWriter(
-        "localhost", 4200, "timescale", "password", "test", test_model
-    )
+
+    db_writer = PostgreSQLAdapter(config=config, schema=test_schema1)
+
     db_writer.execute_query("SELECT * FROM temperature;")
     cursor.execute.assert_called_with("SELECT * FROM temperature;")
     cursor.fetchall.assert_called()
```

### Comparing `tsperf-1.1.0/tests/test_timescale_db_writer.py` & `tsperf-1.2.0/tests/adapter/test_timescaledb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,230 +1,242 @@
-import mock
-import psycopg2.extras
 from datetime import datetime
+from unittest import mock
+
+import psycopg2.extras
+import pytest
 from datetime_truncate import truncate
-from data_generator.timescale_db_writer import TimescaleDbWriter
-from tests.test_models import test_model, test_model2, test_model3
+
+from tests.write.schema import test_schema1, test_schema2, test_schema3
+from tsperf.adapter.timescaledb import TimescaleDbAdapter
+from tsperf.model.configuration import DatabaseConnectionConfiguration
+from tsperf.model.interface import DatabaseInterfaceType
+
+
+@pytest.fixture
+def config():
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.TimescaleDB,
+        address="localhost:5432",
+    )
+    return config
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
 def test_close_connection(mock_connect):
     """
     This function tests if the .close() functions of the self.conn and self.cursor objects is called
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
-    -> mock_connect is called by TimescaleDbWriter with values given the constructor
+        TimescaleDbAdapter is called.
+    -> mock_connect is called by TimescaleDbAdapter with values given the constructor
 
     Test Case 1:
-    when calling TimescaleDbWriter.close_connection() conn.close() and cursor.close() are called
+    when calling TimescaleDbAdapter.close_connection() conn.close() and cursor.close() are called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = TimescaleDbWriter(
-        "localhost", 4200, "timescale", "password", "test", test_model
+
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.TimescaleDB,
+        address="localhost:5432",
+        username="foobar",
+        password=None,
+        database="test",
+        schema=test_schema1,
     )
+    db_writer = TimescaleDbAdapter(config=config, schema=test_schema1)
+
     mock_connect.assert_called_with(
-        dbname="test",
-        user="timescale",
-        password="password",
         host="localhost",
-        port=4200,
+        port=5432,
+        user="foobar",
+        password=None,
+        dbname="test",
     )
     # Test Case 1:
     db_writer.close_connection()
     conn.close.assert_called()
     cursor.close.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_prepare_database1(mock_connect):
+def test_prepare_database_auth(mock_connect, config):
     """
     This function tests if the .prepare_database() function uses the correct statment to create the database table
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
-    -> mock_connect is called by TimescaleDbWriter with values given the constructor
+        TimescaleDbAdapter is called.
+    -> mock_connect is called by TimescaleDbAdapter with values given the constructor
 
-    Test Case 1: calling TimescaleDbWriter.prepare_database()
+    Test Case 1: calling TimescaleDbAdapter.prepare_database()
     -> "temperature" is in stmt (table name)
     -> "ts_week" is in stmt (partitioning of hyper_table)
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = TimescaleDbWriter(
-        "localhost", 4200, "timescale", "password2", "test", test_model
-    )
+
+    db_writer = TimescaleDbAdapter(config=config, schema=test_schema1)
+
     mock_connect.assert_called_with(
-        dbname="test",
-        user="timescale",
-        password="password2",
         host="localhost",
-        port=4200,
+        port=5432,
+        user="postgres",
+        password=None,
+        dbname=None,
     )
+
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     # table name is in stmt
     assert "temperature" in stmt
     # partition is default
     assert "ts_week" in stmt
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_prepare_database2(mock_connect):
+def test_prepare_database_table_partition(mock_connect, config):
     """
-    This function tests if the .prepare_database() function uses the correct statment to create the database table
+    This function tests if the .prepare_database() function uses the correct statement to create the database table
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.prepare_database() with default values overwritten by constructor arguments
-    -> "table_name" is in stmt (table name)
+    Test Case 1: calling TimescaleDbAdapter.prepare_database() with default values overwritten by constructor arguments
+    -> "table" is in stmt (table name)
     -> "ts_day is in stmt (partitioning of hyper_table)
     -> conn.commit function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = TimescaleDbWriter(
-        "localhost",
-        4200,
-        "timescale3",
-        "password3",
-        "test",
-        test_model2,
-        "table_name",
-        "day",
-    )
+
+    config.table = "foobar"
+    config.partition = "day"
+    db_writer = TimescaleDbAdapter(config=config, schema=test_schema2)
+
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     # table name is in stmt
-    assert "table_name" in stmt
+    assert "foobar" in stmt
     # partition is correctly set
     assert "ts_day" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_prepare_database3(mock_connect):
+def test_prepare_database_distributed(mock_connect, config):
     """
     This function tests if the .prepare_database() function uses the correct statement to create the database table
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.prepare_database() with default values overwritten by constructor arguments
+    Test Case 1: calling TimescaleDbAdapter.prepare_database() with default values overwritten by constructor arguments
     -> "distributed" is in stmt (table name)
     -> conn.commit function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = TimescaleDbWriter(
-        "localhost",
-        4200,
-        "timescale3",
-        "password3",
-        "test",
-        test_model2,
-        "table_name",
-        "day",
-        True,
-        True,
-    )
+
+    config.partition = "day"
+    config.timescaledb_distributed = True
+
+    db_writer = TimescaleDbAdapter(config=config, schema=test_schema2)
+
     # Test Case 1:
     db_writer.prepare_database()
     stmt = cursor.execute.call_args.args[0]
     # distributed is in stmt
     assert "distributed" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_prepare_database4(mock_connect):
+def test_prepare_database_test_schema(mock_connect, config):
     """
-    This function tests if the .prepare_database() function uses the correct statment to create the database table
+    This function tests if the .prepare_database() function uses the correct statement to create the database table
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.prepare_database() with default values overwritten by constructor arguments
+    Test Case 1: calling TimescaleDbAdapter.prepare_database() with default values overwritten by constructor arguments
     -> tags are of type TEXT
     -> conn.commit function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = TimescaleDbWriter(
-        "localhost", 4200, "timescale3", "password3", "test", test_model3
-    )
+
+    db_writer = TimescaleDbAdapter(config=config, schema=test_schema3)
+
     # Test Case 1:
     db_writer.prepare_database()
-    stmt = str(cursor.execute.call_args_list[0])
+    stmt = str(cursor.execute.call_args_list[1])
     assert "plant TEXT" in stmt
     assert "line TEXT" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_insert_stmt(mock_connect):
+def test_insert_vanilla(mock_connect, config):
     """
     This function tests if the .insert_stmt() function uses the correct statement to insert values
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.insert_stmt()
+    Test Case 1: calling TimescaleDbAdapter.insert_stmt()
     -> "plant" is in stmt
     -> "line" is in stmt
     -> "sensor_id" is in stmt
     -> "value" is in stmt
     -> "button_press" is in stmt
     -> conn.commit() function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = TimescaleDbWriter(
-        "localhost", 4200, "timescale", "password", "test", test_model
-    )
+
+    db_writer = TimescaleDbAdapter(config=config, schema=test_schema1)
+
     # Test Case 1:
     db_writer.insert_stmt(
         [1586327807000],
         [{"plant": 1, "line": 1, "sensor_id": 1, "value": 6.7, "button_press": False}],
     )
     call_arguments = cursor.execute.call_args.args
     stmt = call_arguments[0]
@@ -234,42 +246,42 @@
     assert "sensor_id" in stmt
     assert "value" in stmt
     assert "button_press" in stmt
     conn.commit.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-@mock.patch("data_generator.timescale_db_writer.CopyManager", autospec=True)
-def test_insert_stmt_copy(mock_copy_manager, mock_connect):
+@mock.patch("tsperf.adapter.timescaledb.CopyManager", autospec=True)
+def test_insert_pgcopy(mock_copy_manager, mock_connect, config):
     """
     This function tests if the the copy_manager is called correctly if timescale is used with
     copy insert method
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called with copy=True.
+        TimescaleDbAdapter is called with copy=True.
 
-    Test Case 1: calling TimescaleDbWriter.insert_stmt()
+    Test Case 1: calling TimescaleDbAdapter.insert_stmt()
     -> "plant" is in stmt
     -> "line" is in stmt
     -> "sensor_id" is in stmt
     -> "value" is in stmt
     -> "button_press" is in stmt
     -> conn.commit() function has been called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.MagicMock()
     cursor = mock.MagicMock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = TimescaleDbWriter(
-        "localhost", 4200, "timescale", "password", "test", test_model, copy=True
-    )
+
+    config.timescaledb_pgcopy = True
+    db_writer = TimescaleDbAdapter(config=config, schema=test_schema1)
 
     copy_manager = mock.MagicMock()
     mock_copy_manager.return_value = copy_manager
     # Test Case 1:
     db_writer.insert_stmt(
         [1586327807000],
         [{"plant": 1, "line": 1, "sensor_id": 1, "value": 6.7, "button_press": False}],
@@ -291,32 +303,31 @@
     assert 1 in call_arguments_copy
     assert 6.7 in call_arguments_copy
     assert False in call_arguments_copy
     conn.commit.assert_called()
 
 
 @mock.patch.object(psycopg2, "connect", autospec=True)
-def test_execute_query(mock_connect):
+def test_execute_query(mock_connect, config):
     """
     This function tests if the .execute_query() function uses the given query
 
     Pre Condition: psycopg2.client.connect() returns a Mock Object conn which returns a Mock Object
         cursor when its .cursor() function is called.
-        TimescaleDbWriter is called.
+        TimescaleDbAdapter is called.
 
-    Test Case 1: calling TimescaleDbWriter.execute_query()
+    Test Case 1: calling TimescaleDbAdapter.execute_query()
     -> cursor.execute function is called with given argument
     -> cursor.fetchall function is called
 
     :param mock_connect: mocked function call from psycopg2.client.connect()
     """
     # Pre Condition:
     conn = mock.Mock()
     cursor = mock.Mock()
     mock_connect.return_value = conn
     conn.cursor.return_value = cursor
-    db_writer = TimescaleDbWriter(
-        "localhost", 4200, "timescale", "password", "test", test_model
-    )
+
+    db_writer = TimescaleDbAdapter(config=config, schema=test_schema1)
     db_writer.execute_query("SELECT * FROM temperature;")
     cursor.execute.assert_called_with("SELECT * FROM temperature;")
     cursor.fetchall.assert_called()
```

### Comparing `tsperf-1.1.0/tests/test_timestream_db_writer.py` & `tsperf-1.2.0/tests/adapter/test_timestream.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,75 @@
-import mock
-from data_generator.timestream_db_writer import TimeStreamWriter
-from tests.test_models import test_model
+from unittest import mock
 
+import pytest
 
-@mock.patch("data_generator.timestream_db_writer.boto3", autospec=True)
-def test_close_connection(mock_boto):
+from tests.write.schema import test_schema1
+from tsperf.adapter.timestream import AmazonTimestreamAdapter
+from tsperf.model.configuration import DatabaseConnectionConfiguration
+from tsperf.model.interface import DatabaseInterfaceType
+
+
+@pytest.fixture
+def config():
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.Timestream,
+        # TODO: address="ingest-cell1.timestream.us-west-2.amazonaws.com",
+    )
+    return config
+
+
+@mock.patch("tsperf.adapter.timestream.boto3", autospec=True)
+def test_close_connection(mock_boto, config):
     """
-    Test if the .close_connection() function of TimeStreamWriter calls the close() function of self.client
+    Test if the .close_connection() function of AmazonTimestreamAdapter calls the close() function of self.client
 
     Test Case 1:boto.session.Session() returns a Mock Object session
-        TimeStreamWriter is called.
-    -> Parameters of TimeStreamWriter match constructor parameters
+        AmazonTimestreamAdapter is called.
+    -> Parameters of AmazonTimestreamAdapter match constructor parameters
 
     :param mock_boto: mocked boto3 class
     """
     session = mock.MagicMock()
     mock_boto.session.Session.return_value = session
-    _ = TimeStreamWriter(
-        "aws_key_id", "aws_secrete", "aws_region", "db_name", test_model
-    )
-    mock_boto.session.Session.assert_called_with(
-        "aws_key_id", aws_secret_access_key="aws_secrete", region_name="aws_region"
+
+    config = DatabaseConnectionConfiguration(
+        adapter=DatabaseInterfaceType.Timestream,
+        # TODO: address="ingest-cell1.timestream.us-west-2.amazonaws.com",
+        aws_access_key_id="foobar",
+        aws_secret_access_key="bazqux",
+        aws_region_name="us-west-2",
     )
+    _ = AmazonTimestreamAdapter(config=config, schema=test_schema1)
 
+    mock_boto.session.Session.assert_called_with("foobar", aws_secret_access_key="bazqux", region_name="us-west-2")
 
-@mock.patch("data_generator.timestream_db_writer.boto3", autospec=True)
-def test_insert_stmt(mock_boto):
+
+@mock.patch("tsperf.adapter.timestream.boto3", autospec=True)
+def test_insert_stmt(mock_boto, config):
     """
-    This function tests if the .insert_stmt() function of TimeStreamWriter creates the correct json object
+    This function tests if the .insert_stmt() function of AmazonTimestreamAdapter creates the correct json object
 
     Pre Condition: boto.session.Session() returns a Mock Object session
-        TimeStreamWriter is called.
-    -> Parameters of TimeStreamWriter match constructor parameters
+        AmazonTimestreamAdapter is called.
+    -> Parameters of AmazonTimestreamAdapter match constructor parameters
 
     Test Case 1:
-    calling TimeStreamWriter.insert_stmt()
+    calling AmazonTimestreamAdapter.insert_stmt()
     -> the function call has on argument
     -> the argument is the same as the record
 
     :param mock_boto: mocked boto3 class
     """
     session = mock.MagicMock()
     mock_boto.session.Session.return_value = session
     write_client = mock.MagicMock()
     session.client.return_value = write_client
-    db_writer = TimeStreamWriter(
-        "aws_key_id", "aws_secrete", "aws_region", "db_name", test_model
-    )
+
+    db_writer = AmazonTimestreamAdapter(config=config, schema=test_schema1)
+
     # Test Case 1:
     db_writer.insert_stmt(
         [1586327807000],
         [{"plant": 2, "line": 2, "sensor_id": 2, "value": 6.7, "button_press": False}],
     )
     """
     records = [
@@ -102,96 +121,93 @@
         ]
     }
     assert len(args) == 4
     assert args["Records"] == rec_arg
     assert args["CommonAttributes"] == common_attr
 
 
-@mock.patch("data_generator.timestream_db_writer.boto3", autospec=True)
-def test_execute_query(mock_boto):
+@mock.patch("tsperf.adapter.timestream.boto3", autospec=True)
+def test_execute_query(mock_boto, config):
     """
-    This function tests if the .execute_query() function of TimeStreamWriter uses the correct argument
+    This function tests if the .execute_query() function of AmazonTimestreamAdapter uses the correct argument
 
     Pre Condition: boto.session.Session() returns a Mock Object session
-        TimeStreamWriter is called.
+        AmazonTimestreamAdapter is called.
 
     Test Case 1:
-    calling TimeStreamWriter.execute_query()
+    calling AmazonTimestreamAdapter.execute_query()
     -> the function call has on argument
     -> the argument is the same as execute_query argument
 
     :param mock_boto: mocked boto3 class
     """
     session = mock.MagicMock()
     mock_boto.session.Session.return_value = session
     query_client = mock.MagicMock()
     session.client.return_value = query_client
     paginator = mock.MagicMock()
     query_client.get_paginator.return_value = paginator
-    db_writer = TimeStreamWriter(
-        "aws_key_id", "aws_secrete", "aws_region", "db_name", test_model
-    )
+
     # Test Case 1:
+    db_writer = AmazonTimestreamAdapter(config=config, schema=test_schema1)
     query = "SELECT * FROM temperature;"
     db_writer.execute_query(query)
     paginator.paginate.assert_called_once()
     args = paginator.paginate.call_args.kwargs
     assert len(args) == 1
     assert args["QueryString"] == query
 
 
-@mock.patch("data_generator.timestream_db_writer.boto3", autospec=True)
-def test_prepare_database_not_existing_db_and_table(mock_boto):
+@mock.patch("tsperf.adapter.timestream.boto3", autospec=True)
+def test_prepare_database_not_existing_db_and_table(mock_boto, config):
     """
-    This function tests if the .execute_query() function of TimeStreamWriter uses the correct argument
+    This function tests if the .execute_query() function of AmazonTimestreamAdapter uses the correct argument
 
     Pre Condition: boto.session.Session() returns a Mock Object session
-        TimeStreamWriter is called.
+        AmazonTimestreamAdapter is called.
 
     Test Case 1:
-    calling TimeStreamWriter.prepare_database()
+    calling AmazonTimestreamAdapter.prepare_database()
     -> write_client.create_database is called once
     -> write_client.create_table is called once
 
     :param mock_boto: mocked boto3 class
     """
     session = mock.MagicMock()
     mock_boto.session.Session.return_value = session
     write_client = mock.MagicMock()
     session.client.return_value = write_client
-    db_writer = TimeStreamWriter(
-        "aws_key_id", "aws_secrete", "aws_region", "db_name", test_model
-    )
+
     # Test Case 1:
+    db_writer = AmazonTimestreamAdapter(config=config, schema=test_schema1)
     db_writer.prepare_database()
     write_client.create_database.assert_called_once()
     write_client.create_table.assert_called_once()
 
 
-@mock.patch("data_generator.timestream_db_writer.boto3", autospec=True)
-def test_prepare_database_existing_db_and_table(mock_boto):
+@mock.patch("tsperf.adapter.timestream.boto3", autospec=True)
+def test_prepare_database_existing_db_and_table(mock_boto, config):
     """
-    This function tests if the .execute_query() function of TimeStreamWriter uses the correct argument
+    This function tests if the .execute_query() function of AmazonTimestreamAdapter uses the correct argument
 
     Pre Condition: boto.session.Session() returns a Mock Object session
-        TimeStreamWriter is called.
+        AmazonTimestreamAdapter is called.
 
     Test Case 1:
-    calling TimeStreamWriter.prepare_database()
+    calling AmazonTimestreamAdapter.prepare_database()
     -> write_client.create_database is called once
     -> write_client.create_table is called once
 
     :param mock_boto: mocked boto3 class
     """
     session = mock.MagicMock()
     mock_boto.session.Session.return_value = session
     write_client = mock.MagicMock()
     session.client.return_value = write_client
-    db_writer = TimeStreamWriter(
-        "aws_key_id", "aws_secrete", "aws_region", "db_name", test_model
-    )
+
     # Test Case 1:
+    db_writer = AmazonTimestreamAdapter(config=config, schema=test_schema1)
     write_client.create_database.side_effect = Exception()
     write_client.create_table.side_effect = Exception()
     db_writer.prepare_database()
     write_client.create_database.assert_called_once()
     write_client.create_table.assert_called_once()
```

### Comparing `tsperf-1.1.0/tests/util/test_batch_size_automator.py` & `tsperf-1.2.0/tests/util/test_batch_size_automator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from batch_size_automator import BatchSizeAutomator
+from tsperf.util.batch_size_automator import BatchSizeAutomator
 
 
 def test_is_auto_batch_mode():
     """
     This function tests if the auto_batch_mode of the BatchSizeAutomator is correctly caluclated.
 
     Test Case 1: batch_size is bigger than 0 and => auto_batch_mode is False
@@ -107,102 +107,87 @@
     batch_size_automator = BatchSizeAutomator(0)
     initial_batch_size = 2500
     assert batch_size_automator.get_next_batch_size() == initial_batch_size
 
     # Test Case 1:
     # ten will be the first best time
     duration = 10
-    for i in range(0, batch_size_automator.test_size):
+    for _ in range(0, batch_size_automator.test_size):
         batch_size_automator.insert_batch_time(duration)
 
     assert batch_size_automator.batch_times["best"]["avg_time"] == duration
-    assert (
-        batch_size_automator.batch_times["best"]["batch_per_second"]
-        == initial_batch_size / duration
-    )
+    assert batch_size_automator.batch_times["best"]["batch_per_second"] == initial_batch_size / duration
     # because for the next iteration batch_size is increased by 500
     initial_step_size = 500
-    assert (
-        batch_size_automator.get_next_batch_size()
-        == initial_batch_size + initial_step_size
-    )
+    assert batch_size_automator.get_next_batch_size() == initial_batch_size + initial_step_size
 
     # Test Case 2:
     # five will be the first best time making 3000 the best batchsize
     duration = 5
-    for i in range(0, batch_size_automator.test_size):
+    for _ in range(0, batch_size_automator.test_size):
         batch_size_automator.insert_batch_time(duration)
     current_batch_size = initial_batch_size + initial_step_size
     current_batch_per_second = current_batch_size / duration
 
     assert batch_size_automator.batch_times["best"]["avg_time"] == duration
-    assert (
-        batch_size_automator.batch_times["best"]["batch_per_second"]
-        == current_batch_per_second
-    )
+    assert batch_size_automator.batch_times["best"]["batch_per_second"] == current_batch_per_second
     batch_size = 3000 + batch_size_automator.step_size * batch_size_automator.alpha
     assert batch_size_automator.get_next_batch_size() == batch_size
 
     # Test Case 3:
     # next is worse
     duration = 7
-    for i in range(0, batch_size_automator.test_size):
+    for _ in range(0, batch_size_automator.test_size):
         batch_size_automator.insert_batch_time(duration)
 
     assert batch_size_automator.batch_times["best"]["avg_time"] == 5  # last duration
-    assert (
-        batch_size_automator.batch_times["best"]["batch_per_second"]
-        == current_batch_per_second
-    )
+    assert batch_size_automator.batch_times["best"]["batch_per_second"] == current_batch_per_second
     # batch_size is decreased this time because no better value was found and calculated based on best_size
     batch_size = (
-        batch_size_automator.batch_times["best"]["size"]
-        - batch_size_automator.step_size * batch_size_automator.alpha
+        batch_size_automator.batch_times["best"]["size"] - batch_size_automator.step_size * batch_size_automator.alpha
     )
     assert batch_size_automator.get_next_batch_size() == batch_size
 
     # Test Case 4:
     # next is best
     duration = 4
-    for i in range(0, batch_size_automator.test_size):
+    for _ in range(0, batch_size_automator.test_size):
         batch_size_automator.insert_batch_time(duration)
 
     assert batch_size_automator.batch_times["best"]["avg_time"] == duration
     assert (
         batch_size_automator.batch_times["best"]["batch_per_second"]
         == batch_size_automator.batch_times["best"]["size"] / duration
     )
     # batch_size is further decreased
-    batch_size = (
-        batch_size - batch_size_automator.step_size * batch_size_automator.alpha
-    )
+    batch_size = batch_size - batch_size_automator.step_size * batch_size_automator.alpha
     assert batch_size_automator.get_next_batch_size() == batch_size
 
     # Test Case 5:
     # we insert batch times until we switch to surveillance mode
     duration = 5
     while not batch_size_automator.surveillance_mode:
         batch_size_automator.insert_batch_time(duration)
 
     # for the next surveillance period we have no change in best batch size
     duration = 3
-    for i in range(0, batch_size_automator.test_size):
+    for _ in range(0, batch_size_automator.test_size):
         batch_size_automator.insert_batch_time(duration)
 
     assert batch_size_automator.batch_times["best"]["avg_time"] == duration
     assert (
         batch_size_automator.batch_times["best"]["batch_per_second"]
         == batch_size_automator.batch_times["best"]["size"] / duration
     )
     assert batch_size_automator.surveillance_mode
 
     # Test Case 6:
     # performance is worse so we switch out of surveillance mode and try to find best batch size again
     duration = 5
-    for i in range(0, batch_size_automator.test_size):
+    for _ in range(0, batch_size_automator.test_size):
         batch_size_automator.insert_batch_time(duration)
 
     assert not batch_size_automator.surveillance_mode
 
 
 def test_insert_batch_time_smallest_batch():
     """
@@ -220,33 +205,29 @@
     # Pre Condition:
     batch_size_automator = BatchSizeAutomator(0)
 
     # Test Case 1:
     # batch size will allways get smaller until we are under 1
     # first we have a baseline
     long_duration = 10000
-    for i in range(0, batch_size_automator.test_size):
+    for _ in range(0, batch_size_automator.test_size):
         batch_size_automator.insert_batch_time(long_duration)
 
     # then we get worse so direction of optimization is reversed
     worse_duration = 100000
-    for i in range(0, batch_size_automator.test_size):
+    for _ in range(0, batch_size_automator.test_size):
         batch_size_automator.insert_batch_time(worse_duration)
 
     # now we get better each time until we reach batch_size 1
-    duration = (
-        batch_size_automator.batch_size
-        / batch_size_automator.batch_times["best"]["batch_per_second"]
-    ) - 10
+    duration = (batch_size_automator.batch_size / batch_size_automator.batch_times["best"]["batch_per_second"]) - 10
     batch_size = batch_size_automator.batch_size
     while batch_size_automator.batch_size != 1:
         if batch_size != batch_size_automator.batch_size:
             duration = (
-                batch_size_automator.batch_size
-                / batch_size_automator.batch_times["best"]["batch_per_second"]
+                batch_size_automator.batch_size / batch_size_automator.batch_times["best"]["batch_per_second"]
             ) - 10
             batch_size = batch_size_automator.batch_size
         batch_size_automator.insert_batch_time(duration)
 
     # once we reached a negative batch_size and it was reset to 1 the batch_size should get bigger again
     assert batch_size_automator.bigger_batch_size
 
@@ -279,59 +260,43 @@
 
     assert batch_size_automator.step_size == default_step_size
 
 
 def test_step_size_is_data_batch_size():
     default_step_size = 500
     data_batch_size = 1000
-    batch_size_automator = BatchSizeAutomator(
-        0, data_batch_size=data_batch_size, step_size=default_step_size
-    )
+    batch_size_automator = BatchSizeAutomator(0, data_batch_size=data_batch_size, step_size=default_step_size)
 
     assert batch_size_automator.step_size == data_batch_size
 
 
 def test_batch_size_is_multitude_of_data_batch_size():
     data_batch_size = 500
     batch_size = 700
-    batch_size_automator = BatchSizeAutomator(
-        batch_size, data_batch_size=data_batch_size
-    )
+    batch_size_automator = BatchSizeAutomator(batch_size, data_batch_size=data_batch_size)
 
     assert batch_size_automator.batch_size == 500
 
     data_batch_size = 500
     batch_size = 800
-    batch_size_automator = BatchSizeAutomator(
-        batch_size, data_batch_size=data_batch_size
-    )
+    batch_size_automator = BatchSizeAutomator(batch_size, data_batch_size=data_batch_size)
 
     assert batch_size_automator.batch_size == 1000
 
     data_batch_size = 500
     batch_size = 400
-    batch_size_automator = BatchSizeAutomator(
-        batch_size, data_batch_size=data_batch_size
-    )
+    batch_size_automator = BatchSizeAutomator(batch_size, data_batch_size=data_batch_size)
 
     assert batch_size_automator.batch_size == 500
 
 
 def test_batch_size_change_is_at_least_data_batch_size():
     data_batch_size = 500
     test_size = 1
-    batch_size_automator = BatchSizeAutomator(
-        0, data_batch_size=data_batch_size, test_size=test_size
-    )
+    batch_size_automator = BatchSizeAutomator(0, data_batch_size=data_batch_size, test_size=test_size)
 
     # initial test cycle:
     batch_size_automator.insert_batch_time(1)
-    assert (
-        batch_size_automator.get_next_batch_size() == 3000
-    )  # initially bath_size will go up
+    assert batch_size_automator.get_next_batch_size() == 3000  # initially bath_size will go up
     # second test cycle:
-    batch_size_automator.insert_batch_time(
-        2
-    )  # worse batch performance reduces alpha and leads to smaller step_size
-    assert (
-        batch_size_automator.get_next_batch_size() == 2000
-    )  # batch_size is changed by at least data_batch_size
+    batch_size_automator.insert_batch_time(2)  # worse batch performance reduces alpha and leads to smaller step_size
+    assert batch_size_automator.get_next_batch_size() == 2000  # batch_size is changed by at least data_batch_size
```

### Comparing `tsperf-1.1.0/tests/util/test_ticktrack.py` & `tsperf-1.2.0/tests/util/test_ticktrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import mock
-import pytest
 import statistics
-import tictrack
+from unittest import mock
+
+import pytest
+
+from tsperf.util import tictrack
 
 
 @pytest.fixture(scope="session", autouse=True)
 def reset_tictoc_baseline():
     tictrack.reset("foo")
     tictrack.reset_delta("foo")
 
@@ -140,17 +142,15 @@
 
 
 @mock.patch("builtins.print", autospec=True)
 def test_wrapper_print_not_save(mock_print):
     def foo(a, b):
         return a + b
 
-    return_value = tictrack.execute_timed_function(
-        foo, 1, 2, do_print=True, save_result=False
-    )
+    return_value = tictrack.execute_timed_function(foo, 1, 2, do_print=True, save_result=False)
     assert return_value == 3
     assert mock_print.call_count == 1
     assert "foo" not in tictrack.tic_toc
     assert "foo" not in tictrack.tic_toc_delta
 
 
 def test_wrapper_simple_kwargs():
@@ -259,17 +259,15 @@
 
 
 def test_stats_args_kwargs_delta():
     def bar(a, b, c, d):
         return sum(a) + (c / b) - d
 
     tictrack.tic_toc_delta["foo"] = [1, 2, 3, 4, 5, 6, 7]
-    return_value = tictrack.timed_function_statistics(
-        "foo", bar, 2, delta=True, d=4, c=2
-    )
+    return_value = tictrack.timed_function_statistics("foo", bar, 2, delta=True, d=4, c=2)
     assert return_value == 25
 
 
 def test_consolidate_no_values():
     with pytest.raises(ValueError):
         tictrack.consolidate("foo")
```

### Comparing `tsperf-1.1.0/tictrack/__init__.py` & `tsperf-1.2.0/tsperf/util/tictrack/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import time
 import statistics
-
-from typing import Callable, Any
-
+import time
+from typing import Any, Callable
 
 tic_toc = {}
 tic_toc_delta = {}
 enabled = True
 delta_enabled = True
 
 
@@ -39,26 +37,22 @@
     :param do_print: boolean to decide if result is printed or not (optional) default False.
     :param save_result: boolean to decide if result is saved for later statistical analysis (optional) default True
     :return: decorator
     """
 
     def decorator(func: Callable) -> Callable:
         def wrapper(*args, **kwargs) -> Any:
-            return execute_timed_function(
-                func, *args, **kwargs, do_print=do_print, save_result=save_result
-            )
+            return execute_timed_function(func, *args, **kwargs, do_print=do_print, save_result=save_result)
 
         return wrapper
 
     return decorator
 
 
-def execute_timed_function(
-    func: Callable, *args, do_print: bool = False, save_result: bool = True, **kwargs
-) -> Any:
+def execute_timed_function(func: Callable, *args, do_print: bool = False, save_result: bool = True, **kwargs) -> Any:
     """
     function that takes another function as an argument and measures its execution time and saves it to a dictionary
     so statistical functions can be used for many executions of the given function
 
     :param func: function where execution time should be measured
     :param args: arguments for func
     :param do_print: boolean to decide if result is printed or not (optional) default False
@@ -82,15 +76,15 @@
         if delta_enabled:
             if func.__name__ not in tic_toc_delta:
                 tic_toc_delta[func.__name__] = []
 
             tic_toc_delta[func.__name__].append(toc)
 
     if do_print:
-        print(f"{func.__name__} took: {toc} seconds")
+        print(f"{func.__name__} took: {toc} seconds")  # noqa: T201
     return function_return
 
 
 def timed_function_statistics(
     function_name: str,
     func: Callable = statistics.mean,
     *args,
@@ -111,18 +105,16 @@
     :return: return value of func
     """
     times = tic_toc_delta if delta else tic_toc
 
     if function_name in times:
         try:
             return func(times[function_name], *args, **kwargs)
-        except Exception as e:
-            raise SyntaxError(
-                f"calling {func.__name__} on result raises an exception: {e}\n"
-            )
+        except Exception as ex:
+            raise SyntaxError(f"calling {func.__name__} on result raises an exception: {ex}") from ex
     else:
         raise ValueError(f"no execution times saved for {function_name}")
 
 
 def consolidate(
     function_name: str,
     func: Callable = statistics.mean,
@@ -144,26 +136,22 @@
     :param delta: boolean if set to True the calculation is done on the delta values (optional) default False
     :param kwargs: keyword arguments for func
     """
     times = tic_toc_delta if delta else tic_toc
     if function_name in times:
         try:
             consolidated_value = func(times[function_name], *args, **kwargs)
-        except Exception as e:
-            raise SyntaxError(
-                f"calling {func.__name__} on result raises an exception: {e}\n"
-            )
+        except Exception as ex:
+            raise SyntaxError(f"calling {func.__name__} on result raises an exception: {ex}") from ex
         if _valid_value(consolidated_value):
-            if type(consolidated_value) == int or type(consolidated_value) == float:
+            if isinstance(consolidated_value, int) or isinstance(consolidated_value, float):
                 consolidated_value = [consolidated_value]
             times[function_name] = consolidated_value
         else:
-            raise SyntaxError(
-                f"{func.__name__} must return either int, float, list<int> or list<float>"
-            )
+            raise SyntaxError(f"{func.__name__} must return either int, float, list<int> or list<float>")
     else:
         raise ValueError(f"no execution times saved for {function_name}")
 
 
 def _valid_value(value):
     """
     this function is used to determine if the result of the consolidate function is valid. Valid types include int,
```

