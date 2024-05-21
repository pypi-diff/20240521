# Comparing `tmp/ridgeplot_py-0.3.0.tar.gz` & `tmp/ridgeplot_py-0.4.0.tar.gz`

## Comparing `ridgeplot_py-0.3.0.tar` & `ridgeplot_py-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    63867 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/Example.ipynb
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/requirements-dev.lock
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/requirements.lock
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/colors.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/dotted_heatmap.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/ridge_plot.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/docs/stats.md
--rw-r--r--   0        0        0    21909 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/img/ridgeplot.png
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/__init__.py
--rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/colors.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/dotted_heatmap.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/ridge_plot.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/src/ridgeplot/stats.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/test/test_colors.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/test/test_dotted_heatmap.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/test/test_ridge_plot.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/test/test_stats.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/LICENSE
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/README.md
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 ridgeplot_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    63867 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/Example.ipynb
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/requirements.lock
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/docs/colors.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/docs/dotted_heatmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/docs/index.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/docs/ridge_plot.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/docs/stats.md
+-rw-r--r--   0        0        0    21909 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/img/ridgeplot.png
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/src/ridgeplot/__init__.py
+-rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/src/ridgeplot/colors.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/src/ridgeplot/dotted_heatmap.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/src/ridgeplot/ridge_plot.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/src/ridgeplot/stats.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/test/test_colors.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/test/test_dotted_heatmap.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/test/test_ridge_plot.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/test/test_stats.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/README.md
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 ridgeplot_py-0.4.0/PKG-INFO
```

### Comparing `ridgeplot_py-0.3.0/Example.ipynb` & `ridgeplot_py-0.4.0/Example.ipynb`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/requirements-dev.lock` & `ridgeplot_py-0.4.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/requirements.lock` & `ridgeplot_py-0.4.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/.github/workflows/ci.yaml` & `ridgeplot_py-0.4.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/docs/index.md` & `ridgeplot_py-0.4.0/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 This is a simple module for plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem](https://www.scipy.org/about.html).
 
 Ridgeplot is a great data visualization technique to compare distributions from multiple groups at the same time, and was first introduced in 2017 as joy plot:
 
-<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I hereby propose that we call these &quot;joy plots&quot; <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/uuLGpQLAwY">https://t.co/uuLGpQLAwY</a></p>&mdash; Jenny Bryan (@JennyBryan) <a href="https://twitter.com/JennyBryan/status/856674638981550080?ref_src=twsrc%5Etfw">April 25, 2017</a></blockquote> 
+<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I hereby propose that we call these &quot;joy plots&quot; <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/uuLGpQLAwY">https://t.co/uuLGpQLAwY</a></p>&mdash; Jenny Bryan (@JennyBryan) <a href="https://twitter.com/JennyBryan/status/856674638981550080?ref_src=twsrc%5Etfw">April 25, 2017</a></blockquote>
 
 [ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with scikit-learn syntax for manipulating color annotations in a consistent way [through out manuscripts or presentations].
 
-
 # Modules
 
 1. [colors](colors.md)
 2. [ridgeplot](ridge_plot.md)
 3. [stats](stats.md)
+4. [dotted_heatmap](dotted_heatmap.md)
```

#### html2text {}

```diff
@@ -8,8 +8,9 @@
      — Jenny Bryan (@JennyBryan) _A_p_r_i_l_ _2_5_,_ _2_0_1_7
 [ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to
 produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder]
 (https://github.com/wckdouglas/ridgeplot-py/blob/
 0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with
 scikit-learn syntax for manipulating color annotations in a consistent way
 [through out manuscripts or presentations]. # Modules 1. [colors](colors.md) 2.
-[ridgeplot](ridge_plot.md) 3. [stats](stats.md)
+[ridgeplot](ridge_plot.md) 3. [stats](stats.md) 4. [dotted_heatmap]
+(dotted_heatmap.md)
```

### Comparing `ridgeplot_py-0.3.0/img/ridgeplot.png` & `ridgeplot_py-0.4.0/img/ridgeplot.png`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/src/ridgeplot/colors.py` & `ridgeplot_py-0.4.0/src/ridgeplot/colors.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/src/ridgeplot/dotted_heatmap.py` & `ridgeplot_py-0.4.0/src/ridgeplot/dotted_heatmap.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/src/ridgeplot/ridge_plot.py` & `ridgeplot_py-0.4.0/src/ridgeplot/ridge_plot.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/src/ridgeplot/stats.py` & `ridgeplot_py-0.4.0/src/ridgeplot/stats.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/test/test_colors.py` & `ridgeplot_py-0.4.0/test/test_colors.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/test/test_ridge_plot.py` & `ridgeplot_py-0.4.0/test/test_ridge_plot.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/test/test_stats.py` & `ridgeplot_py-0.4.0/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/LICENSE` & `ridgeplot_py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/README.md` & `ridgeplot_py-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/pyproject.toml` & `ridgeplot_py-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.3.0/PKG-INFO` & `ridgeplot_py-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ridgeplot-py
-Version: 0.3.0
+Version: 0.4.0
 Summary: Plotting ridgeplots with matplotlib
 Author-email: Douglas Wu <wckdouglas@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: more-itertools>=8.9.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: ridgeplot-py Version: 0.3.0 Summary: Plotting
+Metadata-Version: 2.3 Name: ridgeplot-py Version: 0.4.0 Summary: Plotting
 ridgeplots with matplotlib Author-email: Douglas Wu
 gmail.com> License-Expression: MIT License-File: LICENSE Requires-Python: >=3.9
 Requires-Dist: matplotlib>=3.8 Requires-Dist: more-itertools>=8.9.0 Requires-
 Dist: numpy>=1.21.1 Requires-Dist: pandas>=2.2.2 Requires-Dist: scipy>=1.8.0
 Description-Content-Type: text/markdown # ridgeplot-py # [![CI](https://
 github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https:
 //github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov]
```

