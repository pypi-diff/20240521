# Comparing `tmp/pytest_json_ctrf-0.1.2.tar.gz` & `tmp/pytest_json_ctrf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_json_ctrf-0.1.2.tar", last modified: Mon May 20 19:46:40 2024, max compression
+gzip compressed data, was "pytest_json_ctrf-0.2.1.tar", last modified: Tue May 21 05:50:20 2024, max compression
```

## Comparing `pytest_json_ctrf-0.1.2.tar` & `pytest_json_ctrf-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.221834 pytest_json_ctrf-0.1.2/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/BaseMetadataReport.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/CommonTestReportPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/TestObject.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/plugin/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:46:40.000000 pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.225834 pytest_json_ctrf-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-20 19:46:35.000000 pytest_json_ctrf-0.1.2/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:50:20.324940 pytest_json_ctrf-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-21 05:50:20.324940 pytest_json_ctrf-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:50:20.324940 pytest_json_ctrf-0.2.1/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/plugin/BaseMetadataReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/plugin/CommonTestReportPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/plugin/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/plugin/TestObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/plugin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:50:20.324940 pytest_json_ctrf-0.2.1/pytest_json_ctrf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-21 05:50:20.000000 pytest_json_ctrf-0.2.1/pytest_json_ctrf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-21 05:50:20.000000 pytest_json_ctrf-0.2.1/pytest_json_ctrf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 05:50:20.000000 pytest_json_ctrf-0.2.1/pytest_json_ctrf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 05:50:20.000000 pytest_json_ctrf-0.2.1/pytest_json_ctrf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 05:50:20.000000 pytest_json_ctrf-0.2.1/pytest_json_ctrf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 05:50:20.000000 pytest_json_ctrf-0.2.1/pytest_json_ctrf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 05:50:20.324940 pytest_json_ctrf-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:50:20.324940 pytest_json_ctrf-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-21 05:50:15.000000 pytest_json_ctrf-0.2.1/tests/test_example.py
```

### Comparing `pytest_json_ctrf-0.1.2/PKG-INFO` & `pytest_json_ctrf-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-json-ctrf
-Version: 0.1.2
+Version: 0.2.1
 Summary: Pytest plugin to generate json report in CTRF (Common Test Report Format)
 Author: Oleksii Ostapov
 Project-URL: Infopulse, https://infopulse.com/
 Project-URL: Homepage, https://github.com/infopulse/pytest-common-test-report-json
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -80,14 +80,20 @@
   }
 }
 ```
 
 ## Report Example
 ![Example Image](./assets/report_example.png)
 
+## Technical details
+For future me and others who are interested in the technical details of the implementation.  
+The main idea is to handle xdist plugin because without it collecting report is quite straightforward.  
+By the example of putest-json-report plugin, I have learned that different plugins can be registered for the controller and workers node.  
+The `pytest_runtest_logreport` hook in the controller node is used to collect the test results from all the nodes so other nodes can just add some details to the `TestReport` object.
+
 ## Credits
 
 - https://ctrf.io/ -> nice data format
 - https://github.com/numirias/pytest-json-report -> Source of inspiration and dealing with xdist sync
 - https://github.com/testomatio/pytestomatio -> Source of inspiration for creating pytest plugins
 - https://github.com/infopulse/Playwright-course-python -> The report will be used in the demo project as +1 report option
```

### Comparing `pytest_json_ctrf-0.1.2/README.md` & `pytest_json_ctrf-0.2.1/pytest_json_ctrf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pytest-json-ctrf
+Version: 0.2.1
+Summary: Pytest plugin to generate json report in CTRF (Common Test Report Format)
+Author: Oleksii Ostapov
+Project-URL: Infopulse, https://infopulse.com/
+Project-URL: Homepage, https://github.com/infopulse/pytest-common-test-report-json
+Classifier: Framework :: Pytest
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Requires-Dist: pytest>6.0.0
+
 # CTRF for pytest
 
 Pytest implementation of Common Test Report Format (CTRF) for test results.  
 Test report will be generated in JSON format.  
 Test report can be used to prettify the report in GitHub Actions with [github-actions-ctrf](https://github.com/ctrf-io/github-actions-ctrf).  
 Do not worry if report in GitHub does not appear immediately. It takes some time to process the report. 
 
@@ -65,14 +80,20 @@
   }
 }
 ```
 
 ## Report Example
 ![Example Image](./assets/report_example.png)
 
+## Technical details
+For future me and others who are interested in the technical details of the implementation.  
+The main idea is to handle xdist plugin because without it collecting report is quite straightforward.  
+By the example of putest-json-report plugin, I have learned that different plugins can be registered for the controller and workers node.  
+The `pytest_runtest_logreport` hook in the controller node is used to collect the test results from all the nodes so other nodes can just add some details to the `TestReport` object.
+
 ## Credits
 
 - https://ctrf.io/ -> nice data format
 - https://github.com/numirias/pytest-json-report -> Source of inspiration and dealing with xdist sync
 - https://github.com/testomatio/pytestomatio -> Source of inspiration for creating pytest plugins
 - https://github.com/infopulse/Playwright-course-python -> The report will be used in the demo project as +1 report option
```

### Comparing `pytest_json_ctrf-0.1.2/plugin/BaseMetadataReport.py` & `pytest_json_ctrf-0.2.1/plugin/BaseMetadataReport.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.2/plugin/CommonTestReportPlugin.py` & `pytest_json_ctrf-0.2.1/plugin/CommonTestReportPlugin.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.2/plugin/Report.py` & `pytest_json_ctrf-0.2.1/plugin/Report.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.2/plugin/TestObject.py` & `pytest_json_ctrf-0.2.1/plugin/TestObject.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from enum import Enum
 from pytest import TestReport
 
-
 class TestStatus(Enum):
     PASSED = "passed"
     FAILED = "failed"
     SKIPPED = "skipped"
     PENDING = "pending"
     OTHER = "other"
 
@@ -14,14 +13,15 @@
     name: str = None
     status: TestStatus = TestStatus.PENDING
     raw_status: str = None
     duration: float = 0
     start: float = None
     stop: float = None
     retries: int = 0
+    message: str = ''
 
     worker_id: str = None
     file_path: str = None
     tags: list[str] = None
     browser: str = None
     trace: str = None
 
@@ -29,14 +29,20 @@
         if self.status in (TestStatus.SKIPPED, TestStatus.FAILED):
             return
         elif report.skipped:
             self.status = TestStatus.SKIPPED
         elif report.failed:
             self.status = TestStatus.FAILED
             self.raw_status = f"{report.when}_{report.outcome}"
+            self.message = f"The test failed in the {report.when} phase"
+            if hasattr(report, 'longreprtext'):
+                if "AssertionError" in report.longreprtext:
+                    self.message += " due to an assertion error"
+                elif "Exception" in report.longreprtext:
+                    self.message += " due to an exception"
         elif report.passed:
             self.status = TestStatus.PASSED
         else:
             self.status = TestStatus.OTHER
 
     def update(self, report: TestReport, worker_id: str = None) -> None:
         self.name = report.head_line.split('[')[0]
@@ -62,12 +68,13 @@
             'duration': self.duration,
             'start': self.start,
             'stop': self.stop,
             'retries': None if self.retries == 1 else self.retries,
             'file_path': self.file_path,
             'tags': self.tags,
             'browser': self.browser,
-            'trace': self.trace
+            'trace': self.trace,
+            'message': self.message
         }
         if self.worker_id:
             result['extra'] = {'worker': self.worker_id}
         return {key: value for key, value in result.items() if value not in [None, '', []]}
```

### Comparing `pytest_json_ctrf-0.1.2/plugin/main.py` & `pytest_json_ctrf-0.2.1/plugin/main.py`

 * *Files identical despite different names*

### Comparing `pytest_json_ctrf-0.1.2/pyproject.toml` & `pytest_json_ctrf-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = [".github", "tests", "build", "dist", ".venv", "pytestomatio.egg-info", ".env", ".gitignore", "CHANGELOG.md", "assets"]
 
 [project]
 name = "pytest-json-ctrf"
-version = "0.1.2"
+version = "0.2.1"
 
 dependencies = [
     "pytest>6.0.0",
 ]
 
 authors = [
     { name = "Oleksii Ostapov" },
```

### Comparing `pytest_json_ctrf-0.1.2/pytest_json_ctrf.egg-info/PKG-INFO` & `pytest_json_ctrf-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pytest-json-ctrf
-Version: 0.1.2
-Summary: Pytest plugin to generate json report in CTRF (Common Test Report Format)
-Author: Oleksii Ostapov
-Project-URL: Infopulse, https://infopulse.com/
-Project-URL: Homepage, https://github.com/infopulse/pytest-common-test-report-json
-Classifier: Framework :: Pytest
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Requires-Dist: pytest>6.0.0
-
 # CTRF for pytest
 
 Pytest implementation of Common Test Report Format (CTRF) for test results.  
 Test report will be generated in JSON format.  
 Test report can be used to prettify the report in GitHub Actions with [github-actions-ctrf](https://github.com/ctrf-io/github-actions-ctrf).  
 Do not worry if report in GitHub does not appear immediately. It takes some time to process the report. 
 
@@ -80,14 +65,20 @@
   }
 }
 ```
 
 ## Report Example
 ![Example Image](./assets/report_example.png)
 
+## Technical details
+For future me and others who are interested in the technical details of the implementation.  
+The main idea is to handle xdist plugin because without it collecting report is quite straightforward.  
+By the example of putest-json-report plugin, I have learned that different plugins can be registered for the controller and workers node.  
+The `pytest_runtest_logreport` hook in the controller node is used to collect the test results from all the nodes so other nodes can just add some details to the `TestReport` object.
+
 ## Credits
 
 - https://ctrf.io/ -> nice data format
 - https://github.com/numirias/pytest-json-report -> Source of inspiration and dealing with xdist sync
 - https://github.com/testomatio/pytestomatio -> Source of inspiration for creating pytest plugins
 - https://github.com/infopulse/Playwright-course-python -> The report will be used in the demo project as +1 report option
```

### Comparing `pytest_json_ctrf-0.1.2/tests/test_example.py` & `pytest_json_ctrf-0.2.1/tests/test_example.py`

 * *Files identical despite different names*

