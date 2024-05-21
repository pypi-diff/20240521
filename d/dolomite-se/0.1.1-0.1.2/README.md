# Comparing `tmp/dolomite-se-0.1.1.tar.gz` & `tmp/dolomite_se-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolomite-se-0.1.1.tar", last modified: Fri Feb  9 16:42:44 2024, max compression
+gzip compressed data, was "dolomite_se-0.1.2.tar", last modified: Tue May 21 19:18:30 2024, max compression
```

## Comparing `dolomite-se-0.1.1.tar` & `dolomite_se-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.619727 dolomite-se-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.607727 dolomite-se-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.611727 dolomite-se-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-02-09 16:42:44.619727 dolomite-se-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.615727 dolomite-se-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.615727 dolomite-se-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-09 16:42:44.619727 dolomite-se-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.607727 dolomite-se-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.615727 dolomite-se-0.1.1/src/dolomite_se/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/src/dolomite_se/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/src/dolomite_se/read_ranged_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/src/dolomite_se/read_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/src/dolomite_se/save_ranged_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/src/dolomite_se/save_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/src/dolomite_se/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.615727 dolomite-se-0.1.1/src/dolomite_se.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-02-09 16:42:44.000000 dolomite-se-0.1.1/src/dolomite_se.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-09 16:42:44.000000 dolomite-se-0.1.1/src/dolomite_se.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:42:44.000000 dolomite-se-0.1.1/src/dolomite_se.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:42:44.000000 dolomite-se-0.1.1/src/dolomite_se.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-09 16:42:44.000000 dolomite-se-0.1.1/src/dolomite_se.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-09 16:42:44.000000 dolomite-se-0.1.1/src/dolomite_se.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.615727 dolomite-se-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/tests/test_range_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/tests/test_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-09 16:41:49.000000 dolomite-se-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.723629 dolomite_se-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.715629 dolomite_se-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.719629 dolomite_se-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-21 19:18:30.723629 dolomite_se-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.719629 dolomite_se-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.719629 dolomite_se-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-21 19:18:30.723629 dolomite_se-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.715629 dolomite_se-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.719629 dolomite_se-0.1.2/src/dolomite_se/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/src/dolomite_se/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/src/dolomite_se/read_ranged_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/src/dolomite_se/read_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/src/dolomite_se/save_ranged_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/src/dolomite_se/save_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/src/dolomite_se/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.723629 dolomite_se-0.1.2/src/dolomite_se.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-21 19:18:30.000000 dolomite_se-0.1.2/src/dolomite_se.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-21 19:18:30.000000 dolomite_se-0.1.2/src/dolomite_se.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:18:30.000000 dolomite_se-0.1.2/src/dolomite_se.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:18:30.000000 dolomite_se-0.1.2/src/dolomite_se.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 19:18:30.000000 dolomite_se-0.1.2/src/dolomite_se.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 19:18:30.000000 dolomite_se-0.1.2/src/dolomite_se.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:18:30.723629 dolomite_se-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/tests/test_range_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/tests/test_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-21 19:17:29.000000 dolomite_se-0.1.2/tox.ini
```

### Comparing `dolomite-se-0.1.1/.coveragerc` & `dolomite_se-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/.github/workflows/pypi-publish.yml` & `dolomite_se-0.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/.github/workflows/pypi-test.yml` & `dolomite_se-0.1.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/.gitignore` & `dolomite_se-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/.readthedocs.yml` & `dolomite_se-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/CONTRIBUTING.md` & `dolomite_se-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/LICENSE.txt` & `dolomite_se-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/PKG-INFO` & `dolomite_se-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dolomite-se
-Version: 0.1.1
+Version: 0.1.2
 Summary: Save and load summarized experiments in the dolomite framework!
 Home-page: https://github.com/ArtifactDB/dolomite-se
 Author: LTLA
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-se
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: dolomite-base>=0.2.0
-Requires-Dist: dolomite-matrix>=0.1.0
-Requires-Dist: dolomite-ranges>=0.1.0
-Requires-Dist: summarizedexperiment<0.5.0,>=0.4.2
+Requires-Dist: dolomite-base>=0.2.3
+Requires-Dist: dolomite-matrix>=0.2.1
+Requires-Dist: dolomite-ranges>=0.1.3
+Requires-Dist: summarizedexperiment>=0.4.4
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: numpy; extra == "testing"
 
 <!-- These are examples of badges you might want to add to your README:
```

### Comparing `dolomite-se-0.1.1/README.md` & `dolomite_se-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/docs/Makefile` & `dolomite_se-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/docs/conf.py` & `dolomite_se-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/docs/index.md` & `dolomite_se-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/setup.cfg` & `dolomite_se-0.1.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	dolomite-base>=0.2.0
-	dolomite-matrix>=0.1.0
-	dolomite-ranges>=0.1.0
-	summarizedexperiment>=0.4.2,<0.5.0
+	dolomite-base>=0.2.3
+	dolomite-matrix>=0.2.1
+	dolomite-ranges>=0.1.3
+	summarizedexperiment>=0.4.4
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `dolomite-se-0.1.1/setup.py` & `dolomite_se-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/src/dolomite_se/__init__.py` & `dolomite_se-0.1.2/src/dolomite_se/__init__.py`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/src/dolomite_se/read_ranged_summarized_experiment.py` & `dolomite_se-0.1.2/src/dolomite_se/read_ranged_summarized_experiment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
 
 import dolomite_base as dl
 from dolomite_base.read_object import read_object_registry
 from summarizedexperiment import RangedSummarizedExperiment
 
-from .utils import read_common_se_props
-
-read_object_registry[
-    "ranged_summarized_experiment"
-] = "dolomite_se.read_ranged_summarized_experiment"
+read_object_registry["ranged_summarized_experiment"] = (
+    "dolomite_se.read_ranged_summarized_experiment"
+)
 
 
 def read_ranged_summarized_experiment(
     path: str, metadata: dict, **kwargs
 ) -> RangedSummarizedExperiment:
     """Load a
     :py:class:`~summarizedexperiment.RangedSummarizedExperiment.RangedSummarizedExperiment`
@@ -32,27 +30,23 @@
             Further arguments, ignored.
 
     Returns:
         A
         :py:class:`~summarizedexperiment.RangedSummarizedExperiment.RangedSummarizedExperiment`
         with file-backed arrays in the assays.
     """
-
-    _row_data, _column_data, _assays = read_common_se_props(path)
+    metadata["type"] = "summarized_experiment"
+    se = dl.alt_read_object(path, metadata=metadata, **kwargs)
 
     rse = RangedSummarizedExperiment(
-        assays=_assays,
-        row_data=_row_data,
-        column_data=_column_data,
+        assays=se.get_assays(),
+        row_data=se.get_row_data(),
+        column_data=se.get_column_data(),
+        metadata=se.get_metadata(),
     )
 
-    _meta_path = os.path.join(path, "other_data")
-    if os.path.exists(_meta_path):
-        _meta = dl.read_object(_meta_path)
-        rse = rse.set_metadata(_meta.as_dict())
-
     _ranges_path = os.path.join(path, "row_ranges")
     if os.path.exists(_ranges_path):
-        _ranges = dl.read_object(_ranges_path)
+        _ranges = dl.alt_read_object(_ranges_path, **kwargs)
         rse = rse.set_row_ranges(_ranges)
 
     return rse
```

### Comparing `dolomite-se-0.1.1/src/dolomite_se/read_summarized_experiment.py` & `dolomite_se-0.1.2/src/dolomite_se/read_summarized_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,11 +39,11 @@
 
     se = SummarizedExperiment(
         assays=_assays, row_data=_row_data, column_data=_column_data
     )
 
     _meta_path = os.path.join(path, "other_data")
     if os.path.exists(_meta_path):
-        _meta = dl.read_object(_meta_path)
+        _meta = dl.alt_read_object(_meta_path, **kwargs)
         se = se.set_metadata(_meta.as_dict())
 
     return se
```

### Comparing `dolomite-se-0.1.1/src/dolomite_se/save_ranged_summarized_experiment.py` & `dolomite_se-0.1.2/src/dolomite_se/save_ranged_summarized_experiment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import dolomite_base as dl
-from summarizedexperiment import RangedSummarizedExperiment
+from summarizedexperiment import RangedSummarizedExperiment, SummarizedExperiment
 
-from .utils import save_common_se_props
+# from .utils import save_common_se_props
 
 
 @dl.save_object.register
 @dl.validate_saves
 def save_ranged_summarized_experiment(
     x: RangedSummarizedExperiment,
     path: str,
@@ -36,34 +36,36 @@
             assays.
 
         kwargs: Further arguments, ignored.
 
     Returns:
         ``x`` is saved to path.
     """
-    os.mkdir(path)
 
     if data_frame_args is None:
         data_frame_args = {}
 
     if assay_args is None:
         assay_args = {}
 
-    _se_meta = f"{list(x.shape)}"
-
-    with open(os.path.join(path, "OBJECT"), "w", encoding="utf-8") as handle:
-        handle.write(
-            '{ "type": "ranged_summarized_experiment", "ranged_summarized_experiment": { "version": "1.0" },'
-            + '"summarized_experiment": {"version": "1.0", "dimensions": '
-            + _se_meta
-            + " } }"
-        )
-
-    save_common_se_props(
-        x, path, data_frame_args=data_frame_args, assay_args=assay_args
+    # convert to SE
+    _se = SummarizedExperiment(
+        assays=x.get_assays(),
+        row_data=x.get_row_data(),
+        column_data=x.get_column_data(),
+        metadata=x.get_metadata(),
+    )
+    dl.alt_save_object(
+        _se, path, data_frame_args=data_frame_args, assay_args=assay_args, **kwargs
     )
 
+    # save row_ranges
     _ranges = x.get_row_ranges()
     if _ranges is not None:
-        dl.save_object(_ranges, path=os.path.join(path, "row_ranges"))
+        dl.alt_save_object(_ranges, path=os.path.join(path, "row_ranges"), **kwargs)
+
+    # Modify OBJECT
+    _info = dl.read_object_file(path)
+    _info["ranged_summarized_experiment"] = {"version": "1.0"}
+    dl.save_object_file(path, "ranged_summarized_experiment", _info)
 
     return
```

### Comparing `dolomite-se-0.1.1/src/dolomite_se/save_summarized_experiment.py` & `dolomite_se-0.1.2/src/dolomite_se/save_summarized_experiment.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,20 +44,12 @@
 
     if data_frame_args is None:
         data_frame_args = {}
 
     if assay_args is None:
         assay_args = {}
 
-    _se_meta = f"{list(x.shape)}"
-    with open(os.path.join(path, "OBJECT"), "w", encoding="utf-8") as handle:
-        handle.write(
-            '{ "type": "summarized_experiment", "summarized_experiment": { "version": "1.0", "dimensions": '
-            + _se_meta
-            + " } }"
-        )
-
     save_common_se_props(
-        x, path, data_frame_args=data_frame_args, assay_args=assay_args
+        x, path, data_frame_args=data_frame_args, assay_args=assay_args, **kwargs
     )
 
     return
```

### Comparing `dolomite-se-0.1.1/src/dolomite_se/utils.py` & `dolomite_se-0.1.2/src/dolomite_se/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 
 import dolomite_base as dl
 
 
-def save_common_se_props(x, path, data_frame_args, assay_args):
+def save_common_se_props(x, path, data_frame_args, assay_args, **kwargs):
     """Save common :py:class:`~summarizedexperiment.SummarizedExperiment.SummarizedExperiment`
     properties to the specified path.
 
     Mostly for reuse in derivatives of SE.
 
     Args:
         x:
@@ -21,86 +21,94 @@
             Further arguments to pass to the ``save_object`` method for the
             row/column data.
 
         assay_args:
             Further arguments to pass to the ``save_object`` method for the
             assays.
     """
+    # save OBJECT
+    _info = {"summarized_experiment": {"version": "1.0", "dimensions": list(x.shape)}}
+    dl.save_object_file(path, "summarized_experiment", _info)
+
     # save assays
     _assay_names = x.get_assay_names()
     if len(_assay_names) > 0:
         _assays_path = os.path.join(path, "assays")
         os.mkdir(_assays_path)
 
         with open(os.path.join(_assays_path, "names.json"), "w") as handle:
             json.dump(_assay_names, handle)
 
         for _aidx, _aname in enumerate(_assay_names):
             _assay_save_path = os.path.join(_assays_path, str(_aidx))
             try:
-                dl.save_object(x.assays[_aname], path=_assay_save_path, **assay_args)
+                dl.alt_save_object(
+                    x.assays[_aname], path=_assay_save_path, **assay_args
+                )
             except Exception as ex:
                 raise RuntimeError(
                     "failed to stage assay '"
                     + _aname
                     + "' for "
                     + str(type(x))
                     + "; "
                     + str(ex)
                 )
 
     # save row data
     _rdata = x.get_row_data()
     if _rdata is not None and (_rdata.row_names is not None or _rdata.shape[1] > 0):
-        dl.save_object(_rdata, path=os.path.join(path, "row_data"), **data_frame_args)
+        dl.alt_save_object(
+            _rdata, path=os.path.join(path, "row_data"), **data_frame_args
+        )
 
     # save column data
     _cdata = x.get_column_data()
     if _cdata is not None and (_cdata.row_names is not None or _cdata.shape[1] > 0):
-        dl.save_object(
+        dl.alt_save_object(
             _cdata, path=os.path.join(path, "column_data"), **data_frame_args
         )
 
     _meta = x.get_metadata()
     if _meta is not None and len(_meta) > 0:
-        dl.save_object(_meta, path=os.path.join(path, "other_data"))
+        dl.alt_save_object(_meta, path=os.path.join(path, "other_data"), **kwargs)
 
 
-def read_common_se_props(path):
+def read_common_se_props(path, **kwargs):
     """Read shared properties from a directory containing
     :py:class:`~summarizedexperiment.SummarizedExperiment.SummarizedExperiment` or
     its derivatives.
 
     Args:
         path:
             Path to the directory containing the object.
 
     Returns:
         A tuple containing row data, column data and the assays.
     """
     _row_data = None
     _rdata_path = os.path.join(path, "row_data")
     if os.path.exists(_rdata_path):
-        _row_data = dl.read_object(_rdata_path)
+        _row_data = dl.alt_read_object(_rdata_path, **kwargs)
 
     _column_data = None
     _cdata_path = os.path.join(path, "column_data")
     if os.path.exists(_cdata_path):
-        _column_data = dl.read_object(_cdata_path)
+        _column_data = dl.alt_read_object(_cdata_path, **kwargs)
 
     _assays = {}
     _assays_path = os.path.join(path, "assays")
     if os.path.exists(_assays_path):
         with open(os.path.join(_assays_path, "names.json"), "r") as handle:
             _assay_names = json.load(handle)
 
         for _aidx, _aname in enumerate(_assay_names):
             _assay_read_path = os.path.join(_assays_path, str(_aidx))
 
             try:
-                _assays[_aname] = dl.read_object(_assay_read_path)
+                _assays[_aname] = dl.alt_read_object(_assay_read_path, **kwargs)
             except Exception as ex:
                 raise RuntimeError(
                     f"failed to load assay '{_aname}' from '{path}'; " + str(ex)
                 )
 
     return _row_data, _column_data, _assays
```

### Comparing `dolomite-se-0.1.1/src/dolomite_se.egg-info/PKG-INFO` & `dolomite_se-0.1.2/src/dolomite_se.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dolomite-se
-Version: 0.1.1
+Version: 0.1.2
 Summary: Save and load summarized experiments in the dolomite framework!
 Home-page: https://github.com/ArtifactDB/dolomite-se
 Author: LTLA
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-se
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: dolomite-base>=0.2.0
-Requires-Dist: dolomite-matrix>=0.1.0
-Requires-Dist: dolomite-ranges>=0.1.0
-Requires-Dist: summarizedexperiment<0.5.0,>=0.4.2
+Requires-Dist: dolomite-base>=0.2.3
+Requires-Dist: dolomite-matrix>=0.2.1
+Requires-Dist: dolomite-ranges>=0.1.3
+Requires-Dist: summarizedexperiment>=0.4.4
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: numpy; extra == "testing"
 
 <!-- These are examples of badges you might want to add to your README:
```

### Comparing `dolomite-se-0.1.1/src/dolomite_se.egg-info/SOURCES.txt` & `dolomite_se-0.1.2/src/dolomite_se.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/tests/test_range_summarized_experiment.py` & `dolomite_se-0.1.2/tests/test_range_summarized_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/tests/test_summarized_experiment.py` & `dolomite_se-0.1.2/tests/test_summarized_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite-se-0.1.1/tox.ini` & `dolomite_se-0.1.2/tox.ini`

 * *Files identical despite different names*

