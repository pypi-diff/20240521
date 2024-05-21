# Comparing `tmp/graphene_mlx-0.0.15.tar.gz` & `tmp/graphene_mlx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_mlx-0.0.15.tar", last modified: Sun May 19 07:56:52 2024, max compression
+gzip compressed data, was "graphene_mlx-0.1.0.tar", last modified: Tue May 21 19:01:26 2024, max compression
```

## Comparing `graphene_mlx-0.0.15.tar` & `graphene_mlx-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.880356 graphene_mlx-0.0.15/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.872356 graphene_mlx-0.0.15/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.876356 graphene_mlx-0.0.15/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/.github/workflows/python-precommit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-19 07:56:52.880356 graphene_mlx-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.876356 graphene_mlx-0.0.15/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/examples/cifar_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/examples/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.880356 graphene_mlx-0.0.15/graphene_mlx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-19 07:56:52.000000 graphene_mlx-0.0.15/graphene_mlx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-19 07:56:52.000000 graphene_mlx-0.0.15/graphene_mlx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:56:52.000000 graphene_mlx-0.0.15/graphene_mlx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-19 07:56:52.000000 graphene_mlx-0.0.15/graphene_mlx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 07:56:52.000000 graphene_mlx-0.0.15/graphene_mlx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.876356 graphene_mlx-0.0.15/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/requirements/requirements.dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/requirements/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.876356 graphene_mlx-0.0.15/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/scripts/install.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/scripts/lib.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1335 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/scripts/lock-requirements.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:56:52.880356 graphene_mlx-0.0.15/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.876356 graphene_mlx-0.0.15/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.876356 graphene_mlx-0.0.15/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/callbacks/model_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.880356 graphene_mlx-0.0.15/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/core/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/core/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/core/trainmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.880356 graphene_mlx-0.0.15/src/loops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/loops/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/loops/train_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/loops/validation_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:56:52.880356 graphene_mlx-0.0.15/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-19 07:56:43.000000 graphene_mlx-0.0.15/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.232504 graphene_mlx-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.224504 graphene_mlx-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.228504 graphene_mlx-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/.github/workflows/python-precommit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-21 19:01:26.232504 graphene_mlx-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.228504 graphene_mlx-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/examples/cifar_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/examples/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.228504 graphene_mlx-0.1.0/graphene/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.228504 graphene_mlx-0.1.0/graphene/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/callbacks/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/callbacks/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/callbacks/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.228504 graphene_mlx-0.1.0/graphene/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/core/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/core/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/core/trainmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.228504 graphene_mlx-0.1.0/graphene/loops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/loops/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/loops/train_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/loops/validation_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.232504 graphene_mlx-0.1.0/graphene/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/graphene/metrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.232504 graphene_mlx-0.1.0/graphene_mlx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-21 19:01:26.000000 graphene_mlx-0.1.0/graphene_mlx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 19:01:26.000000 graphene_mlx-0.1.0/graphene_mlx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:01:26.000000 graphene_mlx-0.1.0/graphene_mlx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 19:01:26.000000 graphene_mlx-0.1.0/graphene_mlx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 19:01:26.000000 graphene_mlx-0.1.0/graphene_mlx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.232504 graphene_mlx-0.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/requirements/requirements.dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/requirements/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:01:26.232504 graphene_mlx-0.1.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/scripts/install.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/scripts/lib.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1335 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/scripts/lock-requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:01:26.232504 graphene_mlx-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-21 19:01:16.000000 graphene_mlx-0.1.0/train.py
```

### Comparing `graphene_mlx-0.0.15/.github/workflows/package.yml` & `graphene_mlx-0.1.0/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/.github/workflows/python-precommit.yml` & `graphene_mlx-0.1.0/.github/workflows/python-precommit.yml`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/.gitignore` & `graphene_mlx-0.1.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -160,7 +160,8 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 # VS CODE
 .vscode/
 
 requirements/*.lock
+wandb/*
```

### Comparing `graphene_mlx-0.0.15/.pre-commit-config.yaml` & `graphene_mlx-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/.readthedocs.yaml` & `graphene_mlx-0.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/LICENSE` & `graphene_mlx-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/PKG-INFO` & `graphene_mlx-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: graphene-mlx
-Version: 0.0.15
+Version: 0.1.0
 Summary: Neural Network Trainer for MLX
 Author-email: Petru Radulescu <petruradulescu.v@gmail.com>
 License: Apache License, Version 2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: mlx
 Requires-Dist: mlx-data
 Requires-Dist: setuptools
+Requires-Dist: tqdm
+Requires-Dist: wandb
 Provides-Extra: dev
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: ruff>=0.0.282; extra == "dev"
 Requires-Dist: pre-commit>=3.3.0; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: ruff-lsp; extra == "dev"
```

### Comparing `graphene_mlx-0.0.15/README.md` & `graphene_mlx-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/examples/cifar_datamodule.py` & `graphene_mlx-0.1.0/examples/cifar_datamodule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from types import SimpleNamespace
 
 import numpy as np
 from mlx.data.datasets.cifar import load_cifar10
 
-from src.core.datamodule import DataModule
+from graphene import DataModule
 
 
 class Cifar10DataModule(DataModule):
     mean = np.array([0.485, 0.456, 0.406]).reshape((1, 1, 3))
     std = np.array([0.229, 0.224, 0.225]).reshape((1, 1, 3))
 
     @staticmethod
```

### Comparing `graphene_mlx-0.0.15/examples/resnet.py` & `graphene_mlx-0.1.0/examples/resnet.py`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/graphene_mlx.egg-info/PKG-INFO` & `graphene_mlx-0.1.0/graphene_mlx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: graphene-mlx
-Version: 0.0.15
+Version: 0.1.0
 Summary: Neural Network Trainer for MLX
 Author-email: Petru Radulescu <petruradulescu.v@gmail.com>
 License: Apache License, Version 2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: mlx
 Requires-Dist: mlx-data
 Requires-Dist: setuptools
+Requires-Dist: tqdm
+Requires-Dist: wandb
 Provides-Extra: dev
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: ruff>=0.0.282; extra == "dev"
 Requires-Dist: pre-commit>=3.3.0; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: ruff-lsp; extra == "dev"
```

### Comparing `graphene_mlx-0.0.15/graphene_mlx.egg-info/SOURCES.txt` & `graphene_mlx-0.1.0/graphene_mlx.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,32 +7,35 @@
 pyproject.toml
 train.py
 .github/workflows/package.yml
 .github/workflows/python-precommit.yml
 examples/__init__.py
 examples/cifar_datamodule.py
 examples/resnet.py
+graphene/__init__.py
+graphene/callbacks/__init__.py
+graphene/callbacks/callback.py
+graphene/callbacks/model_summary.py
+graphene/callbacks/progress_bar.py
+graphene/callbacks/wandb.py
+graphene/core/__init__.py
+graphene/core/datamodule.py
+graphene/core/trainer.py
+graphene/core/trainmodule.py
+graphene/loops/__init__.py
+graphene/loops/loop.py
+graphene/loops/train_loop.py
+graphene/loops/validation_loop.py
+graphene/metrics/__init__.py
+graphene/metrics/accumulation.py
+graphene/metrics/accuracy.py
+graphene/metrics/metric.py
 graphene_mlx.egg-info/PKG-INFO
 graphene_mlx.egg-info/SOURCES.txt
 graphene_mlx.egg-info/dependency_links.txt
 graphene_mlx.egg-info/requires.txt
 graphene_mlx.egg-info/top_level.txt
 requirements/requirements.dev.in
 requirements/requirements.in
 scripts/install.sh
 scripts/lib.sh
-scripts/lock-requirements.sh
-src/__init__.py
-src/callbacks/callback.py
-src/callbacks/model_summary.py
-src/core/__init__.py
-src/core/datamodule.py
-src/core/trainer.py
-src/core/trainmodule.py
-src/loops/__init__.py
-src/loops/loop.py
-src/loops/train_loop.py
-src/loops/validation_loop.py
-src/metrics/__init__.py
-src/metrics/accumulation.py
-src/metrics/accuracy.py
-src/metrics/metric.py
+scripts/lock-requirements.sh
```

### Comparing `graphene_mlx-0.0.15/pyproject.toml` & `graphene_mlx-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [tool.setuptools_scm]
 fallback_version = "0.1.0"
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
-include = ["src"]
+include = ["graphene"]
 exclude = ["data", "tests"]
 
 [tool.black]
 line-length = 119
 preview = true
 
 [tool.pytest]
```

### Comparing `graphene_mlx-0.0.15/scripts/install.sh` & `graphene_mlx-0.1.0/scripts/install.sh`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/scripts/lock-requirements.sh` & `graphene_mlx-0.1.0/scripts/lock-requirements.sh`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/src/callbacks/callback.py` & `graphene_mlx-0.1.0/graphene/callbacks/callback.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
     def on_train_batch_start(self, trainer):
         pass
 
     def training_step(self, trainer):
         pass
 
-    def on_train_batch_end(self, trainer):
+    def on_train_batch_end(self, trainer, *args, **kwargs):
         pass
 
     def on_validation_epoch_start(self, trainer):
         pass
 
-    def on_validation_step_start(self, trainer):
+    def on_validation_batch_start(self, trainer):
         pass
 
-    def on_validation_step_end(self, trainer):
+    def on_validation_batch_end(self, trainer, *args, **kwargs):
         pass
 
     def on_validation_epoch_end(self, trainer):
         pass
```

### Comparing `graphene_mlx-0.0.15/src/core/trainer.py` & `graphene_mlx-0.1.0/graphene/core/trainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 
+import mlx.core as mx
 from mlx import nn
 
-from src.callbacks.model_summary import ModelSummary
-from src.core.datamodule import DataModule
-from src.core.trainmodule import TrainModule
-from src.loops.loop import LoopType
-from src.loops.train_loop import TrainLoop
-from src.loops.validation_loop import ValidationLoop
+from graphene.callbacks.model_summary import ModelSummary
+from graphene.callbacks.progress_bar import ProgressCallback
+from graphene.callbacks.wandb import WandbCallback
+from graphene.loops.loop import LoopType
+from graphene.loops.train_loop import TrainLoop
+from graphene.loops.validation_loop import ValidationLoop
 
 
 class Trainer:
     def __init__(
         self,
-        train_module: TrainModule,
-        data_module: DataModule,
+        train_module,
+        data_module,
         max_epochs: int,
         run_validation_every_n_epochs: int = 1,
-        run_sanity_validation: bool = True,
+        run_sanity_validation: bool = False,
+        limit_train_batches: int | None = None,
+        limit_validation_batches: int | None = None,
+        seed: int = 42,
         **kwargs,
     ) -> None:
         self.train_module = train_module
         self.train_module.trainer = self  # Set reference to the trainer inside the train module
         self.data_module = data_module
         self.max_epochs = max_epochs
         self.run_validation_every_n_epochs = run_validation_every_n_epochs
         self.run_sanity_validation = run_sanity_validation
+        self.limit_train_batches = limit_train_batches
+        self.limit_validation_batches = limit_validation_batches
+        self.seed = seed
 
         # Initialize model and optimizer
         self.model = train_module.model
         self.optimizer = self.train_module.configure_optimizers()
 
         # Initialize callbacks
-        self.callbacks = [ModelSummary()]
+        self.callbacks = [ModelSummary(), ProgressCallback(), WandbCallback()]
 
         # Initialize loops
         self.loops = {
             LoopType.VALIDATION: ValidationLoop(self, train_module, data_module),
             LoopType.TRAINING: TrainLoop(self, train_module, data_module),
         }
 
@@ -97,19 +104,19 @@
         active_loop = self.loops[self.active_loop]
         active_loop.log(name, value)
 
     def register_callback(self, callback):
         """Registers a new callback."""
         self.callbacks.append(callback)
 
-    def _trigger_event(self, event):
+    def _trigger_event(self, event, *args, **kwargs):
         """Triggers a specific event for all registered callbacks."""
         for callback in self.callbacks:
             if hasattr(callback, event):
-                getattr(callback, event)(self)
+                getattr(callback, event)(self, *args, **kwargs)
 
     def fit(self):
         """Runs the fit process for the given number of epochs.
 
         Handles setup, sanity validation, training, and validation loops.
         """
         self._setup()
@@ -124,14 +131,15 @@
             self._run_training_loop()
 
             if self._should_run_validation():
                 self._run_validation_loop()
 
     def _setup(self):
         """Configures the data and training modules."""
+        mx.random.seed(self.seed)
         self.data_module.setup()
         self.train_module.setup()
 
     def _should_run_sanity_validation(self):
         """Determines if sanity validation should run."""
         return self.run_sanity_validation and self.current_epoch == 0
```

### Comparing `graphene_mlx-0.0.15/src/core/trainmodule.py` & `graphene_mlx-0.1.0/graphene/core/trainmodule.py`

 * *Files identical despite different names*

### Comparing `graphene_mlx-0.0.15/src/loops/loop.py` & `graphene_mlx-0.1.0/graphene/loops/loop.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from __future__ import annotations
 
 import enum
 from abc import ABC, abstractmethod
 
 from mlx import nn
 
-from src.core.datamodule import DataModule
-from src.core.trainmodule import TrainModule
-
 
 class LoopType(enum.Enum):
     TRAINING = enum.auto()
     VALIDATION = enum.auto()
 
 
 class Loop(ABC):
     """Base class for loops."""
 
-    def __init__(self, trainer, train_module: TrainModule, data_module: DataModule) -> None:
+    def __init__(self, trainer, train_module, data_module) -> None:
         super().__init__()
         self.train_module = train_module
         self.data_module = data_module
         self.trainer = trainer
 
     def setup(self):
         """Method which makes sure both the train module and the data modules are properly
@@ -77,27 +74,34 @@
                 }
             batch_iterator (iterable): Iterator for the batches.
             step_method (callable): Method to perform the step operation.
         """
         # Trigger start of epoch events and methods
         self.trainer._trigger_event(epoch_events["start_event"])
         epoch_events["start_method"]()
+        stopping_criteria = (
+            self.trainer.limit_train_batches
+            if self.trainer.active_loop == LoopType.TRAINING
+            else self.trainer.limit_validation_batches
+        )
 
         for batch_idx, batch in enumerate(batch_iterator):
+            if stopping_criteria is not None and batch_idx >= stopping_criteria:
+                break
             # Trigger start of batch events and methods
             self.trainer._trigger_event(batch_events["start_event"])
             batch = batch_events["start_method"](batch, batch_idx)
 
             # Perform the step operation
             loss = step_method(batch, batch_idx)
             self.trainer._trigger_event(batch_events["step_event"])
 
             # Trigger end of batch events and methods
             batch_events["end_method"](loss)
-            self.trainer._trigger_event(batch_events["end_event"])
+            self.trainer._trigger_event(batch_events["end_event"], batch_idx=batch_idx)
 
         # Trigger end of epoch events and methods
         epoch_events["end_method"]()
         self.trainer._trigger_event(epoch_events["end_event"])
 
     @abstractmethod
     def iterate(self):
```

### Comparing `graphene_mlx-0.0.15/src/loops/train_loop.py` & `graphene_mlx-0.1.0/graphene/loops/train_loop.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from __future__ import annotations
 
 import mlx.core as mx
 import numpy as np
 from mlx import nn
 
-from src.core.datamodule import DataModule
-from src.core.trainmodule import TrainModule
-from src.loops.loop import Loop
-from src.metrics import Accumulation
-from src.metrics.metric import Metric
+from graphene.loops.loop import Loop
+from graphene.metrics import Accumulation, Metric
 
 
 class TrainLoop(Loop):
-    def __init__(self, trainer, train_module: TrainModule, data_module: DataModule) -> None:
+    def __init__(self, trainer, train_module, data_module) -> None:
         super().__init__(trainer, train_module, data_module)
         self.metrics: dict[str, Metric] = {"loss": Accumulation()}
 
     def on_train_epoch_start(self, *args, **kwargs):
         """Training hook which triggers at the beginning of a training epoch.
 
         - Sets the model to training mode.
@@ -50,14 +47,15 @@
 
         - Calls user-defined methods.
         - Evaluates the model state and updates metrics.
         """
         self._call_user_method("on_train_batch_end", loss)
         mx.eval(self.state)
         self.metrics["loss"].update(loss)
+        self.log("loss", self.metrics["loss"])
 
     def training_step(self, batch, batch_idx) -> tuple[mx.array, mx.array]:
         """Executes a training step, computing loss and gradients.
 
         Args:
             batch: A batch of data.
             batch_idx: Index of the batch.
@@ -75,15 +73,14 @@
 
         - Calls user-defined methods.
         - Resets the data loader.
         - Logs the training metrics.
         """
         self._call_user_method("on_train_epoch_end", args, kwargs)
         self.data_module.train_dataloader().reset()
-        self._log_epoch_metrics()
 
     def iterate(self):
         """Main loop iteration for training.
 
         - Triggers events and hooks at the start and end of each epoch and batch.
         - Executes the training step for each batch.
         """
@@ -104,19 +101,7 @@
 
         self._execute_with_events(
             epoch_events=epoch_events,
             batch_events=batch_events,
             batch_iterator=self.data_module.train_dataloader(),
             step_method=self.training_step,
         )
-
-    def _log_epoch_metrics(self):
-        """Logs the metrics at the end of an epoch."""
-        print(
-            " | ".join(
-                (
-                    f"Epoch {self.current_epoch:02d}",
-                    f"Training loss: {self.metrics['loss'].compute().item():.3f}",
-                    f"Training accuracy: {self.metrics['train_accuracy'].compute():.3f}",
-                )
-            )
-        )
```

### Comparing `graphene_mlx-0.0.15/src/loops/validation_loop.py` & `graphene_mlx-0.1.0/graphene/loops/validation_loop.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from __future__ import annotations
 
 import mlx.core as mx
 import numpy as np
 
-from src.core.datamodule import DataModule
-from src.core.trainmodule import TrainModule
-from src.loops.loop import Loop
-from src.metrics import Accumulation
-from src.metrics.metric import Metric
+from graphene.loops.loop import Loop
+from graphene.metrics import Accumulation
+from graphene.metrics.metric import Metric
 
 
 class ValidationLoop(Loop):
-    def __init__(self, trainer, train_module: TrainModule, data_module: DataModule) -> None:
+    def __init__(self, trainer, train_module, data_module) -> None:
         super().__init__(trainer, train_module, data_module)
         self.metrics: dict[str, Metric] = {"loss": Accumulation()}
 
     def on_validation_epoch_start(self, *args, **kwargs):
         """Validation hook which triggers at the beginning of a validation epoch.
 
         - Sets the model to validation mode.
@@ -46,14 +44,15 @@
         """Validation hook which triggers at the end of a validation batch.
 
         - Calls user-defined methods.
         - Updates the loss metric.
         """
         self._call_user_method("on_validation_batch_end", loss)
         self.metrics["loss"].update(loss)
+        self.log("loss", self.metrics["loss"])
 
     def validation_step(self, batch, batch_idx) -> tuple[mx.array, mx.array]:
         """Executes a validation step, computing loss.
 
         Args:
             batch: A batch of data.
             batch_idx: Index of the batch.
@@ -70,15 +69,14 @@
 
         - Calls user-defined methods.
         - Resets the data loader.
         - Logs the validation metrics.
         """
         self._call_user_method("on_validation_epoch_end", args, kwargs)
         self.data_module.valid_dataloader().reset()
-        self._log_epoch_metrics()
 
     def iterate(self):
         """Main loop iteration for validation.
 
         - Triggers events and hooks at the start and end of each epoch and batch.
         - Executes the validation step for each batch.
         """
@@ -99,19 +97,7 @@
 
         self._execute_with_events(
             epoch_events=epoch_events,
             batch_events=batch_events,
             batch_iterator=self.data_module.valid_dataloader(),
             step_method=self.validation_step,
         )
-
-    def _log_epoch_metrics(self):
-        """Logs the metrics at the end of an epoch."""
-        print(
-            " | ".join(
-                (
-                    f"Epoch {self.current_epoch:02d}",
-                    f"Validation loss: {self.metrics['loss'].compute().item():.3f}",
-                    f"Validation accuracy: {self.metrics['validation_accuracy'].compute():.3f}",
-                )
-            )
-        )
```

### Comparing `graphene_mlx-0.0.15/src/metrics/accuracy.py` & `graphene_mlx-0.1.0/graphene/metrics/accuracy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import mlx.core as mx
 
-from src.metrics.metric import Metric
+from graphene.metrics.metric import Metric
 
 
 class Accuracy(Metric):
     def __init__(self):
         super().__init__("accuracy")
         self.add_state("correct", 0, reduce_fx=None)
         self.add_state("total", 0, reduce_fx=None)
```

### Comparing `graphene_mlx-0.0.15/train.py` & `graphene_mlx-0.1.0/train.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,50 +4,60 @@
 from typing import Any
 
 import mlx.optimizers as optim
 from mlx import nn
 
 from examples.cifar_datamodule import Cifar10DataModule
 from examples.resnet import resnet20
-from src.core.trainer import Trainer
-from src.core.trainmodule import TrainModule
-from src.metrics import Accuracy
+from graphene import Trainer, TrainModule
+from graphene.metrics import Accuracy
 
 
 class CifarTrainModule(TrainModule):
     def __init__(self, args: SimpleNamespace) -> None:
         super().__init__(args)
         self.model = resnet20()
 
     def configure_optimizers(self):
-        return optim.Adam(learning_rate=1e-3)
+        warmup = optim.linear_schedule(0, 1e-1, steps=4 * 190)
+        cosine = optim.cosine_decay(1e-1, 26 * 190)
+        lr_schedule = optim.join_schedules([warmup, cosine], [4 * 190])
+        optimizer = optim.Adam(learning_rate=lr_schedule)
+        return optimizer
 
     def forward(self, x) -> Any:
         return self.model(x)
 
     def setup(self):
         self.accs = []
         self.validation_accuracy = Accuracy()
         self.train_accuracy = Accuracy()
 
     def training_step(self, batch: dict, batch_idx):
         x, y = batch["image"], batch["label"]
         y_hat = self.forward(x)
         loss = nn.losses.cross_entropy(y_hat, y, reduction="mean")
         self.train_accuracy(y_hat, y)
-        self.log("train_accuracy", self.train_accuracy)
+        self.log("accuracy", self.train_accuracy)
         return loss
 
     def validation_step(self, batch: dict, batch_idx):
         x, y = batch["image"], batch["label"]
         y_hat = self.forward(x)
         loss = nn.losses.cross_entropy(y_hat, y, reduction="mean")
         self.validation_accuracy(y_hat, y)
-        self.log("validation_accuracy", self.validation_accuracy)
+        self.log("accuracy", self.validation_accuracy)
         return loss
 
 
 if __name__ == "__main__":
     datamodule = Cifar10DataModule(args=SimpleNamespace(batch_size=256))
     trainmodule = CifarTrainModule(args=None)
-    trainer = Trainer(train_module=trainmodule, data_module=datamodule, max_epochs=30, run_validation_every_n_epochs=1)
+    trainer = Trainer(
+        train_module=trainmodule,
+        data_module=datamodule,
+        max_epochs=30,
+        run_validation_every_n_epochs=1,
+        # limit_validation_batches=10,
+        # limit_train_batches=10,/
+    )
     trainer.fit()
```

