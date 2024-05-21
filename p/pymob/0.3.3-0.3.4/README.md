# Comparing `tmp/pymob-0.3.3.tar.gz` & `tmp/pymob-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymob-0.3.3.tar", last modified: Thu May  2 18:29:30 2024, max compression
+gzip compressed data, was "pymob-0.3.4.tar", last modified: Tue May 21 13:06:21 2024, max compression
```

## Comparing `pymob-0.3.3.tar` & `pymob-0.3.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:30.173157 pymob-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 18:29:26.000000 pymob-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-02 18:29:30.173157 pymob-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-02 18:29:26.000000 pymob-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:30.161157 pymob-0.3.3/pymob/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:30.165156 pymob-0.3.3/pymob/inference/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    46901 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/numpyro_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/optimize_indy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/pyabc_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/pymoo_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:30.165156 pymob-0.3.3/pymob/inference/sbi/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/sbi/plot_posterior_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/sbi/posterior_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/sbi/process_simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/sbi/sbi_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/sbi/sbi_snle_sample_posterior.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/sbi/sbi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/inference/sbi/train_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/prior_predictive_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:30.165156 pymob-0.3.3/pymob/sim/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/sim/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/sim/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/sim/solvetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)    38324 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:30.169157 pymob-0.3.3/pymob/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/help.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/math_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/plot_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-02 18:29:26.000000 pymob-0.3.3/pymob/utils/store_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:30.169157 pymob-0.3.3/pymob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-02 18:29:30.000000 pymob-0.3.3/pymob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-02 18:29:30.000000 pymob-0.3.3/pymob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:29:30.000000 pymob-0.3.3/pymob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 18:29:30.000000 pymob-0.3.3/pymob.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-02 18:29:30.000000 pymob-0.3.3/pymob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 18:29:30.000000 pymob-0.3.3/pymob.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-02 18:29:26.000000 pymob-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:29:30.173157 pymob-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:29:30.169157 pymob-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-02 18:29:26.000000 pymob-0.3.3/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 18:29:26.000000 pymob-0.3.3/tests/test_numpyro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-02 18:29:26.000000 pymob-0.3.3/tests/test_sbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-02 18:29:26.000000 pymob-0.3.3/tests/test_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 18:29:26.000000 pymob-0.3.3/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:21.367886 pymob-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 13:06:17.000000 pymob-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-21 13:06:21.367886 pymob-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-21 13:06:17.000000 pymob-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:21.359886 pymob-0.3.4/pymob/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:21.363886 pymob-0.3.4/pymob/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46901 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/numpyro_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/optimize_indy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/pyabc_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/pymoo_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:21.363886 pymob-0.3.4/pymob/inference/sbi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/sbi/plot_posterior_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/sbi/posterior_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/sbi/process_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/sbi/sbi_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/sbi/sbi_snle_sample_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/sbi/sbi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/inference/sbi/train_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/prior_predictive_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:21.363886 pymob-0.3.4/pymob/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/sim/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/sim/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/sim/solvetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38324 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:21.363886 pymob-0.3.4/pymob/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/math_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13820 2024-05-21 13:06:17.000000 pymob-0.3.4/pymob/utils/store_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:21.367886 pymob-0.3.4/pymob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-21 13:06:21.000000 pymob-0.3.4/pymob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-21 13:06:21.000000 pymob-0.3.4/pymob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:06:21.000000 pymob-0.3.4/pymob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 13:06:21.000000 pymob-0.3.4/pymob.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-21 13:06:21.000000 pymob-0.3.4/pymob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 13:06:21.000000 pymob-0.3.4/pymob.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-21 13:06:17.000000 pymob-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:06:21.367886 pymob-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:06:21.367886 pymob-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-21 13:06:17.000000 pymob-0.3.4/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-21 13:06:17.000000 pymob-0.3.4/tests/test_numpyro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-21 13:06:17.000000 pymob-0.3.4/tests/test_sbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-21 13:06:17.000000 pymob-0.3.4/tests/test_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-21 13:06:17.000000 pymob-0.3.4/tests/test_simulation.py
```

### Comparing `pymob-0.3.3/LICENSE` & `pymob-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/PKG-INFO` & `pymob-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymob
-Version: 0.3.3
+Version: 0.3.4
 Summary: Modelling platform for Python
 Author-email: Florian Schunck <fluncki@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Florian
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pymob-0.3.3/README.md` & `pymob-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/infer.py` & `pymob-0.3.4/pymob/infer.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/analysis.py` & `pymob-0.3.4/pymob/inference/analysis.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/interactive.py` & `pymob-0.3.4/pymob/inference/interactive.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/numpyro_backend.py` & `pymob-0.3.4/pymob/inference/numpyro_backend.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/optimization.py` & `pymob-0.3.4/pymob/inference/optimization.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/optimize_indy.py` & `pymob-0.3.4/pymob/inference/optimize_indy.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/pyabc_backend.py` & `pymob-0.3.4/pymob/inference/pyabc_backend.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/pymoo_backend.py` & `pymob-0.3.4/pymob/inference/pymoo_backend.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/sbi/plot_posterior_predictions.py` & `pymob-0.3.4/pymob/inference/sbi/plot_posterior_predictions.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/sbi/posterior_predictions.py` & `pymob-0.3.4/pymob/inference/sbi/posterior_predictions.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/sbi/process_simulations.py` & `pymob-0.3.4/pymob/inference/sbi/process_simulations.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/sbi/sbi_backend.py` & `pymob-0.3.4/pymob/inference/sbi/sbi_backend.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/sbi/sbi_snle_sample_posterior.py` & `pymob-0.3.4/pymob/inference/sbi/sbi_snle_sample_posterior.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/sbi/sbi_utils.py` & `pymob-0.3.4/pymob/inference/sbi/sbi_utils.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/inference/sbi/train_network.py` & `pymob-0.3.4/pymob/inference/sbi/train_network.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/prior_predictive_checks.py` & `pymob-0.3.4/pymob/prior_predictive_checks.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/sim/base.py` & `pymob-0.3.4/pymob/sim/base.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/sim/evaluator.py` & `pymob-0.3.4/pymob/sim/evaluator.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/sim/solvetools.py` & `pymob-0.3.4/pymob/sim/solvetools.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/simulate.py` & `pymob-0.3.4/pymob/simulate.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/simulation.py` & `pymob-0.3.4/pymob/simulation.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/utils/bayesian.py` & `pymob-0.3.4/pymob/utils/bayesian.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/utils/config.py` & `pymob-0.3.4/pymob/utils/config.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/utils/errors.py` & `pymob-0.3.4/pymob/utils/errors.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/utils/help.py` & `pymob-0.3.4/pymob/utils/help.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/utils/math_helpers.py` & `pymob-0.3.4/pymob/utils/math_helpers.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/utils/misc.py` & `pymob-0.3.4/pymob/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/utils/plot_helpers.py` & `pymob-0.3.4/pymob/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pymob/utils/store_file.py` & `pymob-0.3.4/pymob/utils/store_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -361,8 +361,27 @@
             key = child_key
             
         if isinstance(value, dict):
             flat = unnest(d=value, flat=flat, parent_key=key)
         else:            
             flat.append((key, value))
     
-    return flat
+    return flat
+
+
+def go_to_case_studies(case_study_dir="case_studies"):
+    """A convenience method to find the case studies directory from a directory
+    within the case study. And change the working directory respectively"""
+    cwd = os.getcwd()
+    while not os.path.exists(os.path.join(os.getcwd(), case_study_dir)):
+        os.chdir("..")  # navigate one level up
+
+        if os.getcwd() == "/":
+            os.chdir(cwd)
+            raise NotADirectoryError(
+                f"The case study directory {case_study_dir} could not be found"
+                "by upwards traversing the directory tree. Please specify "
+                "manually the location of the parent of your case_studies folder "
+                "by using `os.chdir('path/to/the/parent/of/the/case/studies/folder')`"
+            )
+        
+    print(f"Found case study directory in: {os.getcwd()}")
```

### Comparing `pymob-0.3.3/pymob.egg-info/PKG-INFO` & `pymob-0.3.4/pymob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymob
-Version: 0.3.3
+Version: 0.3.4
 Summary: Modelling platform for Python
 Author-email: Florian Schunck <fluncki@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Florian
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pymob-0.3.3/pymob.egg-info/SOURCES.txt` & `pymob-0.3.4/pymob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/pyproject.toml` & `pymob-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymob"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Florian Schunck", email="fluncki@protonmail.com" },
 ]
 description = "Modelling platform for Python"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies=[
@@ -51,15 +51,15 @@
 dev = ["pytest >= 7.3", "pyinstrument >= 4.5", "bumpver", "sphinx", "myst-parser", "sphinx-book-theme"]
 pyabc = ["pyabc ~= 0.12.3", "pathos ~= 0.3.1"]
 numpyro = ["jax == 0.4.21", "jaxlib == 0.4.21", "sympy == 1.12", "sympy2jax == 0.0.5", "numpyro == 0.13.2", "diffrax == 0.4.1", "graphviz"]
 pymoo = ["pymoo ~= 0.6.0", "pathos ~= 0.3.1"]
 interactive = ["ipywidgets ~= 8.1.1", "IPython ~= 8.17.2"]
 
 [tool.bumpver]
-current_version = "0.3.3"
+current_version = "0.3.4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `pymob-0.3.3/tests/test_inference.py` & `pymob-0.3.4/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/tests/test_numpyro.py` & `pymob-0.3.4/tests/test_numpyro.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/tests/test_sbi.py` & `pymob-0.3.4/tests/test_sbi.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.3/tests/test_simulate.py` & `pymob-0.3.4/tests/test_simulate.py`

 * *Files identical despite different names*

