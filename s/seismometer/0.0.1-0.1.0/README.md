# Comparing `tmp/seismometer-0.0.1.tar.gz` & `tmp/seismometer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismometer-0.0.1.tar", last modified: Mon May  6 18:52:53 2024, max compression
+gzip compressed data, was "seismometer-0.1.0.tar", last modified: Tue May 21 18:34:28 2024, max compression
```

## Comparing `seismometer-0.0.1.tar` & `seismometer-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,84 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 18:52:53.324304 seismometer-0.0.1/
--rw-rw-rw-   0        0        0     1478 2024-05-06 14:46:48.000000 seismometer-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      405 2024-05-06 18:52:53.323288 seismometer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-05-06 18:50:38.000000 seismometer-0.0.1/README.md
--rw-rw-rw-   0        0        0       90 2024-05-06 14:46:36.000000 seismometer-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-06 18:52:53.322288 seismometer-0.0.1/seismometer.egg-info/
--rw-rw-rw-   0        0        0      405 2024-05-06 18:52:53.000000 seismometer-0.0.1/seismometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-06 18:52:53.000000 seismometer-0.0.1/seismometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 18:52:53.000000 seismometer-0.0.1/seismometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-06 18:52:53.000000 seismometer-0.0.1/seismometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      490 2024-05-06 18:52:53.325302 seismometer-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 18:52:53.281288 seismometer-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 18:52:53.320288 seismometer-0.0.1/src/seismometer/
--rw-rw-rw-   0        0        0        0 2024-05-06 14:41:14.000000 seismometer-0.0.1/src/seismometer/__init__.py
--rw-rw-rw-   0        0        0       68 2024-05-06 18:36:32.000000 seismometer-0.0.1/src/seismometer/seismometer.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:29.446732 seismometer-0.1.0/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     1478 2024-05-21 18:33:17.000000 seismometer-0.1.0/LICENSE.txt
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      335 2024-05-21 18:33:17.000000 seismometer-0.1.0/MANIFEST.in
+-rw-r--r--   0 seismo    (1000) seismo    (1000)     2598 2024-05-21 18:34:29.443616 seismometer-0.1.0/PKG-INFO
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2253 2024-05-21 18:33:17.000000 seismometer-0.1.0/README.md
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      113 2024-05-21 18:33:17.000000 seismometer-0.1.0/pyproject.toml
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2115 2024-05-21 18:34:29.453251 seismometer-0.1.0/setup.cfg
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      216 2024-05-21 18:33:17.000000 seismometer-0.1.0/setup.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:27.891881 seismometer-0.1.0/src/
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.062590 seismometer-0.1.0/src/seismometer/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     1269 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/__init__.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    26859 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/_api.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.292639 seismometer-0.1.0/src/seismometer/builder/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2809 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/__init__.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2246 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/arguments.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     4571 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/compile.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     3609 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/extract.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2246 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/jupyter.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.409539 seismometer-0.1.0/src/seismometer/builder/resources/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    37620 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/resources/classifier_bin.ipynb
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      881 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/resources/config.yml
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      960 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/resources/dictionary.yml
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     1465 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/builder/resources/usage_config.yml
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.506509 seismometer-0.1.0/src/seismometer/configuration/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      100 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/configuration/__init__.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    14040 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/configuration/config.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    10907 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/configuration/model.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2376 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/configuration/options.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.562906 seismometer-0.1.0/src/seismometer/controls/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     3723 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/controls/cohort_comparison.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     1286 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/controls/decorators.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     9314 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/controls/selection.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.646570 seismometer-0.1.0/src/seismometer/core/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     4920 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/core/_decorators.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     8864 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/core/io.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     1685 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/core/logger.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      804 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/core/patterns.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.813698 seismometer-0.1.0/src/seismometer/data/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      109 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/__init__.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    11453 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/cohorts.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.877245 seismometer-0.1.0/src/seismometer/data/confidence/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)       95 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/confidence/__init__.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     8454 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/confidence/calculations.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     6020 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/confidence/parameters.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)       71 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/decorators.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     9728 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/filter.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    13786 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/pandas_helpers.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     8555 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/performance.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2213 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/summaries.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     4002 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/data/timeseries.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.895461 seismometer-0.1.0/src/seismometer/html/
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.938013 seismometer-0.1.0/src/seismometer/html/resources/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      511 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/html/resources/cohorts.html
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      992 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/html/resources/info.html
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     1841 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/html/template.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:28.955944 seismometer-0.1.0/src/seismometer/plot/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      121 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/__init__.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:29.240479 seismometer-0.1.0/src/seismometer/plot/mpl/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      241 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/__init__.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    13899 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/_lines.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     7292 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/_util.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     8046 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/_ux.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    14650 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/binary_classifier.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     3717 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/decorators.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    10674 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/multi_classifier.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2152 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/timeseries.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     8641 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/plot/mpl/ux.mplstyle
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:29.377342 seismometer-0.1.0/src/seismometer/report/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     6645 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/report/alerting.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     2788 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/report/auditing.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)      281 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/report/decorators.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    10065 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/report/profiling.py
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     4522 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/report/report_config.yml
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)    19393 2024-05-21 18:33:17.000000 seismometer-0.1.0/src/seismometer/seismogram.py
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:29.429045 seismometer-0.1.0/src/seismometer.egg-info/
+-rw-r--r--   0 seismo    (1000) seismo    (1000)     2598 2024-05-21 18:34:27.000000 seismometer-0.1.0/src/seismometer.egg-info/PKG-INFO
+-rw-r--r--   0 seismo    (1000) seismo    (1000)     2323 2024-05-21 18:34:27.000000 seismometer-0.1.0/src/seismometer.egg-info/SOURCES.txt
+-rw-r--r--   0 seismo    (1000) seismo    (1000)        1 2024-05-21 18:34:27.000000 seismometer-0.1.0/src/seismometer.egg-info/dependency_links.txt
+-rw-r--r--   0 seismo    (1000) seismo    (1000)       61 2024-05-21 18:34:27.000000 seismometer-0.1.0/src/seismometer.egg-info/entry_points.txt
+-rw-r--r--   0 seismo    (1000) seismo    (1000)      781 2024-05-21 18:34:27.000000 seismometer-0.1.0/src/seismometer.egg-info/requires.txt
+-rw-r--r--   0 seismo    (1000) seismo    (1000)       12 2024-05-21 18:34:27.000000 seismometer-0.1.0/src/seismometer.egg-info/top_level.txt
+-rw-r--r--   0 seismo    (1000) seismo    (1000)        1 2024-05-21 18:34:26.000000 seismometer-0.1.0/src/seismometer.egg-info/zip-safe
+drwxr-xr-x   0 seismo    (1000) seismo    (1000)        0 2024-05-21 18:34:29.397348 seismometer-0.1.0/tests/
+-rwxrwxrwx   0 seismo    (1000) seismo    (1000)     1561 2024-05-21 18:33:17.000000 seismometer-0.1.0/tests/test_startup.py
```

### Comparing `seismometer-0.0.1/LICENSE.txt` & `seismometer-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

