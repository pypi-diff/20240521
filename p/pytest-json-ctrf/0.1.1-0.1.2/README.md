# Comparing `tmp/pytest_json_ctrf-0.1.1.tar.gz` & `tmp/pytest_json_ctrf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_json_ctrf-0.1.1.tar", last modified: Mon May 20 19:39:43 2024, max compression
+gzip compressed data, was "pytest_json_ctrf-0.1.2.tar", last modified: Mon May 20 19:46:40 2024, max compression
```

## Comparing `pytest_json_ctrf-0.1.1.tar` & `pytest_json_ctrf-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:39:43.644281 pytest_json_ctrf-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-20 19:39:43.644281 pytest_json_ctrf-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:39:43.644281 pytest_json_ctrf-0.1.1/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/plugin/BaseMetadataReport.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/plugin/CommonTestReportPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/plugin/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/plugin/TestObject.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/plugin/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:39:43.644281 pytest_json_ctrf-0.1.1/pytest_json_ctrf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-20 19:39:43.000000 pytest_json_ctrf-0.1.1/pytest_json_ctrf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-20 19:39:43.000000 pytest_json_ctrf-0.1.1/pytest_json_ctrf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:39:43.000000 pytest_json_ctrf-0.1.1/pytest_json_ctrf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:39:43.000000 pytest_json_ctrf-0.1.1/pytest_json_ctrf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 19:39:43.000000 pytest_json_ctrf-0.1.1/pytest_json_ctrf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:39:43.000000 pytest_json_ctrf-0.1.1/pytest_json_ctrf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:39:43.644281 pytest_json_ctrf-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:39:43.644281 pytest_json_ctrf-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-20 19:39:39.000000 pytest_json_ctrf-0.1.1/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.221834 pytest_json_ctrf-0.1.2/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/BaseMetadataReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/CommonTestReportPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/TestObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/tests/test_example.py
```

### Comparing `pytest_json_ctrf-0.1.1/PKG-INFO` & `pytest_json_ctrf-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pytest-json-ctrf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pytest plugin to generate json report in CTRF (Common Test Report Format)
 Author: Oleksii Ostapov
 Project-URL: Infopulse, https://infopulse.com/
-Project-URL: Homepage, https://infopulse.com/pytest-json-ctrf
+Project-URL: Homepage, https://github.com/infopulse/pytest-common-test-report-json
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pytest>6.0.0
```

### Comparing `pytest_json_ctrf-0.1.1/README.md` & `pytest_json_ctrf-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.1/plugin/BaseMetadataReport.py` & `pytest_json_ctrf-0.1.2/plugin/BaseMetadataReport.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.1/plugin/CommonTestReportPlugin.py` & `pytest_json_ctrf-0.1.2/plugin/CommonTestReportPlugin.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.1/plugin/Report.py` & `pytest_json_ctrf-0.1.2/plugin/Report.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.1/plugin/TestObject.py` & `pytest_json_ctrf-0.1.2/plugin/TestObject.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.1/plugin/main.py` & `pytest_json_ctrf-0.1.2/plugin/main.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.1/pyproject.toml` & `pytest_json_ctrf-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = [".github", "tests", "build", "dist", ".venv", "pytestomatio.egg-info", ".env", ".gitignore", "CHANGELOG.md", "assets"]
 
 [project]
 name = "pytest-json-ctrf"
-version = "0.1.1"
+version = "0.1.2"
 
 dependencies = [
     "pytest>6.0.0",
 ]
 
 authors = [
     { name = "Oleksii Ostapov" },
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Infopulse" = "https://infopulse.com/"
-"Homepage" = "https://infopulse.com/pytest-json-ctrf"
+"Homepage" = "https://github.com/infopulse/pytest-common-test-report-json"
 
 [tool.pytest.ini_options]
 markers = [
     "smoke: marker for smoke tests",
     "regression: marker for regression tests",
 ]
```

### Comparing `pytest_json_ctrf-0.1.1/pytest_json_ctrf.egg-info/PKG-INFO` & `pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pytest-json-ctrf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pytest plugin to generate json report in CTRF (Common Test Report Format)
 Author: Oleksii Ostapov
 Project-URL: Infopulse, https://infopulse.com/
-Project-URL: Homepage, https://infopulse.com/pytest-json-ctrf
+Project-URL: Homepage, https://github.com/infopulse/pytest-common-test-report-json
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pytest>6.0.0
```

### Comparing `pytest_json_ctrf-0.1.1/tests/test_example.py` & `pytest_json_ctrf-0.1.2/tests/test_example.py`

 * *Files identical despite different names*

