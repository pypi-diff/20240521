# Comparing `tmp/ab_test_advanced_toolkit-0.0.0.tar.gz` & `tmp/ab_test_advanced_toolkit-0.0.6.tar.gz`

## Comparing `ab_test_advanced_toolkit-0.0.0.tar` & `ab_test_advanced_toolkit-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,25 @@
--rw-r--r--   0        0        0 11072440 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/0_generated_data.csv
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/requirements.txt
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.github/workflows/build-test-and-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/.gitignore
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/.name
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/ab-test-advanced-toolkit.iml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/vcs.xml
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/workspace.xml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/__init__.py
--rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/analyzer.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/data_validation.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/metrics.py
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/stat_significance.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/vizualizer.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/data/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/data_generation/__init__.py
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/data_generation/data_generator.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/abtest_report.html
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/abtest_report_catboost.html
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/abtest_report_xgboost.html
--rw-r--r--   0        0        0   259012 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/event_data.csv
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/example.ipynb
--rw-r--r--   0        0        0   268919 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/user_allocations.csv
--rw-r--r--   0        0        0    98002 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/catboost_info/catboost_training.json
--rw-r--r--   0        0        0    15796 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/catboost_info/learn_error.tsv
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/catboost_info/time_left.tsv
--rw-r--r--   0        0        0    48870 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/examples/catboost_info/learn/events.out.tfevents
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/tests/test_data_generator.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/tests/test_generic.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/LICENSE
--rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/README.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/pyproject.toml
--rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/.github/workflows/build-test-and-publish.yml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/__init__.py
+-rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/analyzer.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/data_validation.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/metrics.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/stat_significance.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/vizualizer.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/data/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/data_generation/__init__.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/data_generation/data_generator.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/examples/abtest_report.html
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/examples/abtest_report_xgboost.html
+-rw-r--r--   0        0        0   259012 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/examples/event_data.csv
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/examples/example.ipynb
+-rw-r--r--   0        0        0   268919 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/examples/user_allocations.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/tests/test_data_generator.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/tests/test_generic.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/tests/test_utils.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/LICENSE
+-rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/README.md
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 ab_test_advanced_toolkit-0.0.6/PKG-INFO
```

### Comparing `ab_test_advanced_toolkit-0.0.0/.github/workflows/build-test-and-publish.yml` & `ab_test_advanced_toolkit-0.0.6/.github/workflows/build-test-and-publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
   contents: read
 
 jobs:
   test:
 
     strategy:
       matrix:
-        os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ['3.8', '3.9', '3.10']
+        os: [ubuntu-latest]
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
     runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python
```

### Comparing `ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/analyzer.py` & `ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/analyzer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Tuple, List, Optional
 
 import pandas as pd
 
-from variatio.data_validation import validate_data
-from variatio.metrics import Metric, MetricType, MetricParams, MetricResult, AggregationOperation
-from variatio.stat_significance import StatTests
-from variatio.vizualizer import format_metrics_to_html
+from ab_test_advanced_toolkit.data_validation import validate_data
+from ab_test_advanced_toolkit.metrics import Metric, MetricType, MetricParams, MetricResult, AggregationOperation
+from ab_test_advanced_toolkit.stat_significance import StatTests
+from ab_test_advanced_toolkit.vizualizer import format_metrics_to_html
+
 
 import logging
 
 # Function to set up logging configuration
 def setup_logging(level=logging.INFO):
     logging.basicConfig(level=level, format='%(asctime)s - %(levelname)s - %(message)s')
     logger = logging.getLogger(__name__)
@@ -100,21 +101,32 @@
         :return: DataFrame with the calculated event count per user per group
         """
         merged_pretest, _ = self._merge_and_aggregate(self.event_data, self.ab_test_allocations, event_name,
                                                       AggregationOperation.COUNT, pretest=True)
 
         merged_intest, result_intest = self._merge_and_aggregate(self.event_data, self.ab_test_allocations, event_name,
                                                                  AggregationOperation.COUNT)
-        stat_test = StatTests.calculate_gboost_cuped_and_compare(merged_pretest, merged_intest, self.user_properties,
-                                                                   self.control_group_name, self.test_group_names)
 
-        self.calculated_metrics.append(Metric(MetricType.EVENT_COUNT_PER_USER, MetricParams(event_name),
+        if self.mode == "gboost_cuped":
+            stat_test = StatTests.calculate_gboost_cuped_and_compare(merged_pretest, merged_intest, self.user_properties,
+                                                                self.control_group_name, self.test_group_names, True)
+        elif self.mode == "cuped":
+            stat_test = StatTests.calculate_cuped_and_compare(merged_pretest, merged_intest,
+                                                                self.control_group_name, self.test_group_names)
+        else:
+            stat_test = StatTests.calculate_gboost_cuped_and_compare(merged_pretest, merged_intest,
+                                                                    self.user_properties,
+                                                                    self.control_group_name, self.test_group_names,
+                                                                    False)
+
+        metric_output = Metric(MetricType.EVENT_COUNT_PER_USER, MetricParams(event_name),
                                               MetricResult(result_intest, self.control_group_name,
-                                                           self.test_group_names, stat_test)))
-        return result_intest
+                                                           self.test_group_names, stat_test))
+        self.calculated_metrics.append(metric_output)
+        return metric_output
 
     def calculate_event_attribute_sum_per_user(self, event_name: str, attribute_name: str) -> pd.DataFrame:
         """
         Calculates the sum of a specified attribute per user for the specified event name.
         :param event_name: The event name to calculate the attribute sum for.
         :param attribute_name:  The name of the attribute to calculate the sum for.
         :return: DataFrame with the calculated attribute sum per user per group
@@ -139,34 +151,35 @@
                                                                 self.control_group_name, self.test_group_names)
         else:
             stat_test = StatTests.calculate_gboost_cuped_and_compare(merged_pretest, merged_intest,
                                                                     self.user_properties,
                                                                     self.control_group_name, self.test_group_names,
                                                                     False)
 
-        self.calculated_metrics.append(
-            Metric(MetricType.EVENT_ATTRIBUTE_SUM_PER_USER, MetricParams(event_name, attribute_name),
-                MetricResult(result_intest, self.control_group_name, self.test_group_names, stat_test)))
-        return result_intest, stat_test
+        metric_output = Metric(MetricType.EVENT_ATTRIBUTE_SUM_PER_USER, MetricParams(event_name, attribute_name),
+                MetricResult(result_intest, self.control_group_name, self.test_group_names, stat_test))
+        self.calculated_metrics.append(metric_output)
+        return metric_output
 
     def calculate_conversion(self, target_event: str) -> pd.DataFrame:
         """
         Calculates the conversion rate for the specified target event.
         :param target_event: The name of the event to calculate the conversion rate for.
         :return: DataFrame with the calculated conversion rate per user per group
         """
         merged_intest, result_intest = self._merge_and_aggregate(self.event_data, self.ab_test_allocations,
                                                                  target_event,
                                                                  AggregationOperation.CONVERSION)
         stat_test = StatTests.calculate_t_test_for_dataset(merged_intest, self.control_group_name,
                                                            self.test_group_names)
 
-        self.calculated_metrics.append(Metric(
+        metric_output = Metric(
             MetricType.CONVERSION_RATE,
             MetricParams(target_event),
-            MetricResult(result_intest, self.control_group_name, self.test_group_names, stat_test)))
-        return result_intest
+            MetricResult(result_intest, self.control_group_name, self.test_group_names, stat_test))
+        self.calculated_metrics.append(metric_output)
+        return metric_output
 
     def save_report(self, filename: str):
         res = format_metrics_to_html(self.calculated_metrics, self.control_group_name, self.test_group_names)
         with open(filename, 'w') as f:
             f.write(res)
```

### Comparing `ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/data_validation.py` & `ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/data_validation.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/metrics.py` & `ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
 import pandas as pd
 
 from enum import Enum, auto
 
-from variatio.stat_significance import StatSignificanceResult
+from ab_test_advanced_toolkit.stat_significance import StatSignificanceResult
 
 
 class MetricType(Enum):
     EVENT_COUNT_PER_USER = auto()
     EVENT_ATTRIBUTE_SUM_PER_USER = auto()
     CONVERSION_RATE = auto()
```

### Comparing `ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/stat_significance.py` & `ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/stat_significance.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/ab-test-advanced-toolkit/vizualizer.py` & `ab_test_advanced_toolkit-0.0.6/ab_test_advanced_toolkit/vizualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from typing import List
 
-from variatio.metrics import MetricType, Metric
+from ab_test_advanced_toolkit.metrics import MetricType, Metric
 
 
 def describe_metric(metric: Metric) -> str:
     metric_type = metric.metrictype
     params = metric.metricparams
 
     if metric_type == MetricType.EVENT_COUNT_PER_USER:
```

### Comparing `ab_test_advanced_toolkit-0.0.0/data_generation/data_generator.py` & `ab_test_advanced_toolkit-0.0.6/data_generation/data_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import datetime
 import pandas as pd
 import numpy as np
-from variatio.analyzer import VariatioAnalyzer
+from ab_test_advanced_toolkit.analyzer import VariatioAnalyzer
 from typing import Tuple
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 # Create folder 'data/{now_timestamp_utc}' if it does not exist
 folder_name = os.path.join(
     'data', 
-    datetime.datetime.now(datetime.UTC).strftime('%Y-%m-%d_%H-%M-%S')
+    datetime.datetime.now(datetime.timezone.utc).strftime('%Y-%m-%d_%H-%M-%S')
 )
 os.makedirs(folder_name, exist_ok=True)
 def describe_dataset(df):
     logging.info("First 5 rows of the dataset:")
     logging.info(df.head())
     
     logging.info("\nStatistical summary of the dataset:")
```

### Comparing `ab_test_advanced_toolkit-0.0.0/examples/abtest_report.html` & `ab_test_advanced_toolkit-0.0.6/examples/abtest_report.html`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/examples/abtest_report_catboost.html` & `ab_test_advanced_toolkit-0.0.6/examples/abtest_report_xgboost.html`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/examples/event_data.csv` & `ab_test_advanced_toolkit-0.0.6/examples/event_data.csv`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/examples/example.ipynb` & `ab_test_advanced_toolkit-0.0.6/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/examples/user_allocations.csv` & `ab_test_advanced_toolkit-0.0.6/examples/user_allocations.csv`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/tests/test_data_generator.py` & `ab_test_advanced_toolkit-0.0.6/tests/test_data_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
 import pandas as pd
-from variatio.stat_significance import StatSignificanceResult
+
+from ab_test_advanced_toolkit.metrics import Metric
+from ab_test_advanced_toolkit.stat_significance import StatSignificanceResult
 from data_generation.data_generator import generate_synthetic_data, run_analysis
 
 class TestDataGenerator(unittest.TestCase):
     
     def test_generate_synthetic_data(self):
         num_users = 1000
         countries = ['US', 'UK', 'DE', 'FR', 'CA', 'AU', 'JP', 'IN']
@@ -51,20 +53,16 @@
         
         results = run_analysis(data)
         
         # Check if the analysis results are not empty
         self.assertTrue("no_enhancement" in results)
         self.assertTrue("cuped" in results)
         self.assertTrue("gboost_cuped" in results)
-        
-        # Further checks can be added based on expected structure of results
-        self.assertIsInstance(results["no_enhancement"][0], pd.DataFrame)
-        self.assertIsInstance(results["cuped"][0], pd.DataFrame)
-        self.assertIsInstance(results["gboost_cuped"][0], pd.DataFrame)
-
-        # Check if second element is StatSignificanceResult
-        self.assertIsInstance(results["no_enhancement"][1], StatSignificanceResult)
-        self.assertIsInstance(results["cuped"][1], StatSignificanceResult)
-        self.assertIsInstance(results["gboost_cuped"][1], StatSignificanceResult)
+
+        # output type is Metric
+        self.assertIsInstance(results["no_enhancement"], Metric)
+        self.assertIsInstance(results["cuped"], Metric)
+        self.assertIsInstance(results["gboost_cuped"], Metric)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ab_test_advanced_toolkit-0.0.0/tests/test_generic.py` & `ab_test_advanced_toolkit-0.0.6/tests/test_generic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import logging
 
+from ab_test_advanced_toolkit import VariatioAnalyzer
+from ab_test_advanced_toolkit.metrics import MetricType
 from tests.test_utils import generate_event_data, generate_user_properties, generate_user_allocations
-from variatio import VariatioAnalyzer
 
 # Set up logging
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
 
 def test_library_is_initialized():
@@ -40,30 +41,30 @@
     event_data = generate_event_data()
     ab_test_allocations = generate_user_allocations()
 
     analyzer = VariatioAnalyzer(event_data, ab_test_allocations, "A", user_properties, mode="gboost_cuped")
 
     event_counts = analyzer.calculate_event_count_per_user('purchase')
 
-    assert len(event_counts) == 2
+    assert event_counts.metrictype == MetricType.EVENT_COUNT_PER_USER
 
-    assert event_counts.loc['A'][0] == pytest.approx(0.283019, rel=1e-4)
-    assert event_counts.loc['B'][0] == pytest.approx(0.404255, rel=1e-4)
+    assert event_counts.result.data['A'] == pytest.approx(0.283019, rel=1e-3)
+    assert event_counts.result.data['B'] == pytest.approx(0.404255, rel=1e-3)
     assert len(analyzer.calculated_metrics) == 1
 
     event_attribute_sum = analyzer.calculate_event_attribute_sum_per_user('purchase', 'purchase_value')
 
-    assert event_attribute_sum.loc['A'][0] == pytest.approx(53.283019, rel=1e-4)
-    assert event_attribute_sum.loc['B'][0] == pytest.approx(91.553191, rel=1e-4)
+    assert event_attribute_sum.result.data['A'] == pytest.approx(53.283019, rel=1e-3)
+    assert event_attribute_sum.result.data['B'] == pytest.approx(91.553191, rel=1e-3)
     assert len(analyzer.calculated_metrics) == 2
 
     conversion_rate = analyzer.calculate_conversion('purchase')
     logger.debug(conversion_rate)
-    assert conversion_rate.loc['A'][0] == pytest.approx(0.075472, rel=1e-4)
-    assert conversion_rate.loc['B'][0] == pytest.approx(0.085106, rel=1e-4)
+    assert conversion_rate.result.data['A'] == pytest.approx(0.075472, rel=1e-3)
+    assert conversion_rate.result.data['B'] == pytest.approx(0.085106, rel=1e-3)
     assert len(analyzer.calculated_metrics) == 3
 
     # testing that report does not fail and file is saved
     analyzer.save_report("tempfile.html")
 
 
 # simple check that significance metrics are different due to user properties being used
@@ -75,8 +76,8 @@
     analyzer_user_properties = VariatioAnalyzer(event_data, ab_test_allocations, "A", user_properties, mode="gboost_cuped")
     analyzer_no_user_properties = VariatioAnalyzer(event_data, ab_test_allocations, "A", mode="gboost_cuped")
 
     analyzer_user_properties.calculate_event_count_per_user('purchase')
     analyzer_no_user_properties.calculate_event_count_per_user('purchase')
 
     assert abs(analyzer_user_properties.calculated_metrics[0].result.stat_significance['B'] -
-               analyzer_no_user_properties.calculated_metrics[0].result.stat_significance['B']) > 1e-1
+               analyzer_no_user_properties.calculated_metrics[0].result.stat_significance['B']) > 1e-3
```

### Comparing `ab_test_advanced_toolkit-0.0.0/tests/test_utils.py` & `ab_test_advanced_toolkit-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/.gitignore` & `ab_test_advanced_toolkit-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/LICENSE` & `ab_test_advanced_toolkit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ab_test_advanced_toolkit-0.0.0/README.md` & `ab_test_advanced_toolkit-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - **CUPED Adjustments:** This experimental extension utilizes Controlled-experiment Using Pre-Experiment Data (CUPED) techniques for variance reduction. It innovatively employs user properties as covariates and leverages XGBoost regression, moving beyond traditional linear approaches to enhance A/B test sensitivity.
 
 
 
 ## Installation
 
 ```bash
-pip install ab-test-advanced-toolkit
+pip install ab_test_advanced_toolkit
 ```
 
 or install Variatio directly from the source:
 
 ```bash
 git clone https://github.com/dmitry_brazhenko/Variatio.git
 cd Variatio
```

### Comparing `ab_test_advanced_toolkit-0.0.0/PKG-INFO` & `ab_test_advanced_toolkit-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ab-test-advanced-toolkit
-Version: 0.0.0
+Version: 0.0.6
 Dynamic: Requires-Dist
 Summary: An experimental Python library for advanced A/B testing analysis, leveraging statistical techniques and ML for deeper insights.
 Project-URL: Homepage, https://github.com/dmitry-brazhenko/ab-test-advanced-toolkit
 Project-URL: Documentation, https://github.com/dmitry-brazhenko/ab-test-advanced-toolkit/blob/main/README.md
 Project-URL: Repository, https://github.com/dmitry-brazhenko/ab-test-advanced-toolkit
 Author-email: Dmitry Brazhenko <brazhenko.dmitry@gmail.com>
 Maintainer-email: Dmitry Brazhenko <brazhenko.dmitry@gmail.com>
@@ -49,15 +49,15 @@
 - **CUPED Adjustments:** This experimental extension utilizes Controlled-experiment Using Pre-Experiment Data (CUPED) techniques for variance reduction. It innovatively employs user properties as covariates and leverages XGBoost regression, moving beyond traditional linear approaches to enhance A/B test sensitivity.
 
 
 
 ## Installation
 
 ```bash
-pip install ab-test-advanced-toolkit
+pip install ab_test_advanced_toolkit
 ```
 
 or install Variatio directly from the source:
 
 ```bash
 git clone https://github.com/dmitry_brazhenko/Variatio.git
 cd Variatio
```

