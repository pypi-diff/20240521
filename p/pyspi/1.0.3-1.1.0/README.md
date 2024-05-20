# Comparing `tmp/pyspi-1.0.3.tar.gz` & `tmp/pyspi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspi-1.0.3.tar", last modified: Mon Apr 22 19:49:40 2024, max compression
+gzip compressed data, was "pyspi-1.1.0.tar", last modified: Mon May 20 20:02:14 2024, max compression
```

## Comparing `pyspi-1.0.3.tar` & `pyspi-1.1.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.172096 pyspi-1.0.3/
--rw-r--r--   0 joshua     (501) staff       (20)    35137 2024-01-18 09:06:40.000000 pyspi-1.0.3/LICENSE.txt
--rw-r--r--   0 joshua     (501) staff       (20)    13215 2024-04-22 19:49:40.171772 pyspi-1.0.3/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)    11354 2024-03-15 02:59:54.000000 pyspi-1.0.3/README.md
--rw-r--r--   0 joshua     (501) staff       (20)     1229 2024-04-22 19:48:06.000000 pyspi-1.0.3/pyproject.toml
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.157341 pyspi-1.0.3/pyspi/
--rw-r--r--   0 joshua     (501) staff       (20)      532 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     4511 2024-02-10 05:15:52.000000 pyspi-1.0.3/pyspi/base.py
--rw-r--r--   0 joshua     (501) staff       (20)    31205 2024-03-15 02:59:54.000000 pyspi-1.0.3/pyspi/calculator.py
--rw-r--r--   0 joshua     (501) staff       (20)    25487 2024-04-22 19:48:06.000000 pyspi-1.0.3/pyspi/config.yaml
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.160277 pyspi-1.0.3/pyspi/data/
--rw-r--r--   0 joshua     (501) staff       (20)    40128 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/data/cml.npy
--rw-r--r--   0 joshua     (501) staff       (20)     5728 2024-03-13 19:42:57.000000 pyspi-1.0.3/pyspi/data/cml7.npy
--rw-r--r--   0 joshua     (501) staff       (20)    14128 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/data/forex.npy
--rw-r--r--   0 joshua     (501) staff       (20)     8128 2024-02-09 10:05:41.000000 pyspi-1.0.3/pyspi/data/standard_normal.npy
--rw-r--r--   0 joshua     (501) staff       (20)     9248 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/data.py
--rw-r--r--   0 joshua     (501) staff       (20)     1033 2024-04-21 00:57:22.000000 pyspi-1.0.3/pyspi/fabfour_config.yaml
--rw-r--r--   0 joshua     (501) staff       (20)    21968 2024-04-22 19:48:06.000000 pyspi-1.0.3/pyspi/fast_config.yaml
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.160623 pyspi-1.0.3/pyspi/lib/
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.160763 pyspi-1.0.3/pyspi/lib/PhiToolbox/
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.162788 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     2188 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss.m
--rw-r--r--   0 joshua     (501) staff       (20)     3266 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_AL.m
--rw-r--r--   0 joshua     (501) staff       (20)     5053 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_LBFGS.m
--rw-r--r--   0 joshua     (501) staff       (20)     4099 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_Gauss.m
--rw-r--r--   0 joshua     (501) staff       (20)     1913 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_comp.m
--rw-r--r--   0 joshua     (501) staff       (20)     2181 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_comp_probs.m
--rw-r--r--   0 joshua     (501) staff       (20)     3442 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_star_Gauss.m
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/__init__.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.163405 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.164410 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/Gauss/
--rw-r--r--   0 joshua     (501) staff       (20)     1539 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/Gauss/Cov_comp.m
--rw-r--r--   0 joshua     (501) staff       (20)      321 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/Gauss/Cov_cond.m
--rw-r--r--   0 joshua     (501) staff       (20)      420 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/Gauss/H_gauss.m
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/Gauss/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)      173 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/Gauss/logdet.m
--rw-r--r--   0 joshua     (501) staff       (20)      740 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/I_s_I_s_d.m
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     2699 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/data_to_probs.m
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/__init__.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.164885 pyspi-1.0.3/pyspi/lib/jidt/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/lib/jidt/__init__.py
--rwxr-xr-x   0 joshua     (501) staff       (20)   658934 2024-04-22 19:48:06.000000 pyspi-1.0.3/pyspi/lib/jidt/infodynamics.jar
--rw-r--r--   0 joshua     (501) staff       (20)     3626 2024-04-21 00:57:22.000000 pyspi-1.0.3/pyspi/sonnet_config.yaml
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.169749 pyspi-1.0.3/pyspi/statistics/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/statistics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     5759 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/statistics/basic.py
--rw-r--r--   0 joshua     (501) staff       (20)     5118 2024-04-22 19:48:06.000000 pyspi-1.0.3/pyspi/statistics/causal.py
--rw-r--r--   0 joshua     (501) staff       (20)     9231 2024-04-22 19:48:06.000000 pyspi-1.0.3/pyspi/statistics/distance.py
--rw-r--r--   0 joshua     (501) staff       (20)    20248 2024-04-22 19:48:06.000000 pyspi-1.0.3/pyspi/statistics/infotheory.py
--rw-r--r--   0 joshua     (501) staff       (20)     5235 2024-04-21 00:57:22.000000 pyspi-1.0.3/pyspi/statistics/misc.py
--rw-r--r--   0 joshua     (501) staff       (20)    14437 2024-01-18 09:06:41.000000 pyspi-1.0.3/pyspi/statistics/spectral.py
--rw-r--r--   0 joshua     (501) staff       (20)     6796 2024-04-17 01:42:10.000000 pyspi-1.0.3/pyspi/statistics/wavelet.py
--rw-r--r--   0 joshua     (501) staff       (20)     8458 2024-03-15 20:46:02.000000 pyspi-1.0.3/pyspi/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.171174 pyspi-1.0.3/pyspi.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)    13215 2024-04-22 19:49:40.000000 pyspi-1.0.3/pyspi.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     1524 2024-04-22 19:49:40.000000 pyspi-1.0.3/pyspi.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2024-04-22 19:49:40.000000 pyspi-1.0.3/pyspi.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      326 2024-04-22 19:49:40.000000 pyspi-1.0.3/pyspi.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)        6 2024-04-22 19:49:40.000000 pyspi-1.0.3/pyspi.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2024-04-22 19:49:40.172158 pyspi-1.0.3/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     3134 2024-04-22 19:48:06.000000 pyspi-1.0.3/setup.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-22 19:49:40.170809 pyspi-1.0.3/tests/
--rw-r--r--   0 joshua     (501) staff       (20)     3571 2024-04-22 19:48:06.000000 pyspi-1.0.3/tests/test_SPIs.py
--rw-r--r--   0 joshua     (501) staff       (20)    15412 2024-03-15 20:01:23.000000 pyspi-1.0.3/tests/test_calc.py
--rw-r--r--   0 joshua     (501) staff       (20)     5392 2024-03-15 20:46:02.000000 pyspi-1.0.3/tests/test_utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.530992 pyspi-1.1.0/
+-rw-r--r--   0 joshua     (501) staff       (20)    35137 2024-01-18 09:06:40.000000 pyspi-1.1.0/LICENSE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)    12020 2024-05-20 20:02:14.530647 pyspi-1.1.0/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)    10267 2024-05-20 05:13:11.000000 pyspi-1.1.0/README.md
+-rw-r--r--   0 joshua     (501) staff       (20)     1223 2024-05-19 06:55:15.000000 pyspi-1.1.0/pyproject.toml
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.516961 pyspi-1.1.0/pyspi/
+-rw-r--r--   0 joshua     (501) staff       (20)      532 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     4511 2024-02-10 05:15:52.000000 pyspi-1.1.0/pyspi/base.py
+-rw-r--r--   0 joshua     (501) staff       (20)    31577 2024-05-20 19:24:43.000000 pyspi-1.1.0/pyspi/calculator.py
+-rw-r--r--   0 joshua     (501) staff       (20)    25487 2024-04-22 19:48:06.000000 pyspi-1.1.0/pyspi/config.yaml
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.519587 pyspi-1.1.0/pyspi/data/
+-rw-r--r--   0 joshua     (501) staff       (20)    40128 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/data/cml.npy
+-rw-r--r--   0 joshua     (501) staff       (20)     5728 2024-03-13 19:42:57.000000 pyspi-1.1.0/pyspi/data/cml7.npy
+-rw-r--r--   0 joshua     (501) staff       (20)    14128 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/data/forex.npy
+-rw-r--r--   0 joshua     (501) staff       (20)     8128 2024-02-09 10:05:41.000000 pyspi-1.1.0/pyspi/data/standard_normal.npy
+-rw-r--r--   0 joshua     (501) staff       (20)     9376 2024-05-20 19:12:13.000000 pyspi-1.1.0/pyspi/data.py
+-rw-r--r--   0 joshua     (501) staff       (20)     1033 2024-04-21 00:57:22.000000 pyspi-1.1.0/pyspi/fabfour_config.yaml
+-rw-r--r--   0 joshua     (501) staff       (20)    21968 2024-04-22 19:48:06.000000 pyspi-1.1.0/pyspi/fast_config.yaml
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.519959 pyspi-1.1.0/pyspi/lib/
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.520094 pyspi-1.1.0/pyspi/lib/PhiToolbox/
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.522112 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2188 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss.m
+-rw-r--r--   0 joshua     (501) staff       (20)     3266 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_AL.m
+-rw-r--r--   0 joshua     (501) staff       (20)     5053 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_LBFGS.m
+-rw-r--r--   0 joshua     (501) staff       (20)     4099 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_Gauss.m
+-rw-r--r--   0 joshua     (501) staff       (20)     1913 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_comp.m
+-rw-r--r--   0 joshua     (501) staff       (20)     2181 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_comp_probs.m
+-rw-r--r--   0 joshua     (501) staff       (20)     3442 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_star_Gauss.m
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/__init__.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.522841 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.523810 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/Gauss/
+-rw-r--r--   0 joshua     (501) staff       (20)     1539 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/Gauss/Cov_comp.m
+-rw-r--r--   0 joshua     (501) staff       (20)      321 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/Gauss/Cov_cond.m
+-rw-r--r--   0 joshua     (501) staff       (20)      420 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/Gauss/H_gauss.m
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/Gauss/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)      173 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/Gauss/logdet.m
+-rw-r--r--   0 joshua     (501) staff       (20)      740 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/I_s_I_s_d.m
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2699 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/data_to_probs.m
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/__init__.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.524116 pyspi-1.1.0/pyspi/lib/jidt/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/lib/jidt/__init__.py
+-rwxr-xr-x   0 joshua     (501) staff       (20)   658934 2024-04-22 19:48:06.000000 pyspi-1.1.0/pyspi/lib/jidt/infodynamics.jar
+-rw-r--r--   0 joshua     (501) staff       (20)     3626 2024-04-21 00:57:22.000000 pyspi-1.1.0/pyspi/sonnet_config.yaml
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.528460 pyspi-1.1.0/pyspi/statistics/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/statistics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5759 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/statistics/basic.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5581 2024-05-19 07:30:32.000000 pyspi-1.1.0/pyspi/statistics/causal.py
+-rw-r--r--   0 joshua     (501) staff       (20)     9231 2024-04-22 19:48:06.000000 pyspi-1.1.0/pyspi/statistics/distance.py
+-rw-r--r--   0 joshua     (501) staff       (20)    20248 2024-04-22 19:48:06.000000 pyspi-1.1.0/pyspi/statistics/infotheory.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5465 2024-05-19 03:48:46.000000 pyspi-1.1.0/pyspi/statistics/misc.py
+-rw-r--r--   0 joshua     (501) staff       (20)    14437 2024-01-18 09:06:41.000000 pyspi-1.1.0/pyspi/statistics/spectral.py
+-rw-r--r--   0 joshua     (501) staff       (20)     6796 2024-04-17 01:42:10.000000 pyspi-1.1.0/pyspi/statistics/wavelet.py
+-rw-r--r--   0 joshua     (501) staff       (20)    10291 2024-05-20 07:21:02.000000 pyspi-1.1.0/pyspi/utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.530049 pyspi-1.1.0/pyspi.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)    12020 2024-05-20 20:02:14.000000 pyspi-1.1.0/pyspi.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     1524 2024-05-20 20:02:14.000000 pyspi-1.1.0/pyspi.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2024-05-20 20:02:14.000000 pyspi-1.1.0/pyspi.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      209 2024-05-20 20:02:14.000000 pyspi-1.1.0/pyspi.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        6 2024-05-20 20:02:14.000000 pyspi-1.1.0/pyspi.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2024-05-20 20:02:14.531045 pyspi-1.1.0/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     3028 2024-05-19 06:55:04.000000 pyspi-1.1.0/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-20 20:02:14.529636 pyspi-1.1.0/tests/
+-rw-r--r--   0 joshua     (501) staff       (20)     3571 2024-05-17 23:12:38.000000 pyspi-1.1.0/tests/test_SPIs.py
+-rw-r--r--   0 joshua     (501) staff       (20)    15816 2024-05-20 19:42:49.000000 pyspi-1.1.0/tests/test_calc.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5392 2024-03-15 20:46:02.000000 pyspi-1.1.0/tests/test_utils.py
```

### Comparing `pyspi-1.0.3/LICENSE.txt` & `pyspi-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/PKG-INFO` & `pyspi-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspi
-Version: 1.0.3
+Version: 1.1.0
 Summary: Library for pairwise analysis of time series data.
 Home-page: https://github.com/DynamicsAndNeuralSystems/pyspi
 Author: Oliver M. Cliff
 Author-email: "Oliver M. Cliff" <oliver.m.cliff@gmail.com>
 Maintainer: Joshua B. Moore
 Maintainer-email: joshua.moore@sydney.edu.au
 License: GNU General Public License v3 (GPLv3)
@@ -17,37 +17,38 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: <3.10,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: scikit-learn==1.0.1
-Requires-Dist: scipy==1.7.3
-Requires-Dist: numpy>=1.21.1
-Requires-Dist: pandas==1.5.0
-Requires-Dist: statsmodels==0.12.1
-Requires-Dist: pyyaml==5.4
-Requires-Dist: tqdm==4.50.2
-Requires-Dist: nitime==0.9
-Requires-Dist: hyppo==0.2.1
-Requires-Dist: pyEDM==1.9.3
-Requires-Dist: jpype1==1.2.0
-Requires-Dist: sktime==0.8.0
-Requires-Dist: dill==0.3.2
-Requires-Dist: spectral-connectivity==0.2.4.dev0
-Requires-Dist: torch==1.13.1
+Requires-Dist: h5py
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: statsmodels
+Requires-Dist: pyyaml
+Requires-Dist: tqdm
+Requires-Dist: nitime
+Requires-Dist: hyppo
+Requires-Dist: pyEDM==1.15.2.0
+Requires-Dist: jpype1
+Requires-Dist: sktime
+Requires-Dist: dill
+Requires-Dist: spectral-connectivity
+Requires-Dist: torch
 Requires-Dist: cdt==0.5.23
-Requires-Dist: oct2py==5.2.0
-Requires-Dist: tslearn==0.5.2
+Requires-Dist: oct2py
+Requires-Dist: tslearn
 Requires-Dist: mne==0.23.0
-Requires-Dist: seaborn==0.11.0
+Requires-Dist: seaborn
 Provides-Extra: testing
 Requires-Dist: pytest==5.4.2; extra == "testing"
 
 <p align="center">
   <picture>
     <source srcset="img/pyspi_logo_darkmode.png" media="(prefers-color-scheme: dark)">
     <img src="img/pyspi_logo.png" alt="pyspi logo" height="200"/>
@@ -59,15 +60,15 @@
 
 
 <p align="center">
  	<a href="https://zenodo.org/badge/latestdoi/601919618"><img src="https://zenodo.org/badge/601919618.svg" height="20"/></a>
     <a href="https://www.gnu.org/licenses/gpl-3.0"><img src="https://img.shields.io/badge/License-GPLv3-blue.svg" height="20"/></a>
     <a href="https://github.com/DynamicsAndNeuralSystems/pyspi/actions/workflows/run_unit_tests.yaml"><img src="https://github.com/DynamicsAndNeuralSystems/pyspi/actions/workflows/run_unit_tests.yaml/badge.svg" height="20"/></a>
     <a href="https://twitter.com/compTimeSeries"><img src="https://img.shields.io/twitter/url/https/twitter.com/compTimeSeries.svg?style=social&label=Follow%20%40compTimeSeries" height="20"/></a><br>
-    <a href="https://www.python.org"><img src="https://img.shields.io/badge/Python-3.8%20|%203.9-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.8 | 3.9"></a>
+    <a href="https://www.python.org"><img src="https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.8 | 3.9 | 3.10 | 3.11 | 3.12"></a>
 </p>
 
 _pyspi_ is a comprehensive python library for computing statistics of pairwise interactions (SPIs) from multivariate time-series (MTS) data.
 The toolbox provides easy access to hundreds of methods for evaluating the relationship between pairs of time series, from simple statistics (like correlation) to advanced multi-step algorithms (like Granger causality).
 The code is licensed under the [GNU GPL v3 license](http://www.gnu.org/licenses/gpl-3.0.html) (or later).
 
 **Feel free to reach out for help with real-world applications.**
@@ -119,29 +120,14 @@
 - [Finance: stock price time series](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/finance-stock-price-time-series)
 
 
 - [Neuroimaging: fMRI time series)](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/neuroimaging-fmri-time-series)
 
 ### Advanced Usage
 For advanced users, we offer several additional guides in the [full documentation](https://time-series-features.gitbook.io/pyspi/usage/advanced-usage) on how you can distribute your _pyspi_ jobs across PBS clusters, as well as how you can construct your own subsets of SPIs. 
-Click one of the following dropdowns for more information:
-
-<details closed>
-<summary>Distributing pyspi calculations</summary>
-<p>If you have access to a PBS cluster and are processing MTS with many processes (or are analyzing many MTS), then you may find the <a href="https://github.com/DynamicsAndNeuralSystems/pyspi-distribute"><em>pyspi distribute</em></a> repository helpful.
-In the full <a href="https://time-series-features.gitbook.io/pyspi/usage/advanced-usage/distributing-calculations-on-a-cluster">documentation </a>, we provide a comprehensive guide on how you can distribute <em>pyspi</em> calculations on a PBS cluster, along with the necessary scripts and commands to get started!</p>
-</details>
-
-<details closed>
-<summary>Reduced subsets</summary>
-<p>If your dataset is large (containing many processes and/or observations), you can use a pre-configured set of reduced statistics or create your own subsets.
-Follow the guide in the <a href="https://time-series-features.gitbook.io/pyspi/usage/advanced-usage/using-a-reduced-spi-set">documentation </a> to learn how you can create your own reduced subsets.</p>
-</details>
-
-
 
 ## SPI Descriptions 📋
 To access a table with a high-level overview of the _pyspi_ library of SPIs, including their associated identifiers, see the [table of SPIs](https://time-series-features.gitbook.io/pyspi/spis/table-of-spis) in the full documentation.
 For detailed descriptions of each SPI, as well as its associated estimators, we provide a full breakdown in the [SPI descriptions](https://time-series-features.gitbook.io/pyspi/spis/spi-descriptions) page of our documentation. 
 
 ## Documentation
 The full documentation is hosted on [GitBooks](https://time-series-features.gitbook.io/pyspi/). 
@@ -212,8 +198,7 @@
 
 <a href="https://github.com/DynamicsAndNeuralSystems/pyspi/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=DynamicsAndNeuralSystems/pyspi" />
 </a>
 
 ## License 🧾
 _pyspi_ is released under the [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0).
-
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1 Name: pyspi Version: 1.0.3 Summary: Library for pairwise
+Metadata-Version: 2.1 Name: pyspi Version: 1.1.0 Summary: Library for pairwise
 analysis of time series data. Home-page: https://github.com/
 DynamicsAndNeuralSystems/pyspi Author: Oliver M. Cliff Author-email: "Oliver M.
 Cliff"
 gmail.com> Maintainer: Joshua B. Moore Maintainer-email:
 joshua.moore@sydney.edu.au License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/DynamicsAndNeuralSystems/pyspi
 Project-URL: Documentation, https://time-series-features.gitbook.io/pyspi/
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Development Status :: 1 - Planning Classifier:
 Operating System :: POSIX :: Linux Classifier: Intended Audience :: Science/
 Research Classifier: Environment :: Console Classifier: Environment :: Other
 Environment Classifier: Topic :: Scientific/Engineering :: Physics Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Scientific/
-Engineering :: Medical Science Apps. Requires-Python: <3.10,>=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist: scikit-
-learn==1.0.1 Requires-Dist: scipy==1.7.3 Requires-Dist: numpy>=1.21.1 Requires-
-Dist: pandas==1.5.0 Requires-Dist: statsmodels==0.12.1 Requires-Dist:
-pyyaml==5.4 Requires-Dist: tqdm==4.50.2 Requires-Dist: nitime==0.9 Requires-
-Dist: hyppo==0.2.1 Requires-Dist: pyEDM==1.9.3 Requires-Dist: jpype1==1.2.0
-Requires-Dist: sktime==0.8.0 Requires-Dist: dill==0.3.2 Requires-Dist:
-spectral-connectivity==0.2.4.dev0 Requires-Dist: torch==1.13.1 Requires-Dist:
-cdt==0.5.23 Requires-Dist: oct2py==5.2.0 Requires-Dist: tslearn==0.5.2
-Requires-Dist: mne==0.23.0 Requires-Dist: seaborn==0.11.0 Provides-Extra:
-testing Requires-Dist: pytest==5.4.2; extra == "testing"
+Engineering :: Medical Science Apps. Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist: h5py
+Requires-Dist: scikit-learn Requires-Dist: scipy Requires-Dist: numpy Requires-
+Dist: pandas Requires-Dist: statsmodels Requires-Dist: pyyaml Requires-Dist:
+tqdm Requires-Dist: nitime Requires-Dist: hyppo Requires-Dist: pyEDM==1.15.2.0
+Requires-Dist: jpype1 Requires-Dist: sktime Requires-Dist: dill Requires-Dist:
+spectral-connectivity Requires-Dist: torch Requires-Dist: cdt==0.5.23 Requires-
+Dist: oct2py Requires-Dist: tslearn Requires-Dist: mne==0.23.0 Requires-Dist:
+seaborn Provides-Extra: testing Requires-Dist: pytest==5.4.2; extra ==
+"testing"
                                  [pyspi logo]
   ************ ppyyssppii:: PPyytthhoonn TToooollkkiitt ooff SSttaattiissttiiccss ffoorr PPaaiirrwwiissee IInntteerraaccttiioonnss ************
 _[_h_t_t_p_s_:_/_/_z_e_n_o_d_o_._o_r_g_/_b_a_d_g_e_/_6_0_1_9_1_9_6_1_8_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-
   _G_P_L_v_3_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_D_y_n_a_m_i_c_s_A_n_d_N_e_u_r_a_l_S_y_s_t_e_m_s_/_p_y_s_p_i_/_a_c_t_i_o_n_s_/
  _w_o_r_k_f_l_o_w_s_/_r_u_n___u_n_i_t___t_e_s_t_s_._y_a_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_u_r_l_/
                               _h_t_t_p_s_/_t_w_i_t_t_e_r_._c_o_m_/
        _c_o_m_p_T_i_m_e_S_e_r_i_e_s_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_c_o_m_p_T_i_m_e_S_e_r_i_e_s_]
-                              _[_P_y_t_h_o_n_ _3_._8_ _|_ _3_._9_]
+                    _[_P_y_t_h_o_n_ _3_._8_ _|_ _3_._9_ _|_ _3_._1_0_ _|_ _3_._1_1_ _|_ _3_._1_2_]
 _pyspi_ is a comprehensive python library for computing statistics of pairwise
 interactions (SPIs) from multivariate time-series (MTS) data. The toolbox
 provides easy access to hundreds of methods for evaluating the relationship
 between pairs of time series, from simple statistics (like correlation) to
 advanced multi-step algorithms (like Granger causality). The code is licensed
 under the [GNU GPL v3 license](http://www.gnu.org/licenses/gpl-3.0.html) (or
 later). **Feel free to reach out for help with real-world applications.**
@@ -83,40 +82,28 @@
 series](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-
 tutorials/finance-stock-price-time-series) - [Neuroimaging: fMRI time series)]
 (https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/
 neuroimaging-fmri-time-series) ### Advanced Usage For advanced users, we offer
 several additional guides in the [full documentation](https://time-series-
 features.gitbook.io/pyspi/usage/advanced-usage) on how you can distribute your
 _pyspi_ jobs across PBS clusters, as well as how you can construct your own
-subsets of SPIs. Click one of the following dropdowns for more information:
-Distributing pyspi calculations
-If you have access to a PBS cluster and are processing MTS with many processes
-(or are analyzing many MTS), then you may find the _pp_yy_ss_pp_ii_ _dd_ii_ss_tt_rr_ii_bb_uu_tt_ee repository
-helpful. In the full _d_o_c_u_m_e_n_t_a_t_i_o_n_ , we provide a comprehensive guide on how
-you can distribute ppyyssppii calculations on a PBS cluster, along with the
-necessary scripts and commands to get started!
-Reduced subsets
-If your dataset is large (containing many processes and/or observations), you
-can use a pre-configured set of reduced statistics or create your own subsets.
-Follow the guide in the _d_o_c_u_m_e_n_t_a_t_i_o_n_ to learn how you can create your own
-reduced subsets.
-## SPI Descriptions ð To access a table with a high-level overview of the
-_pyspi_ library of SPIs, including their associated identifiers, see the [table
-of SPIs](https://time-series-features.gitbook.io/pyspi/spis/table-of-spis) in
-the full documentation. For detailed descriptions of each SPI, as well as its
-associated estimators, we provide a full breakdown in the [SPI descriptions]
-(https://time-series-features.gitbook.io/pyspi/spis/spi-descriptions) page of
-our documentation. ## Documentation The full documentation is hosted on
-[GitBooks](https://time-series-features.gitbook.io/pyspi/). Use the following
-links to quickly access some of the key sections: - [Full installation guide]
-(https://time-series-features.gitbook.io/pyspi/installation) -
-[Troubleshooting](https://time-series-features.gitbook.io/pyspi/installation/
-troubleshooting) - [Alternative installation options](https://time-series-
-features.gitbook.io/pyspi/installation/alternative-installation-options) -
-[Usage guide](https://time-series-features.gitbook.io/pyspi/usage) -
+subsets of SPIs. ## SPI Descriptions ð To access a table with a high-level
+overview of the _pyspi_ library of SPIs, including their associated
+identifiers, see the [table of SPIs](https://time-series-features.gitbook.io/
+pyspi/spis/table-of-spis) in the full documentation. For detailed descriptions
+of each SPI, as well as its associated estimators, we provide a full breakdown
+in the [SPI descriptions](https://time-series-features.gitbook.io/pyspi/spis/
+spi-descriptions) page of our documentation. ## Documentation The full
+documentation is hosted on [GitBooks](https://time-series-features.gitbook.io/
+pyspi/). Use the following links to quickly access some of the key sections: -
+[Full installation guide](https://time-series-features.gitbook.io/pyspi/
+installation) - [Troubleshooting](https://time-series-features.gitbook.io/
+pyspi/installation/troubleshooting) - [Alternative installation options](https:
+//time-series-features.gitbook.io/pyspi/installation/alternative-installation-
+options) - [Usage guide](https://time-series-features.gitbook.io/pyspi/usage) -
 [Distributing _pyspi_ computations](https://time-series-features.gitbook.io/
 pyspi/usage/advanced-usage/distributing-calculations-on-a-cluster) - [Table of
 SPIs and descriptions](https://time-series-features.gitbook.io/pyspi/spis) -
 [FAQ](https://time-series-features.gitbook.io/pyspi/usage/faq) - [API
 Reference](https://time-series-features.gitbook.io/pyspi/api-reference) -
 [Development guide](https://time-series-features.gitbook.io/pyspi/development)
 ## Contributing to _pyspi_ ð¨âð¨âð¦âð¦ Contributions play a vital
```

### Comparing `pyspi-1.0.3/README.md` & `pyspi-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 <p align="center">
  	<a href="https://zenodo.org/badge/latestdoi/601919618"><img src="https://zenodo.org/badge/601919618.svg" height="20"/></a>
     <a href="https://www.gnu.org/licenses/gpl-3.0"><img src="https://img.shields.io/badge/License-GPLv3-blue.svg" height="20"/></a>
     <a href="https://github.com/DynamicsAndNeuralSystems/pyspi/actions/workflows/run_unit_tests.yaml"><img src="https://github.com/DynamicsAndNeuralSystems/pyspi/actions/workflows/run_unit_tests.yaml/badge.svg" height="20"/></a>
     <a href="https://twitter.com/compTimeSeries"><img src="https://img.shields.io/twitter/url/https/twitter.com/compTimeSeries.svg?style=social&label=Follow%20%40compTimeSeries" height="20"/></a><br>
-    <a href="https://www.python.org"><img src="https://img.shields.io/badge/Python-3.8%20|%203.9-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.8 | 3.9"></a>
+    <a href="https://www.python.org"><img src="https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.8 | 3.9 | 3.10 | 3.11 | 3.12"></a>
 </p>
 
 _pyspi_ is a comprehensive python library for computing statistics of pairwise interactions (SPIs) from multivariate time-series (MTS) data.
 The toolbox provides easy access to hundreds of methods for evaluating the relationship between pairs of time series, from simple statistics (like correlation) to advanced multi-step algorithms (like Granger causality).
 The code is licensed under the [GNU GPL v3 license](http://www.gnu.org/licenses/gpl-3.0.html) (or later).
 
 **Feel free to reach out for help with real-world applications.**
@@ -70,29 +70,14 @@
 - [Finance: stock price time series](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/finance-stock-price-time-series)
 
 
 - [Neuroimaging: fMRI time series)](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/neuroimaging-fmri-time-series)
 
 ### Advanced Usage
 For advanced users, we offer several additional guides in the [full documentation](https://time-series-features.gitbook.io/pyspi/usage/advanced-usage) on how you can distribute your _pyspi_ jobs across PBS clusters, as well as how you can construct your own subsets of SPIs. 
-Click one of the following dropdowns for more information:
-
-<details closed>
-<summary>Distributing pyspi calculations</summary>
-<p>If you have access to a PBS cluster and are processing MTS with many processes (or are analyzing many MTS), then you may find the <a href="https://github.com/DynamicsAndNeuralSystems/pyspi-distribute"><em>pyspi distribute</em></a> repository helpful.
-In the full <a href="https://time-series-features.gitbook.io/pyspi/usage/advanced-usage/distributing-calculations-on-a-cluster">documentation </a>, we provide a comprehensive guide on how you can distribute <em>pyspi</em> calculations on a PBS cluster, along with the necessary scripts and commands to get started!</p>
-</details>
-
-<details closed>
-<summary>Reduced subsets</summary>
-<p>If your dataset is large (containing many processes and/or observations), you can use a pre-configured set of reduced statistics or create your own subsets.
-Follow the guide in the <a href="https://time-series-features.gitbook.io/pyspi/usage/advanced-usage/using-a-reduced-spi-set">documentation </a> to learn how you can create your own reduced subsets.</p>
-</details>
-
-
 
 ## SPI Descriptions 📋
 To access a table with a high-level overview of the _pyspi_ library of SPIs, including their associated identifiers, see the [table of SPIs](https://time-series-features.gitbook.io/pyspi/spis/table-of-spis) in the full documentation.
 For detailed descriptions of each SPI, as well as its associated estimators, we provide a full breakdown in the [SPI descriptions](https://time-series-features.gitbook.io/pyspi/spis/spi-descriptions) page of our documentation. 
 
 ## Documentation
 The full documentation is hosted on [GitBooks](https://time-series-features.gitbook.io/pyspi/). 
@@ -163,8 +148,7 @@
 
 <a href="https://github.com/DynamicsAndNeuralSystems/pyspi/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=DynamicsAndNeuralSystems/pyspi" />
 </a>
 
 ## License 🧾
 _pyspi_ is released under the [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0).
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                                  [pyspi logo]
   ************ ppyyssppii:: PPyytthhoonn TToooollkkiitt ooff SSttaattiissttiiccss ffoorr PPaaiirrwwiissee IInntteerraaccttiioonnss ************
 _[_h_t_t_p_s_:_/_/_z_e_n_o_d_o_._o_r_g_/_b_a_d_g_e_/_6_0_1_9_1_9_6_1_8_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-
   _G_P_L_v_3_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_D_y_n_a_m_i_c_s_A_n_d_N_e_u_r_a_l_S_y_s_t_e_m_s_/_p_y_s_p_i_/_a_c_t_i_o_n_s_/
  _w_o_r_k_f_l_o_w_s_/_r_u_n___u_n_i_t___t_e_s_t_s_._y_a_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_u_r_l_/
                               _h_t_t_p_s_/_t_w_i_t_t_e_r_._c_o_m_/
        _c_o_m_p_T_i_m_e_S_e_r_i_e_s_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_c_o_m_p_T_i_m_e_S_e_r_i_e_s_]
-                              _[_P_y_t_h_o_n_ _3_._8_ _|_ _3_._9_]
+                    _[_P_y_t_h_o_n_ _3_._8_ _|_ _3_._9_ _|_ _3_._1_0_ _|_ _3_._1_1_ _|_ _3_._1_2_]
 _pyspi_ is a comprehensive python library for computing statistics of pairwise
 interactions (SPIs) from multivariate time-series (MTS) data. The toolbox
 provides easy access to hundreds of methods for evaluating the relationship
 between pairs of time series, from simple statistics (like correlation) to
 advanced multi-step algorithms (like Granger causality). The code is licensed
 under the [GNU GPL v3 license](http://www.gnu.org/licenses/gpl-3.0.html) (or
 later). **Feel free to reach out for help with real-world applications.**
@@ -57,40 +57,28 @@
 series](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-
 tutorials/finance-stock-price-time-series) - [Neuroimaging: fMRI time series)]
 (https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/
 neuroimaging-fmri-time-series) ### Advanced Usage For advanced users, we offer
 several additional guides in the [full documentation](https://time-series-
 features.gitbook.io/pyspi/usage/advanced-usage) on how you can distribute your
 _pyspi_ jobs across PBS clusters, as well as how you can construct your own
-subsets of SPIs. Click one of the following dropdowns for more information:
-Distributing pyspi calculations
-If you have access to a PBS cluster and are processing MTS with many processes
-(or are analyzing many MTS), then you may find the _pp_yy_ss_pp_ii_ _dd_ii_ss_tt_rr_ii_bb_uu_tt_ee repository
-helpful. In the full _d_o_c_u_m_e_n_t_a_t_i_o_n_ , we provide a comprehensive guide on how
-you can distribute ppyyssppii calculations on a PBS cluster, along with the
-necessary scripts and commands to get started!
-Reduced subsets
-If your dataset is large (containing many processes and/or observations), you
-can use a pre-configured set of reduced statistics or create your own subsets.
-Follow the guide in the _d_o_c_u_m_e_n_t_a_t_i_o_n_ to learn how you can create your own
-reduced subsets.
-## SPI Descriptions ð To access a table with a high-level overview of the
-_pyspi_ library of SPIs, including their associated identifiers, see the [table
-of SPIs](https://time-series-features.gitbook.io/pyspi/spis/table-of-spis) in
-the full documentation. For detailed descriptions of each SPI, as well as its
-associated estimators, we provide a full breakdown in the [SPI descriptions]
-(https://time-series-features.gitbook.io/pyspi/spis/spi-descriptions) page of
-our documentation. ## Documentation The full documentation is hosted on
-[GitBooks](https://time-series-features.gitbook.io/pyspi/). Use the following
-links to quickly access some of the key sections: - [Full installation guide]
-(https://time-series-features.gitbook.io/pyspi/installation) -
-[Troubleshooting](https://time-series-features.gitbook.io/pyspi/installation/
-troubleshooting) - [Alternative installation options](https://time-series-
-features.gitbook.io/pyspi/installation/alternative-installation-options) -
-[Usage guide](https://time-series-features.gitbook.io/pyspi/usage) -
+subsets of SPIs. ## SPI Descriptions ð To access a table with a high-level
+overview of the _pyspi_ library of SPIs, including their associated
+identifiers, see the [table of SPIs](https://time-series-features.gitbook.io/
+pyspi/spis/table-of-spis) in the full documentation. For detailed descriptions
+of each SPI, as well as its associated estimators, we provide a full breakdown
+in the [SPI descriptions](https://time-series-features.gitbook.io/pyspi/spis/
+spi-descriptions) page of our documentation. ## Documentation The full
+documentation is hosted on [GitBooks](https://time-series-features.gitbook.io/
+pyspi/). Use the following links to quickly access some of the key sections: -
+[Full installation guide](https://time-series-features.gitbook.io/pyspi/
+installation) - [Troubleshooting](https://time-series-features.gitbook.io/
+pyspi/installation/troubleshooting) - [Alternative installation options](https:
+//time-series-features.gitbook.io/pyspi/installation/alternative-installation-
+options) - [Usage guide](https://time-series-features.gitbook.io/pyspi/usage) -
 [Distributing _pyspi_ computations](https://time-series-features.gitbook.io/
 pyspi/usage/advanced-usage/distributing-calculations-on-a-cluster) - [Table of
 SPIs and descriptions](https://time-series-features.gitbook.io/pyspi/spis) -
 [FAQ](https://time-series-features.gitbook.io/pyspi/usage/faq) - [API
 Reference](https://time-series-features.gitbook.io/pyspi/api-reference) -
 [Development guide](https://time-series-features.gitbook.io/pyspi/development)
 ## Contributing to _pyspi_ ð¨âð¨âð¦âð¦ Contributions play a vital
```

### Comparing `pyspi-1.0.3/pyspi/__init__.py` & `pyspi-1.1.0/pyspi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/base.py` & `pyspi-1.1.0/pyspi/base.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/calculator.py` & `pyspi-1.1.0/pyspi/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy, yaml, importlib, time, warnings, os
 from tqdm import tqdm
 from collections import Counter
 from scipy import stats
 
 # From this package
 from .data import Data
-from .utils import convert_mdf_to_ddf, check_optional_deps
+from .utils import convert_mdf_to_ddf, check_optional_deps, inspect_calc_results
 
 
 class Calculator:
     """Compute all pairwise interactions.
 
     The calculator takes in a multivariate time-series dataset, computes and stores all pairwise interactions for the dataset.
     It uses a YAML configuration file that can be modified in order to compute a reduced set of pairwise methods.
@@ -30,22 +30,26 @@
             The name of the calculator. Mainly used for printing the results but can be useful if you have multiple instances, defaults to None.
         labels (array_like, optional):
             Any set of strings by which you want to label the calculator. This can be useful later for classification purposes, defaults to None.
         subset (str, optional):
             A pre-configured subset of SPIs to use. Options are "all", "fast", "sonnet", or "fabfour", defaults to "all".
         configfile (str, optional):
             The location of the YAML configuration file for a user-defined subset. See :ref:`Using a reduced SPI set`, defaults to :code:`'</path/to/pyspi>/pyspi/config.yaml'`
+        normalise (bool, optional):
+            Normalise the dataset along the time axis before computing SPIs, defaults to True.
     """
     _optional_dependencies = None
 
     def __init__(
-        self, dataset=None, name=None, labels=None, subset="all", configfile=None
+        self, dataset=None, name=None, labels=None, subset="all", configfile=None,
+        normalise=True
     ):
         self._spis = {}
         self._excluded_spis = list()
+        self._normalise = normalise
 
         # Define configfile by subset if it was not specified
         if configfile is None:
             if subset == "fast":
                 configfile = (
                     os.path.dirname(os.path.abspath(__file__)) + "/fast_config.yaml"
                 )
@@ -248,15 +252,15 @@
         """Load new dataset into existing instance.
 
         Args:
             dataset (:class:`~pyspi.data.Data`, array_list):
                 New dataset to attach to calculator.
         """
         if not isinstance(dataset, Data):
-            self._dataset = Data(Data.convert_to_numpy(dataset))
+            self._dataset = Data(Data.convert_to_numpy(dataset), normalise=self._normalise)
         else:
             self._dataset = dataset
 
         columns = pd.MultiIndex.from_product(
             [self.spis.keys(), self._dataset.procnames], names=["spi", "process"]
         )
         self._table = pd.DataFrame(
@@ -289,15 +293,17 @@
 
                 # Save results
                 self._table[spi] = S
             except Exception as err:
                 warnings.warn(f'Caught {type(err)} for SPI "{spi}": {err}')
                 self._table[spi] = np.NaN
         pbar.close()
-
+        print(f"\nCalculation complete. Time taken: {pbar.format_dict['elapsed']:.4f}s")
+        inspect_calc_results(self)
+        
     def _rmmin(self):
         """Iterate through all spis and remove the minimum (fixes absolute value errors when correlating)"""
         for spi in self.spis:
             mpi = self.table[spi]
             if not self.spis[spi].issigned():
                 self.table[spi] = mpi - np.nanmin(mpi)
```

### Comparing `pyspi-1.0.3/pyspi/config.yaml` & `pyspi-1.1.0/pyspi/config.yaml`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/data/cml.npy` & `pyspi-1.1.0/pyspi/data/cml.npy`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/data/cml7.npy` & `pyspi-1.1.0/pyspi/data/cml7.npy`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/data/forex.npy` & `pyspi-1.1.0/pyspi/data/forex.npy`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/data/standard_normal.npy` & `pyspi-1.1.0/pyspi/data/standard_normal.npy`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/data.py` & `pyspi-1.1.0/pyspi/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,19 +173,22 @@
 
         if n_processes is not None:
             data = data[:n_processes]
         if n_observations is not None:
             data = data[:, :n_observations]
 
         if self.normalise:
+            print("Normalising the dataset...\n")
             data = zscore(data, axis=1, nan_policy="omit", ddof=1)
             try:
                 data = detrend(data, axis=1)
             except ValueError as err:
                 print(f"Could not detrend data: {err}")
+        else:
+            print("Skipping normalisation of the dataset...\n")
 
         nans = np.isnan(data)
         if nans.any():
             raise ValueError(
                 f"Dataset {name} contains non-numerics (NaNs) in processes: {np.unique(np.where(nans)[0])}."
             )
```

### Comparing `pyspi-1.0.3/pyspi/fabfour_config.yaml` & `pyspi-1.1.0/pyspi/fabfour_config.yaml`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/fast_config.yaml` & `pyspi-1.1.0/pyspi/fast_config.yaml`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_AL.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_AL.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_LBFGS.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_LBFGS.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_Gauss.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_Gauss.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_comp.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_comp.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_comp_probs.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_comp_probs.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/Phi/phi_star_Gauss.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/Phi/phi_star_Gauss.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/Gauss/Cov_comp.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/Gauss/Cov_comp.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/I_s_I_s_d.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/I_s_I_s_d.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/PhiToolbox/utility/data_to_probs.m` & `pyspi-1.1.0/pyspi/lib/PhiToolbox/utility/data_to_probs.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/lib/jidt/infodynamics.jar` & `pyspi-1.1.0/pyspi/lib/jidt/infodynamics.jar`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/sonnet_config.yaml` & `pyspi-1.1.0/pyspi/sonnet_config.yaml`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/statistics/basic.py` & `pyspi-1.1.0/pyspi/statistics/basic.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/statistics/causal.py` & `pyspi-1.1.0/pyspi/statistics/causal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 import numpy as np
 import pandas as pd
 from cdt.causality.pairwise import ANM, CDS, IGCI, RECI
 import pyEDM
+from sklearn.gaussian_process import GaussianProcessRegressor
+from cdt.causality.pairwise.ANM import normalized_hsic
 
 from pyspi.base import Directed, Unsigned, Signed, parse_bivariate, parse_multivariate
 
 
 class AdditiveNoiseModel(Directed, Unsigned):
 
     name = "Additive noise model"
     identifier = "anm"
     labels = ["unsigned", "causal", "unordered", "linear", "directed"]
+    
+    # monkey-patch the anm_score function, see cdt PR #155
+    def corrected_anm_score(self, x, y):
+        gp = GaussianProcessRegressor(random_state=42).fit(x, y)
+        y_predict = gp.predict(x).reshape(-1, 1) 
+        indepscore = normalized_hsic(y_predict - y, x)
+        return indepscore
+    
+    ANM.anm_score = corrected_anm_score
 
     @parse_bivariate
     def bivariate(self, data, i=None, j=None):
         z = data.to_numpy()
         return ANM().anm_score(z[i], z[j])
```

### Comparing `pyspi-1.0.3/pyspi/statistics/distance.py` & `pyspi-1.1.0/pyspi/statistics/distance.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/statistics/infotheory.py` & `pyspi-1.1.0/pyspi/statistics/infotheory.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/statistics/misc.py` & `pyspi-1.1.0/pyspi/statistics/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import warnings
 import numpy as np
+import inspect
 
 from statsmodels.tsa import stattools
 from statsmodels.tsa.vector_ar.vecm import coint_johansen
 from sklearn.gaussian_process import kernels, GaussianProcessRegressor
 from sklearn.metrics import mean_squared_error
 from sklearn import linear_model
 import mne.connectivity as mnec
@@ -111,15 +112,19 @@
         self._model = getattr(linear_model, model)
 
     @parse_bivariate
     def bivariate(self, data, i=None, j=None):
         z = data.to_numpy()
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            mdl = self._model().fit(z[i], np.ravel(z[j]))
+            model_params = inspect.signature(self._model).parameters
+            if "random_state" in model_params:
+                mdl = self._model(random_state=42).fit(z[i], np.ravel(z[j]))
+            else:
+                mdl = self._model().fit(z[i], np.ravel(z[j]))
         y_predict = mdl.predict(z[i])
         return mean_squared_error(y_predict, np.ravel(z[j]))
 
 
 class GPModel(Directed, Unsigned):
     name = "Gaussian process regression"
     identifier = "gpfit"
```

### Comparing `pyspi-1.0.3/pyspi/statistics/spectral.py` & `pyspi-1.1.0/pyspi/statistics/spectral.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/statistics/wavelet.py` & `pyspi-1.1.0/pyspi/statistics/wavelet.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/pyspi/utils.py` & `pyspi-1.1.0/pyspi/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -224,7 +224,51 @@
 -----------------
 - {source_file_info}
 - Total SPIs Matched: {spis_found} SPI(s) were found with the specific keywords: {keywords}.
 - New File Created: A YAML file named `{output_name}.yaml` has been saved in the current directory: `{output_file}'
 - Next Steps: To utilise the filtered set of SPIs, please initialise a new Calculator instance with the following command:
 `Calculator(configfile='{output_file}')`
 """)
+
+def inspect_calc_results(calc):
+    total_num_spis = calc.n_spis
+    num_procs = calc.dataset.n_processes
+    spi_results = dict({'Successful': list(), 'NaNs': list(), 'Partial NaNs': list()})
+    for key in calc.spis.keys():
+        if calc.table[key].isna().all().all():
+            spi_results['NaNs'].append(key)
+        elif calc.table[key].isnull().values.sum() > num_procs:
+            # off-diagonal NaNs
+            spi_results['Partial NaNs'].append(key)
+        else:
+            # returned numeric values (i.e., not NaN)
+            spi_results['Successful'].append(key)
+    
+    # print summary
+    double_line_60 = "="*60
+    single_line_60 = "-"*60
+    print("\nSPI Computation Results Summary")
+    print(double_line_60)
+    print(f"\nTotal number of SPIs attempted: {total_num_spis}")
+    print(f"Number of SPIs successfully computed: {len(spi_results['Successful'])} ({len(spi_results['Successful']) / total_num_spis * 100:.2f}%)")
+    print(single_line_60)
+    print("Category       | Count | Percentage")
+    print(single_line_60)
+    for category, spis in spi_results.items():
+        count = len(spis)
+        percentage = (count / total_num_spis) * 100
+        print(f"{category:14} | {count:5} | {percentage:6.2f}%")
+    print(single_line_60)
+
+    if spi_results['NaNs']:
+        print(f"\n[{len(spi_results['NaNs'])}] SPI(s) produced NaN outputs:")
+        print(single_line_60)
+        for i, spi in enumerate(spi_results['NaNs']):
+            print(f"{i+1}. {spi}")
+        print(single_line_60 + "\n")
+    if spi_results['Partial NaNs']:
+        print(f"\n[{len(spi_results['Partial NaNs'])}] SPIs which produced partial NaN outputs:")
+        print(single_line_60)
+        for i, spi in enumerate(spi_results['Partial NaNs']):
+            print(f"{i+1}. {spi}")
+        print(single_line_60 + "\n")
+
```

### Comparing `pyspi-1.0.3/pyspi.egg-info/PKG-INFO` & `pyspi-1.1.0/pyspi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspi
-Version: 1.0.3
+Version: 1.1.0
 Summary: Library for pairwise analysis of time series data.
 Home-page: https://github.com/DynamicsAndNeuralSystems/pyspi
 Author: Oliver M. Cliff
 Author-email: "Oliver M. Cliff" <oliver.m.cliff@gmail.com>
 Maintainer: Joshua B. Moore
 Maintainer-email: joshua.moore@sydney.edu.au
 License: GNU General Public License v3 (GPLv3)
@@ -17,37 +17,38 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: <3.10,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: scikit-learn==1.0.1
-Requires-Dist: scipy==1.7.3
-Requires-Dist: numpy>=1.21.1
-Requires-Dist: pandas==1.5.0
-Requires-Dist: statsmodels==0.12.1
-Requires-Dist: pyyaml==5.4
-Requires-Dist: tqdm==4.50.2
-Requires-Dist: nitime==0.9
-Requires-Dist: hyppo==0.2.1
-Requires-Dist: pyEDM==1.9.3
-Requires-Dist: jpype1==1.2.0
-Requires-Dist: sktime==0.8.0
-Requires-Dist: dill==0.3.2
-Requires-Dist: spectral-connectivity==0.2.4.dev0
-Requires-Dist: torch==1.13.1
+Requires-Dist: h5py
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: statsmodels
+Requires-Dist: pyyaml
+Requires-Dist: tqdm
+Requires-Dist: nitime
+Requires-Dist: hyppo
+Requires-Dist: pyEDM==1.15.2.0
+Requires-Dist: jpype1
+Requires-Dist: sktime
+Requires-Dist: dill
+Requires-Dist: spectral-connectivity
+Requires-Dist: torch
 Requires-Dist: cdt==0.5.23
-Requires-Dist: oct2py==5.2.0
-Requires-Dist: tslearn==0.5.2
+Requires-Dist: oct2py
+Requires-Dist: tslearn
 Requires-Dist: mne==0.23.0
-Requires-Dist: seaborn==0.11.0
+Requires-Dist: seaborn
 Provides-Extra: testing
 Requires-Dist: pytest==5.4.2; extra == "testing"
 
 <p align="center">
   <picture>
     <source srcset="img/pyspi_logo_darkmode.png" media="(prefers-color-scheme: dark)">
     <img src="img/pyspi_logo.png" alt="pyspi logo" height="200"/>
@@ -59,15 +60,15 @@
 
 
 <p align="center">
  	<a href="https://zenodo.org/badge/latestdoi/601919618"><img src="https://zenodo.org/badge/601919618.svg" height="20"/></a>
     <a href="https://www.gnu.org/licenses/gpl-3.0"><img src="https://img.shields.io/badge/License-GPLv3-blue.svg" height="20"/></a>
     <a href="https://github.com/DynamicsAndNeuralSystems/pyspi/actions/workflows/run_unit_tests.yaml"><img src="https://github.com/DynamicsAndNeuralSystems/pyspi/actions/workflows/run_unit_tests.yaml/badge.svg" height="20"/></a>
     <a href="https://twitter.com/compTimeSeries"><img src="https://img.shields.io/twitter/url/https/twitter.com/compTimeSeries.svg?style=social&label=Follow%20%40compTimeSeries" height="20"/></a><br>
-    <a href="https://www.python.org"><img src="https://img.shields.io/badge/Python-3.8%20|%203.9-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.8 | 3.9"></a>
+    <a href="https://www.python.org"><img src="https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.8 | 3.9 | 3.10 | 3.11 | 3.12"></a>
 </p>
 
 _pyspi_ is a comprehensive python library for computing statistics of pairwise interactions (SPIs) from multivariate time-series (MTS) data.
 The toolbox provides easy access to hundreds of methods for evaluating the relationship between pairs of time series, from simple statistics (like correlation) to advanced multi-step algorithms (like Granger causality).
 The code is licensed under the [GNU GPL v3 license](http://www.gnu.org/licenses/gpl-3.0.html) (or later).
 
 **Feel free to reach out for help with real-world applications.**
@@ -119,29 +120,14 @@
 - [Finance: stock price time series](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/finance-stock-price-time-series)
 
 
 - [Neuroimaging: fMRI time series)](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/neuroimaging-fmri-time-series)
 
 ### Advanced Usage
 For advanced users, we offer several additional guides in the [full documentation](https://time-series-features.gitbook.io/pyspi/usage/advanced-usage) on how you can distribute your _pyspi_ jobs across PBS clusters, as well as how you can construct your own subsets of SPIs. 
-Click one of the following dropdowns for more information:
-
-<details closed>
-<summary>Distributing pyspi calculations</summary>
-<p>If you have access to a PBS cluster and are processing MTS with many processes (or are analyzing many MTS), then you may find the <a href="https://github.com/DynamicsAndNeuralSystems/pyspi-distribute"><em>pyspi distribute</em></a> repository helpful.
-In the full <a href="https://time-series-features.gitbook.io/pyspi/usage/advanced-usage/distributing-calculations-on-a-cluster">documentation </a>, we provide a comprehensive guide on how you can distribute <em>pyspi</em> calculations on a PBS cluster, along with the necessary scripts and commands to get started!</p>
-</details>
-
-<details closed>
-<summary>Reduced subsets</summary>
-<p>If your dataset is large (containing many processes and/or observations), you can use a pre-configured set of reduced statistics or create your own subsets.
-Follow the guide in the <a href="https://time-series-features.gitbook.io/pyspi/usage/advanced-usage/using-a-reduced-spi-set">documentation </a> to learn how you can create your own reduced subsets.</p>
-</details>
-
-
 
 ## SPI Descriptions 📋
 To access a table with a high-level overview of the _pyspi_ library of SPIs, including their associated identifiers, see the [table of SPIs](https://time-series-features.gitbook.io/pyspi/spis/table-of-spis) in the full documentation.
 For detailed descriptions of each SPI, as well as its associated estimators, we provide a full breakdown in the [SPI descriptions](https://time-series-features.gitbook.io/pyspi/spis/spi-descriptions) page of our documentation. 
 
 ## Documentation
 The full documentation is hosted on [GitBooks](https://time-series-features.gitbook.io/pyspi/). 
@@ -212,8 +198,7 @@
 
 <a href="https://github.com/DynamicsAndNeuralSystems/pyspi/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=DynamicsAndNeuralSystems/pyspi" />
 </a>
 
 ## License 🧾
 _pyspi_ is released under the [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0).
-
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1 Name: pyspi Version: 1.0.3 Summary: Library for pairwise
+Metadata-Version: 2.1 Name: pyspi Version: 1.1.0 Summary: Library for pairwise
 analysis of time series data. Home-page: https://github.com/
 DynamicsAndNeuralSystems/pyspi Author: Oliver M. Cliff Author-email: "Oliver M.
 Cliff"
 gmail.com> Maintainer: Joshua B. Moore Maintainer-email:
 joshua.moore@sydney.edu.au License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/DynamicsAndNeuralSystems/pyspi
 Project-URL: Documentation, https://time-series-features.gitbook.io/pyspi/
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Development Status :: 1 - Planning Classifier:
 Operating System :: POSIX :: Linux Classifier: Intended Audience :: Science/
 Research Classifier: Environment :: Console Classifier: Environment :: Other
 Environment Classifier: Topic :: Scientific/Engineering :: Physics Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Scientific/
-Engineering :: Medical Science Apps. Requires-Python: <3.10,>=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist: scikit-
-learn==1.0.1 Requires-Dist: scipy==1.7.3 Requires-Dist: numpy>=1.21.1 Requires-
-Dist: pandas==1.5.0 Requires-Dist: statsmodels==0.12.1 Requires-Dist:
-pyyaml==5.4 Requires-Dist: tqdm==4.50.2 Requires-Dist: nitime==0.9 Requires-
-Dist: hyppo==0.2.1 Requires-Dist: pyEDM==1.9.3 Requires-Dist: jpype1==1.2.0
-Requires-Dist: sktime==0.8.0 Requires-Dist: dill==0.3.2 Requires-Dist:
-spectral-connectivity==0.2.4.dev0 Requires-Dist: torch==1.13.1 Requires-Dist:
-cdt==0.5.23 Requires-Dist: oct2py==5.2.0 Requires-Dist: tslearn==0.5.2
-Requires-Dist: mne==0.23.0 Requires-Dist: seaborn==0.11.0 Provides-Extra:
-testing Requires-Dist: pytest==5.4.2; extra == "testing"
+Engineering :: Medical Science Apps. Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist: h5py
+Requires-Dist: scikit-learn Requires-Dist: scipy Requires-Dist: numpy Requires-
+Dist: pandas Requires-Dist: statsmodels Requires-Dist: pyyaml Requires-Dist:
+tqdm Requires-Dist: nitime Requires-Dist: hyppo Requires-Dist: pyEDM==1.15.2.0
+Requires-Dist: jpype1 Requires-Dist: sktime Requires-Dist: dill Requires-Dist:
+spectral-connectivity Requires-Dist: torch Requires-Dist: cdt==0.5.23 Requires-
+Dist: oct2py Requires-Dist: tslearn Requires-Dist: mne==0.23.0 Requires-Dist:
+seaborn Provides-Extra: testing Requires-Dist: pytest==5.4.2; extra ==
+"testing"
                                  [pyspi logo]
   ************ ppyyssppii:: PPyytthhoonn TToooollkkiitt ooff SSttaattiissttiiccss ffoorr PPaaiirrwwiissee IInntteerraaccttiioonnss ************
 _[_h_t_t_p_s_:_/_/_z_e_n_o_d_o_._o_r_g_/_b_a_d_g_e_/_6_0_1_9_1_9_6_1_8_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-
   _G_P_L_v_3_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_D_y_n_a_m_i_c_s_A_n_d_N_e_u_r_a_l_S_y_s_t_e_m_s_/_p_y_s_p_i_/_a_c_t_i_o_n_s_/
  _w_o_r_k_f_l_o_w_s_/_r_u_n___u_n_i_t___t_e_s_t_s_._y_a_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_u_r_l_/
                               _h_t_t_p_s_/_t_w_i_t_t_e_r_._c_o_m_/
        _c_o_m_p_T_i_m_e_S_e_r_i_e_s_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_c_o_m_p_T_i_m_e_S_e_r_i_e_s_]
-                              _[_P_y_t_h_o_n_ _3_._8_ _|_ _3_._9_]
+                    _[_P_y_t_h_o_n_ _3_._8_ _|_ _3_._9_ _|_ _3_._1_0_ _|_ _3_._1_1_ _|_ _3_._1_2_]
 _pyspi_ is a comprehensive python library for computing statistics of pairwise
 interactions (SPIs) from multivariate time-series (MTS) data. The toolbox
 provides easy access to hundreds of methods for evaluating the relationship
 between pairs of time series, from simple statistics (like correlation) to
 advanced multi-step algorithms (like Granger causality). The code is licensed
 under the [GNU GPL v3 license](http://www.gnu.org/licenses/gpl-3.0.html) (or
 later). **Feel free to reach out for help with real-world applications.**
@@ -83,40 +82,28 @@
 series](https://time-series-features.gitbook.io/pyspi/usage/walkthrough-
 tutorials/finance-stock-price-time-series) - [Neuroimaging: fMRI time series)]
 (https://time-series-features.gitbook.io/pyspi/usage/walkthrough-tutorials/
 neuroimaging-fmri-time-series) ### Advanced Usage For advanced users, we offer
 several additional guides in the [full documentation](https://time-series-
 features.gitbook.io/pyspi/usage/advanced-usage) on how you can distribute your
 _pyspi_ jobs across PBS clusters, as well as how you can construct your own
-subsets of SPIs. Click one of the following dropdowns for more information:
-Distributing pyspi calculations
-If you have access to a PBS cluster and are processing MTS with many processes
-(or are analyzing many MTS), then you may find the _pp_yy_ss_pp_ii_ _dd_ii_ss_tt_rr_ii_bb_uu_tt_ee repository
-helpful. In the full _d_o_c_u_m_e_n_t_a_t_i_o_n_ , we provide a comprehensive guide on how
-you can distribute ppyyssppii calculations on a PBS cluster, along with the
-necessary scripts and commands to get started!
-Reduced subsets
-If your dataset is large (containing many processes and/or observations), you
-can use a pre-configured set of reduced statistics or create your own subsets.
-Follow the guide in the _d_o_c_u_m_e_n_t_a_t_i_o_n_ to learn how you can create your own
-reduced subsets.
-## SPI Descriptions ð To access a table with a high-level overview of the
-_pyspi_ library of SPIs, including their associated identifiers, see the [table
-of SPIs](https://time-series-features.gitbook.io/pyspi/spis/table-of-spis) in
-the full documentation. For detailed descriptions of each SPI, as well as its
-associated estimators, we provide a full breakdown in the [SPI descriptions]
-(https://time-series-features.gitbook.io/pyspi/spis/spi-descriptions) page of
-our documentation. ## Documentation The full documentation is hosted on
-[GitBooks](https://time-series-features.gitbook.io/pyspi/). Use the following
-links to quickly access some of the key sections: - [Full installation guide]
-(https://time-series-features.gitbook.io/pyspi/installation) -
-[Troubleshooting](https://time-series-features.gitbook.io/pyspi/installation/
-troubleshooting) - [Alternative installation options](https://time-series-
-features.gitbook.io/pyspi/installation/alternative-installation-options) -
-[Usage guide](https://time-series-features.gitbook.io/pyspi/usage) -
+subsets of SPIs. ## SPI Descriptions ð To access a table with a high-level
+overview of the _pyspi_ library of SPIs, including their associated
+identifiers, see the [table of SPIs](https://time-series-features.gitbook.io/
+pyspi/spis/table-of-spis) in the full documentation. For detailed descriptions
+of each SPI, as well as its associated estimators, we provide a full breakdown
+in the [SPI descriptions](https://time-series-features.gitbook.io/pyspi/spis/
+spi-descriptions) page of our documentation. ## Documentation The full
+documentation is hosted on [GitBooks](https://time-series-features.gitbook.io/
+pyspi/). Use the following links to quickly access some of the key sections: -
+[Full installation guide](https://time-series-features.gitbook.io/pyspi/
+installation) - [Troubleshooting](https://time-series-features.gitbook.io/
+pyspi/installation/troubleshooting) - [Alternative installation options](https:
+//time-series-features.gitbook.io/pyspi/installation/alternative-installation-
+options) - [Usage guide](https://time-series-features.gitbook.io/pyspi/usage) -
 [Distributing _pyspi_ computations](https://time-series-features.gitbook.io/
 pyspi/usage/advanced-usage/distributing-calculations-on-a-cluster) - [Table of
 SPIs and descriptions](https://time-series-features.gitbook.io/pyspi/spis) -
 [FAQ](https://time-series-features.gitbook.io/pyspi/usage/faq) - [API
 Reference](https://time-series-features.gitbook.io/pyspi/api-reference) -
 [Development guide](https://time-series-features.gitbook.io/pyspi/development)
 ## Contributing to _pyspi_ ð¨âð¨âð¦âð¦ Contributions play a vital
```

### Comparing `pyspi-1.0.3/pyspi.egg-info/SOURCES.txt` & `pyspi-1.1.0/pyspi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/setup.py` & `pyspi-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,34 +4,35 @@
 # https://pypi.python.org/pypi?:action=list_classifiers
 
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 
 install_requires = [
-        'scikit-learn==1.0.1',
-        'scipy==1.7.3',
-        'numpy>=1.21.1',
-        'pandas==1.5.0',
-        'statsmodels==0.12.1',
-        'pyyaml==5.4',
-        'tqdm==4.50.2',
-        'nitime==0.9',
-        'hyppo==0.2.1',
-        'pyEDM==1.9.3',
-        'jpype1==1.2.0',
-        'sktime==0.8.0',
-        'dill==0.3.2',
-        'spectral-connectivity==0.2.4.dev0',
-        'torch==1.13.1',
+        'h5py',
+        'scikit-learn',
+        'scipy',
+        'numpy',
+        'pandas',
+        'statsmodels',
+        'pyyaml',
+        'tqdm',
+        'nitime',
+        'hyppo',
+        'pyEDM==1.15.2.0',
+        'jpype1',
+        'sktime',
+        'dill',
+        'spectral-connectivity',
+        'torch',
         'cdt==0.5.23',
-        'oct2py==5.2.0',
-        'tslearn==0.5.2',
+        'oct2py',
+        'tslearn',
         'mne==0.23.0',
-        'seaborn==0.11.0'
+        'seaborn'
 ]
 
 testing_extras = [
     'pytest==5.4.2',  # unittest.TestCase funkyness, see commit 77c1505ab
 ]
 
 
@@ -57,15 +58,15 @@
                         'lib/PhiToolbox/utility/Gauss/H_gauss.m',
                         'lib/PhiToolbox/utility/Gauss/logdet.m',
                         'data/cml.npy',
                         'data/forex.npy',
                         'data/standard_normal.npy',
                         'data/cml7.npy']},
     include_package_data=True,
-    version='1.0.3',
+    version='1.1.0',
     description='Library for pairwise analysis of time series data.',
     author='Oliver M. Cliff',
     author_email='oliver.m.cliff@gmail.com',
     url='https://github.com/DynamicsAndNeuralSystems/pyspi',
     long_description=long_description,
     classifiers=[
         "Programming Language :: Python",
```

### Comparing `pyspi-1.0.3/tests/test_SPIs.py` & `pyspi-1.1.0/tests/test_SPIs.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.3/tests/test_calc.py` & `pyspi-1.1.0/tests/test_calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,20 +280,29 @@
     for (index, calc) in enumerate(calc_frame.calculators[0]):
         assert calc.name == dataset_names[index], "Indiviudal calculator has unexpected name."
         assert calc.labels == dataset_labels[index], "Indiviudal calculator has unexpected label."
     
     # check that compute runs
     calc_frame.compute()
 
-
 def test_correlation_frame_normal_operation():
     """Test whether the correlation frame instantiates as expected.""" 
     datasets = [np.random.randn(3, 100) for _ in range(3)]
     dataset_names = ['d1', 'd2', 'd3']
     dataset_labels = ['label1', 'label2', 'label3']
     calc_frame = CalculatorFrame(name="MyCalcFrame", datasets=[Data(data=data, dim_order='ps') for data in datasets], 
                                  names=dataset_names, labels=dataset_labels, subset='fabfour')
     
     calc_frame.compute()
     cf = calc_frame.get_correlation_df()
 
     assert not(cf[0].empty), "Correlation frame is empty."
+
+def test_normalisation_flag():
+    """Test whether the normalisation flag when instantiating
+    the calculator works as expected."""
+    data = np.random.randn(3, 100)
+    calc = Calculator(dataset=data, normalise=False)
+    calc_loaded_dataset = calc.dataset.to_numpy().squeeze()
+    
+    assert (calc_loaded_dataset == data).all(), f"Calculator normalise=False not producing the correct output." 
+
```

### Comparing `pyspi-1.0.3/tests/test_utils.py` & `pyspi-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

