# Comparing `tmp/ridgeplot_py-0.2.7.tar.gz` & `tmp/ridgeplot_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ridgeplot_py-0.2.7.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ridgeplot_py-0.2.7.tar` & `ridgeplot_py-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-05-10 05:28:19.487476 ridgeplot_py-0.2.7/LICENSE
--rw-r--r--   0        0        0     2960 2024-05-10 05:28:19.487476 ridgeplot_py-0.2.7/README.md
--rw-r--r--   0        0        0     1465 2024-05-10 05:28:34.991564 ridgeplot_py-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       73 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/__init__.py
--rw-r--r--   0        0        0     8818 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/colors.py
--rw-r--r--   0        0        0     2168 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/dotted_heatmap.py
--rw-r--r--   0        0        0     3354 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/ridge_plot.py
--rw-r--r--   0        0        0      687 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/stats.py
--rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    63867 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/Example.ipynb
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/requirements.lock
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/colors.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/dotted_heatmap.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/ridge_plot.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/stats.md
+-rw-r--r--   0        0        0    21909 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/img/ridgeplot.png
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/__init__.py
+-rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/colors.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/dotted_heatmap.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/ridge_plot.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/stats.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/test/test_colors.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/test/test_dotted_heatmap.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/test/test_ridge_plot.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/test/test_stats.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/README.md
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/PKG-INFO
```

### Comparing `ridgeplot_py-0.2.7/LICENSE` & `ridgeplot_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.7/README.md` & `ridgeplot_py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.7/ridgeplot/colors.py` & `ridgeplot_py-0.3.0/src/ridgeplot/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from collections import OrderedDict
 from typing import Any, Dict, List, Tuple
 
 import matplotlib.axes
 import matplotlib.patches as mpatches
 from matplotlib import legend
-from matplotlib.cm import get_cmap
 from matplotlib.colors import to_hex
+from matplotlib.pyplot import get_cmap
 
 ColorPalette: Dict[str, List[str]] = dict(
     # 1. maximum
     # modified from:
     # https://sashat.me/2017/01/11/list-of-20-simple-distinct-colors/
     maximum=[
         "#f58231",
```

### Comparing `ridgeplot_py-0.2.7/ridgeplot/dotted_heatmap.py` & `ridgeplot_py-0.3.0/src/ridgeplot/dotted_heatmap.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.7/ridgeplot/ridge_plot.py` & `ridgeplot_py-0.3.0/src/ridgeplot/ridge_plot.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.7/ridgeplot/stats.py` & `ridgeplot_py-0.3.0/src/ridgeplot/stats.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.7/PKG-INFO` & `ridgeplot_py-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ridgeplot-py
-Version: 0.2.7
+Version: 0.3.0
 Summary: Plotting ridgeplots with matplotlib
-License: MIT
-Author: Douglas Wu
-Author-email: wckdouglas@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: matplotlib (>=3.8,<4.0)
-Requires-Dist: more-itertools (>=8.9.0,<9.0.0)
-Requires-Dist: numpy (>=1.21.1,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: poetry (>=1.8.3,<2.0.0)
-Requires-Dist: scipy (>=1.8.0,<2.0.0)
+Author-email: Douglas Wu <wckdouglas@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Requires-Python: >=3.9
+Requires-Dist: matplotlib>=3.8
+Requires-Dist: more-itertools>=8.9.0
+Requires-Dist: numpy>=1.21.1
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: scipy>=1.8.0
 Description-Content-Type: text/markdown
 
 # ridgeplot-py #
 
 [![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/ridgeplot-py)
 
 
@@ -93,8 +86,7 @@
 scipy may cause error and may be able to solved by the [this stackoverflow answer](https://stackoverflow.com/a/71764028):
 
 ```
 brew install openblas
 export OPENBLAS="$(brew --prefix openblas)" 
 poetry install
 ```
-
```

#### html2text {}

```diff
@@ -1,20 +1,15 @@
-Metadata-Version: 2.1 Name: ridgeplot-py Version: 0.2.7 Summary: Plotting
-ridgeplots with matplotlib License: MIT Author: Douglas Wu Author-email:
-wckdouglas@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
-(>=3.8,<4.0) Requires-Dist: more-itertools (>=8.9.0,<9.0.0) Requires-Dist:
-numpy (>=1.21.1,<2.0.0) Requires-Dist: pandas (>=2.2.2,<3.0.0) Requires-Dist:
-poetry (>=1.8.3,<2.0.0) Requires-Dist: scipy (>=1.8.0,<2.0.0) Description-
-Content-Type: text/markdown # ridgeplot-py # [![CI](https://github.com/
-wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://
-github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov]
+Metadata-Version: 2.3 Name: ridgeplot-py Version: 0.3.0 Summary: Plotting
+ridgeplots with matplotlib Author-email: Douglas Wu
+gmail.com> License-Expression: MIT License-File: LICENSE Requires-Python: >=3.9
+Requires-Dist: matplotlib>=3.8 Requires-Dist: more-itertools>=8.9.0 Requires-
+Dist: numpy>=1.21.1 Requires-Dist: pandas>=2.2.2 Requires-Dist: scipy>=1.8.0
+Description-Content-Type: text/markdown # ridgeplot-py # [![CI](https://
+github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https:
+//github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov]
 (https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/
 badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [!
 [PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://
 badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-
 forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/
 ridgeplot-py) This is a simple module for plotting [ridgeplot](https://
 clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem]
```

