# Comparing `tmp/dream-tools-2.1.9.tar.gz` & `tmp/dream-tools-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dream-tools-2.1.9.tar", last modified: Fri Apr  5 09:41:23 2024, max compression
+gzip compressed data, was "dream-tools-2.2.0.tar", last modified: Tue May 21 11:40:26 2024, max compression
```

## Comparing `dream-tools-2.1.9.tar` & `dream-tools-2.2.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.823083 dream-tools-2.1.9/
--rw-rw-rw-   0        0        0     1093 2020-08-12 11:00:01.000000 dream-tools-2.1.9/LICENSE
--rw-rw-rw-   0        0        0     1438 2024-04-05 09:41:23.819110 dream-tools-2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      877 2023-02-28 12:24:28.000000 dream-tools-2.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.816130 dream-tools-2.1.9/dream_tools.egg-info/
--rw-rw-rw-   0        0        0     1438 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1337 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.718737 dream-tools-2.1.9/dreamtools/
--rw-rw-rw-   0        0        0      681 2024-04-05 09:33:37.000000 dream-tools-2.1.9/dreamtools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.748118 dream-tools-2.1.9/dreamtools/gamY/
--rw-rw-rw-   0        0        0       29 2020-01-24 14:37:03.000000 dream-tools-2.1.9/dreamtools/gamY/__init__.py
--rw-rw-rw-   0        0        0     3814 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/classes.py
--rw-rw-rw-   0        0        0     4423 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/excel_endo_exo.py
--rw-rw-rw-   0        0        0     2488 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/extract_equations.py
--rw-rw-rw-   0        0        0     1062 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/extract_variables.py
--rw-rw-rw-   0        0        0    55936 2022-12-13 10:01:56.000000 dream-tools-2.1.9/dreamtools/gamY/gamY.py
--rw-rw-rw-   0        0        0     1541 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/gekko_endo_exo.py
--rw-rw-rw-   0        0        0     4532 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/patterns.py
--rw-rw-rw-   0        0        0     1135 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/rename_set.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.761235 dream-tools-2.1.9/dreamtools/gams_excel/
--rw-rw-rw-   0        0        0       25 2020-01-31 12:41:21.000000 dream-tools-2.1.9/dreamtools/gams_excel/__init__.py
--rw-rw-rw-   0        0        0     3138 2024-04-05 09:32:29.000000 dream-tools-2.1.9/dreamtools/gams_excel/excel_endo_exo.py
--rw-rw-rw-   0        0        0     2666 2020-10-09 09:58:26.000000 dream-tools-2.1.9/dreamtools/gams_excel/gams_excel.py
--rw-rw-rw-   0        0        0     4045 2023-10-22 19:05:11.000000 dream-tools-2.1.9/dreamtools/gams_excel/gdx_to_excel.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.777317 dream-tools-2.1.9/dreamtools/gams_pandas/
--rw-rw-rw-   0        0        0       89 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/gams_pandas/__init__.py
--rw-rw-rw-   0        0        0    17187 2024-04-05 09:32:21.000000 dream-tools-2.1.9/dreamtools/gams_pandas/gams_pandas.py
--rw-rw-rw-   0        0        0     1481 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/gams_pandas/gdx.py
--rw-rw-rw-   0        0        0    11969 2023-10-26 19:08:17.000000 dream-tools-2.1.9/dreamtools/gams_pandas/test_gams_pandas.py
--rw-rw-rw-   0        0        0     3321 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/gams_pandas/utility.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.811984 dream-tools-2.1.9/dreamtools/multiindex_plotly/
--rw-rw-rw-   0        0        0      385 2023-03-01 08:59:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/__init__.py
--rw-rw-rw-   0        0        0     2854 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/age_plot.py
--rw-rw-rw-   0        0        0     2084 2023-02-24 13:26:37.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/dream_plotly_template.py
--rw-rw-rw-   0        0        0    22704 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/dream_settings.py
--rw-rw-rw-   0        0        0      891 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/makro_settings.py
--rw-rw-rw-   0        0        0        3 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/plotly_util.py
--rw-rw-rw-   0        0        0     4445 2023-09-14 08:18:26.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/reporting.py
--rw-rw-rw-   0        0        0     7201 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/scratch.py
--rw-rw-rw-   0        0        0     1897 2023-03-01 10:04:19.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/test_plot.py
--rw-rw-rw-   0        0        0     2330 2023-01-25 09:50:54.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/test_timeseries_analysis.py
--rw-rw-rw-   0        0        0    10640 2023-03-01 10:03:09.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/timeseries_analysis.py
--rw-rw-rw-   0        0        0       42 2024-04-05 09:41:23.823580 dream-tools-2.1.9/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-03-01 09:02:40.000000 dream-tools-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:40:26.280597 dream-tools-2.2.0/
+-rw-rw-rw-   0        0        0     1093 2020-08-12 11:00:01.000000 dream-tools-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1454 2024-05-21 11:40:26.278597 dream-tools-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2024-05-21 11:37:08.000000 dream-tools-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 11:40:26.277597 dream-tools-2.2.0/dream_tools.egg-info/
+-rw-rw-rw-   0        0        0     1454 2024-05-21 11:40:26.000000 dream-tools-2.2.0/dream_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1389 2024-05-21 11:40:26.000000 dream-tools-2.2.0/dream_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 11:40:26.000000 dream-tools-2.2.0/dream_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-21 11:40:26.000000 dream-tools-2.2.0/dream_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-21 11:40:26.000000 dream-tools-2.2.0/dream_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 11:40:26.227251 dream-tools-2.2.0/dreamtools/
+-rw-rw-rw-   0        0        0      729 2024-05-21 09:09:27.000000 dream-tools-2.2.0/dreamtools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:40:26.244234 dream-tools-2.2.0/dreamtools/gamY/
+-rw-rw-rw-   0        0        0       19 2024-05-21 09:13:24.000000 dream-tools-2.2.0/dreamtools/gamY/__init__.py
+-rw-rw-rw-   0        0        0     3825 2024-05-17 10:42:49.000000 dream-tools-2.2.0/dreamtools/gamY/classes.py
+-rw-rw-rw-   0        0        0     4423 2022-12-13 11:41:07.000000 dream-tools-2.2.0/dreamtools/gamY/excel_endo_exo.py
+-rw-rw-rw-   0        0        0     2488 2024-05-17 10:42:49.000000 dream-tools-2.2.0/dreamtools/gamY/extract_equations.py
+-rw-rw-rw-   0        0        0     1060 2024-05-17 10:42:49.000000 dream-tools-2.2.0/dreamtools/gamY/extract_variables.py
+-rw-rw-rw-   0        0        0    53186 2024-05-21 10:49:46.000000 dream-tools-2.2.0/dreamtools/gamY/gamY.py
+-rw-rw-rw-   0        0        0     4288 2024-05-17 10:42:49.000000 dream-tools-2.2.0/dreamtools/gamY/gdx_to_excel.py
+-rw-rw-rw-   0        0        0     1541 2024-05-17 10:42:49.000000 dream-tools-2.2.0/dreamtools/gamY/gekko_endo_exo.py
+-rw-rw-rw-   0        0        0     4532 2024-05-17 10:42:49.000000 dream-tools-2.2.0/dreamtools/gamY/patterns.py
+-rw-rw-rw-   0        0        0     1135 2024-05-17 10:42:49.000000 dream-tools-2.2.0/dreamtools/gamY/rename_set.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:40:26.250235 dream-tools-2.2.0/dreamtools/gams_excel/
+-rw-rw-rw-   0        0        0       25 2020-01-31 12:41:21.000000 dream-tools-2.2.0/dreamtools/gams_excel/__init__.py
+-rw-rw-rw-   0        0        0     3138 2024-04-05 09:32:29.000000 dream-tools-2.2.0/dreamtools/gams_excel/excel_endo_exo.py
+-rw-rw-rw-   0        0        0     2666 2020-10-09 09:58:26.000000 dream-tools-2.2.0/dreamtools/gams_excel/gams_excel.py
+-rw-rw-rw-   0        0        0     4288 2024-05-17 10:42:49.000000 dream-tools-2.2.0/dreamtools/gams_excel/gdx_to_excel.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:40:26.260002 dream-tools-2.2.0/dreamtools/gams_pandas/
+-rw-rw-rw-   0        0        0       89 2023-01-13 09:23:38.000000 dream-tools-2.2.0/dreamtools/gams_pandas/__init__.py
+-rw-rw-rw-   0        0        0    17187 2024-04-05 09:32:21.000000 dream-tools-2.2.0/dreamtools/gams_pandas/gams_pandas.py
+-rw-rw-rw-   0        0        0     1481 2023-01-13 09:23:38.000000 dream-tools-2.2.0/dreamtools/gams_pandas/gdx.py
+-rw-rw-rw-   0        0        0    11969 2023-10-26 19:08:17.000000 dream-tools-2.2.0/dreamtools/gams_pandas/test_gams_pandas.py
+-rw-rw-rw-   0        0        0     3321 2023-01-13 09:23:38.000000 dream-tools-2.2.0/dreamtools/gams_pandas/utility.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:40:26.276596 dream-tools-2.2.0/dreamtools/multiindex_plotly/
+-rw-rw-rw-   0        0        0      385 2023-03-01 08:59:38.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/__init__.py
+-rw-rw-rw-   0        0        0     2854 2023-01-13 09:23:38.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/age_plot.py
+-rw-rw-rw-   0        0        0     2084 2023-02-24 13:26:37.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/dream_plotly_template.py
+-rw-rw-rw-   0        0        0    22704 2023-01-13 09:23:38.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/dream_settings.py
+-rw-rw-rw-   0        0        0      891 2023-01-13 09:23:38.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/makro_settings.py
+-rw-rw-rw-   0        0        0        3 2023-01-13 09:23:38.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/plotly_util.py
+-rw-rw-rw-   0        0        0     4445 2023-09-14 08:18:26.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/reporting.py
+-rw-rw-rw-   0        0        0     7201 2023-01-13 09:23:38.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/scratch.py
+-rw-rw-rw-   0        0        0     1897 2023-03-01 10:04:19.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/test_plot.py
+-rw-rw-rw-   0        0        0     2330 2023-01-25 09:50:54.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/test_timeseries_analysis.py
+-rw-rw-rw-   0        0        0    10640 2023-03-01 10:03:09.000000 dream-tools-2.2.0/dreamtools/multiindex_plotly/timeseries_analysis.py
+-rw-rw-rw-   0        0        0      841 2024-05-21 10:52:06.000000 dream-tools-2.2.0/dreamtools/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 11:40:26.280597 dream-tools-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      843 2024-05-21 11:34:28.000000 dream-tools-2.2.0/setup.py
```

### Comparing `dream-tools-2.1.9/LICENSE` & `dream-tools-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/PKG-INFO` & `dream-tools-2.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dream-tools
-Version: 2.1.9
-Summary: A collection of tools used by the Danish institute for economic modelling and forecasting, DREAM (http://dreammodel.dk).
+Version: 2.2.0
+Summary: A collection of tools used by the Danish Research Institute for Economic Analysis and Modelling, DREAM (https://dreamgruppen.dk/).
 Home-page: https://github.com/MartinBonde/dream-tools
 Author: Martin Kirk Bonde
 Author-email: martin@bonde.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: plotly
 
 # DREAM-tools
-A collection of tools used by [the Danish institute for economic modelling and forecasting, DREAM](http://dreammodel.dk).
+A collection of tools used by [DREAM, Danish Research Institute for Economic Analysis and Modelling](https://dreamgruppen.dk/).
 
 ## Gams-Pandas
 A wrapper around the [GAMS Python api](https://www.gams.com/latest/docs/API_PY_OVERVIEW.html) to move smoothly between GAMS and [Pandas](https://pandas.pydata.org/).
 GAMS parameters are represented as Pandas Series, using a MultiIndex in cases of multiple sets.
 The level value of variables are represented in the same way. GAMS sets are represented as Pandas Index to facilitate easy use of label based indexing.
 
 ## Excel-gdx
```

### Comparing `dream-tools-2.1.9/README.md` & `dream-tools-2.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DREAM-tools
-A collection of tools used by [the Danish institute for economic modelling and forecasting, DREAM](http://dreammodel.dk).
+A collection of tools used by [DREAM, Danish Research Institute for Economic Analysis and Modelling](https://dreamgruppen.dk/).
 
 ## Gams-Pandas
 A wrapper around the [GAMS Python api](https://www.gams.com/latest/docs/API_PY_OVERVIEW.html) to move smoothly between GAMS and [Pandas](https://pandas.pydata.org/).
 GAMS parameters are represented as Pandas Series, using a MultiIndex in cases of multiple sets.
 The level value of variables are represented in the same way. GAMS sets are represented as Pandas Index to facilitate easy use of label based indexing.
 
 ## Excel-gdx
```

### Comparing `dream-tools-2.1.9/dream_tools.egg-info/PKG-INFO` & `dream-tools-2.2.0/dream_tools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dream-tools
-Version: 2.1.9
-Summary: A collection of tools used by the Danish institute for economic modelling and forecasting, DREAM (http://dreammodel.dk).
+Version: 2.2.0
+Summary: A collection of tools used by the Danish Research Institute for Economic Analysis and Modelling, DREAM (https://dreamgruppen.dk/).
 Home-page: https://github.com/MartinBonde/dream-tools
 Author: Martin Kirk Bonde
 Author-email: martin@bonde.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: plotly
 
 # DREAM-tools
-A collection of tools used by [the Danish institute for economic modelling and forecasting, DREAM](http://dreammodel.dk).
+A collection of tools used by [DREAM, Danish Research Institute for Economic Analysis and Modelling](https://dreamgruppen.dk/).
 
 ## Gams-Pandas
 A wrapper around the [GAMS Python api](https://www.gams.com/latest/docs/API_PY_OVERVIEW.html) to move smoothly between GAMS and [Pandas](https://pandas.pydata.org/).
 GAMS parameters are represented as Pandas Series, using a MultiIndex in cases of multiple sets.
 The level value of variables are represented in the same way. GAMS sets are represented as Pandas Index to facilitate easy use of label based indexing.
 
 ## Excel-gdx
```

### Comparing `dream-tools-2.1.9/dream_tools.egg-info/SOURCES.txt` & `dream-tools-2.2.0/dream_tools.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 setup.py
 dream_tools.egg-info/PKG-INFO
 dream_tools.egg-info/SOURCES.txt
 dream_tools.egg-info/dependency_links.txt
 dream_tools.egg-info/requires.txt
 dream_tools.egg-info/top_level.txt
 dreamtools/__init__.py
+dreamtools/utils.py
 dreamtools/gamY/__init__.py
 dreamtools/gamY/classes.py
 dreamtools/gamY/excel_endo_exo.py
 dreamtools/gamY/extract_equations.py
 dreamtools/gamY/extract_variables.py
 dreamtools/gamY/gamY.py
+dreamtools/gamY/gdx_to_excel.py
 dreamtools/gamY/gekko_endo_exo.py
 dreamtools/gamY/patterns.py
 dreamtools/gamY/rename_set.py
 dreamtools/gams_excel/__init__.py
 dreamtools/gams_excel/excel_endo_exo.py
 dreamtools/gams_excel/gams_excel.py
 dreamtools/gams_excel/gdx_to_excel.py
```

### Comparing `dream-tools-2.1.9/dreamtools/__init__.py` & `dream-tools-2.2.0/dreamtools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .gams_pandas import *
 
-__version__ = "2.1.9"
+__version__ = "2.2.0"
 
 # Global setting controlling the default name of the time index
 X_AXIS_NAME = "t"
 # Default axis position if no level named dt.X_AXIS_NAME is found
 X_AXIS_INDEX = -1 #  (-1 = last index is time)
 
 # Time settings, used for plot and prt functions
@@ -19,7 +19,11 @@
 REFERENCE_DATABASE = None
 
 # Ploting
 from .multiindex_plotly import *
 
 # Model specific settings
 from .multiindex_plotly.makro_settings import DEFAULT_SET_AGGREGATIONS, AGE_AXIS_TITLE, TIME_AXIS_TITLE, YAXIS_TITLE_FROM_OPERATOR
+
+from .utils import *
+
+from .gamY import gamY
```

### Comparing `dream-tools-2.1.9/dreamtools/gamY/classes.py` & `dream-tools-2.2.0/dreamtools/gamY/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import collections
+from collections.abc import MutableMapping, Mapping
 
+class CaseInsensitiveDict(MutableMapping):
 
-class CaseInsensitiveDict(collections.MutableMapping):
     """A case-insensitive ``dict``-like object.
     Implements all methods and operations of
     ``collections.MutableMapping`` as well as dict's ``copy``. Also
     provides ``lower_items``.
     All keys are expected to be strings. The structure remembers the
     case of the last key to be set, and ``iter(instance)``,
     ``keys()``, ``items()``, ``iterkeys()``, and ``iteritems()``
@@ -51,15 +51,15 @@
         return (
             (lowerkey, keyval[1])
             for (lowerkey, keyval)
             in self._store.items()
         )
 
     def __eq__(self, other):
-        if isinstance(other, collections.Mapping):
+        if isinstance(other, Mapping):
             other = CaseInsensitiveDict(other)
         else:
             return NotImplemented
         # Compare insensitively
         return dict(self.lower_items()) == dict(other.lower_items())
 
     # Copy is required
@@ -120,7 +120,8 @@
         self.groups = ["".join(self.groups)] + self.groups
 
     def group(self, i):
         return self.groups[i]
 
     def groups(self, i):
         return self.groups
+
```

### Comparing `dream-tools-2.1.9/dreamtools/gamY/excel_endo_exo.py` & `dream-tools-2.2.0/dreamtools/gamY/excel_endo_exo.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gamY/extract_equations.py` & `dream-tools-2.2.0/dreamtools/gamY/extract_equations.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gamY/extract_variables.py` & `dream-tools-2.2.0/dreamtools/gamY/extract_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # assert len(args) > 2, "GAMS path and input path must be specified"
 # ws = GamsWorkspace(system_directory=sys.argv[1])
 # input_path = os.path.abspath(args[2])
 # assert input_path[-4:] == ".gdx", "%s is not a .gdx file" % input_path
 
 ws = GamsWorkspace()
-input_path = os.path.abspath("..\\Model\\Gdx\\previous_smooth_calibration.gdx")
+input_path = os.path.abspath("..\\Model\\Gdx\\previous_deep_calibration.gdx")
 
 db = ws.add_database_from_gdx(input_path)
 
 # fp = os.path.join(file_dir, file_name+'_variables.xlsx')
 # fp = "../Analysis/Templates/skabelon.xlsx"
 fp = "../Konjunktur/konjunktur_ny.xlsx"
```

### Comparing `dream-tools-2.1.9/dreamtools/gamY/gamY.py` & `dream-tools-2.2.0/dreamtools/gamY/gamY.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,18 +109,28 @@
 from math import ceil, floor
 from heapq import heappush
 from timeit import default_timer as timer
 
 import itertools # Useful in FOR loops in MAKRO
 
 # gamY data objects
-from classes import Variable, Equation, Function, MockMatch, Group, Block, CaseInsensitiveDict
+from .classes import Variable, Equation, Function, MockMatch, Group, Block, CaseInsensitiveDict
 
 #  The regex patterns used to match commands
-from patterns import PATTERNS
+from .patterns import PATTERNS
+
+
+def get_lst_path(file_path):
+  """Return the path to the LST file corresponding to the GAMS file"""
+  file_dir, file_name = os.path.split(file_path)
+  list_file_dir = os.path.join(file_dir, "LST")
+  if not os.path.exists(list_file_dir):
+    os.makedirs(list_file_dir)
+  list_file_name = file_name.replace(".gms", ".lst")
+  return os.path.join(list_file_dir, list_file_name)
 
 
 class Precompiler:
   """Object with methods to parse each gamY command"""
 
   def __init__(self, file_path, patterns=PATTERNS, add_adjust=None, mult_adjust=None):
     self.groups = CaseInsensitiveDict({"all": {}})
@@ -147,20 +157,15 @@
 
     self.model_counter = 0  # As models cannot be redefined, we increment the names of temporary models defined
 
     self.patterns = patterns
     self.file_path = os.path.abspath(file_path)
     self.file_dir, self.file_name = os.path.split(self.file_path)
 
-    # Check that LST folder exists
-    list_file_dir = os.path.join(self.file_dir, "LST")
-    if not os.path.exists(list_file_dir):
-      os.makedirs(list_file_dir)
-    list_file_name = self.file_name.replace(".gms", ".lst")
-    self.list_file_path = os.path.join(list_file_dir, list_file_name)
+    self.list_file_path = get_lst_path(self.file_path)
 
     #  In cases where a command should be parsed by gamY, but also left for GAMS to parse, we replace special characters temporarily
     self.DOLLAR_SUB = "¤dollar¤"
     self.SEMICOLON_SUB = "¤semicolon¤"
     self.PERCENT_SUB = "¤percent¤"
     self.AT_SUB = "¤at¤"
     self.star_comment_pattern = re.compile(r"^\*.*", re.MULTILINE)
@@ -209,24 +214,25 @@
   def error(self, msg):
     error_text = "ERROR!\ngamY could not process the file due to the following error:\n" + msg
     with open(self.list_file_path, 'w+') as file:
       file.write(error_text)
     sys.exit(error_text)
 
   def __call__(self):
-    #  Read GAMS file
+    """Read GAMS file"""
     with open(self.file_path, 'r') as f:
       text = "\n" + f.read()
     if not self.has_read_file:
       text = "$ONEOLCOM\n$EOLCOM #\n\n" + text  # Add option for # comments if this is the first file being run
     self.processed_text = ""
     text = self.parse(text, top_level=True)
     text = self.processed_text + text
     text = self.dedent_dollar(text)
-    return self.restore_temporary_substitutions(text)
+    text = self.restore_temporary_substitutions(text)
+    return text
 
   def parse(self, text, top_level=False):
     while True:
       text = self.clean_comments(text)
       match = self.patterns["Any"].search(text)
       if match and (repr(match) == repr(self.prev_match) and text == self.prev_text):
         match = self.patterns["Any"].search(text, match.start() + 1)  # Check one character in, so that we don't match the same pattern forever
@@ -325,15 +331,15 @@
     """
     key = match.group(1)
 
     in_scope = self.in_scope()
     if key in in_scope:
       return in_scope[key]
     else:
-      self.warning(f"\%{key}\% is not defined and was not replaced")
+      self.warning(f"\\%{key}\\% is not defined and was not replaced")
       return self.PERCENT_SUB + key + self.PERCENT_SUB
 
   def user_function(self, match, text):
     """
     Insert user defined function call, e.g. @my_funct(), defined using $FUNCTION
     """
     func_name, args = match.group(1), match.group(2)
@@ -645,14 +651,33 @@
         self.groups_conditions[j_group_name] = {}
         for eq in new_model.values():
           j_name = j+eq._name
           self.groups[j_group_name][j_name] = self.groups[j][j_name]
 
     return replacement_text
 
+  def sets_to_conditions(self, set, var, item_conditions):
+    """
+    Used in Group defition to turn sub-sets into dollar-conditons
+    x[a,b]
+    x[a1,'b']$(a2[a1]) -> x[a,b]$(a1[a] and sameas['b',b] and a2[a])
+    """
+    condition_sets = set[1:-1].split(",")
+    definition_sets = var.sets[1:-1].split(",")
+    for con_set, def_set in zip(condition_sets, definition_sets):
+      if con_set == def_set:
+        continue
+      if item_conditions:
+        item_conditions = re.sub(fr"\b{con_set}\b", def_set, item_conditions, flags=re.IGNORECASE)
+      if "'" in con_set or '"' in con_set:
+        item_conditions = self.combine_conditions(item_conditions, f"sameas({con_set},{def_set})")
+      else:
+        item_conditions = self.combine_conditions(item_conditions, f"{con_set}[{def_set}]")
+    return item_conditions
+
   def group_define(self, match, text, init_val="0", parameter_group=False):
     """
     Parse $GROUP command
     Syntax example:
     $GROUP G_newGroup
       var1[a,t] "label for variable 1"
       var2[t]   "label for variable 2"
@@ -718,14 +743,17 @@
 
       for var in variables:
         if sets and "$" in sets:
           self.error(
             f"""Conditionals in the GROUP statement must be surrounded by parentheses, e.g. $(d1[d]).
 Error in {group_name}: {name}{sets}{item_conditions}""")
 
+        if sets and (sets != var.sets):
+          item_conditions = self.sets_to_conditions(sets, var, item_conditions)
+
         if remove:
           if var.name not in new_group:
             replacement_text += f"# {var.name} is not in group and could therefor not be removed""\n"
           else:
             remove_conditions = self.combine_conditions(item_conditions, old_group_conditions.get(var.name, None))
             if remove_conditions:
               new_group_conditions[var.name] = self.combine_conditions(new_group_conditions[var.name], "not " + remove_conditions)
@@ -1216,253 +1244,163 @@
       if char == br[1]:
         open_count -= 1
       if open_count < 0:
         return False
   return True
 
 
-def cmd_call():
-  start_time = timer()
-
-  # Read any execution paremeters
-  args = sys.argv
-  if len(args) < 2 or args[1][-4:] != ".gms":
-    raise ValueError("No .gms file specified")
-  else:
-    file_path = args[1]
-
-  precompiler = Precompiler(file_path, add_adjust=None, mult_adjust=None)
-
-  # Read optional command line arguments
-  save_file, gams_path = None, None
-  for arg in args:
-    #  Read blocks, groups, and variables from saved file if the r=<file_path> option is used.
-    if arg[:2] == "r=":
-      precompiler.read(arg[2:])
-
-    #  Save definitions if s=<file_path> is used
-    elif arg[:2] == "s=":
-      save_file = arg[2:]
-
-    #  Transfer command line parameters to data structure
-    elif arg[:2] == "--":
-      assert "=" in arg[2:], f"'{arg}' command line parameter starts with '--' but does not contain a '=' symbol."
-      k, v = arg[2:].split(sep="=")
-      precompiler.locals[k] = v
-
-    #  Get gams from command line arguments
-    elif arg[:5].lower() == "gams=":
-      gams_path = arg[5:]
-
-  #  Find GAMS program if it was not set as command line argument
-  if not gams_path:
-    if "GAMS" in os.environ:
-      gams_path = os.environ["GAMS"]
-    else:
-      gams_path = shutil.which("GAMS")
+def find_gams():
+    """
+    Find GAMS executable
+    """
+    gams_path = os.environ.get("GAMS") or os.environ.get("gams") or shutil.which("GAMS") or shutil.which("gams")
+    
     if not gams_path:
-      sys.exit("ERROR: gamY could not not find GAMS. Set GAMS path as environmental variable with variable name GAMS")
-  else:
-    #  Clean path for common errors
-    while gams_path[0] in ["'",'"'," "]:
-      gams_path = gams_path[1:]
-    while gams_path[-1] in ["'",'"'," "]:
-      gams_path = gams_path[:-1]
-    if gams_path[-4:] != ".exe":
-      sys.exit("ERROR: " + gams_path + " is not an executable file. Make sure GAMS path is correctly set.")
-
-  #  Parse file using recursive descent
-  text = precompiler()
-
-  if save_file: # Save gamY data structure if gamY is called with s= argument
-    precompiler.save(save_file)
-
-  #  Save pre-compiled GAMS file in 'Expanded' folder
-  expanded_dir = os.path.join(precompiler.file_dir, "Expanded")
-  if not os.path.exists(expanded_dir):
-    os.makedirs(expanded_dir)
-  new_file = os.path.join(expanded_dir, precompiler.file_name.replace(".gms", ".gmy"))
-  with open(new_file, 'w') as f:
-    f.write(text)
-
-  compilation_time = timer() - start_time
+      sys.exit("ERROR: gamY could not find GAMS. Set GAMS path as environmental variable with variable name GAMS")
+    
+    return gams_path
 
-  #  Run file using GAMS (path needs to be set for system or user)
-  prev_line = ""
-  call_parameters = [
-    "LO=3",
-    "Workdir=" + precompiler.file_dir,
-    "CurDir=" + precompiler.file_dir,
-    "ErrMsg=1",
-    "O=" + precompiler.list_file_path,
-    "pageSize=0",
-    "pageWidth=9999",
-  ]
-  call_parameters += [arg for arg in args[2:] if (arg[:5] != "gams=")]
-  process = subprocess.Popen(
-    [gams_path, new_file, *call_parameters],
-    stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-    universal_newlines=True, shell=True
-  )
 
-  while process.poll() is None:
-    for line in iter(process.stdout.readline, ""):
-      if not (line[:3] == "---" and prev_line[:10] == line[:10]):  # For almost identical lines, only print the last one
-        sys.stdout.write(prev_line)
-        sys.stdout.flush()
-      prev_line = line
-  sys.stdout.write(prev_line)
-  sys.stdout.flush()
+def run(file_path, r=None, s=None, shell=False, **kwargs):
+  """
+  Run a GAMS file after precompiling it with optional adjustments.
 
-#  Print errors and messages from listing file (lines starting with ****)
-  error_pattern = re.compile(r"^(\*{4}.+)", re.MULTILINE)
-  model_pattern = re.compile(r"(?<=Model Statistics    SOLVE |Model Analysis      SOLVE )\S+", re.MULTILINE)
-  with open(precompiler.list_file_path, 'r') as f:
-    for line in f:
-      if error_pattern.match(line):
-        print(error_pattern.match(line).group(0))
-      elif model_pattern.search(line):
-        print("")
-        print(model_pattern.search(line).group(0))
+  Parameters:
+  - file_path (str): Path to the GAMS file to be precompiled and executed.
+  - r (str, optional): Optional argument to read the gamY data structure.
+  - s (str, optional): Optional argument to save the gamY data structure.
+  - shell (bool, optional): If True, the command will be executed through the shell.
+  - **kwargs: Additional keyword arguments to be passed to the GAMS executable.
+
+  Raises:
+  - AssertionError: If the GAMS executable is not found or if the provided path is not an executable.
+  - Exception: If there is an error in GAMS execution.
+  """
 
-  execution_time = timer() - start_time - compilation_time
-  print("Precompiler time: %.2f seconds" % compilation_time)
-  print("Execution time: %.2f seconds" % execution_time)
-  print("Total run time: %.2f seconds" % (execution_time + compilation_time))
-  #  print("Return code: %i" % process.returncode)
+  start_time = timer()
 
-  sys.exit(process.returncode)
+  precompiler = Precompiler(file_path, add_adjust=None, mult_adjust=None)
 
-def py_call(args):
-  start_time = timer()
+  expanded_dir = os.path.join(precompiler.file_dir, "Expanded")
+  parsed_file_path = os.path.join(expanded_dir, precompiler.file_name.replace(".gms", ".gmy"))
 
-  # Read any execution paremeters
-  if len(args) < 2 or args[1][-4:] != ".gms":
-    raise ValueError("No .gms file specified")
-  else:
-    file_path = args[1]
+  call_parameters = [find_gams(), parsed_file_path]
 
-  precompiler = Precompiler(file_path, add_adjust=None, mult_adjust=None)
+  if r is not None: # Read gamY data structure if gamY is called with r= argument and pass r= argument to GAMS
+    precompiler.read(r)
+    call_parameters.append(f"r={r}")
 
-  # Read optional command line arguments
-  save_file, gams_path = None, None
-  for arg in args:
-    #  Read blocks, groups, and variables from saved file if the r=<file_path> option is used.
-    if arg[:2] == "r=":
-      precompiler.read(arg[2:])
-
-    #  Save definitions if s=<file_path> is used
-    elif arg[:2] == "s=":
-      save_file = arg[2:]
-
-    #  Transfer command line parameters to data structure
-    elif arg[:2] == "--":
-      assert "=" in arg[2:], f"'{arg}' command line parameter starts with '--' but does not contain a '=' symbol."
-      k, v = arg[2:].split(sep="=")
-      precompiler.locals[k] = v
-
-    #  Get gams from command line arguments
-    elif arg[:5].lower() == "gams=":
-      gams_path = arg[5:]
-
-  #  Find GAMS program if it was not set as command line argument
-  if not gams_path:
-    if "GAMS" in os.environ:
-      gams_path = os.environ["GAMS"]
-    else:
-      gams_path = shutil.which("GAMS")
-    if not gams_path:
-      sys.exit("ERROR: gamY could not not find GAMS. Set GAMS path as environmental variable with variable name GAMS")
-  else:
-    #  Clean path for common errors
-    while gams_path[0] in ["'",'"'," "]:
-      gams_path = gams_path[1:]
-    while gams_path[-1] in ["'",'"'," "]:
-      gams_path = gams_path[:-1]
-    if gams_path[-4:] != ".exe":
-      sys.exit("ERROR: " + gams_path + " is not an executable file. Make sure GAMS path is correctly set.")
+  for k, v in kwargs.items():
+    precompiler.locals[k] = v
+    call_parameters.append(f"--{k}={v}")
 
   #  Parse file using recursive descent
   text = precompiler()
 
-  if save_file: # Save gamY data structure if gamY is called with s= argument
-    precompiler.save(save_file)
+  if s is not None: # Save gamY data structure if gamY is called with s= argument and pass s= argument to GAMS
+    precompiler.save(s)
+    call_parameters.append(f"s={s}")
 
   #  Save pre-compiled GAMS file in 'Expanded' folder
-  expanded_dir = os.path.join(precompiler.file_dir, "Expanded")
-  if not os.path.exists(expanded_dir):
-    os.makedirs(expanded_dir)
-  new_file = os.path.join(expanded_dir, precompiler.file_name.replace(".gms", ".gmy"))
-  with open(new_file, 'w') as f:
+  os.makedirs(expanded_dir, exist_ok=True)
+  with open(parsed_file_path, 'w') as f:
     f.write(text)
 
   compilation_time = timer() - start_time
 
   #  Run file using GAMS (path needs to be set for system or user)
   prev_line = ""
-  call_parameters = [
+  call_parameters += [
     "LO=3",
-    "Workdir=" + precompiler.file_dir,
-    "CurDir=" + precompiler.file_dir,
+    f"Workdir={precompiler.file_dir}",
+    f"CurDir={precompiler.file_dir}",
     "ErrMsg=1",
-    "O=" + precompiler.list_file_path,
+    f"O={precompiler.list_file_path}",
     "pageSize=0",
     "pageWidth=9999",
   ]
-  call_parameters += [arg for arg in args[2:] if (arg[:5] != "gams=")]
   process = subprocess.Popen(
-    [gams_path, new_file, *call_parameters],
+    call_parameters,
     stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-    universal_newlines=True, shell=False
+    universal_newlines=True, shell=shell
   )
 
   while process.poll() is None:
     for line in iter(process.stdout.readline, ""):
       if not (line[:3] == "---" and prev_line[:10] == line[:10]):  # For almost identical lines, only print the last one
         sys.stdout.write(prev_line)
         sys.stdout.flush()
       prev_line = line
   sys.stdout.write(prev_line)
   sys.stdout.flush()
 
-#  Print errors and messages from listing file (lines starting with ****)
-  error_pattern = re.compile(r"^(\*{4}.+)", re.MULTILINE)
-  model_pattern = re.compile(r"(?<=Model Statistics    SOLVE |Model Analysis      SOLVE )\S+", re.MULTILINE)
-  with open(precompiler.list_file_path, 'r') as f:
-    for line in f:
-      if error_pattern.match(line):
-        print(error_pattern.match(line).group(0))
-      elif model_pattern.search(line):
-        print("")
-        print(model_pattern.search(line).group(0))
+  print(get_status_from_lst(precompiler.list_file_path))
 
   execution_time = timer() - start_time - compilation_time
-  print("Precompiler time: %.2f seconds" % compilation_time)
-  print("Execution time: %.2f seconds" % execution_time)
-  print("Total run time: %.2f seconds" % (execution_time + compilation_time))
-  #  print("Return code: %i" % process.returncode)
+  print(f"Precompiler time: {compilation_time:.2f} seconds")
+  print(f"Execution time: {execution_time:.2f} seconds")
+  print(f"Total run time: {execution_time + compilation_time:.2f} seconds")
 
   process.terminate() # terminate process
   process.wait()
+  
+  if shell:
+    sys.exit(process.returncode)
+  elif process.returncode != 0:
+    raise Exception(f"Error in GAMS execution. Return code: {process.returncode}")
+
+
+status_message_patterns = [
+  "****",
+  "Model Statistics    SOLVE",
+  "SINGLE =E|X= EQUS",
+]
+
+error_message_patterns = [
+  "USER ERROR(S) ENCOUNTERED",
+  "** Infeasible solution to a square system",
+  "Locally Infeasible",
+  "Terminated By Solver",
+  "Solver Failure",
+  "Intermediate Infeasible",
+]
+
+status_message_exclude_patterns = [
+  "**** REPORT FILE SUMMARY",
+  "**** FILE SUMMARY",
+  "**** WARNING - COMPILER OPTIONS ARE NON DEFAULT",
+]
+
+def get_status_from_lst(list_file_path):
+  """Extract status messages from the listing file (lines starting with ****)"""
+  with open(list_file_path, 'r') as f:
+      status_messages = [
+          line for line in f
+          if any(line.startswith(pattern) for pattern in status_message_patterns + error_message_patterns)
+          and not any(line.startswith(exclude_pattern) for exclude_pattern in status_message_exclude_patterns)
+      ]
+  return "\n" + "".join(status_messages)
+
+def print_status(gams_file):
+  print(get_status_from_lst(get_lst_path(gams_file)))
+
+
+def cmd_call():
+  """Wrapper for calling gamY from command line."""
+  # Translate command line arguments to key-word arguments for the run function
+  cmd_args = sys.argv
+  kwargs = {"file_path": cmd_args[1]}
+
+  # Read optional command line arguments
+  for arg in cmd_args[2:]:
+    # Remove the '--' prefix if it exists
+    if arg.startswith("--"):
+      arg = arg[2:]
+    # Split the argument into key and value
+    key, value = arg.split("=", 1)
+    kwargs[key] = value
+
+  return run(**kwargs, shell=True)
 
-def gams_error(gams_file, check_error=False):
-    print(f"Error messages for {gams_file}")
-    lst_path = f"LST\\{gams_file[:-4]}.lst"
-    with open(lst_path, mode='r') as lst:
-      for line in lst.readlines():
-          if '****' in line:
-              print(line)
-          if check_error:
-              errors = [
-                '**** USER ERROR(S) ENCOUNTERED',
-                '** Infeasible solution to a square system',
-                'Locally Infeasible',
-                'Terminated By Solver',
-                'Solver Failure',
-                "**** MODEL STATUS      6 Intermediate Infeasible",
-              ]
-              for error in errors:
-                  if error in line:
-                    raise RuntimeError(f"Error in {gams_file}:\n{line}")
 
 if __name__ == "__main__":
   cmd_call()
```

### Comparing `dream-tools-2.1.9/dreamtools/gamY/gekko_endo_exo.py` & `dream-tools-2.2.0/dreamtools/gamY/gekko_endo_exo.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gamY/patterns.py` & `dream-tools-2.2.0/dreamtools/gamY/patterns.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gamY/rename_set.py` & `dream-tools-2.2.0/dreamtools/gamY/rename_set.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gams_excel/excel_endo_exo.py` & `dream-tools-2.2.0/dreamtools/gams_excel/excel_endo_exo.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gams_excel/gams_excel.py` & `dream-tools-2.2.0/dreamtools/gams_excel/gams_excel.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gams_excel/gdx_to_excel.py` & `dream-tools-2.2.0/dreamtools/gamY/gdx_to_excel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,57 @@
-"""
-Script takes three arguments:
-1. Path to an Excel workbook
-2. Path to GDX file
-3. Name of a sheet in the workbook
-In that sheet, the script expects a table with variables as index and years as column headers,
-starting in cell A1.
-The script will then fill the table with data from the GDX file.
-The script assumes that the time index is always last.
-"""
 import os
 import sys
 import xlwings as xw
 import pandas as pd
 import dreamtools as dt
 import re
 
-workbook_path = sys.argv[1]
-gdx_path = sys.argv[2]
-sheet_name = sys.argv[3]
 
 # workbook_path = "../Konjunktur/konjunktur.xlsx"
 # gdx_path = "../Konjunktur/Gdx/OER23August_nominal.gdx"
 # sheet_name = "data"
 
+def gdx_to_excel(gdx_path, workbook_path, sheet_name):
+    """
+    Fill an Excel worksheet with data from a GDX file.
+
+    Parameters
+    ----------
+    gdx_path : str
+        Path to GDX file
+    workbook_path : str
+        Path to an Excel workbook
+    sheet_name : str
+        Name of a sheet in the workbook
+        In that sheet, the script expects a table with variables as index and years as column headers,
+        starting in cell A1.
+        The function will then fill the table with data from the GDX file.
+        The function assumes that the time index is always last.
+    """
+
+    assert os.path.isfile(gdx_path), f"{gdx_path} not found"
+    db = dt.Gdx(gdx_path)
+
+    assert os.path.isfile(workbook_path), f"{workbook_path} not found"
+    wb = xw.Book(workbook_path)
+
+    assert sheet_name in wb.sheet_names, f'"{sheet_name}" not found in {workbook_path}'
+    sheet = wb.sheets[sheet_name]
+
+    data_range = sheet.range("A1", "B2").expand()
+    df = data_range.options(pd.DataFrame, index=True).value
+    try:
+        fill_dataframe(df, db)
+        data_range.offset(1, 1).resize(*df.shape).value = df.values
+    except Exception as e:
+        data_range.offset(1, 1).resize(*df.shape).value = None
+        raise e
+    
+    wb.save()
+
 def get_variable_name(variable_key):
     """Returns the variable name from a variable key, e.g. "qY[tje]" -> "qY" """
     return variable_key.split("[")[0]
 
 def get_index(variable_key):
     """Returns the index from a variable key, e.g. "qY[tje]" -> "tje" """
     if "[" in variable_key:
@@ -95,25 +120,7 @@
         except Exception as e:
             error_message = f"{e}"
             print(f"Error getting {variable_key}: {error_message}")
         if error_message is not None:
             df.loc[variable_key] = error_message
 
     return df
-
-assert os.path.isfile(gdx_path), f"{gdx_path} not found"
-db = dt.Gdx(gdx_path)
-
-assert os.path.isfile(workbook_path), f"{workbook_path} not found"
-wb = xw.Book(workbook_path)
-
-assert sheet_name in wb.sheet_names, f'"{sheet_name}" not found in {workbook_path}'
-sheet = wb.sheets[sheet_name]
-
-data_range = sheet.range("A1", "B2").expand()
-df = data_range.options(pd.DataFrame, index=True).value
-try:
-    fill_dataframe(df, db)
-    data_range.offset(1, 1).resize(*df.shape).value = df.values
-except Exception as e:
-    data_range.offset(1, 1).resize(*df.shape).value = None
-    raise e
```

### Comparing `dream-tools-2.1.9/dreamtools/gams_pandas/gams_pandas.py` & `dream-tools-2.2.0/dreamtools/gams_pandas/gams_pandas.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gams_pandas/gdx.py` & `dream-tools-2.2.0/dreamtools/gams_pandas/gdx.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gams_pandas/test_gams_pandas.py` & `dream-tools-2.2.0/dreamtools/gams_pandas/test_gams_pandas.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/gams_pandas/utility.py` & `dream-tools-2.2.0/dreamtools/gams_pandas/utility.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/age_plot.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/age_plot.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/dream_plotly_template.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/dream_plotly_template.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/dream_settings.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/dream_settings.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/makro_settings.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/makro_settings.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/reporting.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/reporting.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/scratch.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/scratch.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/test_plot.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/test_plot.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/test_timeseries_analysis.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/test_timeseries_analysis.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/dreamtools/multiindex_plotly/timeseries_analysis.py` & `dream-tools-2.2.0/dreamtools/multiindex_plotly/timeseries_analysis.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.9/setup.py` & `dream-tools-2.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   long_description = file.read()
 
 setuptools.setup(
   name="dream-tools",
   version=__version__,
   author="Martin Kirk Bonde",
   author_email="martin@bonde.dk",
-  description="A collection of tools used by the Danish institute for economic modelling and forecasting, DREAM (http://dreammodel.dk).",
+  description="A collection of tools used by the Danish Research Institute for Economic Analysis and Modelling, DREAM (https://dreamgruppen.dk/).",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/MartinBonde/dream-tools",
   packages=setuptools.find_packages(),
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

