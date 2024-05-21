# Comparing `tmp/datasynthesis131-0.0.1.tar.gz` & `tmp/datasynthesis131-0.0.2.tar.gz`

## Comparing `datasynthesis131-0.0.1.tar` & `datasynthesis131-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/DataSynthesis131/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/DataSynthesis131/common/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/DataSynthesis131/common/common.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/DataSynthesis131/metrics131/__init__.py
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/DataSynthesis131/metrics131/quality_evaluator.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/DataSynthesis131/synthesizer131/__init__.py
--rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/DataSynthesis131/synthesizer131/synthesizer.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/LICENSE
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 datasynthesis131-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/DataSynthesis131/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/DataSynthesis131/common/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/DataSynthesis131/common/common.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/DataSynthesis131/metrics131/__init__.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/DataSynthesis131/metrics131/quality_evaluator.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/DataSynthesis131/synthesizer131/__init__.py
+-rw-r--r--   0        0        0     9100 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/DataSynthesis131/synthesizer131/synthesizer.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/LICENSE
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 datasynthesis131-0.0.2/PKG-INFO
```

### Comparing `datasynthesis131-0.0.1/DataSynthesis131/common/common.py` & `datasynthesis131-0.0.2/DataSynthesis131/common/common.py`

 * *Files identical despite different names*

### Comparing `datasynthesis131-0.0.1/DataSynthesis131/metrics131/quality_evaluator.py` & `datasynthesis131-0.0.2/DataSynthesis131/metrics131/quality_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
     def get_visual_evaluation(self):
         all_cols_set = set(self.metadata.get_column_names())
         numerical_cols_set = set(self.metadata.get_column_names(sdtype='numerical'))
         
         cat_cols = list(all_cols_set - numerical_cols_set)
 
-        table_evaluator = TableEvaluator(self.data, self.data_generated, cat_cols=cat_cols)
+        table_evaluator = TableEvaluator(self.data, self.data_generated, cat_cols=cat_cols, verbose=False)
         table_evaluator.evaluate(target_col=self.target_variable)
         table_evaluator.visual_evaluation()
 
     def print_column_plot(self, column_name, word_to_add = ''):
         fig = get_column_plot(
             real_data=self.data,
             synthetic_data=self.data_generated,
```

### Comparing `datasynthesis131-0.0.1/DataSynthesis131/synthesizer131/synthesizer.py` & `datasynthesis131-0.0.2/DataSynthesis131/synthesizer131/synthesizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,17 @@
         logging.getLogger().setLevel(current_logging_level)
     
     def _prepare_dataset(self):
         if (self.generation_params.target_variable is None):
             self._log_info("You did not specify the name of the target variable (target_variable), so the dataset will be clustered and the target_variable will be - \"cluster\".")
             self._add_cluster_label()
             self.target_variable="cluster"
+            self.metadata.add_column(
+                column_name='cluster',
+                sdtype='categorical')
         if (not self.generation_params.with_missing_values):
             self._impute_missing_values(self.data)
 
     def _impute_missing_values(self, data):
         numeric_columns = data.select_dtypes(include=['int64', 'float64']).columns
         categorical_columns = data.select_dtypes(include=['object']).columns
```

### Comparing `datasynthesis131-0.0.1/LICENSE` & `datasynthesis131-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasynthesis131-0.0.1/README.md` & `datasynthesis131-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `datasynthesis131-0.0.1/pyproject.toml` & `datasynthesis131-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DataSynthesis131"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{name = "Marat Elagin", email = "maratelagin@gmail.com"}]
 license = "MIT"
 requires-python = ">=3.8"
 description = "A package for generating synthetic tabular data and evaluating the quality."
 readme = "README.md"
 
 classifiers = [
```

### Comparing `datasynthesis131-0.0.1/PKG-INFO` & `datasynthesis131-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: DataSynthesis131
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for generating synthetic tabular data and evaluating the quality.
 Project-URL: Homepage, https://github.com/MaratElagin/DataSynthesis131
 Project-URL: Issues, https://github.com/MaratElagin/DataSynthesis131/issues
 Author-email: Marat Elagin <maratelagin@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

