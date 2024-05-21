# Comparing `tmp/scores-0.8.1.tar.gz` & `tmp/scores-0.8.2.tar.gz`

## Comparing `scores-0.8.1.tar` & `scores-0.8.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8.1/environment.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.8.1/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.1/py.typed
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8.1/readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.1/setup.cfg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8.1/.binder/postBuild
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8.1/.binder/requirements.txt
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.1/.github/pull_request_template.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 scores-0.8.1/.github/ISSUE_TEMPLATE/new_score.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8.1/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8.1/.github/workflows/run-pre-commit.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/__init__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/functions.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/sample_data.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/typing.py
--rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/utils.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/categorical/__init__.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/categorical/binary_impl.py
--rw-r--r--   0        0        0    21558 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/categorical/contingency_impl.py
--rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/categorical/multicategorical_impl.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/__init__.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/flip_flop_impl.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/murphy_impl.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/quantile_loss_impl.py
--rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/standard_impl.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/emerging/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/pandas/__init__.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/pandas/continuous.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/pandas/typing.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/brier_impl.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/checks.py
--rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/crps_impl.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/roc_impl.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/__init__.py
--rw-r--r--   0        0        0    12438 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/discretise.py
--rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/isoreg_impl.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/matching.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/cdf/__init__.py
--rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/cdf/cdf_functions.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/stats/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/stats/statistical_tests/__init__.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/stats/statistical_tests/acovf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/stats/statistical_tests/diebold_mariano_impl.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.1/.gitignore
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8.1/LICENSE
--rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 scores-0.8.1/README.md
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 scores-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 scores-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8.2/environment.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.8.2/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.2/py.typed
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8.2/readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.2/setup.cfg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8.2/.binder/postBuild
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8.2/.binder/requirements.txt
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.2/.github/pull_request_template.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 scores-0.8.2/.github/ISSUE_TEMPLATE/new_score.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8.2/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8.2/.github/workflows/run-pre-commit.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/functions.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/sample_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/typing.py
+-rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/utils.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/categorical/__init__.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/categorical/binary_impl.py
+-rw-r--r--   0        0        0    21558 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/categorical/contingency_impl.py
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/categorical/multicategorical_impl.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/__init__.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/flip_flop_impl.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/murphy_impl.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/quantile_loss_impl.py
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/standard_impl.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/emerging/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/pandas/__init__.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/pandas/continuous.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/pandas/typing.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/brier_impl.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/checks.py
+-rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/crps_impl.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/roc_impl.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/__init__.py
+-rw-r--r--   0        0        0    12438 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/discretise.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/isoreg_impl.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/matching.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/cdf/__init__.py
+-rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/cdf/cdf_functions.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/stats/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/stats/statistical_tests/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/stats/statistical_tests/acovf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/stats/statistical_tests/diebold_mariano_impl.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.2/.gitignore
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8.2/LICENSE
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 scores-0.8.2/README.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 scores-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 scores-0.8.2/PKG-INFO
```

### Comparing `scores-0.8.1/.pre-commit-config.yaml` & `scores-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/CODE_OF_CONDUCT.md` & `scores-0.8.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/readthedocs.yaml` & `scores-0.8.2/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/.binder/requirements.txt` & `scores-0.8.2/.binder/requirements.txt`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/.github/pull_request_template.md` & `scores-0.8.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `scores-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/.github/ISSUE_TEMPLATE/new_score.md` & `scores-0.8.2/.github/ISSUE_TEMPLATE/new_score.md`

 * *Files 21% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 **I would like the following metric, statistical test or data processing tool to be considered for addition to the `scores` repository**  
 Please briefly describe the metric, statistical test, or tool and why you think it would be useful.
 
 **Please provide a reference that describes the metric, statistical test or data processing tool**  
 Note: if the reference includes multiple versions of the metric, and you are interested in a specific version, please note that (e.g. specify which theorem or corollary). 
 
 **(Please delete this section if not applicable) I intend to submit a pull request for the new metric, statistical test or data processing tool**
-- [ ] Please read the [Contributing Guide](https://scores.readthedocs.io/en/latest/contributing.html#contributing-guide), in particular the [Development Process for a New Score or Metric](https://scores.readthedocs.io/en/latest/contributing.html#development-process-for-a-new-score-or-metric) section
+- [ ] Please read the [Contributing Guide](https://scores.readthedocs.io/en/develop/contributing.html#contributing-guide)
 - [ ] Please read the [pull request checklist](https://github.com/nci/scores/blob/develop/.github/pull_request_template.md)
-- [ ] I understand that, due to practical constraints, it may not always be possible for a metric or statistical test to be added
+- [ ] I understand that, due to practical constraints, it may not always be possible for a metric, statistical test, or tool to be added
```

### Comparing `scores-0.8.1/.github/workflows/python-app.yml` & `scores-0.8.2/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/.github/workflows/run-pre-commit.yml` & `scores-0.8.2/.github/workflows/run-pre-commit.yml`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/__init__.py` & `scores-0.8.2/src/scores/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import scores.functions
 import scores.pandas
 import scores.probability
 import scores.processing
 import scores.sample_data
 import scores.stats.statistical_tests  # noqa: F401
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 __all__ = [
     "scores.categorical",
     "scores.contingency",
     "scores.continuous",
     "scores.functions",
     "scores.pandas",
```

### Comparing `scores-0.8.1/src/scores/functions.py` & `scores-0.8.2/src/scores/functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/sample_data.py` & `scores-0.8.2/src/scores/sample_data.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/typing.py` & `scores-0.8.2/src/scores/typing.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/utils.py` & `scores-0.8.2/src/scores/utils.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/categorical/__init__.py` & `scores-0.8.2/src/scores/categorical/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/categorical/binary_impl.py` & `scores-0.8.2/src/scores/categorical/binary_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/categorical/contingency_impl.py` & `scores-0.8.2/src/scores/categorical/contingency_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/categorical/multicategorical_impl.py` & `scores-0.8.2/src/scores/categorical/multicategorical_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/continuous/__init__.py` & `scores-0.8.2/src/scores/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/continuous/flip_flop_impl.py` & `scores-0.8.2/src/scores/continuous/flip_flop_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/continuous/murphy_impl.py` & `scores-0.8.2/src/scores/continuous/murphy_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/continuous/quantile_loss_impl.py` & `scores-0.8.2/src/scores/continuous/quantile_loss_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/continuous/standard_impl.py` & `scores-0.8.2/src/scores/continuous/standard_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/pandas/continuous.py` & `scores-0.8.2/src/scores/pandas/continuous.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/probability/__init__.py` & `scores-0.8.2/src/scores/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/probability/brier_impl.py` & `scores-0.8.2/src/scores/probability/brier_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/probability/checks.py` & `scores-0.8.2/src/scores/probability/checks.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/probability/crps_impl.py` & `scores-0.8.2/src/scores/probability/crps_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/probability/roc_impl.py` & `scores-0.8.2/src/scores/probability/roc_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/processing/__init__.py` & `scores-0.8.2/src/scores/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/processing/discretise.py` & `scores-0.8.2/src/scores/processing/discretise.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/processing/isoreg_impl.py` & `scores-0.8.2/src/scores/processing/isoreg_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/processing/matching.py` & `scores-0.8.2/src/scores/processing/matching.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/processing/cdf/cdf_functions.py` & `scores-0.8.2/src/scores/processing/cdf/cdf_functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/stats/statistical_tests/acovf.py` & `scores-0.8.2/src/scores/stats/statistical_tests/acovf.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/src/scores/stats/statistical_tests/diebold_mariano_impl.py` & `scores-0.8.2/src/scores/stats/statistical_tests/diebold_mariano_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/.gitignore` & `scores-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/LICENSE` & `scores-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scores-0.8.1/README.md` & `scores-0.8.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# Scores: Forecast and Model Verification and Evaluation Software
+# Scores: Verification and Evaluation for Forecasts and Models
 > 
 > **A list of over 50 metrics, statistical techniques and data processing tools contained in `scores` is [available here](https://scores.readthedocs.io/en/latest/included.html).**
 
 `scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the meteorological, climatological and geoscience communities. In addition to supporting the Earth system science communities, it also has wide potential application in machine learning and other domains.
 
-**Notice -- This repository is currently undergoing initial construction and maintenance. It is getting much closer to our goals for version one, but there are a few more things to add. This notice will be removed after the first feature release. In the meantime, please feel free to look around, and don't hesitate to get in touch with any questions (see the contributing guide for how).**
-
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io).  
 Source code is hosted at [github.com/nci/scores](https://github.com/nci/scores).  
 The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Explanation.html).
 
 ## Overview
 Here is a **curated selection** of the metrics, tools and statistical tests included in `scores`:
 
 |                       	| **Description** 	| **Selection of Included Functions** 	|
 |-----------------------	|-----------------	|--------------	|
 | **[Continuous](https://scores.readthedocs.io/en/latest/included.html#continuous)**        	|Scores for evaluating single-valued continuous forecasts.                  	|Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Additive Bias, Multiplicative Bias, Pearson's Correlation Coefficient, Flip-Flop Index, Quantile loss, Murphy score.              	|
 | **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensembles, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
 | **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Rate (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
 | **[Statistical Tests](https://scores.readthedocs.io/en/latest/included.html#statistical-tests)** 	|Tools to conduct statistical tests and generate confidence intervals.                 	|Diebold Mariano.              	|
-| **[Processing Tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretization, Cumulative Density Function Manipulation.              	|
+| **[Processing Tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretisation, Cumulative Density Function Manipulation.              	|
 
 
 `scores` not only includes common scores (e.g. MAE, RMSE), it includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including cumulative distribution functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
 `scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
 
 All of the scores and metrics in this package have undergone a thorough scientific review. Every score has a companion Jupyter Notebook tutorial that demonstrates its use in practice.
```

### Comparing `scores-0.8.1/pyproject.toml` & `scores-0.8.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "scores"
 dynamic = ["version"]
 authors = [
   { name="Tennessee Leeuwenburg", email="tennessee.leeuwenburg@bom.gov.au" },
 ]
 description = """\
 Scores is a package containing mathematical functions \
-for the verification, evaluation and optimisation of model outputs and predictions.
+for the verification, evaluation and optimisation of forecasts, predictions or models.
 """
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
@@ -60,15 +60,16 @@
               "twine",
               "pandoc",
               "pip-tools",
 ]
 all = ["scores[dev,tutorial]"]
 
 [project.urls]
-"Homepage" = "http://www.bom.gov.au"
+"Repository" = "https://github.com/nci/scores" 
+"Documentation" = "https://scores.readthedocs.io/en/latest/"
 
 [tool.hatch.build]
 exclude = [
     "/tutorials/",
     "/docs/",
     "/tests/"
 ]
```

### Comparing `scores-0.8.1/PKG-INFO` & `scores-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.3
 Name: scores
-Version: 0.8.1
-Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of model outputs and predictions.
-Project-URL: Homepage, http://www.bom.gov.au
+Version: 0.8.2
+Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of forecasts, predictions or models.
+Project-URL: Repository, https://github.com/nci/scores
+Project-URL: Documentation, https://scores.readthedocs.io/en/latest/
 Author-email: Tennessee Leeuwenburg <tennessee.leeuwenburg@bom.gov.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: bottleneck
@@ -61,36 +62,34 @@
 Requires-Dist: jupyterlab; extra == 'tutorial'
 Requires-Dist: matplotlib; extra == 'tutorial'
 Requires-Dist: plotly; extra == 'tutorial'
 Requires-Dist: rasterio; extra == 'tutorial'
 Requires-Dist: rioxarray; extra == 'tutorial'
 Description-Content-Type: text/markdown
 
-# Scores: Forecast and Model Verification and Evaluation Software
+# Scores: Verification and Evaluation for Forecasts and Models
 > 
 > **A list of over 50 metrics, statistical techniques and data processing tools contained in `scores` is [available here](https://scores.readthedocs.io/en/latest/included.html).**
 
 `scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the meteorological, climatological and geoscience communities. In addition to supporting the Earth system science communities, it also has wide potential application in machine learning and other domains.
 
-**Notice -- This repository is currently undergoing initial construction and maintenance. It is getting much closer to our goals for version one, but there are a few more things to add. This notice will be removed after the first feature release. In the meantime, please feel free to look around, and don't hesitate to get in touch with any questions (see the contributing guide for how).**
-
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io).  
 Source code is hosted at [github.com/nci/scores](https://github.com/nci/scores).  
 The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Explanation.html).
 
 ## Overview
 Here is a **curated selection** of the metrics, tools and statistical tests included in `scores`:
 
 |                       	| **Description** 	| **Selection of Included Functions** 	|
 |-----------------------	|-----------------	|--------------	|
 | **[Continuous](https://scores.readthedocs.io/en/latest/included.html#continuous)**        	|Scores for evaluating single-valued continuous forecasts.                  	|Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Additive Bias, Multiplicative Bias, Pearson's Correlation Coefficient, Flip-Flop Index, Quantile loss, Murphy score.              	|
 | **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensembles, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
 | **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Rate (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
 | **[Statistical Tests](https://scores.readthedocs.io/en/latest/included.html#statistical-tests)** 	|Tools to conduct statistical tests and generate confidence intervals.                 	|Diebold Mariano.              	|
-| **[Processing Tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretization, Cumulative Density Function Manipulation.              	|
+| **[Processing Tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretisation, Cumulative Density Function Manipulation.              	|
 
 
 `scores` not only includes common scores (e.g. MAE, RMSE), it includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including cumulative distribution functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
 `scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
 
 All of the scores and metrics in this package have undergone a thorough scientific review. Every score has a companion Jupyter Notebook tutorial that demonstrates its use in practice.
```

