# Comparing `tmp/psifr-0.9.0.tar.gz` & `tmp/psifr-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psifr-0.9.0.tar", last modified: Mon Jun  5 23:14:17 2023, max compression
+gzip compressed data, was "psifr-0.9.2.tar", last modified: Tue May 21 20:42:24 2024, max compression
```

## Comparing `psifr-0.9.0.tar` & `psifr-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.214196 psifr-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 23:14:05.000000 psifr-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-05 23:14:17.214196 psifr-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-06-05 23:14:05.000000 psifr-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-05 23:14:05.000000 psifr-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 23:14:17.214196 psifr-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.202195 psifr-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.202195 psifr-0.9.0/src/psifr/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.202195 psifr-0.9.0/src/psifr/data/
--rw-r--r--   0 runner    (1001) docker     (123)  4050433 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/data/Morton2013.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.210196 psifr-0.9.0/src/psifr/distances/
--rw-r--r--   0 runner    (1001) docker     (123)  4802050 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/distances/Morton2013.npz
--rw-r--r--   0 runner    (1001) docker     (123)    65710 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/fr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/maskers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    32940 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.202195 psifr-0.9.0/src/psifr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.214196 psifr-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_category_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_distance_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_fr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_lag_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_maskers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_output_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_pair_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:42:24.572882 psifr-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 20:42:19.000000 psifr-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-21 20:42:24.572882 psifr-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-21 20:42:19.000000 psifr-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-21 20:42:19.000000 psifr-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:42:24.572882 psifr-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:42:24.556882 psifr-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:42:24.556882 psifr-0.9.2/src/psifr/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 20:42:19.000000 psifr-0.9.2/src/psifr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:42:24.560882 psifr-0.9.2/src/psifr/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  4050433 2024-05-21 20:42:19.000000 psifr-0.9.2/src/psifr/data/Morton2013.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:42:24.564882 psifr-0.9.2/src/psifr/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)  4802050 2024-05-21 20:42:19.000000 psifr-0.9.2/src/psifr/distances/Morton2013.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    68402 2024-05-21 20:42:19.000000 psifr-0.9.2/src/psifr/fr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-05-21 20:42:19.000000 psifr-0.9.2/src/psifr/maskers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-05-21 20:42:19.000000 psifr-0.9.2/src/psifr/measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33170 2024-05-21 20:42:19.000000 psifr-0.9.2/src/psifr/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:42:24.572882 psifr-0.9.2/src/psifr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-21 20:42:24.000000 psifr-0.9.2/src/psifr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-21 20:42:24.000000 psifr-0.9.2/src/psifr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:42:24.000000 psifr-0.9.2/src/psifr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-21 20:42:24.000000 psifr-0.9.2/src/psifr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 20:42:24.000000 psifr-0.9.2/src/psifr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:42:24.572882 psifr-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-21 20:42:19.000000 psifr-0.9.2/tests/test_category_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-21 20:42:19.000000 psifr-0.9.2/tests/test_distance_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20471 2024-05-21 20:42:19.000000 psifr-0.9.2/tests/test_fr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-21 20:42:19.000000 psifr-0.9.2/tests/test_lag_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-21 20:42:19.000000 psifr-0.9.2/tests/test_maskers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-21 20:42:19.000000 psifr-0.9.2/tests/test_output_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-21 20:42:19.000000 psifr-0.9.2/tests/test_pair_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-21 20:42:19.000000 psifr-0.9.2/tests/test_plots.py
```

### Comparing `psifr-0.9.0/LICENSE` & `psifr-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psifr-0.9.0/PKG-INFO` & `psifr-0.9.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: psifr
-Version: 0.9.0
-Summary: Psifr: Analysis and visualization of free recall data
-Author-email: Neal W Morton <mortonne@gmail.com>
-License: GPL-3.0-or-later
-Keywords: psychology,memory,free recall
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: perf
-License-File: LICENSE
-
 # Psifr
 [![PyPI version](https://badge.fury.io/py/psifr.svg)](https://badge.fury.io/py/psifr)
 [![Documentation Status](https://readthedocs.org/projects/psifr/badge/?version=latest)](https://psifr.readthedocs.io/en/latest/?badge=latest)
 [![Pytest](https://github.com/mortonne/psifr/actions/workflows/pytest.yml/badge.svg)](https://github.com/mortonne/psifr/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/mortonne/psifr/branch/master/graph/badge.svg)](https://codecov.io/gh/mortonne/psifr)
 [![status](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299/status.svg)](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299)
 [![DOI](https://zenodo.org/badge/248593723.svg)](https://zenodo.org/badge/latestdoi/248593723)
```

### Comparing `psifr-0.9.0/pyproject.toml` & `psifr-0.9.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "psifr"
-version = "0.9.0"
+version = "0.9.2"
 authors = [
     {name = "Neal W Morton", email = "mortonne@gmail.com"}
 ]
 description = "Psifr: Analysis and visualization of free recall data"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["psychology", "memory", "free recall"]
@@ -13,21 +13,21 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "numpy",
     "scipy",
-    "pandas>=1.0.0",
+    "pandas>=1.0.0, <2.2.0",
     "matplotlib!=3.3.1",
-    "seaborn>=0.9.1",
+    "seaborn>=0.9.2",
 ]
 
 [project.optional-dependencies]
-docs = ["sphinx", "pydata-sphinx-theme", "ipython", "sphinxcontrib-bibtex"]
+docs = ["sphinx", "pydata-sphinx-theme", "ipython", "sphinxcontrib-bibtex", "pickleshare"]
 test = ["pytest", "codecov", "pytest-cov"]
 perf = ["snakeviz", "asv"]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `psifr-0.9.0/src/psifr/data/Morton2013.csv` & `psifr-0.9.2/src/psifr/data/Morton2013.csv`

 * *Files identical despite different names*

### Comparing `psifr-0.9.0/src/psifr/distances/Morton2013.npz` & `psifr-0.9.2/src/psifr/distances/Morton2013.npz`

 * *Files identical despite different names*

### Comparing `psifr-0.9.0/src/psifr/fr.py` & `psifr-0.9.2/src/psifr/fr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """Utilities for working with free recall data."""
 
-from pkg_resources import resource_filename
+from importlib import resources
 import warnings
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
 from psifr import stats
 from psifr import measures
 
 
 def sample_data(study):
     """Read sample data."""
-    data_file = resource_filename('psifr', f'data/{study}.csv')
+    if hasattr(resources, 'files'):
+        data_file = resources.files('psifr') / 'data' / f'{study}.csv'
+    else:
+        from pkg_resources import resource_filename
+        data_file = resource_filename('psifr', f'data/{study}.csv')
     df = pd.read_csv(data_file)
     return df
 
 
 def sample_distances(study):
     """Read sample distances."""
-    distance_file = resource_filename('psifr', f'distances/{study}.npz')
+    if hasattr(resources, 'files'):
+        distance_file = resources.files('psifr') / 'distances' / f'{study}.npz'
+    else:
+        from pkg_resources import resource_filename
+        distance_file = resource_filename('psifr', f'distances/{study}.npz')
     f = np.load(distance_file)
     return f['items'], f['distances']
 
 
 def table_from_lists(subjects, study, recall, lists=None, **kwargs):
     """
     Create table format data from list format data.
@@ -1006,15 +1014,15 @@
     116       46         3      0  0.000000  0.000000
     117       47         1      5  0.111111  0.277778
     118       47         2      1  0.022222  0.055556
     119       47         3      0  0.000000  0.000000
     <BLANKLINE>
     [120 rows x 5 columns]
     """
-    result = df.groupby('subject').apply(_subject_pli_list_lag, max_lag)
+    result = df.groupby('subject')[df.columns].apply(_subject_pli_list_lag, max_lag)
     result = result.reset_index()
     return result
 
 
 def lag_crp(
     df, lag_key='input', count_unique=False, item_query=None, test_key=None, test=None
 ):
@@ -1545,15 +1553,22 @@
         test=test,
     )
     rank = measure.analyze(df)
     return rank
 
 
 def distance_rank_window(
-    df, index_key, distances, window_lags, item_query=None, test_key=None, test=None
+    df,
+    index_key,
+    distances,
+    window_lags,
+    item_query=None,
+    test_key=None,
+    test=None,
+    exclude_prev_window=False,
 ):
     """
     Rank of transition distances relative to items in a window.
 
     Transitions are ranked based on their distance relative to items
     at specified lags from the previous item in the input list.
 
@@ -1585,28 +1600,100 @@
         Name of column with labels to use when testing transitions for
         inclusion.
 
     test : callable, optional
         Callable that takes in previous and current item values and
         returns True for transitions that should be included.
 
+    exclude_prev_window : bool, optional
+        If true, transitions preceded by items in the window around the
+        previous item in the list will be excluded.
+
     Returns
     -------
     stat : pandas.DataFrame
         Has fields 'subject', 'lag', and 'rank'.
     """
     list_length = int(df['input'].max())
     measure = measures.TransitionDistanceRankWindow(
         index_key,
         distances,
         list_length,
         window_lags,
         item_query=item_query,
         test_key=test_key,
         test=test,
+        exclude_prev_window=exclude_prev_window,
+    )
+    rank = measure.analyze(df)
+    return rank
+
+
+def distance_rank_window_asym(
+    df,
+    index_key,
+    distances,
+    item_query=None,
+    test_key=None,
+    test=None,
+    exclude_prev_window=False,
+):
+    """
+    Rank of transition distances relative to items in a window.
+
+    Transitions are ranked based on their distance relative to items
+    at specified lags from the previous item in the input list.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        Merged study and recall data. See merge_lists. List length is
+        assumed to be the same for all lists within each subject.
+        Must have fields: subject, list, input, output, recalled.
+        Input position must be defined such that the first serial
+        position is 1, not 0.
+
+    index_key : str
+        Name of column containing the index of each item in the
+        `distances` matrix.
+
+    distances : numpy.array
+        Items x items matrix of pairwise distances or similarities.
+
+    item_query : str, optional
+        Query string to select items to include in the pool of possible
+        recalls to be examined. See `pandas.DataFrame.query` for
+        allowed format.
+
+    test_key : str, optional
+        Name of column with labels to use when testing transitions for
+        inclusion.
+
+    test : callable, optional
+        Callable that takes in previous and current item values and
+        returns True for transitions that should be included.
+
+    exclude_prev_window : bool, optional
+        If true, transitions preceded by items in the window around the
+        previous item in the list will be excluded.
+
+    Returns
+    -------
+    stat : pandas.DataFrame
+        Has fields 'subject', 'lag', and 'rank'.
+    """
+    list_length = int(df['input'].max())
+    measure = measures.TransitionDistanceRankWindowAsym(
+        index_key,
+        distances,
+        list_length,
+        item_query=item_query,
+        test_key=test_key,
+        test=test,
+        exclude_prev_window=exclude_prev_window,
     )
     rank = measure.analyze(df)
     return rank
 
 
 def category_crp(df, category_key, item_query=None, test_key=None, test=None):
     """
@@ -1731,15 +1818,17 @@
     2        3  3.363768  0.627371
     3        4  4.444928  0.688761
     4        5  7.530435  0.873755
     """
     # these analyses are undefined when there are repeats and
     # intrusions, so strip them out
     clean = df.query('~intrusion and repeat == 0')
-    stats = clean.groupby('subject').apply(_subject_category_clustering, category_key)
+    stats = clean.groupby('subject')[clean.columns].apply(
+        _subject_category_clustering, category_key
+    )
     stats = stats.reset_index()
     return stats
 
 
 def plot_spc(recall, **facet_kws):
     """
     Plot a serial position curve.
@@ -1864,15 +1953,17 @@
     facet_kws
         Additional keywords for the FacetGrid.
     """
     g = sns.FacetGrid(data=data.reset_index(), dropna=False, **facet_kws)
     g.map_dataframe(
         sns.swarmplot, x=x, y=y, color=swarm_color, size=swarm_size, zorder=1
     )
-    g.map_dataframe(sns.pointplot, x=x, y=y, color=point_color, join=False, capsize=0.5)
+    g.map_dataframe(
+        sns.pointplot, x=x, y=y, color=point_color, linestyle='none', capsize=0.5
+    )
     return g
 
 
 def plot_raster(
     df,
     hue='input',
     palette=None,
```

### Comparing `psifr-0.9.0/src/psifr/maskers.py` & `psifr-0.9.2/src/psifr/maskers.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,14 +357,15 @@
     pool_items,
     recall_items,
     pool_output,
     recall_output,
     pool_test=None,
     recall_test=None,
     test=None,
+    exclude_prev_window=False,
 ):
     """
     Yield windows around previous items in the input list.
 
     Parameters
     ----------
     list_length : int
@@ -396,14 +397,18 @@
         Used to test whether individual transitions should be included,
         based on test values.
 
             test(prev, curr) - test for included transition
 
             test(prev, poss) - test for included possible transition
 
+    exclude_prev_window : bool, optional
+        If true, transitions preceded by items in the window around the
+        previous item in the list will be excluded.
+
     Yields
     ------
     output : int
         Output positions of included transitions. The first transition
         is 1.
 
     prev : list
@@ -445,14 +450,19 @@
         # get windowed items in the input list
         prev = int(recall_items[n]) + window_lags
 
         # exclude if any windowed items do not exist or fail test
         if np.any(prev < 1) or np.any(prev > list_length):
             continue
 
+        # exclude current transition if prior transition was from the window
+        if exclude_prev_window and n > 0:
+            if recall_items[n - 1] in prev:
+                continue
+
         # exclude current/possible items in the window
         curr = int(recall_items[n + 1])
         if curr in prev:
             continue
         poss = np.asarray(poss_items, int)
         include_poss = ~np.isin(poss, prev)
         poss = poss[include_poss]
```

### Comparing `psifr-0.9.0/src/psifr/measures.py` & `psifr-0.9.2/src/psifr/measures.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         Query string to indicate trials to include in the measure.
 
     test : callable
         Test of trial inclusion.
     """
 
     def __init__(self, items_key, label_key, item_query=None, test_key=None, test=None):
-
         self.keys = {'items': items_key, 'label': label_key, 'test': test_key}
         self.item_query = item_query
         self.test = test
 
     def split_lists(self, data, phase, item_query=None):
         """
         Get relevant fields and split by list.
@@ -177,15 +176,14 @@
             'input', lag_key, item_query=item_query, test_key=test_key, test=test
         )
         self.list_length = list_length
         self.count_unique = count_unique
         self.compound = compound
 
     def analyze_subject(self, subject, pool, recall):
-
         if self.compound:
             counter = stats.count_lags_compound
         else:
             counter = stats.count_lags
 
         actual, possible = counter(
             self.list_length,
@@ -263,15 +261,14 @@
         if centers is None:
             # if no explicit centers, use halfway between edges
             centers = edges[:-1] + (np.diff(edges) / 2)
         self.centers = centers
         self.count_unique = count_unique
 
     def analyze_subject(self, subject, pool, recall):
-
         actual, possible = stats.count_distance(
             self.distances,
             self.edges,
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
@@ -361,40 +358,90 @@
         index_key,
         distances,
         list_length,
         window_lags,
         item_query=None,
         test_key=None,
         test=None,
+        exclude_prev_window=False,
     ):
         super().__init__(
             'input', index_key, item_query=item_query, test_key=test_key, test=test
         )
         self.distances = distances
         self.list_length = list_length
         self.window_lags = window_lags
+        self.exclude_prev_window = exclude_prev_window
 
     def analyze_subject(self, subject, pool, recall):
         ranks = stats.rank_distance_window(
             self.distances,
             self.list_length,
             self.window_lags,
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
             pool['test'],
             recall['test'],
             self.test,
+            self.exclude_prev_window,
         )
         index = pd.MultiIndex.from_arrays(
             [[subject] * len(self.window_lags), self.window_lags],
             names=['subject', 'lag'],
         )
-        stat = pd.DataFrame({'rank': np.nanmean(ranks, 0)}, index=index)
+        stat = pd.DataFrame(
+            {'n': np.count_nonzero(~np.isnan(ranks), 0), 'rank': np.nanmean(ranks, 0)},
+            index=index,
+        )
+        return stat
+
+
+class TransitionDistanceRankWindowAsym(TransitionMeasure):
+    """Measure asymmetry of transition distance rank in a window."""
+
+    def __init__(
+        self,
+        index_key,
+        distances,
+        list_length,
+        item_query=None,
+        test_key=None,
+        test=None,
+        exclude_prev_window=False,
+    ):
+        super().__init__(
+            'input', index_key, item_query=item_query, test_key=test_key, test=test
+        )
+        self.distances = distances
+        self.list_length = list_length
+        self.window_lags = [-1, 1]
+        self.exclude_prev_window = exclude_prev_window
+
+    def analyze_subject(self, subject, pool, recall):
+        ranks = stats.rank_distance_window(
+            self.distances,
+            self.list_length,
+            self.window_lags,
+            pool['items'],
+            recall['items'],
+            pool['label'],
+            recall['label'],
+            pool['test'],
+            recall['test'],
+            self.test,
+            self.exclude_prev_window,
+        )
+        asym = ranks[:, 1] - ranks[:, 0]
+        stat = pd.DataFrame(
+            {'n': np.count_nonzero(~np.isnan(asym)), 'asym': np.nanmean(asym)},
+            index=[subject],
+        )
+        stat.index.name = 'subject'
         return stat
 
 
 class TransitionCategory(TransitionMeasure):
     """Measure conditional response probability by category transition."""
 
     def __init__(self, category_key, item_query=None, test_key=None, test=None):
```

### Comparing `psifr-0.9.0/src/psifr/stats.py` & `psifr-0.9.2/src/psifr/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -869,14 +869,15 @@
     pool_items,
     recall_items,
     pool_index,
     recall_index,
     pool_test=None,
     recall_test=None,
     test=None,
+    exclude_prev_window=False,
 ):
     """
     Calculate percentile rank of distances relative to items in a window.
 
     Parameters
     ----------
     distances : numpy.array
@@ -906,14 +907,18 @@
     recall_test : list of list, optional
         Test value for each recalled item.
 
     test : callable
         Called as test(prev, curr) or test(prev, poss) to screen
         actual and possible transitions, respectively.
 
+    exclude_prev_window : bool, optional
+        If true, transitions preceded by items in the window around the
+        previous item in the list will be excluded.
+
     Returns
     -------
     rank : numpy.ndarray
         [transitions x window lags] array with distance percentile ranks.
         The rank is 0 if the distance was the largest of the available
         transitions, and 1 if the distance was the smallest. Ties are
         assigned to the average percentile rank.
@@ -928,14 +933,15 @@
             pool_items[i],
             recall_items[i],
             pool_index[i],
             recall_index[i],
             pool_test_list,
             recall_test_list,
             test,
+            exclude_prev_window,
         )
         for output, w_prev, curr, poss in masker:
             curr = int(curr)
             rank_lag = []
             for prev in w_prev:
                 prev = int(prev)
                 poss = poss.astype(int)
```

### Comparing `psifr-0.9.0/src/psifr.egg-info/PKG-INFO` & `psifr-0.9.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 Metadata-Version: 2.1
 Name: psifr
-Version: 0.9.0
+Version: 0.9.2
 Summary: Psifr: Analysis and visualization of free recall data
 Author-email: Neal W Morton <mortonne@gmail.com>
 License: GPL-3.0-or-later
 Keywords: psychology,memory,free recall
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas<2.2.0,>=1.0.0
+Requires-Dist: matplotlib!=3.3.1
+Requires-Dist: seaborn>=0.9.2
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: ipython; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: pickleshare; extra == "docs"
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: codecov; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: perf
-License-File: LICENSE
+Requires-Dist: snakeviz; extra == "perf"
+Requires-Dist: asv; extra == "perf"
 
 # Psifr
 [![PyPI version](https://badge.fury.io/py/psifr.svg)](https://badge.fury.io/py/psifr)
 [![Documentation Status](https://readthedocs.org/projects/psifr/badge/?version=latest)](https://psifr.readthedocs.io/en/latest/?badge=latest)
 [![Pytest](https://github.com/mortonne/psifr/actions/workflows/pytest.yml/badge.svg)](https://github.com/mortonne/psifr/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/mortonne/psifr/branch/master/graph/badge.svg)](https://codecov.io/gh/mortonne/psifr)
 [![status](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299/status.svg)](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299)
```

### Comparing `psifr-0.9.0/src/psifr.egg-info/SOURCES.txt` & `psifr-0.9.2/src/psifr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psifr-0.9.0/tests/test_category_stats.py` & `psifr-0.9.2/tests/test_category_stats.py`

 * *Files identical despite different names*

### Comparing `psifr-0.9.0/tests/test_distance_stats.py` & `psifr-0.9.2/tests/test_lag_stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,255 +1,197 @@
-"""Test distance clustering statistics."""
+"""Test lag clustering statistics."""
 
 import numpy as np
 import pytest
 
 from psifr import stats
 
 
 @pytest.fixture()
 def data():
-    """Create position data for a list."""
-    list_data = {
-        'pool_position': [0, 1, 2, 3, 4, 5, 6, 7],
-        'recall_position': [3, 2, 1, 7, 0, 6, 5],
+    """Create list data with position and category."""
+    test_list = {
+        'list_length': 8,
+        'n_block': 4,
+        'pool_position': [1, 2, 3, 4, 5, 6, 7, 8],
+        'pool_category': [1, 1, 2, 2, 1, 1, 2, 2],
+        'pool_block': [1, 1, 2, 2, 3, 3, 4, 4],
+        'output_position': [1, 3, 4, 8, 5, 4, 7, 6],
+        'output_category': [1, 2, 2, 2, 1, 2, 2, 1],
+        'output_block': [1, 2, 2, 4, 3, 2, 4, 3],
     }
-    return list_data
+    return test_list
 
 
 @pytest.fixture()
 def list_data():
     """Create list data with item and category information."""
     data = {
-        'pool_items': [[0, 1, 2, 3, 4, 5, 6, 7]],
-        'recall_items': [[3, 2, 1, 7, 0, 6, 5]],
-        'pool_test': [[1, 1, 2, 2, 2, 2, 1, 1]],
-        'recall_test': [[2, 2, 1, 1, 1, 1, 2]],
+        'pool_items': [[1, 2, 3, 4, 5, 6]],
+        'recall_items': [[6, 2, 1, 5, 4]],
+        'pool_test': [[1, 1, 1, 2, 2, 2]],
+        'recall_test': [[2, 1, 1, 2, 2]],
     }
     return data
 
 
-@pytest.fixture()
-def distance():
-    """Create a distance matrix."""
-    mat = np.array(
-        [
-            [0, 1, 1, 1, 2, 2, 2, 2],
-            [1, 0, 1, 1, 2, 2, 2, 2],
-            [1, 1, 0, 1, 2, 2, 2, 2],
-            [1, 1, 1, 0, 2, 2, 2, 2],
-            [2, 2, 2, 2, 0, 3, 3, 3],
-            [2, 2, 2, 2, 3, 0, 3, 3],
-            [2, 2, 2, 2, 3, 3, 0, 3],
-            [2, 2, 2, 2, 3, 3, 3, 0],
-        ]
-    )
-    return mat
-
-
-def test_distance_count(data, distance):
-    """Test distance bin count."""
-    edges = [0.5, 1.5, 2.5, 3.5]
-    actual, possible = stats.count_distance(
-        distance,
-        edges,
+def test_lag_count(data):
+    """Test transition counts by serial position lag."""
+    actual, possible = stats.count_lags(
+        data['list_length'], [data['pool_position']], [data['output_position']]
+    )
+    np.testing.assert_array_equal(
+        actual.to_numpy(), np.array([0, 0, 0, 0, 1, 0, 1, 0, 1, 1, 0, 1, 0, 0, 0])
+    )
+    np.testing.assert_array_equal(
+        possible.to_numpy(), np.array([0, 1, 1, 0, 1, 2, 3, 0, 3, 3, 3, 3, 2, 1, 1])
+    )
+
+
+def test_lag_count_category(data):
+    """Test transition counts by lag for within-category transitions."""
+    # within category
+    actual, possible = stats.count_lags(
+        data['list_length'],
         [data['pool_position']],
-        [data['recall_position']],
+        [data['output_position']],
+        pool_test=[data['pool_category']],
+        recall_test=[data['output_category']],
+        test=lambda x, y: x == y,
+    )
+    np.testing.assert_array_equal(
+        actual.to_numpy(), np.array([0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0])
+    )
+    np.testing.assert_array_equal(
+        possible.to_numpy(), np.array([0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 1, 2, 1, 0, 0])
+    )
+
+    # across category
+    actual, possible = stats.count_lags(
+        data['list_length'],
         [data['pool_position']],
-        [data['recall_position']],
+        [data['output_position']],
+        pool_test=[data['pool_category']],
+        recall_test=[data['output_category']],
+        test=lambda x, y: x != y,
+    )
+    np.testing.assert_array_equal(
+        actual.to_numpy(), np.array([0, 0, 0, 0, 1, 0, 1, 0, 0, 1, 0, 0, 0, 0, 0])
+    )
+    np.testing.assert_array_equal(
+        possible.to_numpy(), np.array([0, 1, 1, 0, 1, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1])
+    )
+
+
+def test_lag_count_block(data):
+    """Test transition counts by block lag."""
+    actual, possible = stats.count_lags(
+        data['n_block'],
+        [data['pool_block']],
+        [data['output_block']],
         count_unique=False,
     )
-    # recalls: [3, 2, 1, 7, 0, 6, 5]
-    # actual: [1, 1, 2, 2, 2, 3]
-    # possible: [
-    #     [1, 1, 1, 2, 2, 2, 2],
-    #     [1, 1, 2, 2, 2, 2],
-    #     [1, 2, 2, 2, 2],
-    #     [2, 3, 3, 3],
-    #     [2, 2, 2],
-    #     [3, 3]
-    # ]
-    expected_actual = np.array([2, 3, 1])
-    expected_possible = np.array([6, 16, 5])
-    np.testing.assert_array_equal(actual.to_numpy(), expected_actual)
-    np.testing.assert_array_equal(possible.to_numpy(), expected_possible)
-
-
-def test_distance_count_unique(data, distance):
-    """Test distance bin count by transition."""
-    edges = [0.5, 2.5, 3.5]
-    inputs = [
-        distance,
-        edges,
-        [data['pool_position']],
-        [data['recall_position']],
-        [data['pool_position']],
-        [data['recall_position']],
-    ]
+    np.testing.assert_array_equal(actual.to_numpy(), np.array([0, 0, 2, 1, 1, 1, 0]))
+    np.testing.assert_array_equal(possible.to_numpy(), np.array([2, 0, 5, 3, 6, 6, 2]))
 
-    # first check these bins with count_unique=False
-    actual, possible = stats.count_distance(*inputs, count_unique=False)
-    np.testing.assert_array_equal(actual.to_numpy(), np.array([5, 1]))
-    np.testing.assert_array_equal(possible.to_numpy(), np.array([22, 5]))
-
-    # now test with only one bin increment per transition
-    actual, possible = stats.count_distance(*inputs, count_unique=True)
-    np.testing.assert_array_equal(actual.to_numpy(), np.array([5, 1]))
-    np.testing.assert_array_equal(possible.to_numpy(), np.array([5, 2]))
-
-
-def test_rank_distance(list_data, distance):
-    """Test rank distance measure."""
-    ranks = stats.rank_distance(
-        distance,
+
+def test_lag_count_block_unique(data):
+    """Test transition counts by unique block lag."""
+    actual, possible = stats.count_lags(
+        data['n_block'], [data['pool_block']], [data['output_block']], count_unique=True
+    )
+    np.testing.assert_array_equal(actual.to_numpy(), np.array([0, 0, 2, 1, 1, 1, 0]))
+    np.testing.assert_array_equal(possible.to_numpy(), np.array([2, 0, 4, 3, 3, 3, 1]))
+
+
+def test_compound_lag_count():
+    """Test transition lag count conditional on prior lag."""
+    list_length = 4
+    pool_position = [[1, 2, 3, 4]]
+    output_position = [[4, 1, 2, 3]]
+    # -3: +1 (+1, +2)
+    # +1: +1 (+1)
+    # -3:-3, -3:-2, -3:-1, -3:0, -3:+1, -3:+2, -3:+3, ...
+    expected_actual = np.hstack(
+        (
+            [0, 0, 0, 0, 1, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 1, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+        )
+    )
+    expected_possible = np.hstack(
+        (
+            [0, 0, 0, 0, 1, 1, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 1, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0],
+        )
+    )
+    actual, possible = stats.count_lags_compound(
+        list_length, pool_position, output_position
+    )
+    np.testing.assert_array_equal(actual, expected_actual)
+    np.testing.assert_array_equal(possible, expected_possible)
+
+
+def test_percentile_rank():
+    """Test calculation of percentile rank."""
+    possible = [1, 2, 3, 4]
+    rank = []
+    for actual in possible:
+        rank.append(stats.percentile_rank(actual, possible))
+    np.testing.assert_array_equal(np.array(rank), np.array([0, 1 / 3, 2 / 3, 1]))
+
+
+def test_rank_lag(list_data):
+    """Test temporal lag rank."""
+    ranks = stats.rank_lags(
         list_data['pool_items'],
         list_data['recall_items'],
         list_data['pool_items'],
         list_data['recall_items'],
     )
-    # recalls: [3, 2, 1, 7, 0, 6, 5]
-    # actual: [1, 1, 2, 2, 2, 3]
-    # possible: [
-    #     [1, 1, 1, 2, 2, 2, 2],
-    #     [1, 1, 2, 2, 2, 2],
-    #     [1, 2, 2, 2, 2],
-    #     [2, 3, 3, 3],
-    #     [2, 2, 2],
-    #     [3, 3],
-    # ]
-    # actual_rank: [2.0, 1.5, 3.5, 1.0, 2.0, 1.5]
-    # possible_rank: [
-    #     [2.0, 2.0, 2.0, 5.5, 5.5, 5.5, 5.5],
-    #     [1.5, 1.5, 4.5, 4.5, 4.5, 4.5],
-    #     [1.0, 3.5, 3.5, 3.5, 3.5],
-    #     [1.0, 3.0, 3.0, 3.0],
-    #     [2.0, 2.0, 2.0],
-    #     [1.5, 1.5],
-    # ]
-    expected = np.array(
-        [
-            1 - (1 / 6),
-            1 - (0.5 / 5),
-            1 - (2.5 / 4),
-            1 - (0 / 3),
-            1 - (1 / 2),
-            1 - (0.5 / 1),
-        ]
-    )
+    expected = np.array([1 / 4, 5 / 6, 0, 1])
     np.testing.assert_allclose(ranks, expected)
 
 
-def test_rank_distance_within(list_data, distance):
-    """Test rank distance for within-category transitions."""
-    ranks = stats.rank_distance(
-        distance,
+def test_rank_lag_short(list_data):
+    """Test temporal lag rank without label inputs."""
+    ranks = stats.rank_lags(
         list_data['pool_items'],
         list_data['recall_items'],
-        list_data['pool_items'],
-        list_data['recall_items'],
-        pool_test=list_data['pool_test'],
-        recall_test=list_data['recall_test'],
-        test=lambda x, y: x == y,
     )
-    expected = np.array([1 - (0 / 2), 1 - (1.5 / 2), 1 - (0 / 1), np.nan])
+    expected = np.array([1 / 4, 5 / 6, 0, 1])
     np.testing.assert_allclose(ranks, expected)
 
 
-def test_rank_distance_across(list_data, distance):
-    """Test rank distance for across-category transitions."""
-    ranks = stats.rank_distance(
-        distance,
-        list_data['pool_items'],
-        list_data['recall_items'],
+def test_rank_lag_within(list_data):
+    """Test temporal lag rank for within-category transitions."""
+    ranks = stats.rank_lags(
         list_data['pool_items'],
         list_data['recall_items'],
         pool_test=list_data['pool_test'],
         recall_test=list_data['recall_test'],
-        test=lambda x, y: x != y,
+        test=lambda x, y: x == y,
     )
-    expected = np.array([1 - (0.5 / 3), 1 - (0.5 / 1)])
-    np.testing.assert_allclose(ranks, expected)
+    expected = np.array([0.5, np.nan])
+    np.testing.assert_array_equal(ranks, expected)
 
 
-def test_rank_distance_shifted(list_data, distance):
-    """Test rank distance based on shifted recalls."""
-    list_data['recall_items'] = [[4, 3, 1, 7, 3, 0, 6, 2]]
-    distance[3, 1] = 4
-    distance[1, 3] = 4
-    # sequences: [[4, 3, 1], [3, 1, 7], [0, 6, 5]]
-    # -1
-    # actual: [4, 2, 2]
-    # possible: [
-    #     [1, 1, 2, 2, 2, 4],
-    #     [1, 1, 2, 2, 2],
-    #     [2, 3],
-    # ]
-    # rank: [0.0, 0.25, 1.0]
-    # -2
-    # actual: [2, 2, 1]
-    # possible: [
-    #     [2, 2, 2, 3, 3, 3],
-    #     [1, 1, 2, 2, 2],
-    #     [1, 2],
-    # ]
-    # rank: [0.8, 0.25, 1.0]
-    ranks = stats.rank_distance_shifted(
-        distance,
-        2,
+def test_rank_lag_across(list_data):
+    """Test temporal lag rank for across-category transitions."""
+    ranks = stats.rank_lags(
         list_data['pool_items'],
         list_data['recall_items'],
-        list_data['pool_items'],
-        list_data['recall_items'],
-    )
-    expected = np.array([[0.8, 0.0], [0.25, 0.25], [1.0, 1.0]])
-    np.testing.assert_allclose(ranks, expected)
-
-
-def test_rank_distance_window():
-    """Test rank distance relative to items in a window."""
-    distance = np.array(
-        [
-            [0, 3, 1, 1, 2, 2, 2, 2],
-            [3, 0, 1, 1, 2, 2, 2, 2],
-            [1, 1, 0, 4, 2, 2, 2, 2],
-            [1, 1, 4, 0, 2, 2, 2, 2],
-            [2, 2, 2, 2, 0, 5, 3, 3],
-            [2, 2, 2, 2, 5, 0, 3, 3],
-            [2, 2, 2, 2, 3, 3, 0, 6],
-            [2, 2, 2, 2, 3, 3, 6, 0],
-        ]
-    )
-    pool = [[1, 2, 3, 4, 5, 6, 7, 8]]
-    outputs = [[4, 2, 1, 7, 5, 3, 4]]
-    pool_index = [[4, 5, 6, 7, 0, 1, 2, 3]]
-    outputs_index = [[3, 1, 0, 6, 4, 2, 3]]
-    list_length = 8
-    window_lags = [-1, 0, 1]
-
-    # included: [(4, 2), (7, 5), (5, 3)]
-    # prev: [[3, 4, 5], [6, 7, 8], [4, 5, 6]]
-    # curr: [2, 5, 3]
-    # poss: [[1, 2, 6, 7, 8], [3, 5], [3, 8]]
-
-    # prev: [[6, 7, 0], [1, 2, 3], [7, 0, 1]]
-    # curr: [5, 0, 6]
-    # poss: [[4, 5, 1, 2, 3], [6, 0], [6, 3]]
-
-    # -1
-    # actual: [3, 3, 6]
-    # possible: [[3, 3, 2, 2, 2], [2, 3], [6, 2]]
-    # rank: [0.125, 0.0, 0.0]
-
-    # 0
-    # actual: [3, 1, 2]
-    # possible: [[3, 3, 2, 2, 2], [2, 1], [2, 1]]
-    # rank: [0.125, 1.0, 0.0]
-
-    # +1
-    # actual: [2, 1, 2]
-    # possible: [[2, 2, 3, 1, 1], [2, 1], [2, 1]]
-    # rank: [0.375, 1.0, 0.0]
-    ranks = stats.rank_distance_window(
-        distance, list_length, window_lags, pool, outputs, pool_index, outputs_index
+        pool_test=list_data['pool_test'],
+        recall_test=list_data['recall_test'],
+        test=lambda x, y: x != y,
     )
-    expected = np.array([[0.125, 0.125, 0.375], [0, 1, 1], [0, 0, 0]])
-    np.testing.assert_allclose(ranks, expected)
+    expected = np.array([0.5, 0])
+    np.testing.assert_array_equal(ranks, expected)
```

### Comparing `psifr-0.9.0/tests/test_fr.py` & `psifr-0.9.2/tests/test_fr.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,7 +562,43 @@
     recall = [['fountain', 'hollow', 'absence', 'cat', 'piano', 'pupil', 'fountain']]
     item_index = ([[0, 1, 2, 3, 4, 5, 6, 7]], [[3, 1, 0, 6, 4, 2, 3]])
     raw = fr.table_from_lists(subjects, study, recall, item_index=item_index)
     data = fr.merge_free_recall(raw, list_keys=['item_index'])
     stat = fr.distance_rank_window(data, 'item_index', distances, [-1, 0, 1])
     expected = np.array([[0.875, 0.875, 0.375], [0, 1, 1], [0, 0, 0]])
     np.testing.assert_allclose(np.mean(expected, 0), stat['rank'].to_numpy())
+
+    # example from stats function test
+    distances = np.array(
+        [
+            [0, 3, 1, 1, 2, 2, 2, 2],
+            [3, 0, 1, 1, 2, 2, 2, 2],
+            [1, 1, 0, 4, 2, 2, 2, 2],
+            [1, 1, 4, 0, 2, 2, 2, 2],
+            [2, 2, 2, 2, 0, 5, 3, 3],
+            [2, 2, 2, 2, 5, 0, 3, 3],
+            [2, 2, 2, 2, 3, 3, 0, 6],
+            [2, 2, 2, 2, 3, 3, 6, 0],
+        ]
+    )
+    pool = ['piano', 'pillow', 'cat', 'tree', 'absence', 'hollow', 'pupil', 'fountain']
+    recall = [['fountain', 'hollow', 'absence', 'cat', 'piano', 'pillow', 'tree']]
+    raw = fr.table_from_lists(subjects, study, recall)
+    raw['item_index'] = fr.pool_index(raw['item'], pool)
+    data = fr.merge_free_recall(raw, list_keys=['item_index'])
+
+    # including all transitions outside the window
+    stat = fr.distance_rank_window(data, 'item_index', distances, [-1, 0, 1])
+    expected = np.array([[0.125, 0.125, 0.375], [0, 1, 1], [1, 1, 0]])
+    np.testing.assert_allclose(np.mean(expected, 0), stat['rank'].to_numpy())
+
+    # excluding transitions when the prior transition was from the window
+    stat = fr.distance_rank_window(
+        data, 'item_index', distances, [-1, 0, 1], exclude_prev_window=True
+    )
+    expected = np.array([[0.125, 0.125, 0.375], [0, 1, 1]])
+    np.testing.assert_allclose(np.mean(expected, 0), stat['rank'].to_numpy())
+
+    # just calculating asymmetry
+    stat = fr.distance_rank_window_asym(data, 'item_index', distances)
+    expected = np.array([[.25, 1, -1]])
+    np.testing.assert_allclose(np.mean(expected), stat['asym'].to_numpy())
```

### Comparing `psifr-0.9.0/tests/test_maskers.py` & `psifr-0.9.2/tests/test_maskers.py`

 * *Files 25% similar despite different names*

```diff
@@ -136,23 +136,30 @@
         [[2, 3, 4, 5, 6, 7, 8], [2, 4, 5, 6, 7, 8]],
         [[2, 4, 5, 6, 7, 8], [2, 5, 6, 7, 8]],
         [[2, 5, 6, 7, 8], [2, 5, 6, 7]],
     ]
     assert steps == list(zip(output, prev, curr, poss))
 
 
-def test_windows_position():
-    """Test study position within a window."""
+@pytest.fixture()
+def window_data():
     pool = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16]
     outputs = [16, 15, 9, 1, 4, 8, 13, 14, 4, 7, 5]
-    window_lags = [-1, 0, 1]
     list_length = 16
+    return pool, outputs, list_length
 
+
+def test_windows_position(window_data):
+    """Test study position within a window."""
+    pool, outputs, list_length = window_data
+    window_lags = [-1, 0, 1]
+
+    # outputs: [16, 15, 9, 1, 4, 8, 13, 14, 4, 7, 5]
     # included: [(15, 9), (9, 1), (4, 8), (8, 13), (7, 5)]
-    # excluded: [(16, 15), (1, 4), (13, 14), (14, 4)]
+    # excluded: [(16, 15), (1, 4), (13, 14), (14, 4), (4, 7)]
     output = [2, 3, 5, 6, 10]
     prev = [[14, 15, 16], [8, 9, 10], [3, 4, 5], [7, 8, 9], [6, 7, 8]]
     curr = [9, 1, 8, 13, 5]
     poss = [
         [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13],
         [1, 2, 3, 4, 5, 6, 7, 11, 12, 13, 14],
         [2, 6, 7, 8, 10, 11, 12, 13, 14],
@@ -167,24 +174,52 @@
     for i, (a_output, a_prev, a_curr, a_poss) in enumerate(masker):
         assert a_output == output[i]
         assert a_prev.tolist() == prev[i]
         assert a_curr == curr[i]
         assert a_poss.tolist() == poss[i]
 
 
-def test_windows_position_cond_category():
+def test_windows_position_exclude_prev(window_data):
+    """Test excluding previous recalls within the window."""
+    pool, outputs, list_length = window_data
+    window_lags = [-1, 0, 1]
+
+    # outputs: [16, 15, 9, 1, 4, 8, 13, 14, 4, 7, 5]
+    # included: [(9, 1), (4, 8), (8, 13), (7, 5)]
+    # excluded: [(16, 15), (15, 9), (1, 4), (13, 14), (14, 4), (4, 7)]
+    # excluded due to previous transition: [(15, 9), (14, 4)]
+    output = [3, 5, 6, 10]
+    prev = [[8, 9, 10], [3, 4, 5], [7, 8, 9], [6, 7, 8]]
+    curr = [1, 8, 13, 5]
+    poss = [
+        [1, 2, 3, 4, 5, 6, 7, 11, 12, 13, 14],
+        [2, 6, 7, 8, 10, 11, 12, 13, 14],
+        [2, 3, 5, 6, 10, 11, 12, 13, 14],
+        [2, 3, 5, 10, 11, 12],
+    ]
+    # test the yielded values at each included output position
+    masker = maskers.windows_masker(
+        list_length, window_lags, pool, outputs, pool, outputs, exclude_prev_window=True
+    )
+    for i, (a_output, a_prev, a_curr, a_poss) in enumerate(masker):
+        assert a_output == output[i]
+        assert a_prev.tolist() == prev[i]
+        assert a_curr == curr[i]
+        assert a_poss.tolist() == poss[i]
+
+
+def test_windows_position_cond_category(window_data):
     """Test study position within a window conditional on category."""
-    pool = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16]
+    pool, outputs, list_length = window_data
     pool_category = [1, 1, 1, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2]
-    outputs = [16, 15, 9, 1, 4, 8, 13, 14, 4, 7, 5]
     outputs_category = [2, 2, 2, 1, 1, 1, 2, 2, 1, 1, 1]
     window_lags = [-1, 0, 1]
-    list_length = 16
     test = lambda x, y: x == y
 
+    # outputs: [16, 15, 9, 1, 4, 8, 13, 14, 4, 7, 5]
     # included: [(15, 9), (4, 8), (7, 5)]
     # excluded: [(16, 15), (9, 1), (1, 4), (8, 13), (13, 14), (14, 4), (4, 7)]
     output = [2, 5, 10]
     prev = [[14, 15, 16], [3, 4, 5], [6, 7, 8]]
     curr = [9, 8, 5]
     poss = [[9, 10, 11, 12, 13], [2, 6, 7, 8], [2, 3, 5]]
```

### Comparing `psifr-0.9.0/tests/test_output_stats.py` & `psifr-0.9.2/tests/test_output_stats.py`

 * *Files identical despite different names*

### Comparing `psifr-0.9.0/tests/test_pair_stats.py` & `psifr-0.9.2/tests/test_pair_stats.py`

 * *Files identical despite different names*

### Comparing `psifr-0.9.0/tests/test_plots.py` & `psifr-0.9.2/tests/test_plots.py`

 * *Files identical despite different names*

