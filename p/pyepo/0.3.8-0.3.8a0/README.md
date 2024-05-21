# Comparing `tmp/pyepo-0.3.8.tar.gz` & `tmp/pyepo-0.3.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepo-0.3.8.tar", last modified: Wed Apr 24 20:57:05 2024, max compression
+gzip compressed data, was "pyepo-0.3.8a0.tar", last modified: Tue May 21 20:30:45 2024, max compression
```

## Comparing `pyepo-0.3.8.tar` & `pyepo-0.3.8a0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 20:57:05.652554 pyepo-0.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.644554 pyepo-0.3.8/pyepo/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/EPO.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.644554 pyepo-0.3.8/pyepo/data/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.648554 pyepo-0.3.8/pyepo/func/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/abcmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/perturbed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/spoplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/utlis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.648554 pyepo-0.3.8/pyepo/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/regret.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/unambregret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.648554 pyepo-0.3.8/pyepo/model/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.648554 pyepo-0.3.8/pyepo/model/copt/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/copt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/copt/coptmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/copt/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/copt/shortestpath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/pyepo/model/grb/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/grbmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/pyepo/model/omo/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/omo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/omo/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/omo/omomodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/omo/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/opt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/pyepo/twostage/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/twostage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/twostage/autosklearnpred.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/twostage/sklearnpred.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/utlis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/pyepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:57:05.652554 pyepo-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-24 20:57:00.000000 pyepo-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.277713 pyepo-0.3.8a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 20:30:45.277713 pyepo-0.3.8a0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.269713 pyepo-0.3.8a0/pyepo/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/EPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.269713 pyepo-0.3.8a0/pyepo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/data/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/data/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/data/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/data/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.273713 pyepo-0.3.8a0/pyepo/func/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/func/abcmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/func/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/func/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/func/perturbed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/func/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/func/spoplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/func/utlis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.273713 pyepo-0.3.8a0/pyepo/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/metric/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/metric/mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/metric/regret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/metric/unambregret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.273713 pyepo-0.3.8a0/pyepo/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.273713 pyepo-0.3.8a0/pyepo/model/copt/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/copt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/copt/coptmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/copt/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/copt/shortestpath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.273713 pyepo-0.3.8a0/pyepo/model/grb/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/grb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/grb/grbmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/grb/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/grb/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/grb/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/grb/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.273713 pyepo-0.3.8a0/pyepo/model/omo/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/omo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/omo/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/omo/omomodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/omo/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/model/opt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.277713 pyepo-0.3.8a0/pyepo/twostage/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/twostage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/twostage/autosklearnpred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/twostage/sklearnpred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/pyepo/utlis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:30:45.277713 pyepo-0.3.8a0/pyepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 20:30:45.000000 pyepo-0.3.8a0/pyepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-21 20:30:45.000000 pyepo-0.3.8a0/pyepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:30:45.000000 pyepo-0.3.8a0/pyepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-21 20:30:45.000000 pyepo-0.3.8a0/pyepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 20:30:45.000000 pyepo-0.3.8a0/pyepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:30:45.277713 pyepo-0.3.8a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-21 20:30:41.000000 pyepo-0.3.8a0/setup.py
```

### Comparing `pyepo-0.3.8/PKG-INFO` & `pyepo-0.3.8a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepo
-Version: 0.3.8
+Version: 0.3.8a0
 Summary: PyTorch-based End-to-End Predict-then-Optimize Tool
 Home-page: https://github.com/khalil-research/PyEPO
 Author: Bo Tang
 Author-email: bolucas.tang@mail.utoronto.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyepo-0.3.8/pyepo/data/dataset.py` & `pyepo-0.3.8a0/pyepo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/data/knapsack.py` & `pyepo-0.3.8a0/pyepo/data/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/data/portfolio.py` & `pyepo-0.3.8a0/pyepo/data/portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,9 +48,9 @@
         r[i] = (0.05 * np.dot(B, x[i].reshape(p, 1)).T / np.sqrt(p) + \
                 0.1 ** (1 / deg)) ** deg
         # random noise
         f = rnd.randn(num_features)
         eps = rnd.randn(num_assets)
         r[i] += L @ f + 0.01 * noise_level * eps
     # covariance matrix of the returns
-    cov = L @ L.T + (1e-2 * noise_level) * np.eye(num_assets)
+    cov = L @ L.T + (1e-2 * noise_level) ** 2 * np.eye(num_assets)
     return cov, x, r
```

### Comparing `pyepo-0.3.8/pyepo/data/shortestpath.py` & `pyepo-0.3.8a0/pyepo/data/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/data/tsp.py` & `pyepo-0.3.8a0/pyepo/data/tsp.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/func/abcmodule.py` & `pyepo-0.3.8a0/pyepo/func/abcmodule.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/func/blackbox.py` & `pyepo-0.3.8a0/pyepo/func/blackbox.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/func/contrastive.py` & `pyepo-0.3.8a0/pyepo/func/contrastive.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/func/perturbed.py` & `pyepo-0.3.8a0/pyepo/func/perturbed.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/func/rank.py` & `pyepo-0.3.8a0/pyepo/func/rank.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/func/spoplus.py` & `pyepo-0.3.8a0/pyepo/func/spoplus.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/func/utlis.py` & `pyepo-0.3.8a0/pyepo/func/utlis.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/metric/metrics.py` & `pyepo-0.3.8a0/pyepo/metric/metrics.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/metric/mse.py` & `pyepo-0.3.8a0/pyepo/metric/mse.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/metric/regret.py` & `pyepo-0.3.8a0/pyepo/metric/regret.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/metric/unambregret.py` & `pyepo-0.3.8a0/pyepo/metric/unambregret.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/copt/coptmodel.py` & `pyepo-0.3.8a0/pyepo/model/copt/coptmodel.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/copt/knapsack.py` & `pyepo-0.3.8a0/pyepo/model/copt/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/copt/shortestpath.py` & `pyepo-0.3.8a0/pyepo/model/copt/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/grb/grbmodel.py` & `pyepo-0.3.8a0/pyepo/model/grb/grbmodel.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/grb/knapsack.py` & `pyepo-0.3.8a0/pyepo/model/grb/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/grb/portfolio.py` & `pyepo-0.3.8a0/pyepo/model/grb/portfolio.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 from gurobipy import GRB
 
 from pyepo.model.grb.grbmodel import optGrbModel
 
 
 class portfolioModel(optGrbModel):
     """
-    This class is optimization model for portfolio problem
+    This class is an optimization model for portfolio problem
 
     Attributes:
         _model (GurobiPy model): Gurobi model
         num_assets (int): number of assets
-        cov (numpy.ndarray): covariance matrix of the returns
+        covariance (numpy.ndarray): covariance matrix of the returns
         risk_level (float): risk level
     """
 
     def __init__(self, num_assets, covariance, gamma=2.25):
         """
         Args:
             num_assets (int): number of assets
             covariance (numpy.ndarray): covariance matrix of the returns
             gamma (float): risk level parameter
         """
         self.num_assets = num_assets
-        self.cov = covariance
+        self.covariance = covariance
         self.risk_level = self._getRiskLevel(gamma)
         super().__init__()
 
     def _getRiskLevel(self, gamma):
         """
-        A method to calculate risk level
+        A method to calculate the risk level
 
         Returns:
             float: risk level
         """
         risk_level = gamma * np.mean(self.cov)
         return risk_level
 
@@ -55,29 +55,29 @@
         m = gp.Model("portfolio")
         # varibles
         x = m.addMVar(self.num_assets, ub=1, name="x")
         # sense
         m.modelSense = GRB.MAXIMIZE
         # constraints
         m.addConstr(x.sum() == 1, "budget")
-        m.addConstr(x.T @ self.cov @ x <= self.risk_level, "risk_limit")
+        m.addConstr(x.T @ self.covariance @ x <= self.risk_level, "risk_limit")
         return m, x
 
 
 if __name__ == "__main__":
 
     import random
     from pyepo.data.portfolio import genData
     # random seed
     random.seed(42)
     # set random cost for test
-    cov, _, revenue = genData(num_data=100, num_features=4, num_assets=50, deg=2)
+    covariance, _, revenue = genData(num_data=100, num_features=4, num_assets=50, deg=2)
 
     # solve model
-    optmodel = portfolioModel(num_assets=50, covariance=cov) # init model
+    optmodel = portfolioModel(num_assets=50, covariance=covariance) # init model
     optmodel = optmodel.copy()
     optmodel.setObj(revenue[0]) # set objective function
     sol, obj = optmodel.solve() # solve
     # print res
     print('Obj: {}'.format(obj))
     for i in range(50):
         if sol[i] > 1e-3:
```

### Comparing `pyepo-0.3.8/pyepo/model/grb/shortestpath.py` & `pyepo-0.3.8a0/pyepo/model/grb/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/grb/tsp.py` & `pyepo-0.3.8a0/pyepo/model/grb/tsp.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/omo/knapsack.py` & `pyepo-0.3.8a0/pyepo/model/omo/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/omo/omomodel.py` & `pyepo-0.3.8a0/pyepo/model/omo/omomodel.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/omo/shortestpath.py` & `pyepo-0.3.8a0/pyepo/model/omo/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/model/opt.py` & `pyepo-0.3.8a0/pyepo/model/opt.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/twostage/autosklearnpred.py` & `pyepo-0.3.8a0/pyepo/twostage/autosklearnpred.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo/utlis.py` & `pyepo-0.3.8a0/pyepo/utlis.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/pyepo.egg-info/PKG-INFO` & `pyepo-0.3.8a0/pyepo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepo
-Version: 0.3.8
+Version: 0.3.8a0
 Summary: PyTorch-based End-to-End Predict-then-Optimize Tool
 Home-page: https://github.com/khalil-research/PyEPO
 Author: Bo Tang
 Author-email: bolucas.tang@mail.utoronto.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyepo-0.3.8/pyepo.egg-info/SOURCES.txt` & `pyepo-0.3.8a0/pyepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.8/setup.py` & `pyepo-0.3.8a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # project dir
     packages = setuptools.find_packages(),
     # description
     description = "PyTorch-based End-to-End Predict-then-Optimize Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # version
-    version = "0.3.8",
+    version = "0.3.8a",
     # Github repo
     url = "https://github.com/khalil-research/PyEPO",
     # author name
     author = "Bo Tang",
     # mail address
     author_email = "bolucas.tang@mail.utoronto.ca",
     # dependencies
```

