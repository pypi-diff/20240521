# Comparing `tmp/py50-1.0.5.tar.gz` & `tmp/py50-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py50-1.0.5.tar", max compression
+gzip compressed data, was "py50-1.0.6.tar", max compression
```

## Comparing `py50-1.0.5.tar` & `py50-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.5/LICENSE
--rw-r--r--   0        0        0     4542 2024-05-17 01:24:02.026348 py50-1.0.5/README_pypi.md
--rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.5/py50/.DS_Store
--rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.5/py50/__init__.py
--rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.5/py50/calculator.py
--rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.5/py50/plot_settings.py
--rw-r--r--   0        0        0    43460 2024-04-30 01:26:56.191290 py50-1.0.5/py50/plotcurve.py
--rw-r--r--   0        0        0    94182 2024-05-17 16:34:10.398794 py50-1.0.5/py50/stats.py
--rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.5/py50/utils.py
--rw-r--r--   0        0        0      591 2024-05-20 03:57:29.279193 py50-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 py50-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.6/LICENSE
+-rw-r--r--   0        0        0     4542 2024-05-17 01:24:02.026348 py50-1.0.6/README_pypi.md
+-rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.6/py50/.DS_Store
+-rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.6/py50/__init__.py
+-rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.6/py50/calculator.py
+-rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.6/py50/plot_settings.py
+-rw-r--r--   0        0        0    43460 2024-04-30 01:26:56.191290 py50-1.0.6/py50/plotcurve.py
+-rw-r--r--   0        0        0    94182 2024-05-17 16:34:10.398794 py50-1.0.6/py50/stats.py
+-rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.6/py50/utils.py
+-rw-r--r--   0        0        0      592 2024-05-20 04:00:54.078586 py50-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5451 1970-01-01 00:00:00.000000 py50-1.0.6/PKG-INFO
```

### Comparing `py50-1.0.5/LICENSE` & `py50-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py50-1.0.5/README_pypi.md` & `py50-1.0.6/README_pypi.md`

 * *Files identical despite different names*

### Comparing `py50-1.0.5/py50/.DS_Store` & `py50-1.0.6/py50/.DS_Store`

 * *Files identical despite different names*

### Comparing `py50-1.0.5/py50/calculator.py` & `py50-1.0.6/py50/calculator.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.5/py50/plot_settings.py` & `py50-1.0.6/py50/plot_settings.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.5/py50/plotcurve.py` & `py50-1.0.6/py50/plotcurve.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.5/py50/stats.py` & `py50-1.0.6/py50/stats.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.5/py50/utils.py` & `py50-1.0.6/py50/utils.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.5/pyproject.toml` & `py50-1.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "py50"
-version = "1.0.5"
+version = "1.0.6"
 description = "Generate Dose-Response Curves"
 documentation = "https://py50.readthedocs.io/en/latest/"
 authors = ["Tony Eight Lin <tonyelin@tmu.edu.tw>"]
 license = "GPL-3.0"
 readme = "README_pypi.md"
 packages = [{ include = "py50"}]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
 pandas = "==1.5.0"
 numpy = ">=1.26.2"
 matplotlib = ">=3.8.1"
 scipy = ">=1.11.3"
-seaborn = "<0.13.0"
+seaborn = "<=0.12.2"
 scikit-posthocs = ">=0.7.0"
 pingouin = ">=0.5.4"
 statannotations = ">=0.6.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py50-1.0.5/PKG-INFO` & `py50-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py50
-Version: 1.0.5
+Version: 1.0.6
 Summary: Generate Dose-Response Curves
 License: GPL-3.0
 Author: Tony Eight Lin
 Author-email: tonyelin@tmu.edu.tw
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.1)
 Requires-Dist: numpy (>=1.26.2)
 Requires-Dist: pandas (==1.5.0)
 Requires-Dist: pingouin (>=0.5.4)
 Requires-Dist: scikit-posthocs (>=0.7.0)
 Requires-Dist: scipy (>=1.11.3)
-Requires-Dist: seaborn (<0.13.0)
+Requires-Dist: seaborn (<=0.12.2)
 Requires-Dist: statannotations (>=0.6.0)
 Project-URL: Documentation, https://py50.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # py50: Generate Dose-Response Curves
 
 ![Static Badge](https://img.shields.io/badge/py50_v1.0.4-13406E)
```

