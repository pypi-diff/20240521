# Comparing `tmp/pyrheed-1.0.5.tar.gz` & `tmp/pyrheed-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrheed-1.0.5.tar", last modified: Tue May 21 04:52:46 2024, max compression
+gzip compressed data, was "pyrheed-1.0.6.tar", last modified: Tue May 21 05:06:29 2024, max compression
```

## Comparing `pyrheed-1.0.5.tar` & `pyrheed-1.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:52:46.562806 pyrheed-1.0.5/
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1059 2024-05-19 00:11:40.000000 pyrheed-1.0.5/LICENSE
--rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 04:52:46.562401 pyrheed-1.0.5/PKG-INFO
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7352 2024-05-21 03:40:07.000000 pyrheed-1.0.5/README.md
--rw-r--r--   0 yuuxiang   (504) staff       (20)      951 2024-05-21 04:52:20.000000 pyrheed-1.0.5/pyproject.toml
--rw-r--r--   0 yuuxiang   (504) staff       (20)       38 2024-05-21 04:52:46.562867 pyrheed-1.0.5/setup.cfg
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:52:46.551449 pyrheed-1.0.5/src/
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:52:46.562023 pyrheed-1.0.5/src/PyRHEED.egg-info/
--rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 04:52:46.000000 pyrheed-1.0.5/src/PyRHEED.egg-info/PKG-INFO
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1036 2024-05-21 04:52:46.000000 pyrheed-1.0.5/src/PyRHEED.egg-info/SOURCES.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)        1 2024-05-21 04:52:46.000000 pyrheed-1.0.5/src/PyRHEED.egg-info/dependency_links.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)      305 2024-05-21 04:52:46.000000 pyrheed-1.0.5/src/PyRHEED.egg-info/requires.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)        8 2024-05-21 04:52:46.000000 pyrheed-1.0.5/src/PyRHEED.egg-info/top_level.txt
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:52:46.561333 pyrheed-1.0.5/src/pyrheed/
--rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:49:27.000000 pyrheed-1.0.5/src/pyrheed/__init__.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     9481 2024-05-21 04:51:43.000000 pyrheed-1.0.5/src/pyrheed/__main__.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     5658 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/bar_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7381 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/boundary_statistics.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    44251 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/broadening.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1725 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/browser.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    27635 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/canvas.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2833 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/configuration.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2261 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/cursor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    36260 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/generate_report.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    65698 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/gmm.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    22311 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/graph_3D_surface.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    27092 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/kikuchi.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    17629 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/manual_fit.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    50948 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/my_widgets.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    18518 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/plot_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    12078 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/preference.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)   102526 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/process.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     3481 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/process_monitor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    17710 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/profile_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    15838 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/properties.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    33550 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/reciprocal_space_mapping.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2508 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/regularization.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    24229 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/scenario.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7759 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/scipy_test.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)   147797 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/simulate_RHEED.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    21776 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/statistical_factor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7969 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/translational_antiphase_domain.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    47928 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/window.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     4087 2024-05-21 03:38:01.000000 pyrheed-1.0.5/src/pyrheed/write_scenario.py
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:06:29.349267 pyrheed-1.0.6/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1059 2024-05-19 00:11:40.000000 pyrheed-1.0.6/LICENSE
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 05:06:29.348957 pyrheed-1.0.6/PKG-INFO
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7352 2024-05-21 03:40:07.000000 pyrheed-1.0.6/README.md
+-rw-r--r--   0 yuuxiang   (504) staff       (20)      951 2024-05-21 05:06:23.000000 pyrheed-1.0.6/pyproject.toml
+-rw-r--r--   0 yuuxiang   (504) staff       (20)       38 2024-05-21 05:06:29.349314 pyrheed-1.0.6/setup.cfg
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:06:29.337390 pyrheed-1.0.6/src/
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:06:29.348585 pyrheed-1.0.6/src/PyRHEED.egg-info/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 05:06:29.000000 pyrheed-1.0.6/src/PyRHEED.egg-info/PKG-INFO
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1036 2024-05-21 05:06:29.000000 pyrheed-1.0.6/src/PyRHEED.egg-info/SOURCES.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        1 2024-05-21 05:06:29.000000 pyrheed-1.0.6/src/PyRHEED.egg-info/dependency_links.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)      305 2024-05-21 05:06:29.000000 pyrheed-1.0.6/src/PyRHEED.egg-info/requires.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        8 2024-05-21 05:06:29.000000 pyrheed-1.0.6/src/PyRHEED.egg-info/top_level.txt
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:06:29.347961 pyrheed-1.0.6/src/pyrheed/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:49:27.000000 pyrheed-1.0.6/src/pyrheed/__init__.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     9481 2024-05-21 04:51:43.000000 pyrheed-1.0.6/src/pyrheed/__main__.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     5666 2024-05-21 04:53:36.000000 pyrheed-1.0.6/src/pyrheed/bar_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7381 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/boundary_statistics.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    44314 2024-05-21 04:55:03.000000 pyrheed-1.0.6/src/pyrheed/broadening.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1725 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/browser.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    27635 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/canvas.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2833 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/configuration.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2261 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/cursor.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    36281 2024-05-21 04:55:45.000000 pyrheed-1.0.6/src/pyrheed/generate_report.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    65774 2024-05-21 04:58:41.000000 pyrheed-1.0.6/src/pyrheed/gmm.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    22311 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/graph_3D_surface.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    27121 2024-05-21 04:59:20.000000 pyrheed-1.0.6/src/pyrheed/kikuchi.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    17671 2024-05-21 04:59:42.000000 pyrheed-1.0.6/src/pyrheed/manual_fit.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    50948 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/my_widgets.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    18518 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/plot_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    12078 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/preference.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)   102534 2024-05-21 05:00:41.000000 pyrheed-1.0.6/src/pyrheed/process.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     3481 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/process_monitor.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    17718 2024-05-21 05:00:51.000000 pyrheed-1.0.6/src/pyrheed/profile_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    15838 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/properties.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    33571 2024-05-21 05:01:10.000000 pyrheed-1.0.6/src/pyrheed/reciprocal_space_mapping.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2508 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/regularization.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    24148 2024-05-21 05:02:29.000000 pyrheed-1.0.6/src/pyrheed/scenario.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7759 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/scipy_test.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)   147826 2024-05-21 05:03:10.000000 pyrheed-1.0.6/src/pyrheed/simulate_RHEED.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    21784 2024-05-21 05:03:18.000000 pyrheed-1.0.6/src/pyrheed/statistical_factor.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7998 2024-05-21 05:03:34.000000 pyrheed-1.0.6/src/pyrheed/translational_antiphase_domain.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    47989 2024-05-21 05:04:15.000000 pyrheed-1.0.6/src/pyrheed/window.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     4087 2024-05-21 03:38:01.000000 pyrheed-1.0.6/src/pyrheed/write_scenario.py
```

### Comparing `pyrheed-1.0.5/LICENSE` & `pyrheed-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/PKG-INFO` & `pyrheed-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyRHEED
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package for RHEED data analysis and simulation
 Author-email: Yu Xiang <yux1991@gmail.com>
 Project-URL: Homepage, https://github.com/yux1991/PyRHEED
 Project-URL: Issues, https://github.com/yux1991/PyRHEED/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrheed-1.0.5/README.md` & `pyrheed-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/pyproject.toml` & `pyrheed-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyRHEED"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Yu Xiang", email="yux1991@gmail.com" },
 ]
 description = "A python package for RHEED data analysis and simulation"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `pyrheed-1.0.5/src/PyRHEED.egg-info/PKG-INFO` & `pyrheed-1.0.6/src/PyRHEED.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyRHEED
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package for RHEED data analysis and simulation
 Author-email: Yu Xiang <yux1991@gmail.com>
 Project-URL: Homepage, https://github.com/yux1991/PyRHEED
 Project-URL: Issues, https://github.com/yux1991/PyRHEED/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrheed-1.0.5/src/PyRHEED.egg-info/SOURCES.txt` & `pyrheed-1.0.6/src/PyRHEED.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/__main__.py` & `pyrheed-1.0.6/src/pyrheed/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/bar_chart.py` & `pyrheed-1.0.6/src/pyrheed/bar_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from process import Image
+from pyrheed.process import Image
 from PyQt6 import QtCore, QtWidgets, QtGui, QtCharts, QtSvg
 import numpy as np
 
 class BarChart(QtCharts.QChartView):
     CHART_IS_PRESENT = False
     FONTS_CHANGED = QtCore.pyqtSignal(str,int)
```

### Comparing `pyrheed-1.0.5/src/pyrheed/boundary_statistics.py` & `pyrheed-1.0.6/src/pyrheed/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/broadening.py` & `pyrheed-1.0.6/src/pyrheed/broadening.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from my_widgets import LabelSlider
-from process import Image, FitFunctions, FitBroadening
-from process_monitor import Monitor
+from pyrheed.my_widgets import LabelSlider
+from pyrheed.process import Image, FitFunctions, FitBroadening
+from pyrheed.process_monitor import Monitor
 from PyQt6 import QtCore, QtWidgets, QtGui, QtCharts
 from sys import getsizeof
 import configparser
-import generate_report
+from pyrheed import generate_report
+from pyrheed import manual_fit
+from pyrheed import profile_chart
 import glob
-import manual_fit
 import numpy as np
 import os
-import profile_chart
 
 class Window(QtCore.QObject):
 
     #Public Signals
     STATUS_REQUESTED = QtCore.pyqtSignal()
     PROGRESS_ADVANCE = QtCore.pyqtSignal(int,int,int)
     PROGRESS_END = QtCore.pyqtSignal()
```

### Comparing `pyrheed-1.0.5/src/pyrheed/browser.py` & `pyrheed-1.0.6/src/pyrheed/browser.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/canvas.py` & `pyrheed-1.0.6/src/pyrheed/canvas.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/configuration.py` & `pyrheed-1.0.6/src/pyrheed/configuration.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/cursor.py` & `pyrheed-1.0.6/src/pyrheed/cursor.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/generate_report.py` & `pyrheed-1.0.6/src/pyrheed/generate_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from my_widgets import ColorPicker, DoubleSlider
+from pyrheed.my_widgets import ColorPicker, DoubleSlider
 from PyQt6 import QtCore, QtWidgets, QtGui, QtCharts
 import configparser
 import matplotlib.pyplot as plt
 import numpy as np
 import os
-import plot_chart
+from pyrheed import plot_chart
 from scipy.stats import linregress as lrg
 
 class Window(QtCore.QObject):
 
     STATUS_REQUESTED = QtCore.pyqtSignal()
     POLAR_I_REQUESTED = QtCore.pyqtSignal()
     POLAR_F_REQUESTED = QtCore.pyqtSignal()
```

### Comparing `pyrheed-1.0.5/src/pyrheed/gmm.py` & `pyrheed-1.0.6/src/pyrheed/gmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from my_widgets import LabelSlider
-from process import Image, FitFunctions, FitBroadening
-from process_monitor import Monitor
+from pyrheed.my_widgets import LabelSlider
+from pyrheed.process import Image, FitFunctions, FitBroadening
+from pyrheed.process_monitor import Monitor
 from PyQt6 import QtCore, QtWidgets, QtGui, QtCharts
 from sys import getsizeof
 from sklearn.mixture import BayesianGaussianMixture
 from sklearn.mixture._gaussian_mixture import _estimate_gaussian_parameters
 from sklearn.mixture._gaussian_mixture import _compute_precision_cholesky
 import configparser
-import generate_report
 import glob
-import manual_fit
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import matplotlib.colors as mcolors
 import numpy as np
 import numbers
 import os
 import time
 import sys
-import profile_chart
-import bar_chart
+from pyrheed import profile_chart
+from pyrheed import bar_chart
+from pyrheed import generate_report
+from pyrheed import manual_fit
 import pandas
 from scipy.stats import rv_discrete
 
 class Window(QtCore.QObject):
 
     #Public Signals
     STATUS_REQUESTED = QtCore.pyqtSignal()
```

### Comparing `pyrheed-1.0.5/src/pyrheed/graph_3D_surface.py` & `pyrheed-1.0.6/src/pyrheed/graph_3D_surface.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/kikuchi.py` & `pyrheed-1.0.6/src/pyrheed/kikuchi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import configparser
 import numpy as np
 from numpy.lib import scimath
-from process import Diffraction
-import profile_chart
+from pyrheed.process import Diffraction
+from pyrheed import profile_chart
 from pymatgen.io.cif import CifParser
 from PyQt6 import QtCore, QtWidgets, QtGui, QtCharts
-from my_widgets import LabelMultipleLineEdit, LabelLineEdit, ColorPicker
+from pyrheed.my_widgets import LabelMultipleLineEdit, LabelLineEdit, ColorPicker
 import sys
 import os
 import itertools
 
 class Window(QtCore.QObject):
     STOP_KIKUCHI_WORKER = QtCore.pyqtSignal()
     FONTS_CHANGED = QtCore.pyqtSignal(str,int)
```

### Comparing `pyrheed-1.0.5/src/pyrheed/manual_fit.py` & `pyrheed-1.0.6/src/pyrheed/manual_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from my_widgets import VerticalLabelSlider
-from process import Image, FitFunctions
+from pyrheed.my_widgets import VerticalLabelSlider
+from pyrheed.process import Image, FitFunctions
 from PyQt6 import QtCore, QtWidgets, QtGui, QtCharts
 import configparser
 import glob
 import numpy as np
 import os
-import profile_chart
-import my_widgets
+from pyrheed import profile_chart
+from pyrheed import my_widgets
 
 class Window(QtCore.QObject):
 
     STATUS_REQUESTED = QtCore.pyqtSignal()
     FIT_SATISFIED = QtCore.pyqtSignal(list)
     COLOR = ['magenta','cyan','darkCyan','darkMagenta','red','darkRed','blue','darkBlue','darkGray','green','darkGreen','darkYellow','yellow','black']
```

### Comparing `pyrheed-1.0.5/src/pyrheed/my_widgets.py` & `pyrheed-1.0.6/src/pyrheed/my_widgets.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/plot_chart.py` & `pyrheed-1.0.6/src/pyrheed/plot_chart.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/preference.py` & `pyrheed-1.0.6/src/pyrheed/preference.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/process.py` & `pyrheed-1.0.6/src/pyrheed/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import time
 from astropy.modeling.models import Voigt1D
 from io import StringIO
 from lxml import etree as ET
 from math import pi as Pi
 from matplotlib.patches import Polygon as matPolygon
 from matplotlib.collections import PatchCollection
-from process_monitor import Monitor
+from pyrheed.process_monitor import Monitor
 try:
     import pycuda.compiler as comp
     import pycuda.driver as drv
     CUDA_EXIST = True
 except:
     CUDA_EXIST = False
 from pymatgen.io.cif import CifParser
```

### Comparing `pyrheed-1.0.5/src/pyrheed/process_monitor.py` & `pyrheed-1.0.6/src/pyrheed/process_monitor.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/profile_chart.py` & `pyrheed-1.0.6/src/pyrheed/profile_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from process import Image
+from pyrheed.process import Image
 from PyQt6 import QtCore, QtWidgets, QtGui, QtCharts, QtSvg
 import numpy as np
 
 class ProfileChart(QtCharts.QChartView):
 
     CHART_MOUSE_MOVEMENT = QtCore.pyqtSignal(QtCore.QPointF,str)
     CHART_MOUSE_LEAVE = QtCore.pyqtSignal()
```

### Comparing `pyrheed-1.0.5/src/pyrheed/properties.py` & `pyrheed-1.0.6/src/pyrheed/properties.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/reciprocal_space_mapping.py` & `pyrheed-1.0.6/src/pyrheed/reciprocal_space_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from process import Image, Convertor, ReciprocalSpaceMap
+from pyrheed.process import Image, Convertor, ReciprocalSpaceMap
 from PyQt6 import QtCore, QtWidgets, QtGui
 import configparser
 import os
-import profile_chart
+from pyrheed import profile_chart
 
 class Window(QtCore.QObject):
     #Public Signals
     STATUS_REQUESTED = QtCore.pyqtSignal()
     PROGRESS_ADVANCE = QtCore.pyqtSignal(int,int,int)
     PROGRESS_END = QtCore.pyqtSignal()
     SHOW_3D_GRAPH = QtCore.pyqtSignal(str)
```

### Comparing `pyrheed-1.0.5/src/pyrheed/regularization.py` & `pyrheed-1.0.6/src/pyrheed/regularization.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/scenario.py` & `pyrheed-1.0.6/src/pyrheed/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import broadening, generate_report, main, process, reciprocal_space_mapping, simulate_RHEED, translational_antiphase_domain
+from pyrheed import simulate_RHEED
 from PyQt6 import QtCore, QtGui, QtWidgets, QtDataVisualization
-from my_widgets import IndexedPushButtonWithTag, StartEndStep
+from pyrheed.my_widgets import IndexedPushButtonWithTag, StartEndStep
 import configparser
 import matplotlib.pyplot as plt
 import shutil
 import sys
 import os
 
 class Window(QtWidgets.QWidget):
```

### Comparing `pyrheed-1.0.5/src/pyrheed/scipy_test.py` & `pyrheed-1.0.6/src/pyrheed/scipy_test.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.5/src/pyrheed/simulate_RHEED.py` & `pyrheed-1.0.6/src/pyrheed/simulate_RHEED.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from PyQt6 import QtCore, QtGui, QtWidgets, QtDataVisualization
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 from matplotlib.collections import LineCollection
-from my_widgets import LabelLineEdit, IndexedComboBox, LockableDoubleSlider, LabelSlider, LabelSpinBox, InfoBoard, IndexedPushButton, DynamicalColorMap, IndexedColorPicker
-from process import Convertor, DiffractionPattern, TAPD_Simulation, TAPD_model
+from pyrheed.my_widgets import LabelLineEdit, IndexedComboBox, LockableDoubleSlider, LabelSlider, LabelSpinBox, InfoBoard, IndexedPushButton, DynamicalColorMap, IndexedColorPicker
+from pyrheed.process import Convertor, DiffractionPattern, TAPD_Simulation, TAPD_model
 from pymatgen.io.cif import CifParser
 from pymatgen.core import structure as pgStructure
 from pymatgen.core.operations import SymmOp
 from pymatgen.core.lattice import Lattice
-import browser
+from pyrheed import browser
 import itertools
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import numpy as np
 import pandas as pd
 import os
```

### Comparing `pyrheed-1.0.5/src/pyrheed/statistical_factor.py` & `pyrheed-1.0.6/src/pyrheed/statistical_factor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PyQt6 import QtCore, QtGui, QtWidgets, QtDataVisualization
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 from matplotlib import ticker, cm, colors
-from my_widgets import LabelSlider
+from pyrheed.my_widgets import LabelSlider
 import matplotlib.pyplot as plt
 import numpy as np
 import sys
 
 class Window(QtWidgets.QWidget):
     SHOW_2D_CONTOUR_SIGNAL = QtCore.pyqtSignal(list,float,float,float,float,str,int,str)
     FONTS_CHANGED = QtCore.pyqtSignal(str,int)
```

### Comparing `pyrheed-1.0.5/src/pyrheed/translational_antiphase_domain.py` & `pyrheed-1.0.6/src/pyrheed/translational_antiphase_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PyQt6 import QtCore, QtWidgets
-from my_widgets import LabelSlider
-from process import FitFunctions
+from pyrheed.my_widgets import LabelSlider
+from pyrheed.process import FitFunctions
 import matplotlib.pyplot as plt
 import numpy as np
-import plot_chart
+from pyrheed import plot_chart
 import sys
 
 class Window(QtCore.QObject):
 
     REFRESH_PLOT = QtCore.pyqtSignal(np.ndarray,np.ndarray,str,str,int,str,bool,dict)
 
     def __init__(self):
```

### Comparing `pyrheed-1.0.5/src/pyrheed/window.py` & `pyrheed-1.0.6/src/pyrheed/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from process import Image
+from pyrheed.process import Image
 from PyQt6 import QtCore, QtGui, QtWidgets
-import browser
-import canvas
 import configparser
-import cursor
 import numpy as np
 import os
-import profile_chart
-import properties
-import time
+from pyrheed import browser
+from pyrheed import canvas
+from pyrheed import cursor
+from pyrheed import profile_chart
+from pyrheed import properties
 
 class Window(QtWidgets.QMainWindow):
 
     #Public Signals
     FILE_OPENED = QtCore.pyqtSignal(str)
     IMG_CREATED = QtCore.pyqtSignal(np.ndarray)
     SCALE_FACTOR_CHANGED = QtCore.pyqtSignal(float)
```

### Comparing `pyrheed-1.0.5/src/pyrheed/write_scenario.py` & `pyrheed-1.0.6/src/pyrheed/write_scenario.py`

 * *Files identical despite different names*

