# Comparing `tmp/remayn-1.0.2.tar.gz` & `tmp/remayn-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remayn-1.0.2.tar", last modified: Tue May 21 09:12:18 2024, max compression
+gzip compressed data, was "remayn-1.0.3.tar", last modified: Tue May 21 09:17:51 2024, max compression
```

## Comparing `remayn-1.0.2.tar` & `remayn-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:12:18.752443 remayn-1.0.2/
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1492 2024-04-25 06:08:28.000000 remayn-1.0.2/LICENSE
--rw-r--r--   0 victor   (10038) ayrna     (1001)     6054 2024-05-21 09:12:18.747036 remayn-1.0.2/PKG-INFO
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5118 2024-05-21 08:37:54.000000 remayn-1.0.2/README.md
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1068 2024-05-21 09:08:19.000000 remayn-1.0.2/pyproject.toml
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:12:18.661176 remayn-1.0.2/remayn/
--rw-r--r--   0 victor   (10038) ayrna     (1001)       35 2024-05-21 09:08:26.000000 remayn-1.0.2/remayn/__init__.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:12:18.690511 remayn-1.0.2/remayn/report/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      161 2024-05-19 11:27:24.000000 remayn-1.0.2/remayn/report/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5387 2024-05-21 08:03:44.000000 remayn-1.0.2/remayn/report/excel.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:12:18.704523 remayn-1.0.2/remayn/result/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      142 2024-05-01 12:37:43.000000 remayn-1.0.2/remayn/result/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)    18991 2024-05-19 09:56:20.000000 remayn-1.0.2/remayn/result/result.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     4773 2024-05-21 08:02:55.000000 remayn-1.0.2/remayn/result/result_data.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:12:18.718589 remayn-1.0.2/remayn/result_set/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      100 2024-05-07 11:34:45.000000 remayn-1.0.2/remayn/result_set/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)    17305 2024-05-21 08:07:09.000000 remayn-1.0.2/remayn/result_set/result_set.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5258 2024-05-21 08:05:29.000000 remayn-1.0.2/remayn/result_set/utils.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:12:18.735170 remayn-1.0.2/remayn/utils/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      246 2024-05-12 11:03:44.000000 remayn-1.0.2/remayn/utils/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1635 2024-05-12 12:47:43.000000 remayn-1.0.2/remayn/utils/dicts.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     2008 2024-05-09 10:08:48.000000 remayn-1.0.2/remayn/utils/json.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:12:18.739929 remayn-1.0.2/remayn.egg-info/
--rw-r--r--   0 victor   (10038) ayrna     (1001)     6054 2024-05-21 09:12:18.000000 remayn-1.0.2/remayn.egg-info/PKG-INFO
--rw-r--r--   0 victor   (10038) ayrna     (1001)      494 2024-05-21 09:12:18.000000 remayn-1.0.2/remayn.egg-info/SOURCES.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)        1 2024-05-21 09:12:18.000000 remayn-1.0.2/remayn.egg-info/dependency_links.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)      111 2024-05-21 09:12:18.000000 remayn-1.0.2/remayn.egg-info/requires.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)        7 2024-05-21 09:12:18.000000 remayn-1.0.2/remayn.egg-info/top_level.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-05-21 09:12:18.752961 remayn-1.0.2/setup.cfg
--rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-04-27 10:55:10.000000 remayn-1.0.2/setup.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.988904 remayn-1.0.3/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1492 2024-04-25 06:08:28.000000 remayn-1.0.3/LICENSE
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5943 2024-05-21 09:17:50.964630 remayn-1.0.3/PKG-INFO
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5007 2024-05-21 09:15:50.000000 remayn-1.0.3/README.md
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1068 2024-05-21 09:17:21.000000 remayn-1.0.3/pyproject.toml
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.607350 remayn-1.0.3/remayn/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       35 2024-05-21 09:17:29.000000 remayn-1.0.3/remayn/__init__.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.737295 remayn-1.0.3/remayn/report/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      161 2024-05-19 11:27:24.000000 remayn-1.0.3/remayn/report/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5387 2024-05-21 08:03:44.000000 remayn-1.0.3/remayn/report/excel.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.793807 remayn-1.0.3/remayn/result/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      142 2024-05-01 12:37:43.000000 remayn-1.0.3/remayn/result/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)    18991 2024-05-19 09:56:20.000000 remayn-1.0.3/remayn/result/result.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     4773 2024-05-21 08:02:55.000000 remayn-1.0.3/remayn/result/result_data.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.855765 remayn-1.0.3/remayn/result_set/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      100 2024-05-07 11:34:45.000000 remayn-1.0.3/remayn/result_set/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)    17305 2024-05-21 08:07:09.000000 remayn-1.0.3/remayn/result_set/result_set.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5258 2024-05-21 08:05:29.000000 remayn-1.0.3/remayn/result_set/utils.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.925611 remayn-1.0.3/remayn/utils/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      246 2024-05-12 11:03:44.000000 remayn-1.0.3/remayn/utils/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1635 2024-05-12 12:47:43.000000 remayn-1.0.3/remayn/utils/dicts.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     2008 2024-05-09 10:08:48.000000 remayn-1.0.3/remayn/utils/json.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.947892 remayn-1.0.3/remayn.egg-info/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5943 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/PKG-INFO
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      494 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/SOURCES.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)        1 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/dependency_links.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      111 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/requires.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)        7 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/top_level.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-05-21 09:17:50.989368 remayn-1.0.3/setup.cfg
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-04-27 10:55:10.000000 remayn-1.0.3/setup.py
```

### Comparing `remayn-1.0.2/LICENSE` & `remayn-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remayn-1.0.2/PKG-INFO` & `remayn-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remayn
-Version: 1.0.2
+Version: 1.0.3
 Summary: REsults MAde easY in pythoN
 Author-email: Víctor Manuel Vargas <vvargas@uco.es>
 Project-URL: Source, https://github.com/ayrna/remayn
 Project-URL: Documentation, https://remayn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -34,19 +34,19 @@
 | **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/dlordinal/badge/?version=latest&style=flat)](https://dlordinal.readthedocs.io/en/latest/)  |
 | **Code**  | [![!python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/charliermarsh/ruff)                     |
 
 ## Getting started
 
 ### ⚙️ Installation
 
-`remayn v0.1.0` is the last version supported by Python >=3.8.
+`remayn` is supported by Python >=3.8.
 
-The easiest way to install `remayn` is via `pip`, from this main branch of this GitHub repository:
+The easiest way to install `remayn` is via `pip`:
 
-    pip install git+https://github.com/ayrna/remayn.git@main
+    pip install remayn
 
 ### 💾 Saving the results of a experiment
 A new `Result` object can be created using the `make_result` function. Then, the `Result` can be saved to disk by simply calling the `save()` method.
 ```python
 import numpy as np
 from remayn.result import make_result
```

### Comparing `remayn-1.0.2/README.md` & `remayn-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 | **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/dlordinal/badge/?version=latest&style=flat)](https://dlordinal.readthedocs.io/en/latest/)  |
 | **Code**  | [![!python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/charliermarsh/ruff)                     |
 
 ## Getting started
 
 ### ⚙️ Installation
 
-`remayn v0.1.0` is the last version supported by Python >=3.8.
+`remayn` is supported by Python >=3.8.
 
-The easiest way to install `remayn` is via `pip`, from this main branch of this GitHub repository:
+The easiest way to install `remayn` is via `pip`:
 
-    pip install git+https://github.com/ayrna/remayn.git@main
+    pip install remayn
 
 ### 💾 Saving the results of a experiment
 A new `Result` object can be created using the `make_result` function. Then, the `Result` can be saved to disk by simply calling the `save()` method.
 ```python
 import numpy as np
 from remayn.result import make_result
```

### Comparing `remayn-1.0.2/pyproject.toml` & `remayn-1.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "toml", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "remayn"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     {name = "Víctor Manuel Vargas", email = "vvargas@uco.es"},
 ]
 description = "REsults MAde easY in pythoN"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `remayn-1.0.2/remayn/report/excel.py` & `remayn-1.0.3/remayn/report/excel.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.2/remayn/result/result.py` & `remayn-1.0.3/remayn/result/result.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.2/remayn/result/result_data.py` & `remayn-1.0.3/remayn/result/result_data.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.2/remayn/result_set/result_set.py` & `remayn-1.0.3/remayn/result_set/result_set.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.2/remayn/result_set/utils.py` & `remayn-1.0.3/remayn/result_set/utils.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.2/remayn/utils/dicts.py` & `remayn-1.0.3/remayn/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.2/remayn/utils/json.py` & `remayn-1.0.3/remayn/utils/json.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.2/remayn.egg-info/PKG-INFO` & `remayn-1.0.3/remayn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remayn
-Version: 1.0.2
+Version: 1.0.3
 Summary: REsults MAde easY in pythoN
 Author-email: Víctor Manuel Vargas <vvargas@uco.es>
 Project-URL: Source, https://github.com/ayrna/remayn
 Project-URL: Documentation, https://remayn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -34,19 +34,19 @@
 | **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/dlordinal/badge/?version=latest&style=flat)](https://dlordinal.readthedocs.io/en/latest/)  |
 | **Code**  | [![!python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/charliermarsh/ruff)                     |
 
 ## Getting started
 
 ### ⚙️ Installation
 
-`remayn v0.1.0` is the last version supported by Python >=3.8.
+`remayn` is supported by Python >=3.8.
 
-The easiest way to install `remayn` is via `pip`, from this main branch of this GitHub repository:
+The easiest way to install `remayn` is via `pip`:
 
-    pip install git+https://github.com/ayrna/remayn.git@main
+    pip install remayn
 
 ### 💾 Saving the results of a experiment
 A new `Result` object can be created using the `make_result` function. Then, the `Result` can be saved to disk by simply calling the `save()` method.
 ```python
 import numpy as np
 from remayn.result import make_result
```

