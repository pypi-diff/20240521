# Comparing `tmp/odhpy-0.2.0.tar.gz` & `tmp/odhpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odhpy-0.2.0.tar", last modified: Thu May  2 00:18:35 2024, max compression
+gzip compressed data, was "odhpy-0.2.1.tar", last modified: Tue May 21 02:07:59 2024, max compression
```

## Comparing `odhpy-0.2.0.tar` & `odhpy-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:35.004766 odhpy-0.2.0/
--rw-rw-rw-   0        0        0     2793 2024-05-02 00:18:35.002847 odhpy-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2024-04-03 03:37:24.000000 odhpy-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 00:18:35.004766 odhpy-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      960 2024-03-19 03:03:09.000000 odhpy-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.877772 odhpy-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.910731 odhpy-0.2.0/src/odhpy/
--rw-rw-rw-   0        0        0       76 2024-03-14 03:25:23.000000 odhpy-0.2.0/src/odhpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.931285 odhpy-0.2.0/src/odhpy/clim/
--rw-rw-rw-   0        0        0       21 2024-03-14 03:25:23.000000 odhpy-0.2.0/src/odhpy/clim/__init__.py
--rw-rw-rw-   0        0        0     6756 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/clim/clim.py
--rw-rw-rw-   0        0        0      128 2024-03-14 03:25:23.000000 odhpy-0.2.0/src/odhpy/demo.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.945030 odhpy-0.2.0/src/odhpy/io/
--rw-rw-rw-   0        0        0      128 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/io/__init__.py
--rw-rw-rw-   0        0        0     4256 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/csv_io.py
--rw-rw-rw-   0        0        0     2868 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/idx_io.py
--rw-rw-rw-   0        0        0     6065 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/iqqm_out_reader.py
--rw-rw-rw-   0        0        0     1705 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/lqn_io.py
--rw-rw-rw-   0        0        0     3059 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/res_csv_io.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.951034 odhpy-0.2.0/src/odhpy/maps/
--rw-rw-rw-   0        0        0       29 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/maps/__init__.py
--rw-rw-rw-   0        0        0     5090 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/maps/station_maps.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.963617 odhpy-0.2.0/src/odhpy/plots/
--rw-rw-rw-   0        0        0      121 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/plots/__init__.py
--rw-rw-rw-   0        0        0    31099 2024-05-02 00:09:23.000000 odhpy-0.2.0/src/odhpy/plots/altair_plots.py
--rw-rw-rw-   0        0        0      274 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/plots/node_diagrams.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/plots/plot_functions.py
--rw-rw-rw-   0        0        0        0 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/plots/plotly_helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.975605 odhpy-0.2.0/src/odhpy/stats/
--rw-rw-rw-   0        0        0      111 2024-03-18 23:58:54.000000 odhpy-0.2.0/src/odhpy/stats/__init__.py
--rw-rw-rw-   0        0        0     2498 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/stats/aggregate_stats.py
--rw-rw-rw-   0        0        0    12092 2024-04-03 03:37:24.000000 odhpy-0.2.0/src/odhpy/stats/reliability_stats_class.py
--rw-rw-rw-   0        0        0     9163 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/stats/storage_level_assessment.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.979770 odhpy-0.2.0/src/odhpy/stats/swflo2s/
--rw-rw-rw-   0        0        0       22 2024-04-03 03:37:24.000000 odhpy-0.2.0/src/odhpy/stats/swflo2s/__init__.py
--rw-rw-rw-   0        0        0     6755 2024-04-03 03:37:24.000000 odhpy-0.2.0/src/odhpy/stats/swflo2s/swflo2s.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.987831 odhpy-0.2.0/src/odhpy/stoch/
--rw-rw-rw-   0        0        0       23 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/stoch/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/stoch/analyse.py
--rw-rw-rw-   0        0        0     2867 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/stoch/generate.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.991895 odhpy-0.2.0/src/odhpy/trans/
--rw-rw-rw-   0        0        0       27 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/trans/__init__.py
--rw-rw-rw-   0        0        0     2953 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/trans/transformers.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.999782 odhpy-0.2.0/src/odhpy/utils/
--rw-rw-rw-   0        0        0       99 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/utils/__init__.py
--rw-rw-rw-   0        0        0    11382 2024-04-03 03:37:24.000000 odhpy-0.2.0/src/odhpy/utils/dataframe_functions.py
--rw-rw-rw-   0        0        0    10157 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/utils/datetime_functions.py
--rw-rw-rw-   0        0        0      753 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/utils/interpolation.py
--rw-rw-rw-   0        0        0      210 2024-05-02 00:10:39.000000 odhpy-0.2.0/src/odhpy/version.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.927333 odhpy-0.2.0/src/odhpy.egg-info/
--rw-rw-rw-   0        0        0     2793 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.062307 odhpy-0.2.1/
+-rw-rw-rw-   0        0        0     2793 2024-05-21 02:07:59.061307 odhpy-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2024-04-01 01:31:43.000000 odhpy-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 02:07:59.062307 odhpy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      960 2024-03-19 06:42:42.000000 odhpy-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.033502 odhpy-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.038145 odhpy-0.2.1/src/odhpy/
+-rw-rw-rw-   0        0        0       76 2023-07-21 10:09:08.000000 odhpy-0.2.1/src/odhpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.043119 odhpy-0.2.1/src/odhpy/clim/
+-rw-rw-rw-   0        0        0       21 2023-07-21 10:09:08.000000 odhpy-0.2.1/src/odhpy/clim/__init__.py
+-rw-rw-rw-   0        0        0     6756 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/clim/clim.py
+-rw-rw-rw-   0        0        0      128 2023-07-21 10:09:08.000000 odhpy-0.2.1/src/odhpy/demo.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.048047 odhpy-0.2.1/src/odhpy/io/
+-rw-rw-rw-   0        0        0      128 2023-08-02 02:21:05.000000 odhpy-0.2.1/src/odhpy/io/__init__.py
+-rw-rw-rw-   0        0        0     4256 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/io/csv_io.py
+-rw-rw-rw-   0        0        0      686 2024-05-21 00:57:43.000000 odhpy-0.2.1/src/odhpy/io/general_io.py
+-rw-rw-rw-   0        0        0     2868 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/io/idx_io.py
+-rw-rw-rw-   0        0        0     6065 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/io/iqqm_out_reader.py
+-rw-rw-rw-   0        0        0     1760 2024-04-09 00:20:46.000000 odhpy-0.2.1/src/odhpy/io/lqn_io.py
+-rw-rw-rw-   0        0        0     4553 2024-05-21 02:07:48.000000 odhpy-0.2.1/src/odhpy/io/res_csv_io.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.049441 odhpy-0.2.1/src/odhpy/maps/
+-rw-rw-rw-   0        0        0       29 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/maps/__init__.py
+-rw-rw-rw-   0        0        0     5090 2024-03-19 06:42:09.000000 odhpy-0.2.1/src/odhpy/maps/station_maps.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.052527 odhpy-0.2.1/src/odhpy/plots/
+-rw-rw-rw-   0        0        0      121 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/plots/__init__.py
+-rw-rw-rw-   0        0        0    31099 2024-05-15 00:49:57.000000 odhpy-0.2.1/src/odhpy/plots/altair_plots.py
+-rw-rw-rw-   0        0        0      274 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/plots/node_diagrams.py
+-rw-rw-rw-   0        0        0     1988 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/plots/plot_functions.py
+-rw-rw-rw-   0        0        0        0 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/plots/plotly_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.055301 odhpy-0.2.1/src/odhpy/stats/
+-rw-rw-rw-   0        0        0      111 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/stats/__init__.py
+-rw-rw-rw-   0        0        0     2498 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/stats/aggregate_stats.py
+-rw-rw-rw-   0        0        0    12092 2024-03-29 21:47:29.000000 odhpy-0.2.1/src/odhpy/stats/reliability_stats_class.py
+-rw-rw-rw-   0        0        0     9163 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/stats/storage_level_assessment.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.056305 odhpy-0.2.1/src/odhpy/stats/swflo2s/
+-rw-rw-rw-   0        0        0       22 2024-03-29 13:48:13.000000 odhpy-0.2.1/src/odhpy/stats/swflo2s/__init__.py
+-rw-rw-rw-   0        0        0     6755 2024-04-01 03:18:37.000000 odhpy-0.2.1/src/odhpy/stats/swflo2s/swflo2s.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.057304 odhpy-0.2.1/src/odhpy/stoch/
+-rw-rw-rw-   0        0        0       23 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/stoch/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/stoch/analyse.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/stoch/generate.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.058304 odhpy-0.2.1/src/odhpy/trans/
+-rw-rw-rw-   0        0        0       27 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/trans/__init__.py
+-rw-rw-rw-   0        0        0     2953 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/trans/transformers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.061307 odhpy-0.2.1/src/odhpy/utils/
+-rw-rw-rw-   0        0        0       99 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    11382 2024-04-01 01:06:05.000000 odhpy-0.2.1/src/odhpy/utils/dataframe_functions.py
+-rw-rw-rw-   0        0        0    10157 2024-03-19 06:42:42.000000 odhpy-0.2.1/src/odhpy/utils/datetime_functions.py
+-rw-rw-rw-   0        0        0      753 2023-07-21 10:09:09.000000 odhpy-0.2.1/src/odhpy/utils/interpolation.py
+-rw-rw-rw-   0        0        0      210 2024-05-21 01:45:21.000000 odhpy-0.2.1/src/odhpy/version.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:07:59.041781 odhpy-0.2.1/src/odhpy.egg-info/
+-rw-rw-rw-   0        0        0     2793 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 02:07:58.000000 odhpy-0.2.1/src/odhpy.egg-info/top_level.txt
```

### Comparing `odhpy-0.2.0/PKG-INFO` & `odhpy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odhpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of splashings to master that which has no form and count that which is uncountable.
 Home-page: https://bitbucket.org/odhydrology/odhpy.git
 Author: Chas Egan
 Author-email: chas@odhydrology.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `odhpy-0.2.0/README.md` & `odhpy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/setup.py` & `odhpy-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/clim/clim.py` & `odhpy-0.2.1/src/odhpy/clim/clim.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/io/csv_io.py` & `odhpy-0.2.1/src/odhpy/io/csv_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/io/idx_io.py` & `odhpy-0.2.1/src/odhpy/io/idx_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/io/iqqm_out_reader.py` & `odhpy-0.2.1/src/odhpy/io/iqqm_out_reader.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/io/lqn_io.py` & `odhpy-0.2.1/src/odhpy/io/lqn_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import pandas as pd
 from odhpy import utils
 na_values = ['', ' ', 'null', 'NULL', 'NAN', 'NaN', 'nan', 'NA', 'na', 'N/A' 'n/a', '#N/A', '#NA', '-NaN', '-nan']
 
 
 
 def read_iqqm_lqn_output(filename, col_name=None, df=None) -> pd.DataFrame:
-    """Reads the output of IQQM listquan. This is format is the same for flows and diversions.
+    """
+    Reads the output of IQQM listquan. This is a space-separated is format with two columns (date, value) and data 
+    starting on line 7.
 
     Args:
         filename (_type_): _description_
         df (_type_, optional): _description_. Defaults to None.
 
     Returns:
         pd.DataFrame: _description_
```

### Comparing `odhpy-0.2.0/src/odhpy/maps/station_maps.py` & `odhpy-0.2.1/src/odhpy/maps/station_maps.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/plots/altair_plots.py` & `odhpy-0.2.1/src/odhpy/plots/altair_plots.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/plots/plot_functions.py` & `odhpy-0.2.1/src/odhpy/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/stats/aggregate_stats.py` & `odhpy-0.2.1/src/odhpy/stats/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/stats/reliability_stats_class.py` & `odhpy-0.2.1/src/odhpy/stats/reliability_stats_class.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/stats/storage_level_assessment.py` & `odhpy-0.2.1/src/odhpy/stats/storage_level_assessment.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/stats/swflo2s/swflo2s.py` & `odhpy-0.2.1/src/odhpy/stats/swflo2s/swflo2s.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/stoch/generate.py` & `odhpy-0.2.1/src/odhpy/stoch/generate.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/trans/transformers.py` & `odhpy-0.2.1/src/odhpy/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/utils/dataframe_functions.py` & `odhpy-0.2.1/src/odhpy/utils/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/utils/datetime_functions.py` & `odhpy-0.2.1/src/odhpy/utils/datetime_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy/utils/interpolation.py` & `odhpy-0.2.1/src/odhpy/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.2.0/src/odhpy.egg-info/PKG-INFO` & `odhpy-0.2.1/src/odhpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odhpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of splashings to master that which has no form and count that which is uncountable.
 Home-page: https://bitbucket.org/odhydrology/odhpy.git
 Author: Chas Egan
 Author-email: chas@odhydrology.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `odhpy-0.2.0/src/odhpy.egg-info/SOURCES.txt` & `odhpy-0.2.1/src/odhpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/odhpy.egg-info/dependency_links.txt
 src/odhpy.egg-info/requires.txt
 src/odhpy.egg-info/top_level.txt
 src/odhpy/clim/__init__.py
 src/odhpy/clim/clim.py
 src/odhpy/io/__init__.py
 src/odhpy/io/csv_io.py
+src/odhpy/io/general_io.py
 src/odhpy/io/idx_io.py
 src/odhpy/io/iqqm_out_reader.py
 src/odhpy/io/lqn_io.py
 src/odhpy/io/res_csv_io.py
 src/odhpy/maps/__init__.py
 src/odhpy/maps/station_maps.py
 src/odhpy/plots/__init__.py
```

