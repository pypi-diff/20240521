# Comparing `tmp/dolomite-sce-0.1.1.tar.gz` & `tmp/dolomite_sce-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolomite-sce-0.1.1.tar", last modified: Fri Feb  9 16:45:12 2024, max compression
+gzip compressed data, was "dolomite_sce-0.1.2.tar", last modified: Tue May 21 20:26:27 2024, max compression
```

## Comparing `dolomite-sce-0.1.1.tar` & `dolomite_sce-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.418382 dolomite-sce-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.410382 dolomite-sce-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.414382 dolomite-sce-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-02-09 16:45:12.418382 dolomite-sce-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.414382 dolomite-sce-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.414382 dolomite-sce-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-09 16:45:12.422381 dolomite-sce-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.410382 dolomite-sce-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.418382 dolomite-sce-0.1.1/src/dolomite_sce/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/src/dolomite_sce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/src/dolomite_sce/read_single_cell_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/src/dolomite_sce/save_single_cell_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.418382 dolomite-sce-0.1.1/src/dolomite_sce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-02-09 16:45:12.000000 dolomite-sce-0.1.1/src/dolomite_sce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-09 16:45:12.000000 dolomite-sce-0.1.1/src/dolomite_sce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:45:12.000000 dolomite-sce-0.1.1/src/dolomite_sce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:45:12.000000 dolomite-sce-0.1.1/src/dolomite_sce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-09 16:45:12.000000 dolomite-sce-0.1.1/src/dolomite_sce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-09 16:45:12.000000 dolomite-sce-0.1.1/src/dolomite_sce.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:45:12.418382 dolomite-sce-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/tests/test_stage_single_cell_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-09 16:44:15.000000 dolomite-sce-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.572525 dolomite_sce-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.560525 dolomite_sce-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.564525 dolomite_sce-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-21 20:26:27.572525 dolomite_sce-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.568525 dolomite_sce-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.568525 dolomite_sce-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-21 20:26:27.572525 dolomite_sce-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.560525 dolomite_sce-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.568525 dolomite_sce-0.1.2/src/dolomite_sce/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/src/dolomite_sce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/src/dolomite_sce/read_single_cell_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/src/dolomite_sce/save_single_cell_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.572525 dolomite_sce-0.1.2/src/dolomite_sce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-21 20:26:27.000000 dolomite_sce-0.1.2/src/dolomite_sce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-21 20:26:27.000000 dolomite_sce-0.1.2/src/dolomite_sce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:26:27.000000 dolomite_sce-0.1.2/src/dolomite_sce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:26:27.000000 dolomite_sce-0.1.2/src/dolomite_sce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 20:26:27.000000 dolomite_sce-0.1.2/src/dolomite_sce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 20:26:27.000000 dolomite_sce-0.1.2/src/dolomite_sce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:26:27.568525 dolomite_sce-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/tests/test_stage_single_cell_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-21 20:25:31.000000 dolomite_sce-0.1.2/tox.ini
```

### Comparing `dolomite-sce-0.1.1/.coveragerc` & `dolomite_sce-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/.github/workflows/pypi-publish.yml` & `dolomite_sce-0.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/.github/workflows/pypi-test.yml` & `dolomite_sce-0.1.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/.gitignore` & `dolomite_sce-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/.readthedocs.yml` & `dolomite_sce-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/CONTRIBUTING.md` & `dolomite_sce-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/LICENSE.txt` & `dolomite_sce-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/PKG-INFO` & `dolomite_sce-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dolomite-sce
-Version: 0.1.1
+Version: 0.1.2
 Summary: Save and load single-cell experiments in the dolomite framework!
 Home-page: https://github.com/ArtifactDB/dolomite-sce
 Author: LTLA
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-sce
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: dolomite-base>=0.2.0
-Requires-Dist: dolomite-se>=0.1.1
-Requires-Dist: singlecellexperiment<0.5.0,>=0.4.3
+Requires-Dist: dolomite-base>=0.2.4
+Requires-Dist: dolomite-se>=0.1.3
+Requires-Dist: singlecellexperiment>=0.4.5
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
```

### Comparing `dolomite-sce-0.1.1/README.md` & `dolomite_sce-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/docs/Makefile` & `dolomite_sce-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/docs/conf.py` & `dolomite_sce-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/docs/index.md` & `dolomite_sce-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/setup.cfg` & `dolomite_sce-0.1.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	dolomite-base>=0.2.0
-	dolomite-se>=0.1.1
-	singlecellexperiment>=0.4.3,<0.5.0
+	dolomite-base>=0.2.4
+	dolomite-se>=0.1.3
+	singlecellexperiment>=0.4.5
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `dolomite-sce-0.1.1/setup.py` & `dolomite_sce-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/src/dolomite_sce/__init__.py` & `dolomite_sce-0.1.2/src/dolomite_sce/__init__.py`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/src/dolomite_sce/read_single_cell_experiment.py` & `dolomite_sce-0.1.2/src/dolomite_sce/read_single_cell_experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 import os
 
 import dolomite_base as dl
 from dolomite_base.read_object import read_object_registry
-from dolomite_se import read_common_se_props
 from singlecellexperiment import SingleCellExperiment
 
-read_object_registry[
-    "single_cell_experiment"
-] = "dolomite_sce.read_single_cell_experiment"
+read_object_registry["single_cell_experiment"] = (
+    "dolomite_sce.read_single_cell_experiment"
+)
 
 
 def read_single_cell_experiment(
     path: str, metadata: dict, **kwargs
 ) -> SingleCellExperiment:
     """Load a
     :py:class:`~singlecellexperiment.SingleCellExperiment.SingleCellExperiment`
@@ -25,57 +24,50 @@
         path:
             Path to the directory containing the object.
 
         metadata:
             Metadata for the object.
 
         kwargs:
-            Further arguments, ignored.
+            Further arguments.
 
     Returns:
         A
         :py:class:`~singlecellexperiment.SingleCellExperiment.SingleCellExperiment`
         with file-backed arrays in the assays.
     """
 
-    _row_data, _column_data, _assays = read_common_se_props(path)
+    metadata["type"] = "range_summarized_experiment"
+    rse = dl.alt_read_object(path, metadata=metadata, **kwargs)
 
     _main_expt_name = None
     if "main_experiment_name" in metadata["single_cell_experiment"]:
         _main_expt_name = metadata["single_cell_experiment"]["main_experiment_name"]
 
     sce = SingleCellExperiment(
-        assays=_assays,
-        row_data=_row_data,
-        column_data=_column_data,
+        assays=rse.get_assays(),
+        row_data=rse.get_row_data(),
+        column_data=rse.get_column_data(),
+        row_ranges=rse.get_row_ranges(),
+        metadata=rse.get_metadata(),
         main_experiment_name=_main_expt_name,
     )
 
-    _meta_path = os.path.join(path, "other_data")
-    if os.path.exists(_meta_path):
-        _meta = dl.read_object(_meta_path)
-        sce = sce.set_metadata(_meta.as_dict())
-
-    _ranges_path = os.path.join(path, "row_ranges")
-    if os.path.exists(_ranges_path):
-        _ranges = dl.read_object(_ranges_path)
-        sce = sce.set_row_ranges(_ranges)
-
     _rdim_path = os.path.join(path, "reduced_dimensions")
     if os.path.exists(_rdim_path):
         _rdims = {}
 
         with open(os.path.join(_rdim_path, "names.json"), "r") as handle:
             _rdim_names = json.load(handle)
 
         for _aidx, _aname in enumerate(_rdim_names):
             _rdim_read_path = os.path.join(_rdim_path, str(_aidx))
 
             try:
-                _rdims[_aname] = dl.read_object(_rdim_read_path)
+                _rdims[_aname] = dl.alt_read_object(_rdim_read_path, **kwargs)
             except Exception as ex:
                 raise RuntimeError(
                     f"failed to load reduced dimension '{_aname}' from '{path}'; "
                     + str(ex)
                 )
 
         sce = sce.set_reduced_dims(_rdims)
@@ -87,15 +79,15 @@
         with open(os.path.join(_alt_path, "names.json"), "r") as handle:
             _alt_names = json.load(handle)
 
         for _aidx, _aname in enumerate(_alt_names):
             _alt_read_path = os.path.join(_alt_path, str(_aidx))
 
             try:
-                _alts[_aname] = dl.read_object(_alt_read_path)
+                _alts[_aname] = dl.alt_read_object(_alt_read_path, **kwargs)
             except Exception as ex:
                 raise RuntimeError(
                     f"failed to load alternative experiment '{_aname}' from '{path}'; "
                     + str(ex)
                 )
 
         sce = sce.set_alternative_experiments(_alts)
```

### Comparing `dolomite-sce-0.1.1/src/dolomite_sce/save_single_cell_experiment.py` & `dolomite_sce-0.1.2/src/dolomite_sce/save_single_cell_experiment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 
 import dolomite_base as dl
-from dolomite_se import save_common_se_props
 from singlecellexperiment import SingleCellExperiment
+from summarizedexperiment import RangedSummarizedExperiment
 
 
 @dl.save_object.register
 @dl.validate_saves
 def save_single_cell_experiment(
     x: SingleCellExperiment,
     path: str,
@@ -42,75 +42,69 @@
             reduced dimensions.
 
         alt_expts_args:
             Further arguments to pass to the ``save_object`` method for the
             alternative experiments.
 
         kwargs:
-            Further arguments, ignored.
+            Further arguments.
 
     Returns:
         ``x`` is saved to path.
     """
-    os.mkdir(path)
-
     if data_frame_args is None:
         data_frame_args = {}
 
     if assay_args is None:
         assay_args = {}
 
     if rdim_args is None:
         rdim_args = {}
 
     if alt_expts_args is None:
         alt_expts_args = {}
 
-    _se_meta = f"{list(x.shape)}"
+    ## Convert to RSE
+    _rse = RangedSummarizedExperiment(
+        assays=x.get_assays(),
+        row_data=x.get_row_data(),
+        column_data=x.get_column_data(),
+        row_ranges=x.get_row_ranges(),
+        row_names=x.get_row_names(),
+        column_names=x.get_column_names(),
+        metadata=x.get_metadata(),
+    )
+    dl.alt_save_object(
+        _rse, path, data_frame_args=data_frame_args, assay_args=assay_args, **kwargs
+    )
 
-    _sce_meta = '"single_cell_experiment": { "version": "1.0" }'
+    # Modify OBJECT
+    _info = dl.read_object_file(path)
+    _info["single_cell_experiment"] = {"version": "1.0"}
     if x.get_main_experiment_name() is not None:
-        _sce_meta = (
-            '"single_cell_experiment": { "version": "1.0", "main_experiment_name": "'
-            + str(x.get_main_experiment_name())
-            + '" }'
-        )
-
-    with open(os.path.join(path, "OBJECT"), "w", encoding="utf-8") as handle:
-        handle.write(
-            '{ "type": "single_cell_experiment", '
-            + _sce_meta
-            + ", "
-            + '"ranged_summarized_experiment": { "version": "1.0" },'
-            + '"summarized_experiment": {"version": "1.0", "dimensions": '
-            + _se_meta
-            + " } }"
+        _info["single_cell_experiment"]["main_experiment_name"] = str(
+            x.get_main_experiment_name()
         )
-
-    save_common_se_props(
-        x, path, data_frame_args=data_frame_args, assay_args=assay_args
-    )
-
-    _ranges = x.get_row_ranges()
-    if _ranges is not None:
-        dl.save_object(_ranges, path=os.path.join(path, "row_ranges"))
+    dl.save_object_file(path, "single_cell_experiment", _info)
 
     # save rdims
     _rdim_names = x.get_reduced_dim_names()
     if len(_rdim_names) > 0:
         _rdim_path = os.path.join(path, "reduced_dimensions")
         os.mkdir(_rdim_path)
 
         with open(os.path.join(_rdim_path, "names.json"), "w") as handle:
             json.dump(_rdim_names, handle)
 
         for _aidx, _aname in enumerate(_rdim_names):
             _rdim_save_path = os.path.join(_rdim_path, str(_aidx))
             try:
-                dl.save_object(x.reduced_dim(_aname), path=_rdim_save_path, **rdim_args)
+                dl.alt_save_object(
+                    x.reduced_dim(_aname), path=_rdim_save_path, **rdim_args, **kwargs
+                )
             except Exception as ex:
                 raise RuntimeError(
                     "failed to stage reduced dimension '"
                     + _aname
                     + "' for "
                     + str(type(x))
                     + "; "
@@ -125,18 +119,19 @@
 
         with open(os.path.join(_alt_path, "names.json"), "w") as handle:
             json.dump(_alt_names, handle)
 
         for _aidx, _aname in enumerate(_alt_names):
             _alt_save_path = os.path.join(_alt_path, str(_aidx))
             try:
-                dl.save_object(
+                dl.alt_save_object(
                     x.alternative_experiment(_aname),
                     path=_alt_save_path,
                     **alt_expts_args,
+                    **kwargs,
                 )
             except Exception as ex:
                 raise RuntimeError(
                     "failed to stage alternative experiment '"
                     + _aname
                     + "' for "
                     + str(type(x))
```

### Comparing `dolomite-sce-0.1.1/src/dolomite_sce.egg-info/PKG-INFO` & `dolomite_sce-0.1.2/src/dolomite_sce.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dolomite-sce
-Version: 0.1.1
+Version: 0.1.2
 Summary: Save and load single-cell experiments in the dolomite framework!
 Home-page: https://github.com/ArtifactDB/dolomite-sce
 Author: LTLA
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-sce
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: dolomite-base>=0.2.0
-Requires-Dist: dolomite-se>=0.1.1
-Requires-Dist: singlecellexperiment<0.5.0,>=0.4.3
+Requires-Dist: dolomite-base>=0.2.4
+Requires-Dist: dolomite-se>=0.1.3
+Requires-Dist: singlecellexperiment>=0.4.5
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
```

### Comparing `dolomite-sce-0.1.1/src/dolomite_sce.egg-info/SOURCES.txt` & `dolomite_sce-0.1.2/src/dolomite_sce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/tests/test_stage_single_cell_experiment.py` & `dolomite_sce-0.1.2/tests/test_stage_single_cell_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite-sce-0.1.1/tox.ini` & `dolomite_sce-0.1.2/tox.ini`

 * *Files identical despite different names*

