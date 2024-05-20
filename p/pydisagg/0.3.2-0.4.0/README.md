# Comparing `tmp/pydisagg-0.3.2.tar.gz` & `tmp/pydisagg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisagg-0.3.2.tar", last modified: Wed Oct 18 17:15:29 2023, max compression
+gzip compressed data, was "pydisagg-0.4.0.tar", last modified: Mon May 20 22:55:14 2024, max compression
```

## Comparing `pydisagg-0.3.2.tar` & `pydisagg-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 owlx       (502) staff       (20)        0 2023-10-18 17:15:29.671130 pydisagg-0.3.2/
--rw-r--r--   0 owlx       (502) staff       (20)     1328 2022-12-02 22:58:57.000000 pydisagg-0.3.2/LICENSE
--rw-r--r--   0 owlx       (502) staff       (20)     3199 2023-10-18 17:15:29.671437 pydisagg-0.3.2/PKG-INFO
--rw-r--r--   0 owlx       (502) staff       (20)     2840 2023-08-24 17:52:23.000000 pydisagg-0.3.2/README.md
--rw-r--r--   0 owlx       (502) staff       (20)       81 2022-12-02 22:58:57.000000 pydisagg-0.3.2/pyproject.toml
--rw-r--r--   0 owlx       (502) staff       (20)      615 2023-10-18 17:15:29.693429 pydisagg-0.3.2/setup.cfg
--rw-r--r--   0 owlx       (502) staff       (20)       69 2022-12-02 22:58:57.000000 pydisagg-0.3.2/setup.py
-drwxr-xr-x   0 owlx       (502) staff       (20)        0 2023-10-18 17:15:29.612264 pydisagg-0.3.2/src/
-drwxr-xr-x   0 owlx       (502) staff       (20)        0 2023-10-18 17:15:29.643238 pydisagg-0.3.2/src/pydisagg/
--rw-r--r--   0 owlx       (502) staff       (20)    24184 2023-08-24 17:52:23.000000 pydisagg-0.3.2/src/pydisagg/DisaggModel.py
--rw-r--r--   0 owlx       (502) staff       (20)      722 2023-08-24 17:52:23.000000 pydisagg-0.3.2/src/pydisagg/ParameterTransformation.py
--rw-r--r--   0 owlx       (502) staff       (20)      119 2023-08-24 17:52:23.000000 pydisagg-0.3.2/src/pydisagg/__init__.py
--rw-r--r--   0 owlx       (502) staff       (20)    10451 2023-10-18 17:06:55.000000 pydisagg-0.3.2/src/pydisagg/disaggregate.py
--rw-r--r--   0 owlx       (502) staff       (20)     1812 2023-08-24 17:52:23.000000 pydisagg-0.3.2/src/pydisagg/models.py
--rw-r--r--   0 owlx       (502) staff       (20)     1888 2023-08-24 17:52:23.000000 pydisagg-0.3.2/src/pydisagg/transformations.py
-drwxr-xr-x   0 owlx       (502) staff       (20)        0 2023-10-18 17:15:29.661798 pydisagg-0.3.2/src/pydisagg.egg-info/
--rw-r--r--   0 owlx       (502) staff       (20)     3199 2023-10-18 17:15:28.000000 pydisagg-0.3.2/src/pydisagg.egg-info/PKG-INFO
--rw-r--r--   0 owlx       (502) staff       (20)      519 2023-10-18 17:15:29.000000 pydisagg-0.3.2/src/pydisagg.egg-info/SOURCES.txt
--rw-r--r--   0 owlx       (502) staff       (20)        1 2023-10-18 17:15:28.000000 pydisagg-0.3.2/src/pydisagg.egg-info/dependency_links.txt
--rw-r--r--   0 owlx       (502) staff       (20)        1 2023-02-18 23:44:43.000000 pydisagg-0.3.2/src/pydisagg.egg-info/not-zip-safe
--rw-r--r--   0 owlx       (502) staff       (20)       88 2023-10-18 17:15:28.000000 pydisagg-0.3.2/src/pydisagg.egg-info/requires.txt
--rw-r--r--   0 owlx       (502) staff       (20)        9 2023-10-18 17:15:28.000000 pydisagg-0.3.2/src/pydisagg.egg-info/top_level.txt
-drwxr-xr-x   0 owlx       (502) staff       (20)        0 2023-10-18 17:15:29.669334 pydisagg-0.3.2/tests/
--rw-r--r--   0 owlx       (502) staff       (20)     1012 2023-08-24 17:52:23.000000 pydisagg-0.3.2/tests/test_splitting_consistency.py
--rw-r--r--   0 owlx       (502) staff       (20)      864 2023-08-24 17:52:23.000000 pydisagg-0.3.2/tests/test_transformation_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:55:14.471223 pydisagg-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-20 22:54:46.000000 pydisagg-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-20 22:55:14.471223 pydisagg-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-20 22:54:46.000000 pydisagg-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-20 22:54:46.000000 pydisagg-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:55:14.471223 pydisagg-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:55:14.467223 pydisagg-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:55:14.467223 pydisagg-0.4.0/src/pydisagg/
+-rw-r--r--   0 runner    (1001) docker     (127)    24999 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/DisaggModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/ParameterTransformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/disaggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:55:14.471223 pydisagg-0.4.0/src/pydisagg/ihme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/ihme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/ihme/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/ihme/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-20 22:54:46.000000 pydisagg-0.4.0/src/pydisagg/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:55:14.471223 pydisagg-0.4.0/src/pydisagg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-20 22:55:14.000000 pydisagg-0.4.0/src/pydisagg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 22:55:14.000000 pydisagg-0.4.0/src/pydisagg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:55:14.000000 pydisagg-0.4.0/src/pydisagg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 22:55:14.000000 pydisagg-0.4.0/src/pydisagg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 22:55:14.000000 pydisagg-0.4.0/src/pydisagg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:55:14.471223 pydisagg-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-20 22:54:46.000000 pydisagg-0.4.0/tests/test_disaggregate_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-20 22:54:46.000000 pydisagg-0.4.0/tests/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-20 22:54:46.000000 pydisagg-0.4.0/tests/test_splitting_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 22:54:46.000000 pydisagg-0.4.0/tests/test_transformation_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-20 22:54:46.000000 pydisagg-0.4.0/tests/test_validator.py
```

### Comparing `pydisagg-0.3.2/LICENSE` & `pydisagg-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydisagg-0.3.2/PKG-INFO` & `pydisagg-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 Metadata-Version: 2.1
 Name: pydisagg
-Version: 0.3.2
-Summary: UNKNOWN
-Home-page: https://github.com/ihmeuw-msca/splitting-python-package
-Author: IHME Math Sciences
-Author-email: ihme.math.sciences@gmail.com
+Version: 0.4.0
+Author-email: IHME Math Sciences <ihme.math.sciences@gmail.com>
 License: BSD 2-Clause License
-Platform: UNKNOWN
+Project-URL: homepage, https://github.com/ihmeuw-msca/pydisagg
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: doc
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: pydantic
 
 [![PyPI](https://img.shields.io/pypi/v/pydisagg)](https://pypi.org/project/pydisagg/)
 ![Python](https://img.shields.io/badge/python-3.8,_3.9-blue.svg)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ihmeuw-msca/pyDisagg/build.yml)
 [![GitHub](https://img.shields.io/github/license/ihmeuw-msca/pyDisagg)](./LICENSE)
 
 ## Dissaggregation under Generalized Proportionality Assumptions
@@ -38,9 +50,7 @@
 
 ## Current Package Capabilities and Models
 Currently, the multiplicative-in-rate model RateMultiplicativeModel with $T(x)=\log(x)$ and the Log Modified Odds model LMO_model(m) with $T(x)=\log(\frac{x}{1-x^{m}})$ are implemented. Note that the LMO_model with m=1 gives a multiplicative in odds model.
 
 A useful (but slightly wrong) analogy is that the multiplicative-in-rate is to the multiplicative-in-odds model as ordinary least squares is to logistic regression in terms of the relationship between covariates and output (not in terms of anything like the likelihood)
 
 Increasing m in the model LMO_model(m) gives results that are more similar to the multiplicative-in-rate model currently in use, while preserving the property that rate estimates are bounded by 1. 
-
-
```

### Comparing `pydisagg-0.3.2/README.md` & `pydisagg-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pydisagg-0.3.2/src/pydisagg/DisaggModel.py` & `pydisagg-0.4.0/src/pydisagg/DisaggModel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 """Module with main DisaggModel class and algorithmic implementation"""
+
 from typing import Optional
 
 import numpy as np
 from numpy.typing import NDArray
 from scipy.optimize import root_scalar
-from scipy.stats import norm
 
 from pydisagg.ParameterTransformation import ParameterTransformation
 
 
 class DisaggModel:
     """
     Model for solving splitting/disaggregation problems
 
     parameter_transformation is a class attribute that defines the generalized proportionality assumption that we want to make
-    It should be a ParameterTransformation object which is callable, has an inverse function, and has a derivative. 
+    It should be a ParameterTransformation object which is callable, has an inverse function, and has a derivative.
 
     Notes
     -----
     A possibly confusing code and notation choice is that we enforce
     multiplicativity in some space, but fit an additive parameter beta throughout
 
     We do this because it works better with the delta method calculations, and we assume that we
     have a log in the transormations so additive factors become multiplicative
 
     """
 
-    def __init__(
-        self,
-        parameter_transformation: ParameterTransformation
-    ):
+    def __init__(self, parameter_transformation: ParameterTransformation):
         """Initializes a dissaggregation model
 
         Parameters
         ----------
         parameter_transformation : ParameterTransformation
             Transformation to apply to rate pattern values
         """
 
         self.T = parameter_transformation
         self.T_inverse = parameter_transformation.inverse
         self.T_diff = parameter_transformation.diff
 
-    def predict_rate(
-        self,
-        beta: float,
-        rate_pattern: NDArray
-    ) -> NDArray:
+    def predict_rate(self, beta: float, rate_pattern: NDArray) -> NDArray:
         """
         Predicts the rate in each bucket
 
         Parameters
         ----------
         beta : float
             beta paramter, log of rescaling parameter
@@ -62,35 +55,31 @@
         -------
         NDArray
             estimated occurrences in each bucket
 
         """
         return self.T_inverse(beta + self.T(rate_pattern))
 
-    def rate_diff_beta(
-        self,
-        beta: float,
-        rate_pattern: NDArray
-    ) -> NDArray:
+    def rate_diff_beta(self, beta: float, rate_pattern: NDArray) -> NDArray:
         """Computes the derivative of the predicted rates with respect to beta
 
         Parameters
         ----------
         beta : float
             beta paramter, log of rescaling parameter
         rate_pattern : NDArray
-            rate pattern 
+            rate pattern
         bucket_populations :NDArray
             Populations in each bucket
         Returns
         -------
         NDArray
             derivative of predicted rates in each bucket with respect to beta
         """
-        return 1/self.T_diff(self.T_inverse(beta + self.T(rate_pattern)))
+        return 1 / self.T_diff(self.T_inverse(beta + self.T(rate_pattern)))
 
     def predict_count(
         self,
         beta: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
     ) -> NDArray:
@@ -99,23 +88,23 @@
             multiplicativity in the T-transformed space with the additive parameter beta
 
         Parameters
         ----------
         beta : float
             beta paramter, log of rescaling parameter
         rate_pattern : NDArray
-            rate pattern 
+            rate pattern
         bucket_populations :NDArray
             Populations in each bucket
         Returns
         -------
         NDArray
             Predicted rates in each bucket
         """
-        return self.predict_rate(beta, rate_pattern)*bucket_populations
+        return self.predict_rate(beta, rate_pattern) * bucket_populations
 
     def count_diff_beta(
         self,
         beta: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
     ) -> NDArray:
@@ -123,32 +112,32 @@
         Computes the derivative of the predicted count in each bucket with respect to beta
 
         Parameters
         ----------
         beta : float
             beta paramter, log of rescaling parameter
         rate_pattern : NDArray
-            rate pattern 
+            rate pattern
         bucket_populations :NDArray
             Populations in each bucket
         Returns
         -------
         NDArray
             Derivative of predicted counts in each bucket with respect to beta
         """
-        return self.rate_diff_beta(beta, rate_pattern)*bucket_populations
+        return self.rate_diff_beta(beta, rate_pattern) * bucket_populations
 
     def fit_beta(
         self,
         observed_total: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
         lower_guess: float = -50,
         upper_guess: float = 50,
-        verbose: Optional[int] = 0
+        verbose: Optional[int] = 0,
     ) -> float:
         """Fits the parameter beta to the data
 
         Parameters
         ----------
         observed_total : float
             aggregated observation
@@ -165,22 +154,32 @@
             2 prints the entire rootfinding output, by default 0
 
         Returns
         -------
         float
             computed value for beta
         """
+
         def beta_misfit(beta):
-            return self.H_func(beta, rate_pattern=rate_pattern, bucket_populations=bucket_populations) - observed_total
-        beta_results = root_scalar(beta_misfit, bracket=[
-                                   lower_guess, upper_guess], method='toms748')
+            return (
+                self.H_func(
+                    beta,
+                    rate_pattern=rate_pattern,
+                    bucket_populations=bucket_populations,
+                )
+                - observed_total
+            )
+
+        beta_results = root_scalar(
+            beta_misfit, bracket=[lower_guess, upper_guess], method="toms748"
+        )
         if verbose == 2:
             print(beta_results)
         elif verbose == 1:
-            print(f'beta={beta_results.root}')
+            print(f"beta={beta_results.root}")
         fitted_beta = beta_results.root
         return fitted_beta
 
     def H_func(
         self,
         beta: float,
         rate_pattern: NDArray,
@@ -189,56 +188,59 @@
         """Returns the predicted total function
 
         Parameters
         ----------
         beta : float
             beta paramter, log of rescaling parameter
         rate_pattern : NDArray
-            rate pattern 
+            rate pattern
         bucket_populations :NDArray
             Populations in each bucket
         Returns
         -------
         float
             Predicted total given beta, bucket populations, and rate pattern
             This is matched to observed_total with rootfinding to fit beta
         """
-        return np.sum(self.predict_count(beta, rate_pattern, bucket_populations))
+        return np.sum(
+            self.predict_count(beta, rate_pattern, bucket_populations)
+        )
 
     def H_diff_beta(
         self,
         beta: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
     ) -> float:
         """Returns the derivative of the predicted total function with respect to beta
 
         Parameters
         ----------
         beta : float
             beta paramter, log of rescaling parameter
         rate_pattern : NDArray
-            rate pattern 
+            rate pattern
         bucket_populations :NDArray
             Populations in each bucket
 
         Returns
         -------
         float
             derivative of H_func with respect to beta
         """
-        return np.sum(self.count_diff_beta(beta, rate_pattern, bucket_populations))
+        return np.sum(
+            self.count_diff_beta(beta, rate_pattern, bucket_populations)
+        )
 
     def beta_standard_error(
         self,
         fitted_beta: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
         observed_total_se: float,
-
     ) -> float:
         """Computes delta-method standard error estimate for beta
 
         Parameters
         ----------
         fitted_beta : float
             fitted value of beta. This being fitted is why we don't need what the original observation actually was
@@ -250,17 +252,18 @@
             standard error of the total observed quantity
 
         Returns
         -------
         float
             standard error of beta
         """
-        error_inflation = (1 /
-                           self.H_diff_beta(fitted_beta, rate_pattern, bucket_populations))
-        beta_standard_error = observed_total_se*error_inflation
+        error_inflation = 1 / self.H_diff_beta(
+            fitted_beta, rate_pattern, bucket_populations
+        )
+        beta_standard_error = observed_total_se * error_inflation
         return beta_standard_error
 
     def split_to_rates(
         self,
         observed_total: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
@@ -291,34 +294,42 @@
         reduce_output : bool, by default False
             boolean for whether or not to set groups with zero population to have zero rate
         Returns
         -------
         if observed_total_se is not given, we return
             NDArray
                 predicted counts
-        Otherwise we return 
+        Otherwise we return
             NDArray
                 predicted counts
             NDArray
                 standard error estimates
         """
         fitted_beta = self.fit_beta(
-            observed_total, rate_pattern, bucket_populations, lower_guess, upper_guess
+            observed_total,
+            rate_pattern,
+            bucket_populations,
+            lower_guess,
+            upper_guess,
         )
         rate_point_estimates = self.predict_rate(fitted_beta, rate_pattern)
-        
-        #This is some dirty type casting, if reduce output, we set all groups with population 0 to 0
-        #Otherwise, we're multiplying everything True, which gets casted to 1
-        output_multiplier = ((1-1*reduce_output)+bucket_populations)>0
+
+        # This is some dirty type casting, if reduce output, we set all groups with population 0 to 0
+        # Otherwise, we're multiplying everything True, which gets casted to 1
+        output_multiplier = ((1 - 1 * reduce_output) + bucket_populations) > 0
 
         if observed_total_se is not None:
             standard_errors = self.rate_standard_errors(
-                fitted_beta, rate_pattern, bucket_populations, observed_total_se)
-            return rate_point_estimates*output_multiplier, standard_errors*output_multiplier
-        return rate_point_estimates*output_multiplier
+                fitted_beta, rate_pattern, bucket_populations, observed_total_se
+            )
+            return (
+                rate_point_estimates * output_multiplier,
+                standard_errors * output_multiplier,
+            )
+        return rate_point_estimates * output_multiplier
 
     def rate_standard_errors(
         self,
         fitted_beta,
         rate_pattern,
         bucket_populations,
         observed_total_se,
@@ -333,17 +344,19 @@
             rate pattern
         bucket_populations : NDArray
             populations in each bucket
         observed_total_se : float
             standard error of the total observed quantity
         """
         beta_SE = self.beta_standard_error(
-            fitted_beta, rate_pattern, bucket_populations, observed_total_se)
-        rate_standard_errors = self.rate_diff_beta(
-            fitted_beta, rate_pattern)*beta_SE
+            fitted_beta, rate_pattern, bucket_populations, observed_total_se
+        )
+        rate_standard_errors = (
+            self.rate_diff_beta(fitted_beta, rate_pattern) * beta_SE
+        )
         return rate_standard_errors
 
     def count_split_standard_errors(
         self,
         fitted_beta,
         rate_pattern,
         bucket_populations,
@@ -359,16 +372,20 @@
             rate pattern
         bucket_populations : NDArray
             populations in each bucket
         observed_total_se : float
             standard error of the total observed quantity
         """
         rate_se = self.rate_standard_errors(
-            fitted_beta, rate_pattern, bucket_populations=bucket_populations, observed_total_se=observed_total_se)
-        return rate_se*bucket_populations
+            fitted_beta,
+            rate_pattern,
+            bucket_populations=bucket_populations,
+            observed_total_se=observed_total_se,
+        )
+        return rate_se * bucket_populations
 
     def split_to_counts(
         self,
         observed_total: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
         observed_total_se: Optional[float] = None,
@@ -396,32 +413,42 @@
             2 prints the entire rootfinding output, by default 0
 
         Returns
         -------
         if observed_total_se is not given, we return
             NDArray
                 predicted rates
-        Otherwise we return 
+        Otherwise we return
             NDArray
                 predicted rates
             NDArray
                 standard error estimates
         """
         fitted_beta = self.fit_beta(
-            observed_total, rate_pattern, bucket_populations, lower_guess, upper_guess
+            observed_total,
+            rate_pattern,
+            bucket_populations,
+            lower_guess,
+            upper_guess,
         )
 
         fitted_beta = self.fit_beta(
-            observed_total, rate_pattern, bucket_populations, lower_guess, upper_guess
+            observed_total,
+            rate_pattern,
+            bucket_populations,
+            lower_guess,
+            upper_guess,
         )
         count_point_estimates = self.predict_count(
-            fitted_beta, rate_pattern, bucket_populations)
+            fitted_beta, rate_pattern, bucket_populations
+        )
         if observed_total_se is not None:
             standard_errors = self.count_split_standard_errors(
-                fitted_beta, rate_pattern, bucket_populations, observed_total_se)
+                fitted_beta, rate_pattern, bucket_populations, observed_total_se
+            )
             return count_point_estimates, standard_errors
         return count_point_estimates
 
     def parameter_covariance(
         self,
         fitted_beta: float,
         rate_pattern: NDArray,
@@ -446,32 +473,39 @@
 
         Returns
         -------
         NDArray
             Joint covariance matrix with beta and rate_pattern
         """
         rate_grad = self.Hinv_rate_grad(
-            fitted_beta, rate_pattern, bucket_populations)
-        beta_pattern_cov = (
-            rate_pattern_cov@rate_grad
-        ).reshape(-1, 1)
+            fitted_beta, rate_pattern, bucket_populations
+        )
+        beta_pattern_cov = (rate_pattern_cov @ rate_grad).reshape(-1, 1)
 
         beta_var = np.array(
-            [[
-                self.beta_standard_error(
-                    fitted_beta, rate_pattern, bucket_populations, observed_total_se
-                )**2
-            ]]
+            [
+                [
+                    self.beta_standard_error(
+                        fitted_beta,
+                        rate_pattern,
+                        bucket_populations,
+                        observed_total_se,
+                    )
+                    ** 2
+                ]
+            ]
         )
 
         full_parameter_cov = np.block(
             [
-                [beta_var+rate_grad.T@rate_pattern_cov @
-                    rate_grad, beta_pattern_cov.T],
-                [beta_pattern_cov, rate_pattern_cov]
+                [
+                    beta_var + rate_grad.T @ rate_pattern_cov @ rate_grad,
+                    beta_pattern_cov.T,
+                ],
+                [beta_pattern_cov, rate_pattern_cov],
             ]
         )
 
         return full_parameter_cov
 
     def parameter_fit_jacobian(
         self,
@@ -493,85 +527,88 @@
         Returns
         -------
         NDArray
             Joint covariance matrix with beta and rate_pattern
         """
 
         rate_grad = self.Hinv_rate_grad(
-            fitted_beta, rate_pattern, bucket_populations).reshape(-1, 1)
-        beta_diff = np.array([[(1 /
-                                self.H_diff_beta(fitted_beta, rate_pattern, bucket_populations))]]
-                             )
+            fitted_beta, rate_pattern, bucket_populations
+        ).reshape(-1, 1)
+        beta_diff = np.array(
+            [
+                [
+                    (
+                        1
+                        / self.H_diff_beta(
+                            fitted_beta, rate_pattern, bucket_populations
+                        )
+                    )
+                ]
+            ]
+        )
         full_parameter_jac = np.block(
             [
                 [beta_diff, rate_grad.T],
-                [np.zeros((len(rate_pattern), 1)),
-                 np.identity(len(rate_pattern))]
+                [
+                    np.zeros((len(rate_pattern), 1)),
+                    np.identity(len(rate_pattern)),
+                ],
             ]
         )
 
         return full_parameter_jac
 
-    def Hinv_rate_grad(
-        self,
-        beta,
-        rate_pattern,
-        bucket_populations
-    ) -> NDArray:
+    def Hinv_rate_grad(self, beta, rate_pattern, bucket_populations) -> NDArray:
         """Gradient of H inverse (inverted with respect to beta) with respect to rate_pattern
 
         The inverse is handled implicitly, as beta is the input, not the total.
 
         Parameters
         ----------
         beta : float
             beta parameter, log of rescaling parameter
         rate_pattern : NDArray
-            rate pattern 
+            rate pattern
         bucket_populations :NDArray
             Populations in each bucket
 
         Returns
         -------
         NDArray
             gradient
         """
         denominator = self.H_diff_beta(beta, rate_pattern, bucket_populations)
         # Call this at the fitted beta for the inverse derivative of H at the observed_total
         # assuming that the observed_total is H(beta), the total that beta would give!
 
-        return -1*self.H_rate_grad(beta, rate_pattern, bucket_populations)/denominator
+        return (
+            -1
+            * self.H_rate_grad(beta, rate_pattern, bucket_populations)
+            / denominator
+        )
 
-    def H_rate_grad(
-        self,
-        beta,
-        rate_pattern,
-        bucket_populations
-    ) -> NDArray:
+    def H_rate_grad(self, beta, rate_pattern, bucket_populations) -> NDArray:
         """Gradient of H (inverted with respect to beta) with respect to rate_pattern
 
         Parameters
         ----------
         beta : float
             beta parameter, log of rescaling parameter
         rate_pattern : NDArray
-            rate pattern 
+            rate pattern
         bucket_populations :NDArray
             Populations in each bucket
 
         Returns
         -------
         NDArray
             gradient
         """
-        return (
-            (bucket_populations*self.T_diff(rate_pattern)) /
-            (
-                self.T_diff(self.T_inverse(beta + self.T(rate_pattern)))
-            )
+        return (bucket_populations * self.T_diff(rate_pattern)) / (
+            self.T_diff(self.T_inverse(beta + self.T(rate_pattern)))
         )
 
     def rate_jacobian(
         self,
         beta: float,
         rate_pattern: NDArray,
     ) -> NDArray:
@@ -587,25 +624,24 @@
         -------
         NDArray
             Jacobian, shaped d x (d+1)
 
         """
 
         diag_scaling = np.diag(
-            1/self.T_diff(self.T_inverse(beta + self.T(rate_pattern))))
+            1 / self.T_diff(self.T_inverse(beta + self.T(rate_pattern)))
+        )
         dim = len(rate_pattern)
         right_portion = np.block(
-            [np.ones((dim, 1)), np.diag(self.T_diff(rate_pattern))])
-        return diag_scaling@right_portion
+            [np.ones((dim, 1)), np.diag(self.T_diff(rate_pattern))]
+        )
+        return diag_scaling @ right_portion
 
     def count_jacobian(
-        self,
-        beta: float,
-        rate_pattern: NDArray,
-        bucket_populations: NDArray
+        self, beta: float, rate_pattern: NDArray, bucket_populations: NDArray
     ):
         """Computes the jacobian of the predicted output counts with respect to both beta and the pattern
         Parameters
         ----------
         beta : float
             fitted beta parameter
         rate_pattern : NDArray
@@ -617,15 +653,15 @@
         -------
         NDArray
             Jacobian, shaped d x (d+1)
         """
 
         rate_jac = self.rate_jacobian(beta, rate_pattern)
         diag_pops = np.diag(bucket_populations)
-        return diag_pops@rate_jac
+        return diag_pops @ rate_jac
 
     def rate_split_covariance_uncertainty(
         self,
         fitted_beta: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
         observed_total_se: float,
@@ -653,21 +689,21 @@
             Covariance matrix of errors in splitting rate
         """
         param_covariance = self.parameter_covariance(
             fitted_beta=fitted_beta,
             rate_pattern=rate_pattern,
             bucket_populations=bucket_populations,
             observed_total_se=observed_total_se,
-            rate_pattern_cov=rate_pattern_cov
+            rate_pattern_cov=rate_pattern_cov,
         )
         out_jac = self.rate_jacobian(
             fitted_beta,
             rate_pattern,
         )
-        return out_jac@param_covariance@out_jac.T
+        return out_jac @ param_covariance @ out_jac.T
 
     def count_split_covariance_uncertainty(
         self,
         fitted_beta: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
         observed_total_se: float,
@@ -695,22 +731,20 @@
             Covariance matrix of errors in splitting counts
         """
         param_covariance = self.parameter_covariance(
             fitted_beta=fitted_beta,
             rate_pattern=rate_pattern,
             bucket_populations=bucket_populations,
             observed_total_se=observed_total_se,
-            rate_pattern_cov=rate_pattern_cov
+            rate_pattern_cov=rate_pattern_cov,
         )
         out_jac = self.count_jacobian(
-            fitted_beta,
-            rate_pattern,
-            bucket_populations
+            fitted_beta, rate_pattern, bucket_populations
         )
-        return out_jac@param_covariance@out_jac.T
+        return out_jac @ param_covariance @ out_jac.T
 
     def rate_split_full_jac(
         self,
         observed_total: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
         lower_guess: float = -50,
@@ -737,7 +771,10 @@
         Returns
         -------
         NDArray
             jacobian of prediction output
         """
         beta = self.fit_beta(observed_total, rate_pattern, bucket_populations)
         # denominator = self.T_diff(self.T_inverse(self.))
+        # Check if this is accomplishing what i think it is - SA 4/19
+        # previously not returning anything
+        return self.rate_jacobian(beta, rate_pattern)
```

### Comparing `pydisagg-0.3.2/src/pydisagg/ParameterTransformation.py` & `pydisagg-0.4.0/src/pydisagg/ParameterTransformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module containing abstract ParameterTransformation class
 """
+
 from abc import ABC, abstractmethod
 from typing import Union
 
 from numpy.typing import NDArray
 
 float_or_array = Union[float, NDArray]
```

### Comparing `pydisagg-0.3.2/src/pydisagg/disaggregate.py` & `pydisagg-0.4.0/src/pydisagg/disaggregate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """Module containing high level api for splitting"""
-from typing import Optional, Union, Literal
+
+from typing import Literal, Optional, Union
+
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
 from pandas import DataFrame
 
-from pydisagg.models import LogOdds_model
 from pydisagg.DisaggModel import DisaggModel
+from pydisagg.models import LogOdds_model
 
 
 def split_datapoint(
     observed_total: float,
     bucket_populations: NDArray,
     rate_pattern: NDArray,
     observed_total_se: Optional[float] = None,
     model: Optional[DisaggModel] = LogOdds_model(),
-    output_type: Literal['total', 'rate'] = 'total',
-    normalize_pop_for_average_type_obs:bool = False,
+    output_type: Literal["total", "rate"] = "total",
+    normalize_pop_for_average_type_obs: bool = False,
+    pattern_covariance: Optional[NDArray] = None,
 ) -> Union[tuple, NDArray]:
     """Disaggregate a datapoint using the model given as input.
     Defaults to assuming multiplicativity in the odds ratio
 
     If output_type=='total', then this outputs estimates for the observed amount in each group
         such that the sum of the point estimates equals the original total
-    If output_type=='rate', then this estimates rates for each group 
+    If output_type=='rate', then this estimates rates for each group
         (and doesn't multiply the rates out by the population)
 
 
     Parameters
     ----------
     observed_total : float
         aggregated observed_total across all buckets, value to be split
@@ -37,101 +40,139 @@
         Rate Pattern to use, should be an estimate of the rates in each bucket
             that we want to rescale
     observed_total_se : Optional[float], optional
         standard error of observed_total, by default None
     output_type: Literal['total','rate'], optional
         One of 'total' or 'rate'
         Type of splitting to perform, whether to disaggregate and return the estimated total
-        in each group, or estimate the rate per population unit. 
+        in each group, or estimate the rate per population unit.
     model : Optional[DisaggModel], optional
         DisaggModel to use, by default LMO_model(1)
     normalize_pop_for_average_type_obs: bool = True
         Whether or not to normalize populations to sum to 1, this is appropriate when the output_type is rate
-        and when the aggregated observation is an average--whether an aggregated rate 
+        and when the aggregated observation is an average--whether an aggregated rate
         or a mean of a continuous measure over different groups
+    pattern_covariance: Optional[NDArray], optional
+        2d Numpy array with covariance matrix of pattern.
 
     Returns
     -------
     Union[Tuple,NDArray]
         If standard errors are available, this will return the tuple
             (
                 estimate_in_each_bucket,
                 se_of_estimate_bucket,
             )
-        Otherwise, if standard errors are not available, 
+        Otherwise, if standard errors are not available,
         this will return a numpy array of the disaggregated estimates
 
     Notes
     -----
     If no observed_total_se is given, returns point estimates
     If observed_total_se is given, then returns a tuple
         (point_estimate,standard_error)
     """
-    if output_type not in ['total', 'rate']:
+    if output_type not in ["total", "rate"]:
         raise ValueError("output_type must be one of either 'total' or 'rate'")
 
     if normalize_pop_for_average_type_obs is True:
-        processed_bucket_populations = bucket_populations/np.sum(bucket_populations)
+        processed_bucket_populations = bucket_populations / np.sum(
+            bucket_populations
+        )
     else:
         processed_bucket_populations = bucket_populations.copy()
 
-    if output_type == 'total':
+    if output_type == "total":
         point_estimates = model.split_to_counts(
-            observed_total,
-            rate_pattern,
-            processed_bucket_populations
+            observed_total, rate_pattern, processed_bucket_populations
         )
-        if observed_total_se is not None:
+        if (observed_total_se is not None) and (pattern_covariance is None):
             fitted_beta = model.fit_beta(
-                observed_total, rate_pattern, processed_bucket_populations)
+                observed_total, rate_pattern, processed_bucket_populations
+            )
             standard_errors = model.count_split_standard_errors(
                 fitted_beta,
                 rate_pattern,
                 processed_bucket_populations,
-                observed_total_se
+                observed_total_se,
             )
             return point_estimates, standard_errors
+
+        if (observed_total_se is not None) and (pattern_covariance is not None):
+            fitted_beta = model.fit_beta(
+                observed_total, rate_pattern, processed_bucket_populations
+            )
+
+            cov_mat = model.count_split_covariance_uncertainty(
+                fitted_beta,
+                rate_pattern,
+                processed_bucket_populations,
+                observed_total_se,
+                pattern_covariance,
+            )
+            standard_errors = np.sqrt(np.diag(cov_mat))
+
+            return point_estimates, standard_errors
+
         return point_estimates
 
-    if output_type == 'rate':
+    if output_type == "rate":
         point_estimates = model.split_to_rates(
             observed_total,
             rate_pattern,
             processed_bucket_populations,
-            reduce_output=True
+            reduce_output=True,
         )
-        if observed_total_se is not None:
+        if (observed_total_se is not None) and (pattern_covariance is None):
             fitted_beta = model.fit_beta(
-                observed_total, rate_pattern, processed_bucket_populations)
+                observed_total, rate_pattern, processed_bucket_populations
+            )
             standard_errors = model.rate_standard_errors(
                 fitted_beta,
                 rate_pattern,
                 processed_bucket_populations,
-                observed_total_se
+                observed_total_se,
             )
             return point_estimates, standard_errors
+
+        if (observed_total_se is not None) and (pattern_covariance is not None):
+            fitted_beta = model.fit_beta(
+                observed_total, rate_pattern, processed_bucket_populations
+            )
+
+            cov_mat = model.rate_split_covariance_uncertainty(
+                fitted_beta,
+                rate_pattern,
+                processed_bucket_populations,
+                observed_total_se,
+                pattern_covariance,
+            )
+            standard_errors = np.sqrt(np.diag(cov_mat))
+
+            return point_estimates, standard_errors
+
         return point_estimates
 
 
 def split_dataframe(
     groups_to_split_into: list,
     observation_group_membership_df: DataFrame,
     population_sizes: DataFrame,
     rate_patterns: DataFrame,
     use_se: Optional[bool] = False,
     model: Optional[DisaggModel] = LogOdds_model(),
-    output_type: Literal['total', 'rate'] = 'total',
+    output_type: Literal["total", "rate"] = "total",
     demographic_id_columns: Optional[list] = None,
-    normalize_pop_for_average_type_obs:bool = False,
+    normalize_pop_for_average_type_obs: bool = False,
 ) -> DataFrame:
     """Disaggregate datapoints and pivots observations into estimates for each group per demographic id
 
     If output_type=='total', then this outputs estimates for the observed amount in each group
         such that the sum of the point estimates equals the original total
-    If output_type=='rate', then this estimates rates for each group 
+    If output_type=='rate', then this estimates rates for each group
         (and doesn't multiply the rates out by the population)
 
     Parameters
     ----------
     groups_to_split_into : list
         list of groups to disaggregate observations into
     observation_group_membership_df : DataFrame
@@ -155,92 +196,98 @@
         if set to True, then observation_group_membership_df must have an obs_se column
         , by default False
     model : Optional[DisaggModel], optional
         DisaggModel to use for splitting, by default LogOdds_model()
     output_type: Literal['total','rate'], optional
         One of 'total' or 'rate'
         Type of splitting to perform, whether to disaggregate and return the estimated total
-        in each group, or estimate the rate per population unit. 
+        in each group, or estimate the rate per population unit.
     demographic_id_columns : Optional[list]
         Columns to use as demographic_id
-        Defaults to None. If None is given, then we assume 
-        that there is a already a demographic id column that matches the index in population_sizes. 
+        Defaults to None. If None is given, then we assume
+        that there is a already a demographic id column that matches the index in population_sizes.
         Otherwise, we create a new demographic_id column, zipping the columns chosen into tuples
     normalize_pop_for_average_type_obs: bool = True
         Whether or not to normalize populations to sum to 1, this is appropriate when the output_type is rate
-        and when the aggregated observation is an average--whether an aggregated rate 
+        and when the aggregated observation is an average--whether an aggregated rate
         or a mean of a continuous measure over different groups
 
     Returns
     -------
     DataFrame
         Dataframe where each row corresponds to one of obs, with one or
             two columns for each of the groups_to_split_into, giving the estimate
         If use_se==True, then has a nested column indexing, where both the
             point estimate and standard error for the estimate for each group is given.
     """
-    if (normalize_pop_for_average_type_obs is True) and (output_type=='total'):
-        raise Warning("Normalizing populations may not be appropriate here, as we are working with a total")
-    
+    if (normalize_pop_for_average_type_obs is True) and (
+        output_type == "total"
+    ):
+        raise Warning(
+            "Normalizing populations may not be appropriate here, as we are working with a total"
+        )
+
     splitting_df = observation_group_membership_df.copy()
     if demographic_id_columns is not None:
-        splitting_df['demographic_id'] = list(
-            zip(
-                *[splitting_df[id_col] for id_col in demographic_id_columns]
-            )
+        splitting_df["demographic_id"] = list(
+            zip(*[splitting_df[id_col] for id_col in demographic_id_columns])
         )
 
     if use_se is False:
+
         def split_row(x):
             return split_datapoint(
-                x['obs'],
-                population_sizes.loc[x.name]*x[groups_to_split_into],
-                rate_patterns.loc[x['pattern_id']],
+                x["obs"],
+                population_sizes.loc[x.name] * x[groups_to_split_into],
+                rate_patterns.loc[x["pattern_id"]],
                 model=model,
                 output_type=output_type,
-                normalize_pop_for_average_type_obs=normalize_pop_for_average_type_obs
+                normalize_pop_for_average_type_obs=normalize_pop_for_average_type_obs,
             )
+
         result = (
-            splitting_df
-            .set_index('demographic_id')
-            .apply(
-                split_row,
-                axis=1)
+            splitting_df.set_index("demographic_id")
+            .apply(split_row, axis=1)
             .reset_index()
         )
     else:
+
         def split_row(x):
             raw_split_result = split_datapoint(
-                x['obs'],
-                population_sizes.loc[x.name]*x[groups_to_split_into],
-                rate_patterns.loc[x['pattern_id']],
+                x["obs"],
+                population_sizes.loc[x.name] * x[groups_to_split_into],
+                rate_patterns.loc[x["pattern_id"]],
                 model=model,
-                observed_total_se=x['obs_se'],
+                observed_total_se=x["obs_se"],
                 output_type=output_type,
-                normalize_pop_for_average_type_obs=normalize_pop_for_average_type_obs
+                normalize_pop_for_average_type_obs=normalize_pop_for_average_type_obs,
             )
             return pd.Series(
                 [
-                    (estimate, se) for estimate, se in zip(raw_split_result[0], raw_split_result[1])
+                    (estimate, se)
+                    for estimate, se in zip(
+                        raw_split_result[0], raw_split_result[1]
+                    )
                 ],
-                index=groups_to_split_into)
-        result_raw = (
-            splitting_df
-            .set_index('demographic_id')
-            .apply(
-                split_row,
-                axis=1)
+                index=groups_to_split_into,
+            )
+
+        result_raw = splitting_df.set_index("demographic_id").apply(
+            split_row, axis=1
         )
         point_estimates = result_raw.applymap(lambda x: x[0])
         standard_errors = result_raw.applymap(lambda x: x[1])
-        result = pd.concat([point_estimates, standard_errors], keys=[
-                           'estimate', 'se'], axis=1).reset_index()  # .groupby(level=0).sum()
+        result = pd.concat(
+            [point_estimates, standard_errors], keys=["estimate", "se"], axis=1
+        ).reset_index()  # .groupby(level=0).sum()
 
     if demographic_id_columns is not None:
         demographic_id_df = pd.DataFrame(
-            dict(zip(demographic_id_columns, zip(*result['demographic_id']))),
-            index=result.index
+            dict(zip(demographic_id_columns, zip(*result["demographic_id"]))),
+            index=result.index,
+        )
+        result = pd.concat([demographic_id_df, result], axis=1).drop(
+            "demographic_id", axis=1
         )
-        result = pd.concat([demographic_id_df, result],
-                           axis=1).drop('demographic_id', axis=1)
 
     return result
+    return result
```

### Comparing `pydisagg-0.3.2/src/pydisagg/models.py` & `pydisagg-0.4.0/src/pydisagg/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing specific splitting models with transformations built in"""
+
 from typing import Optional
 
 import numpy as np
 from numpy.typing import NDArray
 
 from pydisagg import transformations
 from pydisagg.DisaggModel import DisaggModel
@@ -24,45 +25,44 @@
         )
 
     def fit_beta(
         self,
         observed_total: float,
         rate_pattern: NDArray,
         bucket_populations: NDArray,
-        lower_guess: Optional[float] = -50,
-        upper_guess: Optional[float] = 50,
-        verbose: Optional[int] = 0
+        lower_guess: float = -50,
+        upper_guess: float = 50,
+        verbose: Optional[int] = 0,
     ) -> None:
         """
-        Custom fit_beta for this model, as we can do it without rootfinding. 
+        Custom fit_beta for this model, as we can do it without rootfinding.
         """
         beta_val = np.log(
-            observed_total/np.sum(bucket_populations*rate_pattern))
+            observed_total / np.sum(bucket_populations * rate_pattern)
+        )
         return beta_val
 
 
 class LMO_model(DisaggModel):
     """
     DisaggModel using the log-modified odds transformation with the exponent m.
     """
 
-    def __init__(
-        self,
-        m: float,
-    ):
+    def __init__(self, m: float):
         super().__init__(
             parameter_transformation=transformations.LogModifiedOddsTransformation(
-                m),
+                m
+            ),
         )
 
 
 class LogOdds_model(DisaggModel):
-    '''
+    """
     Produces an DisaggModel assuming multiplicativity in the odds
-    '''
+    """
 
     def __init__(
         self,
     ):
         super().__init__(
             parameter_transformation=transformations.LogOddsTransformation(),
         )
```

### Comparing `pydisagg-0.3.2/src/pydisagg/transformations.py` & `pydisagg-0.4.0/src/pydisagg/transformations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Module containing classes of ParameterTransformations
 """
-from pydisagg.ParameterTransformation import ParameterTransformation
 
 from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 from scipy.optimize import root_scalar
 
+from pydisagg.ParameterTransformation import ParameterTransformation
+
 float_or_array = Union[float, NDArray]
 
 
 class LogTransformation(ParameterTransformation):
     """
     Logarithmic transformation of parameter
     Since we fit models additively in beta the log makes it multiplicative
@@ -21,15 +22,15 @@
     def __call__(self, x: float_or_array):
         return np.log(x)
 
     def inverse(self, z: float_or_array):
         return np.exp(z)
 
     def diff(self, x: float_or_array):
-        return 1/x
+        return 1 / x
 
 
 class LogModifiedOddsTransformation(ParameterTransformation):
     """
     Log Modified odds transformation
     T(x)=log(x/(1-x**a))
     """
@@ -37,41 +38,42 @@
     def __init__(self, a: float):
         self.a = a
 
     def __call__(self, x: float_or_array):
         """
         Calls transformation function
         """
-        return np.log(x/(1-(x**self.a)))
+        return np.log(x / (1 - (x**self.a)))
 
     def _inverse_single(self, z: float):
         def root_func(x):
-            return np.exp(z)*(1-x**self.a)-x
-        return root_scalar(root_func, bracket=[0, 1], method='toms748').root
+            return np.exp(z) * (1 - x**self.a) - x
+
+        return root_scalar(root_func, bracket=[0, 1], method="toms748").root
 
     def inverse(self, z: float_or_array):
         return np.vectorize(self._inverse_single)(z)
 
     def diff(self, x: float_or_array):
-        numerator = (self.a-1)*(x**self.a)+1
-        denominator = ((x**self.a)-1)*x
-        return -1*numerator/denominator
+        numerator = (self.a - 1) * (x**self.a) + 1
+        denominator = ((x**self.a) - 1) * x
+        return -1 * numerator / denominator
 
 
 class LogOddsTransformation(ParameterTransformation):
     """
     Log-odds transformation
     T(x)=log(x/(1-x))
     """
 
     def __call__(self, x: float_or_array):
         """
         Calls transformation function
         """
-        return np.log(x/(1-x))
+        return np.log(x / (1 - x))
 
     def inverse(self, z: float_or_array):
         expz = np.exp(z)
-        return expz/(1+expz)
+        return expz / (1 + expz)
 
     def diff(self, x: float_or_array):
-        return 1/(x-x**2)
+        return 1 / (x - x**2)
```

### Comparing `pydisagg-0.3.2/src/pydisagg.egg-info/PKG-INFO` & `pydisagg-0.4.0/src/pydisagg.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 Metadata-Version: 2.1
 Name: pydisagg
-Version: 0.3.2
-Summary: UNKNOWN
-Home-page: https://github.com/ihmeuw-msca/splitting-python-package
-Author: IHME Math Sciences
-Author-email: ihme.math.sciences@gmail.com
+Version: 0.4.0
+Author-email: IHME Math Sciences <ihme.math.sciences@gmail.com>
 License: BSD 2-Clause License
-Platform: UNKNOWN
+Project-URL: homepage, https://github.com/ihmeuw-msca/pydisagg
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: doc
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: pydantic
 
 [![PyPI](https://img.shields.io/pypi/v/pydisagg)](https://pypi.org/project/pydisagg/)
 ![Python](https://img.shields.io/badge/python-3.8,_3.9-blue.svg)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ihmeuw-msca/pyDisagg/build.yml)
 [![GitHub](https://img.shields.io/github/license/ihmeuw-msca/pyDisagg)](./LICENSE)
 
 ## Dissaggregation under Generalized Proportionality Assumptions
@@ -38,9 +50,7 @@
 
 ## Current Package Capabilities and Models
 Currently, the multiplicative-in-rate model RateMultiplicativeModel with $T(x)=\log(x)$ and the Log Modified Odds model LMO_model(m) with $T(x)=\log(\frac{x}{1-x^{m}})$ are implemented. Note that the LMO_model with m=1 gives a multiplicative in odds model.
 
 A useful (but slightly wrong) analogy is that the multiplicative-in-rate is to the multiplicative-in-odds model as ordinary least squares is to logistic regression in terms of the relationship between covariates and output (not in terms of anything like the likelihood)
 
 Increasing m in the model LMO_model(m) gives results that are more similar to the multiplicative-in-rate model currently in use, while preserving the property that rate estimates are bounded by 1. 
-
-
```

### Comparing `pydisagg-0.3.2/src/pydisagg.egg-info/SOURCES.txt` & `pydisagg-0.4.0/src/pydisagg.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 src/pydisagg/DisaggModel.py
 src/pydisagg/ParameterTransformation.py
 src/pydisagg/__init__.py
 src/pydisagg/disaggregate.py
 src/pydisagg/models.py
 src/pydisagg/transformations.py
 src/pydisagg.egg-info/PKG-INFO
 src/pydisagg.egg-info/SOURCES.txt
 src/pydisagg.egg-info/dependency_links.txt
-src/pydisagg.egg-info/not-zip-safe
 src/pydisagg.egg-info/requires.txt
 src/pydisagg.egg-info/top_level.txt
+src/pydisagg/ihme/__init__.py
+src/pydisagg/ihme/splitter.py
+src/pydisagg/ihme/validator.py
+tests/test_disaggregate_api.py
+tests/test_splitter.py
 tests/test_splitting_consistency.py
-tests/test_transformation_consistency.py
+tests/test_transformation_consistency.py
+tests/test_validator.py
```

### Comparing `pydisagg-0.3.2/tests/test_splitting_consistency.py` & `pydisagg-0.4.0/tests/test_splitting_consistency.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import numpy as np
 import pytest
 from numpy.testing import assert_approx_equal
 
 from pydisagg import models
-from pydisagg.disaggregate import split_datapoint
 from pydisagg.DisaggModel import DisaggModel
 
+# Need to test
+# from pydisagg.disaggregate import split_datapoint
+
 model_list = [
     models.RateMultiplicativeModel(),
     models.LogOdds_model(),
-    models.LMO_model(5)
+    models.LMO_model(5),
 ]
 
 
-@pytest.mark.parametrize('model', model_list)
+@pytest.mark.parametrize("model", model_list)
 def test_model_consistency(model: DisaggModel):
     populations = np.array([2, 5])
     measured_total = 4.8
     measurement_SE = 1
     rate_pattern = np.array([0.2, 0.4])
 
     split_result = model.split_to_counts(
         measured_total,
         rate_pattern,
         populations,
     )
-    beta = model.fit_beta(
-        measured_total,
-        rate_pattern,
-        populations
-    )
+    beta = model.fit_beta(measured_total, rate_pattern, populations)
     split_SE_vals = model.count_split_standard_errors(
         beta,
         rate_pattern,
         populations,
         measurement_SE,
     )
     assert_approx_equal(measured_total, np.sum(split_result))
```

### Comparing `pydisagg-0.3.2/tests/test_transformation_consistency.py` & `pydisagg-0.4.0/tests/test_transformation_consistency.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     tr.LogModifiedOddsTransformation(4),
     tr.LogOddsTransformation(),
 ]
 
 x_values = [0.02, 0.01, 0.5, 0.98]
 
 
-@pytest.mark.parametrize('T', transformations)
-@pytest.mark.parametrize('x', x_values)
+@pytest.mark.parametrize("T", transformations)
+@pytest.mark.parametrize("x", x_values)
 def test_inverse_consistency(T, x):
     assert_approx_equal(x, T.inverse(T(x)))
 
 
-@pytest.mark.parametrize('T', transformations)
-@pytest.mark.parametrize('x', x_values)
+@pytest.mark.parametrize("T", transformations)
+@pytest.mark.parametrize("x", x_values)
 def test_approximate_derivative(T, x, h=0.001):
     """
     Sanity check that the derivatives are are close to correct with a
     finite difference. It would have been a good idea to just do
     everything with Jax from the start.
     """
-    assert_approx_equal(T.diff(x), (T(x + h) - T(x - h))/(2*h), 2)
+    assert_approx_equal(T.diff(x), (T(x + h) - T(x - h)) / (2 * h), 2)
```

