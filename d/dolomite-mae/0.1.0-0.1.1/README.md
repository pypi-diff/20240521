# Comparing `tmp/dolomite-mae-0.1.0.tar.gz` & `tmp/dolomite_mae-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolomite-mae-0.1.0.tar", last modified: Fri Jan 26 22:56:58 2024, max compression
+gzip compressed data, was "dolomite_mae-0.1.1.tar", last modified: Tue May 21 20:38:39 2024, max compression
```

## Comparing `dolomite-mae-0.1.0.tar` & `dolomite_mae-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.626336 dolomite-mae-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.618336 dolomite-mae-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.622336 dolomite-mae-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-01-26 22:56:58.626336 dolomite-mae-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.622336 dolomite-mae-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.622336 dolomite-mae-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-01-26 22:56:58.626336 dolomite-mae-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.618336 dolomite-mae-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.622336 dolomite-mae-0.1.0/src/dolomite_mae/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/src/dolomite_mae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/src/dolomite_mae/read_multi_assay_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/src/dolomite_mae/save_multi_assay_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.626336 dolomite-mae-0.1.0/src/dolomite_mae.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-01-26 22:56:58.000000 dolomite-mae-0.1.0/src/dolomite_mae.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-26 22:56:58.000000 dolomite-mae-0.1.0/src/dolomite_mae.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 22:56:58.000000 dolomite-mae-0.1.0/src/dolomite_mae.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 22:56:58.000000 dolomite-mae-0.1.0/src/dolomite_mae.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-26 22:56:58.000000 dolomite-mae-0.1.0/src/dolomite_mae.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-26 22:56:58.000000 dolomite-mae-0.1.0/src/dolomite_mae.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:56:58.626336 dolomite-mae-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/tests/test_mae.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-01-26 22:55:55.000000 dolomite-mae-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.304307 dolomite_mae-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.296307 dolomite_mae-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.300307 dolomite_mae-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-21 20:38:39.304307 dolomite_mae-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.300307 dolomite_mae-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.300307 dolomite_mae-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-21 20:38:39.304307 dolomite_mae-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.296307 dolomite_mae-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.304307 dolomite_mae-0.1.1/src/dolomite_mae/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/src/dolomite_mae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/src/dolomite_mae/read_multi_assay_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/src/dolomite_mae/save_multi_assay_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.304307 dolomite_mae-0.1.1/src/dolomite_mae.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-21 20:38:39.000000 dolomite_mae-0.1.1/src/dolomite_mae.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-21 20:38:39.000000 dolomite_mae-0.1.1/src/dolomite_mae.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:38:39.000000 dolomite_mae-0.1.1/src/dolomite_mae.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:38:39.000000 dolomite_mae-0.1.1/src/dolomite_mae.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-21 20:38:39.000000 dolomite_mae-0.1.1/src/dolomite_mae.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 20:38:39.000000 dolomite_mae-0.1.1/src/dolomite_mae.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:39.304307 dolomite_mae-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/tests/test_mae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-21 20:37:33.000000 dolomite_mae-0.1.1/tox.ini
```

### Comparing `dolomite-mae-0.1.0/.coveragerc` & `dolomite_mae-0.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/.github/workflows/pypi-publish.yml` & `dolomite_mae-0.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/.github/workflows/pypi-test.yml` & `dolomite_mae-0.1.1/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/.gitignore` & `dolomite_mae-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/.readthedocs.yml` & `dolomite_mae-0.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/CONTRIBUTING.md` & `dolomite_mae-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/LICENSE.txt` & `dolomite_mae-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/PKG-INFO` & `dolomite_mae-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dolomite-mae
-Version: 0.1.0
+Version: 0.1.1
 Summary: Save and load multi-assay experiments in the dolomite framework!
 Home-page: https://github.com/ArtifactDB/dolomite-mae
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-mae
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: dolomite_base>=0.2.0
-Requires-Dist: dolomite_sce>=0.1.0
-Requires-Dist: dolomite_se>=0.1.0
-Requires-Dist: multiassayexperiment<0.5.0,>=0.4.2
+Requires-Dist: dolomite_base>=0.2.4
+Requires-Dist: dolomite_sce>=0.1.2
+Requires-Dist: dolomite_se>=0.1.3
+Requires-Dist: multiassayexperiment>=0.4.2
 Requires-Dist: biocutils
 Requires-Dist: pandas
 Requires-Dist: numpy
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `dolomite-mae-0.1.0/README.md` & `dolomite_mae-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/docs/Makefile` & `dolomite_mae-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/docs/conf.py` & `dolomite_mae-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/docs/index.md` & `dolomite_mae-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/setup.cfg` & `dolomite_mae-0.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	dolomite_base>=0.2.0
-	dolomite_sce>=0.1.0
-	dolomite_se>=0.1.0
-	multiassayexperiment>=0.4.2,<0.5.0
+	dolomite_base>=0.2.4
+	dolomite_sce>=0.1.2
+	dolomite_se>=0.1.3
+	multiassayexperiment>=0.4.2
 	biocutils
 	pandas
 	numpy
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `dolomite-mae-0.1.0/setup.py` & `dolomite_mae-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/src/dolomite_mae/__init__.py` & `dolomite_mae-0.1.1/src/dolomite_mae/__init__.py`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/src/dolomite_mae/read_multi_assay_experiment.py` & `dolomite_mae-0.1.1/src/dolomite_mae/read_multi_assay_experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import dolomite_base as dl
 import h5py
 from biocframe import BiocFrame
 from dolomite_base.read_object import read_object_registry
 from multiassayexperiment import MultiAssayExperiment
 
-read_object_registry[
-    "multi_sample_dataset"
-] = "dolomite_mae.read_multi_assay_experiment"
+read_object_registry["multi_sample_dataset"] = (
+    "dolomite_mae.read_multi_assay_experiment"
+)
 
 
 def read_multi_assay_experiment(
     path: str, metadata: dict, **kwargs
 ) -> MultiAssayExperiment:
     """Load a
     :py:class:`~multiassayexperiment.MultiAssayExperiment.MultiAssayExperiment`
@@ -26,26 +26,26 @@
         path:
             Path to the directory containing the object.
 
         metadata:
             Metadata for the object.
 
         kwargs:
-            Further arguments, ignored.
+            Further arguments.
 
     Returns:
         A
         :py:class:`~multiassayexperiment.MultiAssayExperiment.MultiAssayExperiment`
         with file-backed arrays in the assays.
     """
 
     _sample_path = os.path.join(path, "sample_data")
     _sample_data = None
     if os.path.exists(_sample_path):
-        _sample_data = dl.read_object(_sample_path)
+        _sample_data = dl.alt_read_object(_sample_path, **kwargs)
 
     if _sample_data is None:
         raise RuntimeError("Cannot read 'sample_data'.")
 
     _srow_names = _sample_data.get_row_names()
     if _srow_names is None:
         raise RuntimeError("'sample_data' does not contain 'row_names'.")
@@ -66,15 +66,15 @@
             _assay = []
             _colname = []
 
             for _aidx, _aname in enumerate(_expt_names):
                 _expt_read_path = os.path.join(_expts_path, str(_aidx))
 
                 try:
-                    _expts[_aname] = dl.read_object(_expt_read_path)
+                    _expts[_aname] = dl.alt_read_object(_expt_read_path, **kwargs)
                 except Exception as ex:
                     raise RuntimeError(
                         f"failed to load experiment '{_aname}' from '{path}'; "
                         + str(ex)
                     )
 
                 _expt_map = dl.load_vector_from_hdf5(
@@ -91,11 +91,11 @@
 
     mae = MultiAssayExperiment(
         experiments=_expts, column_data=_sample_data, sample_map=_sample_map_data
     )
 
     _meta_path = os.path.join(path, "other_data")
     if os.path.exists(_meta_path):
-        _meta = dl.read_object(_meta_path)
+        _meta = dl.alt_read_object(_meta_path, **kwargs)
         mae = mae.set_metadata(_meta.as_dict())
 
     return mae
```

### Comparing `dolomite-mae-0.1.0/src/dolomite_mae/save_multi_assay_experiment.py` & `dolomite_mae-0.1.1/src/dolomite_mae/save_multi_assay_experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,53 +32,53 @@
             Further arguments to pass to the ``save_object`` method for the
             row/column data.
 
         assay_args:
             Further arguments to pass to the ``save_object`` method for the
             assays.
 
-        kwargs: Further arguments, ignored.
+        kwargs: 
+            Further arguments.
 
     Returns:
         ``x`` is saved to path.
     """
     os.mkdir(path)
 
     if data_frame_args is None:
         data_frame_args = {}
 
     if assay_args is None:
         assay_args = {}
 
-    with open(os.path.join(path, "OBJECT"), "w", encoding="utf-8") as handle:
-        handle.write(
-            '{ "type": "multi_sample_dataset", "multi_sample_dataset": { "version": "1.0" } }'
-        )
+    _info = {"multi_sample_dataset": {"version": "1.0"}}
+    dl.save_object_file(path, "multi_sample_dataset", _info)
 
     # sample/column data
     _sample_path = os.path.join(path, "sample_data")
-    dl.save_object(x.get_column_data(), _sample_path, **data_frame_args)
+    dl.alt_save_object(x.get_column_data(), _sample_path, **data_frame_args, **kwargs)
 
     # save alt expts.
     _expt_names = x.get_experiment_names()
     if len(_expt_names) > 0:
         _expt_path = os.path.join(path, "experiments")
         os.mkdir(_expt_path)
 
         with open(os.path.join(_expt_path, "names.json"), "w") as handle:
             json.dump(_expt_names, handle)
 
         for _aidx, _aname in enumerate(_expt_names):
             _expt_save_path = os.path.join(_expt_path, str(_aidx))
             try:
-                dl.save_object(
+                dl.alt_save_object(
                     x.experiment(_aname),
                     path=_expt_save_path,
                     data_frame_args=data_frame_args,
                     assay_args=assay_args,
+                    **kwargs,
                 )
             except Exception as ex:
                 raise RuntimeError(
                     "failed to stage experiment '"
                     + _aname
                     + "' for "
                     + str(type(x))
@@ -121,10 +121,10 @@
 
                 dl.write_integer_vector_to_hdf5(
                     ghandle, name=str(_aidx), h5type="u4", x=reorder
                 )
 
     _meta = x.get_metadata()
     if _meta is not None and len(_meta) > 0:
-        dl.save_object(_meta, path=os.path.join(path, "other_data"))
+        dl.alt_save_object(_meta, path=os.path.join(path, "other_data"), **kwargs)
 
     return
```

### Comparing `dolomite-mae-0.1.0/src/dolomite_mae.egg-info/PKG-INFO` & `dolomite_mae-0.1.1/src/dolomite_mae.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dolomite-mae
-Version: 0.1.0
+Version: 0.1.1
 Summary: Save and load multi-assay experiments in the dolomite framework!
 Home-page: https://github.com/ArtifactDB/dolomite-mae
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-mae
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: dolomite_base>=0.2.0
-Requires-Dist: dolomite_sce>=0.1.0
-Requires-Dist: dolomite_se>=0.1.0
-Requires-Dist: multiassayexperiment<0.5.0,>=0.4.2
+Requires-Dist: dolomite_base>=0.2.4
+Requires-Dist: dolomite_sce>=0.1.2
+Requires-Dist: dolomite_se>=0.1.3
+Requires-Dist: multiassayexperiment>=0.4.2
 Requires-Dist: biocutils
 Requires-Dist: pandas
 Requires-Dist: numpy
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `dolomite-mae-0.1.0/src/dolomite_mae.egg-info/SOURCES.txt` & `dolomite_mae-0.1.1/src/dolomite_mae.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/tests/test_mae.py` & `dolomite_mae-0.1.1/tests/test_mae.py`

 * *Files identical despite different names*

### Comparing `dolomite-mae-0.1.0/tox.ini` & `dolomite_mae-0.1.1/tox.ini`

 * *Files identical despite different names*

