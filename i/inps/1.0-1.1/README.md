# Comparing `tmp/inps-1.0.tar.gz` & `tmp/inps-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inps-1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "inps-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `inps-1.0.tar` & `inps-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-03-11 11:35:06.767079 inps-1.0/LICENSE
--rw-r--r--   0        0        0     8230 2024-03-11 11:40:51.129490 inps-1.0/README.md
--rw-r--r--   0        0        0     8637 2024-03-11 11:30:17.819048 inps-1.0/data/ED/nonprobEd.parquet
--rw-r--r--   0        0        0    71209 2024-03-11 11:30:17.819048 inps-1.0/data/ED/probEd.parquet
--rw-r--r--   0        0        0   163748 2024-03-11 11:30:17.822382 inps-1.0/data/covid/nonprobCovid.parquet
--rw-r--r--   0        0        0     9915 2024-03-11 11:30:17.822382 inps-1.0/data/covid/probCovid.parquet
--rw-r--r--   0        0        0    57744 2024-03-11 11:30:17.822382 inps-1.0/data/health/censusHealth.parquet
--rw-r--r--   0        0        0     7162 2024-03-11 11:30:17.822382 inps-1.0/data/health/nonprobHealth.parquet
--rw-r--r--   0        0        0     6539 2024-03-11 11:37:16.004576 inps-1.0/guide.py
--rw-r--r--   0        0        0     7117 2024-02-15 11:10:49.613034 inps-1.0/inps.py
--rw-r--r--   0        0        0      497 2024-03-11 11:47:26.342800 inps-1.0/pyproject.toml
--rw-r--r--   0        0        0     4925 2024-03-11 11:41:43.599904 inps-1.0/test.py
--rw-r--r--   0        0        0     8698 1970-01-01 00:00:00.000000 inps-1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-21 17:07:56.809071 inps-1.1/LICENSE
+-rw-r--r--   0        0        0     8230 2024-05-21 17:07:56.809071 inps-1.1/README.md
+-rw-r--r--   0        0        0     8637 2024-05-21 17:07:56.809071 inps-1.1/data/ED/nonprobEd.parquet
+-rw-r--r--   0        0        0    71209 2024-05-21 17:07:56.812404 inps-1.1/data/ED/probEd.parquet
+-rw-r--r--   0        0        0   163748 2024-05-21 17:07:56.812404 inps-1.1/data/covid/nonprobCovid.parquet
+-rw-r--r--   0        0        0     9915 2024-05-21 17:07:56.812404 inps-1.1/data/covid/probCovid.parquet
+-rw-r--r--   0        0        0    57744 2024-05-21 17:07:56.812404 inps-1.1/data/health/censusHealth.parquet
+-rw-r--r--   0        0        0     7162 2024-05-21 17:07:56.812404 inps-1.1/data/health/nonprobHealth.parquet
+-rw-r--r--   0        0        0     6539 2024-05-21 17:07:56.812404 inps-1.1/guide.py
+-rw-r--r--   0        0        0     7097 2024-03-12 18:53:36.831633 inps-1.1/inps.py
+-rw-r--r--   0        0        0      497 2024-05-21 17:08:35.965426 inps-1.1/pyproject.toml
+-rw-r--r--   0        0        0     4925 2024-05-21 17:07:56.812404 inps-1.1/test.py
+-rw-r--r--   0        0        0     8698 1970-01-01 00:00:00.000000 inps-1.1/PKG-INFO
```

### Comparing `inps-1.0/LICENSE` & `inps-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inps-1.0/README.md` & `inps-1.1/README.md`

 * *Files identical despite different names*

### Comparing `inps-1.0/data/ED/nonprobEd.parquet` & `inps-1.1/data/ED/nonprobEd.parquet`

 * *Files identical despite different names*

### Comparing `inps-1.0/data/ED/probEd.parquet` & `inps-1.1/data/ED/probEd.parquet`

 * *Files identical despite different names*

### Comparing `inps-1.0/data/covid/nonprobCovid.parquet` & `inps-1.1/data/covid/nonprobCovid.parquet`

 * *Files identical despite different names*

### Comparing `inps-1.0/data/covid/probCovid.parquet` & `inps-1.1/data/covid/probCovid.parquet`

 * *Files identical despite different names*

### Comparing `inps-1.0/data/health/censusHealth.parquet` & `inps-1.1/data/health/censusHealth.parquet`

 * *Files identical despite different names*

### Comparing `inps-1.0/data/health/nonprobHealth.parquet` & `inps-1.1/data/health/nonprobHealth.parquet`

 * *Files identical despite different names*

### Comparing `inps-1.0/guide.py` & `inps-1.1/guide.py`

 * *Files identical despite different names*

### Comparing `inps-1.0/inps.py` & `inps-1.1/inps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 """Python package for statistical inference from non-probability samples"""
 
-__version__ = "1.0"
+__version__ = "1.1"
 
 from math import sqrt
 import numpy as np
 import pandas as pd
+import sklearn
 from pandas.api.types import is_numeric_dtype
 from scipy.stats import iqr
 from sklearn.compose import ColumnTransformer
 from sklearn.compose import make_column_selector as column_selector
 from sklearn.pipeline import Pipeline
 from sklearn.impute import SimpleImputer
 from sklearn.preprocessing import RobustScaler
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.model_selection import StratifiedKFold
 from sklearn.linear_model import RidgeCV, LogisticRegressionCV
 
-class PreprocessEstimator(Pipeline):
-	def __init__(self, **kwargs):
-		super().__init__((
-			("preprocess", kwargs["preprocess"]),
-			("estimator", kwargs["estimator"])
-		))
-	
-	def fit(self, X, y, sample_weight = None):
-		if sample_weight is None:
-			return super().fit(X, y)
-		else:
-			return super().fit(X, y, estimator__sample_weight = sample_weight)
+sklearn.set_config(enable_metadata_routing = True)
 
 def default_preprocess(**kwargs):
-	return ColumnTransformer((
-		("numeric", Pipeline((
+	return ColumnTransformer([
+		("numeric", Pipeline([
 			("normalizer", RobustScaler()),
 			("imputer", SimpleImputer(strategy = 'median', add_indicator = True, copy = False))
-		)), column_selector(dtype_include = 'number')),
+		]), column_selector(dtype_include = 'number')),
 		("categorical",
 			OneHotEncoder(drop = 'if_binary', min_frequency = .05, handle_unknown = 'infrequent_if_exist'),
 		column_selector(dtype_exclude = 'number'))
-	), **kwargs)
+	], **kwargs)
 
 def make_preprocess_estimator(base_estimator, **kwargs):
-	return PreprocessEstimator(preprocess = default_preprocess(**kwargs), estimator = base_estimator)
+	if hasattr(base_estimator, "set_fit_request"):
+		base_estimator = base_estimator.set_fit_request(sample_weight = True)
+	if hasattr(base_estimator, "set_score_request"):
+		base_estimator = base_estimator.set_score_request(sample_weight = True)
+	
+	return Pipeline([
+		("preprocess", default_preprocess(**kwargs)),
+		("estimator", base_estimator)
+	])
 
 def logistic_classifier(**kwargs):
 	return make_preprocess_estimator(LogisticRegressionCV(cv = StratifiedKFold(shuffle = True, random_state = 0), scoring = 'neg_log_loss', max_iter = 1000, **kwargs))
 
 def linear_regressor(**kwargs):
 	return make_preprocess_estimator(RidgeCV(**kwargs))
 
 def calibration_weights(sample, population_totals, weights_column = None, population_size = None, max_steps = 1000, tolerance = 1e-6):
-	X = sample.loc[:, population_totals.index].to_numpy()
+	X = sample.loc[:, population_totals.index].to_numpy(dtype = 'float64')
 	
 	if weights_column is not None:
 		d = sample[weights_column].to_numpy()
 		X = X * d.reshape(-1, 1)
 	elif population_size is not None:
 		d = population_size / X.shape[0]
 		X = X * d
```

### Comparing `inps-1.0/test.py` & `inps-1.1/test.py`

 * *Files identical despite different names*

### Comparing `inps-1.0/PKG-INFO` & `inps-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: inps
-Version: 1.0
+Version: 1.1
 Summary: Python package for statistical inference from non-probability samples
 Author-email: Luis Castro Martín <luiscastro193@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
-Requires-Dist: scikit-learn>=1.1
+Requires-Dist: scikit-learn>=1.5
 Project-URL: Home, https://github.com/luiscastro193/inps
 
 # INPS: Inference from Non-Probability Samples
 
 Python package for statistical inference from non-probability samples.
 
 ## User guide
```

