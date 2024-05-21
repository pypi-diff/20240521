# Comparing `tmp/cellarium-ml-0.0.3.tar.gz` & `tmp/cellarium_ml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellarium-ml-0.0.3.tar", last modified: Wed Dec 13 16:06:03 2023, max compression
+gzip compressed data, was "cellarium_ml-0.0.5.tar", last modified: Tue May 21 15:11:38 2024, max compression
```

## Comparing `cellarium-ml-0.0.3.tar` & `cellarium_ml-0.0.5.tar`

### file list

```diff
@@ -1,75 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.393715 cellarium-ml-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-12-13 16:06:03.393715 cellarium-ml-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.381715 cellarium-ml-0.0.3/cellarium/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.385715 cellarium-ml-0.0.3/cellarium/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.385715 cellarium-ml-0.0.3/cellarium/ml/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/callbacks/prediction_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/callbacks/variance_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15398 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.385715 cellarium-ml-0.0.3/cellarium/ml/core/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/core/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/core/saving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.385715 cellarium-ml-0.0.3/cellarium/ml/data/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/data/dadc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15400 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/data/distributed_anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/data/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/data/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.385715 cellarium-ml-0.0.3/cellarium/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/lr_schedulers/linear_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.389715 cellarium-ml-0.0.3/cellarium/ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10649 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/from_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/geneformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/incremental_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/onepass_mean_var_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/probabilistic_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/models/tdigest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.389715 cellarium-ml-0.0.3/cellarium/ml/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/preprocessing/highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.389715 cellarium-ml-0.0.3/cellarium/ml/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/transforms/divide_by_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/transforms/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/transforms/log1p.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/transforms/normalize_total.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/transforms/z_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.389715 cellarium-ml-0.0.3/cellarium/ml/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/utilities/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/cellarium/ml/utilities/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.393715 cellarium-ml-0.0.3/cellarium_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-12-13 16:06:03.000000 cellarium-ml-0.0.3/cellarium_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-12-13 16:06:03.000000 cellarium-ml-0.0.3/cellarium_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 16:06:03.000000 cellarium-ml-0.0.3/cellarium_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-13 16:06:03.000000 cellarium-ml-0.0.3/cellarium_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-13 16:06:03.000000 cellarium-ml-0.0.3/cellarium_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-13 16:06:03.000000 cellarium-ml-0.0.3/cellarium_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 16:06:03.393715 cellarium-ml-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 16:06:03.393715 cellarium-ml-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_distributed_anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_geneformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_ipca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_onepass_mean_var_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_ppca.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_read_h5ad.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_tdigest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-13 16:05:50.000000 cellarium-ml-0.0.3/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.774249 cellarium_ml-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-21 15:11:38.774249 cellarium_ml-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.758249 cellarium_ml-0.0.5/cellarium/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/callbacks/prediction_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/callbacks/variance_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20755 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/core/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/core/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/dadc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/distributed_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/distributed/gather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/distributions/negative_binomial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/lr_schedulers/linear_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/geneformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/incremental_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/mu_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/onepass_mean_var_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/probabilistic_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/tdigest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/preprocessing/highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/divide_by_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/log1p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/normalize_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/z_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.770249 cellarium_ml-0.0.5/cellarium/ml/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/utilities/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/utilities/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.770249 cellarium_ml-0.0.5/cellarium_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:11:38.774249 cellarium_ml-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.770249 cellarium_ml-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19728 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_distributed_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_geneformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_ipca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_mup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_onepass_mean_var_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_ppca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_read_h5ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_tdigest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_transforms.py
```

### Comparing `cellarium-ml-0.0.3/LICENSE.md` & `cellarium_ml-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cellarium-ml-0.0.3/cellarium/ml/callbacks/prediction_writer.py` & `cellarium_ml-0.0.5/cellarium/ml/callbacks/prediction_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,24 @@
         self.output_dir = output_dir
         self.prediction_size = prediction_size
 
     def write_on_batch_end(
         self,
         trainer: pl.Trainer,
         pl_module: pl.LightningModule,
-        prediction: torch.Tensor,
+        prediction: dict[str, torch.Tensor],
         batch_indices: Sequence[int] | None,
         batch: dict[str, np.ndarray | torch.Tensor],
         batch_idx: int,
         dataloader_idx: int,
     ) -> None:
+        x_ng = prediction["x_ng"]
         if self.prediction_size is not None:
-            prediction = prediction[:, : self.prediction_size]
+            x_ng = x_ng[:, : self.prediction_size]
 
-        assert isinstance(batch["obs_names"], np.ndarray)
+        assert isinstance(batch["obs_names_n"], np.ndarray)
         write_prediction(
-            prediction=prediction,
-            ids=batch["obs_names"],
+            prediction=x_ng,
+            ids=batch["obs_names_n"],
             output_dir=self.output_dir,
             postfix=batch_idx * trainer.world_size + trainer.global_rank,
         )
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/callbacks/variance_monitor.py` & `cellarium_ml-0.0.5/cellarium/ml/callbacks/variance_monitor.py`

 * *Files identical despite different names*

### Comparing `cellarium-ml-0.0.3/cellarium/ml/cli.py` & `cellarium_ml-0.0.5/cellarium/ml/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,268 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
 """
 Command line interface for Cellarium ML.
 """
 
+import copy
 import sys
 import warnings
 from collections.abc import Callable
+from dataclasses import dataclass
+from functools import cache
+from operator import attrgetter
 from typing import Any
 
-from jsonargparse import Namespace
+import numpy as np
+import torch
+import yaml
+from jsonargparse import Namespace, class_from_function
+from jsonargparse._loaders_dumpers import DefaultLoader
+from jsonargparse._util import import_object
 from lightning.pytorch.cli import ArgsType, LightningArgumentParser, LightningCLI
+from torch._subclasses.fake_tensor import FakeCopyMode, FakeTensorMode
+
+from cellarium.ml import CellariumAnnDataDataModule, CellariumModule, CellariumPipeline
+from cellarium.ml.utilities.data import collate_fn
+
+cached_loaders = {}
+
+
+@dataclass
+class FileLoader:
+    """
+    A YAML constructor for loading a file and accessing its attributes.
+
+    Example:
+
+    .. code-block:: yaml
+
+        model:
+          transforms:
+            - class_path: cellarium.ml.transforms.Filter
+              init_args:
+                filter_list:
+                  !FileLoader
+                  file_path: gs://dsp-cellarium-cas-public/test-data/filter_list.csv
+                  loader_fn: pandas.read_csv
+                  attr: index
+                  convert_fn: numpy.ndarray.tolist
+
+    Args:
+        file_path:
+            The file path to load the object from.
+        loader_fn:
+            A function to load the object from the file path.
+        attr:
+            An attribute to get from the loaded object. If ``None`` the loaded object is returned.
+        convert_fn:
+            A function to convert the loaded object. If ``None`` the loaded object is returned.
+    """
+
+    file_path: str
+    loader_fn: Callable[[str], Any] | str
+    attr: str | None = None
+    convert_fn: Callable[[Any], Any] | str | None = None
+
+    def __new__(cls, file_path, loader_fn, attr, convert_fn):
+        if isinstance(loader_fn, str):
+            loader_fn = import_object(loader_fn)
+        if loader_fn not in cached_loaders:
+            cached_loaders[loader_fn] = cache(loader_fn)
+        loader_fn = cached_loaders[loader_fn]
+        obj = loader_fn(file_path)
+
+        if attr is not None:
+            obj = attrgetter(attr)(obj)
+
+        if isinstance(convert_fn, str):
+            convert_fn = import_object(convert_fn)
+        if convert_fn is not None:
+            obj = convert_fn(obj)
+
+        return obj
+
+
+@dataclass
+class CheckpointLoader(FileLoader):
+    """
+    A YAML constructor for loading a :class:`~cellarium.ml.core.CellariumModule` checkpoint and accessing its
+    attributes.
+
+    Example:
+
+    .. code-block:: yaml
+
+        model:
+          transorms:
+            - class_path: cellarium.ml.transforms.DivideByScale
+              init_args:
+                scale_g:
+                  !CheckpointLoader
+                  file_path: gs://dsp-cellarium-cas-public/test-data/tdigest.ckpt
+                  attr: model.median_g
+                  convert_fn: null
+
+    Args:
+        file_path:
+            The file path to load the object from.
+        attr:
+            An attribute to get from the loaded object. If ``None`` the loaded object is returned.
+        convert_fn:
+            A function to convert the loaded object. If ``None`` the loaded object is returned.
+    """
+
+    file_path: str
+    attr: str | None = None
+    convert_fn: Callable[[Any], Any] | str | None = None
+
+    def __new__(cls, file_path, attr, convert_fn):
+        return super().__new__(cls, file_path, CellariumModule.load_from_checkpoint, attr, convert_fn)
+
+
+def file_loader_constructor(loader: yaml.SafeLoader, node: yaml.nodes.MappingNode) -> FileLoader:
+    """Construct an object from a file."""
+    return FileLoader(**loader.construct_mapping(node))  # type: ignore[misc]
+
+
+def checkpoint_loader_constructor(loader: yaml.SafeLoader, node: yaml.nodes.MappingNode) -> CheckpointLoader:
+    """Construct an object from a checkpoint."""
+    return CheckpointLoader(**loader.construct_mapping(node))  # type: ignore[misc]
+
+
+loader = DefaultLoader
+loader.add_constructor("!FileLoader", file_loader_constructor)
+loader.add_constructor("!CheckpointLoader", checkpoint_loader_constructor)
 
-from cellarium.ml import CellariumAnnDataDataModule, CellariumModule
 
 REGISTERED_MODELS = {}
 
 
 def register_model(model: Callable[[ArgsType], None]):
     REGISTERED_MODELS[model.__name__] = model
     return model
 
 
+CellariumModuleLoadFromCheckpoint = class_from_function(CellariumModule.load_from_checkpoint, CellariumModule)
+
+
+@dataclass
+class LinkArguments:
+    """
+    Arguments for linking the value of a target argument to the values of one or more source arguments.
+
+    Args:
+        source:
+            Key(s) from which the target value is derived.
+        target:
+            Key to where the value is set.
+        compute_fn:
+            Function to compute target value from source.
+        apply_on:
+            At what point to set target value, ``"parse"`` or ``"instantiate"``.
+    """
+
+    source: str | tuple[str, ...]
+    target: str
+    compute_fn: Callable | None = None
+    apply_on: str = "instantiate"
+
+
+def compute_n_obs(data: CellariumAnnDataDataModule) -> int:
+    """
+    Compute the number of observations in the data.
+
+    Args:
+        data: A :class:`CellariumAnnDataDataModule` instance.
+
+    Returns:
+        The number of observations in the data.
+    """
+    return data.dadc.n_obs
+
+
+def compute_n_categories(data: CellariumAnnDataDataModule) -> int:
+    """
+    Compute the number of categories in the target variable.
+
+    E.g. if the target variable is ``obs["cell_type"]`` then this function
+    returns the number of categories in ``obs["cell_type"]``::
+
+        >>> len(data.dadc[0].obs["cell_type"].cat.categories)
+
+    Args:
+        data: A :class:`CellariumAnnDataDataModule` instance.
+
+    Returns:
+        The number of categories in the target variable.
+    """
+    field = data.batch_keys["y_n"]
+    value = getattr(data.dadc[0], field.attr)
+    if field.key is not None:
+        value = value[field.key]
+    return len(value.cat.categories)
+
+
+def compute_var_names_g(transforms: list[torch.nn.Module], data: CellariumAnnDataDataModule) -> np.ndarray:
+    """
+    Compute variable names from the data by applying the transforms.
+
+    Args:
+        transforms:
+            A list of transforms.
+        data:
+            A :class:`CellariumAnnDataDataModule` instance.
+
+    Returns:
+        The variable names.
+    """
+    batch = {key: field(data.dadc, 0) for key, field in data.batch_keys.items()}
+    pipeline = CellariumPipeline(transforms)
+    with FakeTensorMode(allow_non_fake_inputs=True) as fake_mode:
+        fake_batch = collate_fn([batch])
+        with FakeCopyMode(fake_mode):
+            fake_pipeline = copy.deepcopy(pipeline)
+        fake_pipeline.to("cpu")
+        output = fake_pipeline(fake_batch)
+    return output["var_names_g"]
+
+
 def lightning_cli_factory(
     model_class_path: str,
-    link_arguments: list[tuple[str, str, Callable[[Any], object] | None]] | None = None,
+    link_arguments: list[LinkArguments] | None = None,
     trainer_defaults: dict[str, Any] | None = None,
 ) -> type[LightningCLI]:
     """
     Factory function for creating a :class:`LightningCLI` with a preset model and custom argument linking.
 
     Example::
 
         cli = lightning_cli_factory(
-            "cellarium.ml.models.IncrementalPCAFromCLI",
-            link_arguments=[("data.n_vars", "model.model.init_args.g_genes", None)],
+            "cellarium.ml.models.IncrementalPCA",
+            link_arguments=[
+                LinkArguments(("model.transforms", "data"), "model.model.init_args.var_names_g", compute_var_names_g)
+            ],
             trainer_defaults={
                 "max_epochs": 1,  # one pass
                 "strategy": {
                     "class_path": "lightning.pytorch.strategies.DDPStrategy",
-                    "init_args": {"broadcast_buffers": False},
+                    "dict_kwargs": {"broadcast_buffers": False},
                 },
             },
         )
 
     Args:
         model_class_path:
-            A string representation of the model class path (e.g., ``"cellarium.ml.models.IncrementalPCAFromCLI"``).
+            A string representation of the model class path (e.g., ``"cellarium.ml.models.IncrementalPCA"``).
         link_arguments:
-            A list of tuples of the form ``(source, target)`` where ``source`` is linked to ``target``.
+            A list of :class:`LinkArguments` that specify how to derive the value of a target
+            argument from the values of one or more source arguments. If ``None`` then no
+            arguments are linked.
         trainer_defaults:
             Default values for the trainer.
 
     Returns:
         A :class:`LightningCLI` class with the given model and argument linking.
     """
 
@@ -63,53 +272,38 @@
                 CellariumModule,
                 CellariumAnnDataDataModule,
                 trainer_defaults=trainer_defaults,
                 args=args,
             )
 
         def instantiate_classes(self) -> None:
-            super().instantiate_classes()
-
-            # impute linked arguments after instantiation
-            if link_arguments is not None:
-                for source, target, compute_fn in link_arguments:
-                    # e.g., source == "data.var_names"
-                    source_key, *source_attrs = source.split(".")
-                    # note that config_init is initialized, so value is an instance
-                    config_init = self.config_init[self.subcommand]
-                    value = config_init[source_key]
-                    for attr in source_attrs:
-                        value = getattr(value, attr)
-                    if compute_fn is not None:
-                        value = compute_fn(value)
-
-                    # e.g., target == "model.model.init_args.feature_schema"
-                    target_keys = target.split(".")
-                    # note that config is dict-like, so assign the value to the last key
-                    config = self.config[self.subcommand]
-                    for key in target_keys[:-1]:
-                        config = config[key]
-                    config[target_keys[-1]] = value
-
-            # save the config to the :attr:`model.hparams` to be able to load the model checkpoint
-            self.model._set_hparams(self.config[self.subcommand])
+            with torch.device("meta"):
+                # skip the initialization of model parameters
+                # parameters are later initialized by the  `CellariumModule.configure_model` method
+                return super().instantiate_classes()
 
         def add_arguments_to_parser(self, parser: LightningArgumentParser) -> None:
             if link_arguments is not None:
-                for arg1, arg2, compute_fn in link_arguments:
-                    parser.link_arguments(arg1, arg2, compute_fn=compute_fn, apply_on="instantiate")
-            parser.set_defaults({"model.model": model_class_path})
+                for link in link_arguments:
+                    parser.link_arguments(link.source, link.target, link.compute_fn, link.apply_on)
+            # this is helpful for generating a default config file with --print_config
+            parser.set_defaults(
+                {
+                    "model.model": model_class_path,
+                    "data.dadc": "cellarium.ml.data.DistributedAnnDataCollection",
+                }
+            )
 
     return NewLightningCLI
 
 
 @register_model
 def geneformer(args: ArgsType = None) -> None:
     r"""
-    CLI to run the :class:`cellarium.ml.models.GeneformerFromCLI` model.
+    CLI to run the :class:`cellarium.ml.models.Geneformer` model.
 
     This example shows how to fit feature count data to the Geneformer model [1].
 
     Example run::
 
         cellarium-ml geneformer fit \
             --data.filenames "gs://dsp-cellarium-cas-public/test-data/test_{0..3}.h5ad" \
@@ -127,32 +321,34 @@
     1. `Transfer learning enables predictions in network biology (Theodoris et al.)
        <https://www.nature.com/articles/s41586-023-06139-9>`_.
 
     Args:
         args: Arguments to parse. If ``None`` the arguments are taken from ``sys.argv``.
     """
     cli = lightning_cli_factory(
-        "cellarium.ml.models.GeneformerFromCLI",
-        link_arguments=[("data.var_names", "model.model.init_args.feature_schema", None)],
+        "cellarium.ml.models.Geneformer",
+        link_arguments=[
+            LinkArguments(("model.transforms", "data"), "model.model.init_args.var_names_g", compute_var_names_g)
+        ],
     )
     cli(args=args)
 
 
 @register_model
 def incremental_pca(args: ArgsType = None) -> None:
     r"""
-    CLI to run the :class:`cellarium.ml.models.IncrementalPCAFromCLI` model.
+    CLI to run the :class:`cellarium.ml.models.IncrementalPCA` model.
 
     This example shows how to fit feature count data to incremental PCA
     model [1, 2].
 
     Example run::
 
         cellarium-ml incremental_pca fit \
-            --model.model.init_args.k_components 50 \
+            --model.model.init_args.n_components 50 \
             --data.filenames "gs://dsp-cellarium-cas-public/test-data/test_{0..3}.h5ad" \
             --data.shard_size 100 \
             --data.max_cache_size 2 \
             --data.batch_size 100 \
             --data.num_workers 4 \
             --trainer.accelerator gpu \
             --trainer.devices 1 \
@@ -165,21 +361,23 @@
     2. `Incremental Learning for Robust Visual Tracking (Ross et al.)
        <https://www.cs.toronto.edu/~dross/ivt/RossLimLinYang_ijcv.pdf>`_.
 
     Args:
         args: Arguments to parse. If ``None`` the arguments are taken from ``sys.argv``.
     """
     cli = lightning_cli_factory(
-        "cellarium.ml.models.IncrementalPCAFromCLI",
-        link_arguments=[("data.n_vars", "model.model.init_args.g_genes", None)],
+        "cellarium.ml.models.IncrementalPCA",
+        link_arguments=[
+            LinkArguments(("model.transforms", "data"), "model.model.init_args.var_names_g", compute_var_names_g)
+        ],
         trainer_defaults={
             "max_epochs": 1,  # one pass
             "strategy": {
                 "class_path": "lightning.pytorch.strategies.DDPStrategy",
-                "init_args": {"broadcast_buffers": False},
+                "dict_kwargs": {"broadcast_buffers": False},
             },
         },
     )
     cli(args=args)
 
 
 @register_model
@@ -191,58 +389,43 @@
 
         cellarium-ml logistic_regression fit \
             --data.filenames "gs://dsp-cellarium-cas-public/test-data/test_{0..3}.h5ad" \
             --data.shard_size 100 \
             --data.max_cache_size 2 \
             --data.batch_keys.x_ng.attr X \
             --data.batch_keys.x_ng.convert_fn cellarium.ml.utilities.data.densify \
-            --data.batch_keys.feature_g.attr var_names \
+            --data.batch_keys.var_names_g.attr var_names \
             --data.batch_keys.y_n.attr obs \
             --data.batch_keys.y_n.key cell_type \
             --data.batch_keys.y_n.convert_fn cellarium.ml.utilities.data.categories_to_codes \
             --data.batch_size 100 \
             --data.num_workers 4 \
             --trainer.accelerator gpu \
             --trainer.devices 1 \
             --trainer.max_steps 1000
 
     Args:
         args: Arguments to parse. If ``None`` the arguments are taken from ``sys.argv``.
     """
 
-    def get_c_categories(data: CellariumAnnDataDataModule) -> int:
-        """
-        Get the number of categories in the target variable.
-
-        E.g. if the target variable is ``obs["cell_type"]`` then this function
-        returns the number of categories in ``obs["cell_type"]``::
-
-            >>> len(data.dadc[0].obs["cell_type"].cat.categories)
-        """
-        field = data.batch_keys["y_n"]
-        value = getattr(data.dadc[0], field.attr)
-        if field.key is not None:
-            value = value[field.key]
-        return len(value.cat.categories)
-
     cli = lightning_cli_factory(
         "cellarium.ml.models.LogisticRegression",
         link_arguments=[
-            ("data.n_obs", "model.model.init_args.n_obs", None),
-            ("data.var_names", "model.model.init_args.feature_schema", None),
-            ("data", "model.model.init_args.c_categories", get_c_categories),
+            LinkArguments(("model.transforms", "data"), "model.model.init_args.var_names_g", compute_var_names_g),
+            LinkArguments("data", "model.model.init_args.n_obs", compute_n_obs),
+            LinkArguments("data", "model.model.init_args.n_categories", compute_n_categories),
         ],
     )
     cli(args=args)
 
 
 @register_model
 def onepass_mean_var_std(args: ArgsType = None) -> None:
     r"""
-    CLI to run the :class:`cellarium.ml.models.OnePassMeanVarStdFromCLI` model.
+    CLI to run the :class:`cellarium.ml.models.OnePassMeanVarStd` model.
 
     This example shows how to calculate mean, variance, and standard deviation of log normalized
     feature count data in one pass [1].
 
     Example run::
 
         cellarium-ml onepass_mean_var_std fit \
@@ -260,31 +443,33 @@
     1. `Algorithms for calculating variance
        <https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance>`_.
 
     Args:
         args: Arguments to parse. If ``None`` the arguments are taken from ``sys.argv``.
     """
     cli = lightning_cli_factory(
-        "cellarium.ml.models.OnePassMeanVarStdFromCLI",
-        link_arguments=[("data.n_vars", "model.model.init_args.g_genes", None)],
+        "cellarium.ml.models.OnePassMeanVarStd",
+        link_arguments=[
+            LinkArguments(("model.transforms", "data"), "model.model.init_args.var_names_g", compute_var_names_g)
+        ],
         trainer_defaults={
             "max_epochs": 1,  # one pass
             "strategy": {
                 "class_path": "lightning.pytorch.strategies.DDPStrategy",
-                "init_args": {"broadcast_buffers": False},
+                "dict_kwargs": {"broadcast_buffers": False},
             },
         },
     )
     cli(args=args)
 
 
 @register_model
 def probabilistic_pca(args: ArgsType = None) -> None:
     r"""
-    CLI to run the :class:`cellarium.ml.models.ProbabilisticPCAFromCLI` model.
+    CLI to run the :class:`cellarium.ml.models.ProbabilisticPCA` model.
 
     This example shows how to fit feature count data to probabilistic PCA
     model [1].
 
     There are two flavors of probabilistic PCA model that are available:
 
     1. ``marginalized`` - latent variable ``z`` is marginalized out [1]. Marginalized
@@ -296,54 +481,51 @@
        global maximum  corresponding to the principal component directions.
        The global maximum of the ELBO objective for the linear VAE  is identical
        to the global maximum for the marginal log-likelihood of probabilistic PCA.
 
     Example run::
 
         cellarium-ml probabilistic_pca fit \
-            --model.model.init_args.mean_var_std_ckpt_path \
-            "runs/onepass/lightning_logs/version_0/checkpoints/module_checkpoint.pt" \
+            --model.model.init_args.n_components 256 \
+            --model.model.init_args.ppca_flavor marginalized \
             --data.filenames "gs://dsp-cellarium-cas-public/test-data/test_{0..3}.h5ad" \
             --data.shard_size 100 \
             --data.max_cache_size 2 \
             --data.batch_size 100 \
             --data.shuffle true \
             --data.num_workers 4 \
             --trainer.accelerator gpu \
             --trainer.devices 1 \
             --trainer.max_steps 1000 \
             --trainer.default_root_dir runs/ppca \
-            --trainer.callbacks cellarium.ml.callbacks.VarianceMonitor \
-            --trainer.callbacks.mean_var_std_ckpt_path \
-            "runs/onepass/lightning_logs/version_0/checkpoints/module_checkpoint.pt"
 
     **References:**
 
     1. `Probabilistic Principal Component Analysis (Tipping et al.)
        <https://www.robots.ox.ac.uk/~cvrg/hilary2006/ppca.pdf>`_.
     2. `Understanding Posterior Collapse in Generative Latent Variable Models (Lucas et al.)
        <https://openreview.net/pdf?id=r1xaVLUYuE>`_.
 
     Args:
         args: Arguments to parse. If ``None`` the arguments are taken from ``sys.argv``.
     """
     cli = lightning_cli_factory(
-        "cellarium.ml.models.ProbabilisticPCAFromCLI",
+        "cellarium.ml.models.ProbabilisticPCA",
         link_arguments=[
-            ("data.n_obs", "model.model.init_args.n_cells", None),
-            ("data.n_vars", "model.model.init_args.g_genes", None),
+            LinkArguments(("model.transforms", "data"), "model.model.init_args.var_names_g", compute_var_names_g),
+            LinkArguments("data", "model.model.init_args.n_obs", compute_n_obs),
         ],
     )
     cli(args=args)
 
 
 @register_model
 def tdigest(args: ArgsType = None) -> None:
     r"""
-    CLI to run the :class:`cellarium.ml.models.TDigestFromCLI` model.
+    CLI to run the :class:`cellarium.ml.models.TDigest` model.
 
     This example shows how to calculate non-zero median of normalized feature count
     data in one pass [1].
 
     Example run::
 
         cellarium-ml tdigest fit \
@@ -361,16 +543,18 @@
     1. `Computing Extremely Accurate Quantiles Using T-Digests (Dunning et al.)
        <https://github.com/tdunning/t-digest/blob/master/docs/t-digest-paper/histo.pdf>`_.
 
     Args:
         args: Arguments to parse. If ``None`` the arguments are taken from ``sys.argv``.
     """
     cli = lightning_cli_factory(
-        "cellarium.ml.models.TDigestFromCLI",
-        link_arguments=[("data.n_vars", "model.model.init_args.g_genes", None)],
+        "cellarium.ml.models.TDigest",
+        link_arguments=[
+            LinkArguments(("model.transforms", "data"), "model.model.init_args.var_names_g", compute_var_names_g)
+        ],
         trainer_defaults={
             "max_epochs": 1,  # one pass
         },
     )
     cli(args=args)
 
 
@@ -380,29 +564,32 @@
 
     Args:
         args: Arguments to parse. If ``None`` the arguments are taken from ``sys.argv``.
             The model name is expected to be the first argument if ``args`` is a list
             or the ``model_name`` key if ``args`` is a dictionary or ``Namespace``.
     """
     if isinstance(args, (dict, Namespace)):
-        assert "model_name" in args, "'model_name' key must be specified in args"
+        if "model_name" not in args:
+            raise ValueError("'model_name' key must be specified in args")
         model_name = args.pop("model_name")
     elif isinstance(args, list):
-        assert len(args) > 0, "'model_name' must be specified as the first argument in args"
+        if len(args) == 0:
+            raise ValueError("'model_name' must be specified as the first argument in args")
         model_name = args.pop(0)
     elif args is None:
         args = sys.argv[1:].copy()
-        assert len(args) > 0, "'model_name' must be specified after cellarium-ml"
+        if len(args) == 0:
+            raise ValueError("'model_name' must be specified after cellarium-ml")
         model_name = args.pop(0)
 
-    assert (
-        model_name in REGISTERED_MODELS
-    ), f"'model_name' must be one of {list(REGISTERED_MODELS.keys())}. Got '{model_name}'"
+    if model_name not in REGISTERED_MODELS:
+        raise ValueError(f"'model_name' must be one of {list(REGISTERED_MODELS.keys())}. Got '{model_name}'")
     model_cli = REGISTERED_MODELS[model_name]
     with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="Transforming to str index.")
         warnings.filterwarnings("ignore", message="LightningCLI's args parameter is intended to run from within Python")
         warnings.filterwarnings("ignore", message="Your `IterableDataset` has `__len__` defined.")
         model_cli(args)  # run the model
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/core/datamodule.py` & `cellarium_ml-0.0.5/cellarium/ml/core/datamodule.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,53 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
-from collections.abc import Iterable, Sequence
 
 import lightning.pytorch as pl
-import numpy as np
 import torch
+from anndata import AnnData
 
 from cellarium.ml.data import DistributedAnnDataCollection, IterableDistributedAnnDataCollectionDataset
+from cellarium.ml.utilities.core import train_val_split
 from cellarium.ml.utilities.data import AnnDataField, collate_fn
 
 
 class CellariumAnnDataDataModule(pl.LightningDataModule):
     """
     DataModule for :class:`~cellarium.ml.data.IterableDistributedAnnDataCollectionDataset`.
 
     Example::
 
         >>> from cellarium.ml import CellariumAnnDataDataModule
+        >>> from cellarium.ml.data import DistributedAnnDataCollection
         >>> from cellarium.ml.utilities.data import AnnDataField, densify
 
         >>> dm = CellariumAnnDataDataModule(
-        ...     "gs://bucket-name/folder/adata{000..005}.h5ad",
-        ...     shard_size=10_000,
+        ...     DistributedAnnDataCollection(
+        ...         "gs://bucket-name/folder/adata{000..005}.h5ad",
+        ...         shard_size=10_000,
+        ...     ),
         ...     max_cache_size=2,
         ...     batch_keys={
         ...         "x_ng": AnnDataField(attr="X", convert_fn=densify),
-        ...         "feature_g": AnnDataField(attr="var_names"),
+        ...         "var_names_g": AnnDataField(attr="var_names"),
         ...     },
         ...     batch_size=5000,
         ...     shuffle=True,
         ...     seed=0,
         ...     drop_last=True,
         ...     num_workers=4,
         ... )
         >>> dm.setup()
         >>> for batch in dm.train_dataloader():
-        ...     print(batch.keys())  # x_ng, feature_g
-
-    Example::
-
-        >>> from cellarium.ml import CellariumAnnDataDataModule
-        >>> from cellarium.ml.utilities.data import AnnDataField, densify
-
-        >>> dm = CellariumAnnDataDataModule(
-        ...     "gs://bucket-name/folder/adata{000..005}.h5ad",
-        ...     shard_size=10_000,
-        ...     max_cache_size=2,
-        ...     batch_keys={
-        ...         "x_ng": AnnDataField(attr="X", convert_fn=densify),
-        ...         "feature_g": AnnDataField(attr="var_names"),
-        ...     },
-        ...     batch_size=5000,
-        ...     shuffle=True,
-        ...     seed=0,
-        ...     drop_last=True,
-        ...     num_workers=4,
-        ... )
-        >>> dm.setup()
-        >>> for batch in dm.train_dataloader():
-        ...     print(batch.keys())  # x_ng, feature_g
+        ...     print(batch.keys())  # x_ng, var_names_g
 
     Args:
-        filenames:
-            Names of anndata files.
-        limits:
-            List of global cell indices (limits) for the last cells in each shard.
-            If ``None``, the limits are inferred from ``shard_size`` and ``last_shard_size``.
-        shard_size:
-            The number of cells in each anndata file (shard).
-            Must be specified if the ``limits`` is not provided.
-        last_shard_size:
-            Last shard size. If not ``None``, the last shard will have this size possibly
-            different from ``shard_size``.
-        max_cache_size:
-            Max size of the cache.
-        cache_size_strictly_enforced:
-            Assert that the number of retrieved anndatas is not more than maxsize.
-        label:
-            Column in :attr:`obs` to place batch information in. If it's ``None``, no column is added.
-        keys:
-            Names for each object being added. These values are used for column values for
-            ``label`` or appended to the index if ``index_unique`` is not ``None``.
-            If ``None``, ``keys`` are set to ``filenames``.
-        index_unique:
-            Whether to make the index unique by using the keys. If provided, this
-            is the delimeter between ``{orig_idx}{index_unique}{key}``. When ``None``,
-            the original indices are kept.
-        indices_strict:
-            If  ``True``, arrays from the subset objects will always have the same order
-            of indices as in selection used to subset.
-            This parameter can be set to ``False`` if the order in the returned arrays
-            is not important, for example, when using them for stochastic gradient descent.
-            In this case the performance of subsetting can be a bit better.
+        dadc:
+            An instance of :class:`~cellarium.ml.data.DistributedAnnDataCollection` or :class:`AnnData`.
         batch_keys:
             Dictionary that specifies which attributes and keys of the :attr:`dadc` to return
             in the batch data and how to convert them. Keys must correspond to
             the input keys of the transforms or the model. Values must be instances of
             :class:`cellarium.ml.utilities.data.AnnDataField`.
         batch_size:
             How many samples per batch to load.
@@ -105,116 +56,122 @@
         seed:
             Random seed used to shuffle the sampler if :attr:`shuffle=True`.
         drop_last:
             If ``True``, then the sampler will drop the tail of the data
             to make it evenly divisible across the number of replicas. If ``False``,
             the sampler will add extra indices to make the data evenly divisible across
             the replicas.
+        train_size:
+            Size of the train split. If :class:`float`, should be between ``0.0`` and ``1.0`` and represent
+            the proportion of the dataset to include in the train split. If :class:`int`, represents
+            the absolute number of train samples. If ``None``, the value is automatically set to the complement
+            of the ``val_size``.
+        val_size:
+            Size of the validation split. If :class:`float`, should be between ``0.0`` and ``1.0`` and represent
+            the proportion of the dataset to include in the validation split. If :class:`int`, represents
+            the absolute number of validation samples. If ``None``, the value is set to the complement of
+            the ``train_size``. If ``train_size`` is also ``None``, it will be set to ``0``.
         test_mode:
             If ``True`` enables tracking of cache and worker informations.
         num_workers:
             How many subprocesses to use for data loading. ``0`` means that the data will be loaded in the main process.
     """
 
     def __init__(
         self,
-        # DistributedAnnDataCollection args
-        filenames: Sequence[str] | str,
-        limits: Iterable[int] | None = None,
-        shard_size: int | None = None,
-        last_shard_size: int | None = None,
-        max_cache_size: int = 1,
-        cache_size_strictly_enforced: bool = True,
-        label: str | None = None,
-        keys: Sequence[str] | None = None,
-        index_unique: str | None = None,
-        indices_strict: bool = True,
+        dadc: DistributedAnnDataCollection | AnnData,
         # IterableDistributedAnnDataCollectionDataset args
         batch_keys: dict[str, AnnDataField] | None = None,
         batch_size: int = 1,
         shuffle: bool = False,
         seed: int = 0,
         drop_last: bool = False,
+        train_size: float | int | None = None,
+        val_size: float | int | None = None,
         test_mode: bool = False,
         # DataLoader args
         num_workers: int = 0,
     ) -> None:
         super().__init__()
-        # DistributedAnnDataCollection args
-        self.filenames = filenames
-        self.limits = limits
-        self.shard_size = shard_size
-        self.last_shard_size = last_shard_size
-        self.max_cache_size = max_cache_size
-        self.cache_size_strictly_enforced = cache_size_strictly_enforced
-        self.label = label
-        self.keys = keys
-        self.index_unique = index_unique
-        self.indices_strict = indices_strict
+        self.save_hyperparameters(logger=False)
+        # Don't save dadc to the checkpoint
+        self.hparams["dadc"] = None
+
+        self.dadc = dadc
         # IterableDistributedAnnDataCollectionDataset args
         self.batch_keys = batch_keys or {}
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.seed = seed
         self.drop_last = drop_last
+        self.n_train, self.n_val = train_val_split(len(dadc), train_size, val_size)
         self.test_mode = test_mode
         # DataLoader args
         self.num_workers = num_workers
-        # DistributedAnnDataCollection
-        obs_columns = [field.obs_column for field in self.batch_keys.values() if field.obs_column is not None]
-        self.dadc = DistributedAnnDataCollection(
-            filenames=self.filenames,
-            limits=self.limits,
-            shard_size=self.shard_size,
-            last_shard_size=self.last_shard_size,
-            max_cache_size=self.max_cache_size,
-            cache_size_strictly_enforced=self.cache_size_strictly_enforced,
-            label=self.label,
-            keys=self.keys,
-            index_unique=self.index_unique,
-            indices_strict=self.indices_strict,
-            obs_columns=obs_columns,
-        )
-
-    @property
-    def n_obs(self) -> int:
-        return self.dadc.n_obs
-
-    @property
-    def n_vars(self) -> int:
-        return self.dadc.n_vars
-
-    @property
-    def var_names(self) -> np.ndarray:
-        return self.dadc.var_names.values
 
     def setup(self, stage: str | None = None) -> None:
         """
         .. note::
            setup is called from every process across all the nodes. Setting state here is recommended.
 
+        .. note::
+            :attr:`val_dataset` is not shuffled.
+
         """
-        self.dataset = IterableDistributedAnnDataCollectionDataset(
-            dadc=self.dadc,
-            batch_keys=self.batch_keys,
-            batch_size=self.batch_size,
-            shuffle=self.shuffle,
-            seed=self.seed,
-            drop_last=self.drop_last,
-            test_mode=self.test_mode,
-        )
+        if stage == "fit":
+            self.train_dataset = IterableDistributedAnnDataCollectionDataset(
+                dadc=self.dadc,
+                batch_keys=self.batch_keys,
+                batch_size=self.batch_size,
+                shuffle=self.shuffle,
+                seed=self.seed,
+                drop_last=self.drop_last,
+                test_mode=self.test_mode,
+                start_idx=0,
+                end_idx=self.n_train,
+            )
+            self.val_dataset = IterableDistributedAnnDataCollectionDataset(
+                dadc=self.dadc,
+                batch_keys=self.batch_keys,
+                batch_size=self.batch_size,
+                shuffle=False,
+                seed=self.seed,
+                drop_last=False,
+                test_mode=self.test_mode,
+                start_idx=self.n_train,
+                end_idx=self.n_train + self.n_val,
+            )
+
+        if stage == "predict":
+            self.predict_dataset = IterableDistributedAnnDataCollectionDataset(
+                dadc=self.dadc,
+                batch_keys=self.batch_keys,
+                batch_size=self.batch_size,
+                shuffle=self.shuffle,
+                seed=self.seed,
+                drop_last=self.drop_last,
+                test_mode=self.test_mode,
+            )
 
     def train_dataloader(self) -> torch.utils.data.DataLoader:
         """Training dataloader."""
         return torch.utils.data.DataLoader(
-            self.dataset,
+            self.train_dataset,
+            num_workers=self.num_workers,
+            collate_fn=collate_fn,
+        )
+
+    def val_dataloader(self) -> torch.utils.data.DataLoader:
+        """Validation dataloader."""
+        return torch.utils.data.DataLoader(
+            self.val_dataset,
             num_workers=self.num_workers,
             collate_fn=collate_fn,
         )
 
     def predict_dataloader(self) -> torch.utils.data.DataLoader:
         """Prediction dataloader."""
         return torch.utils.data.DataLoader(
-            self.dataset,
+            self.predict_dataset,
             num_workers=self.num_workers,
             collate_fn=collate_fn,
         )
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/core/module.py` & `cellarium_ml-0.0.5/cellarium/ml/core/module.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,209 +1,204 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
-from importlib import import_module
-from typing import IO, Any
-from unittest.mock import patch
+import warnings
+from collections.abc import Iterable
+from typing import Any
 
 import lightning.pytorch as pl
 import numpy as np
 import torch
-from jsonargparse import Namespace
-from lightning.fabric.utilities.types import _MAP_LOCATION_TYPE, _PATH
 from lightning.pytorch.utilities.types import STEP_OUTPUT, OptimizerLRSchedulerConfig
 
-from cellarium.ml.core.saving import _load_state
-from cellarium.ml.models import CellariumModel, PredictMixin
+from cellarium.ml.core.pipeline import CellariumPipeline
+from cellarium.ml.models import CellariumModel
+from cellarium.ml.utilities.core import copy_module
 
 
 class CellariumModule(pl.LightningModule):
     """
     ``CellariumModule`` organizes code into following sections:
 
+        * :attr:`transforms`: A list of transforms to apply to the input data before passing it to the model.
         * :attr:`model`: A :class:`cellarium.ml.models.CellariumModel` to train with
           :meth:`training_step` method and epoch end hooks.
         * :attr:`optim_fn` and :attr:`optim_kwargs`: A Pytorch optimizer class and its keyword arguments.
         * :attr:`scheduler_fn` and :attr:`scheduler_kwargs`: A Pytorch lr scheduler class and its
           keyword arguments.
 
     Args:
+        transforms:
+            A list of transforms to apply to the input data before passing it to the model.
+            If ``None``, no transforms are applied.
         model:
             A :class:`cellarium.ml.models.CellariumModel` to train.
         optim_fn:
             A Pytorch optimizer class, e.g., :class:`~torch.optim.Adam`. If ``None``,
-            defaults to :class:`torch.optim.Adam`.
+            no optimizer is used.
         optim_kwargs:
-            Keyword arguments for optimiser. If ``None``, defaults to ``default_lr``.
+            Keyword arguments for optimiser.
         scheduler_fn:
             A Pytorch lr scheduler class, e.g., :class:`~torch.optim.lr_scheduler.CosineAnnealingLR`.
         scheduler_kwargs:
             Keyword arguments for lr scheduler.
-        default_lr:
-            Default learning rate to use if ``optim_kwargs`` does not contain ``lr``.
-        config:
-            A dictionary or :class:`jsonargparse.Namespace` containing the initialization hyperparameters.
-            If not ``None``, the configuration will be saved as ``"hyper_parameters"`` in the checkpoint.
+        is_initialized:
+            Whether the model has been initialized. This is set to ``False`` by default under the assumption that
+            ``torch.device("meta")`` context was used and is set to ``True`` after
+            the first call to :meth:`configure_model`.
     """
 
     def __init__(
         self,
-        model: CellariumModel,
-        optim_fn: type[torch.optim.Optimizer] | str | None = None,
-        optim_kwargs: dict | None = None,
-        scheduler_fn: type[torch.optim.lr_scheduler.LRScheduler] | str | None = None,
-        scheduler_kwargs: dict | None = None,
-        default_lr: float = 1e-3,
-        config: dict[str, Any] | Namespace | None = None,
+        transforms: Iterable[torch.nn.Module] | None = None,
+        model: CellariumModel | None = None,
+        optim_fn: type[torch.optim.Optimizer] | None = None,
+        optim_kwargs: dict[str, Any] | None = None,
+        scheduler_fn: type[torch.optim.lr_scheduler.LRScheduler] | None = None,
+        scheduler_kwargs: dict[str, Any] | None = None,
+        is_initialized: bool = False,
     ) -> None:
         super().__init__()
-        self.model = model
+        self.save_hyperparameters(logger=False)
+        self.pipeline: CellariumPipeline | None = None
 
-        # set up optimizer and scheduler
-        if isinstance(optim_fn, str):
-            class_module, class_name = optim_fn.rsplit(".", 1)
-            optim_module = import_module(class_module)
-            self.optim_fn = getattr(optim_module, class_name)
-        elif optim_fn is None:
-            self.optim_fn = torch.optim.Adam
+    def configure_model(self) -> None:
+        # This hook is called during each of fit/val/test/predict stages in the same process, so ensure that
+        # implementation of this hook is idempotent, i.e., after the first time the hook is called, subsequent
+        # calls to it should be a no-op.
+        if self.pipeline is not None:
+            return
+
+        # Steps involved in configuring the model:
+        # 1. Make a copy of modules on the meta device and assign to hparams.
+        # 2. Send the original modules to the host device and add to self.pipeline.
+        # 3. Reset the model parameters if it has not been initialized before.
+        # For more context, see discussions in
+        # https://dev-discuss.pytorch.org/t/state-of-model-creation-initialization-seralization-in-pytorch-core/1240
+        #
+        # Benefits of this approach:
+        # 1. The checkpoint stores modules on the meta device.
+        # 2. Loading from a checkpoint skips a wasteful step of initializing module parameters
+        #    before loading the state_dict.
+        # 3. The module parameters are directly initialized on the host gpu device instead of being initialized
+        #    on the cpu and then moved to the gpu device (given that modules were instantiated under
+        #    the ``torch.device("meta")`` context).
+        model, self.hparams["model"] = copy_module(
+            self.hparams["model"], self_device=self.device, copy_device=torch.device("meta")
+        )
+        if self.hparams["transforms"]:
+            transforms, self.hparams["transforms"] = zip(
+                *(
+                    copy_module(transform, self_device=self.device, copy_device=torch.device("meta"))
+                    for transform in self.hparams["transforms"]
+                )
+            )
         else:
-            self.optim_fn = optim_fn
+            transforms = None
 
-        if isinstance(scheduler_fn, str):
-            class_module, class_name = scheduler_fn.rsplit(".", 1)
-            scheduler_module = import_module(class_module)
-            self.scheduler_fn = getattr(scheduler_module, class_name)
-        else:
-            self.scheduler_fn = scheduler_fn
+        self.pipeline = CellariumPipeline(transforms)
+        if model is None:
+            raise ValueError(f"`model` must be an instance of {CellariumModel}. Got {model}")
+        self.pipeline.append(model)
+
+        if not self.hparams["is_initialized"]:
+            model.reset_parameters()
+            self.hparams["is_initialized"] = True
+
+    @property
+    def model(self) -> CellariumModel:
+        """The model"""
+        if self.pipeline is None:
+            raise RuntimeError("The model is not configured. Call `configure_model` before accessing the model.")
+
+        return self.pipeline[-1]
+
+    @property
+    def transforms(self) -> CellariumPipeline:
+        """The transforms pipeline"""
+        if self.pipeline is None:
+            raise RuntimeError("The model is not configured. Call `configure_model` before accessing the model.")
 
-        optim_kwargs = {} if optim_kwargs is None else optim_kwargs
-        if "lr" not in optim_kwargs:
-            optim_kwargs["lr"] = default_lr
-        self.optim_kwargs = optim_kwargs
-        self.scheduler_fn = scheduler_fn
-        self.scheduler_kwargs = scheduler_kwargs
-
-        if config is not None:
-            self._set_hparams(config)
-
-    @classmethod
-    @patch("lightning.pytorch.core.saving._load_state", new=_load_state)
-    def load_from_checkpoint(
-        cls,
-        checkpoint_path: _PATH | IO,
-        map_location: _MAP_LOCATION_TYPE = None,
-        hparams_file: _PATH | None = None,
-        strict: bool = True,
-        **kwargs: Any,
-    ) -> CellariumModule:
-        r"""
-        Primary way of loading a model from a checkpoint. When Cellarium ML saves a checkpoint it stores the config
-        argument passed to ``__init__``  in the checkpoint under ``"hyper_parameters"``.
+        return self.pipeline[:-1]
 
-        Any arguments specified through ``**kwargs`` will override args stored in ``"hyper_parameters"``.
+    def training_step(  # type: ignore[override]
+        self, batch: dict[str, np.ndarray | torch.Tensor], batch_idx: int
+    ) -> torch.Tensor | None:
+        """
+        Forward pass for training step.
 
         Args:
-            checkpoint_path:
-                Path to checkpoint. This can also be a URL, or file-like object
-            map_location:
-                If your checkpoint saved a GPU model and you now load on CPUs
-                or a different number of GPUs, use this to map to the new setup.
-                The behaviour is the same as in :func:`torch.load`.
-            hparams_file:
-                Optional path to a ``.yaml`` or ``.csv`` file with hierarchical structure as in this example:
-
-                .. code-block:: yaml
-
-                    model:
-                      model:
-                        class_path: cellarium.ml.models.OnePassMeanVarStdFromCLI
-                        init_args:
-                          g_genes: 36350
-                          target_count: 10000
-                      optim_fn: null
-                      optim_kwargs: null
-                      scheduler_fn: null
-                      scheduler_kwargs: null
-                      default_lr: 0.001
-
-                If you train a model using :mod:`cellarium.ml.cli` module you most likely won't need this
-                since Cellarium ML CLI will always save the hyperparameters to the checkpoint.
-
-                However, if your checkpoint weights don't have the hyperparameters saved,
-                use this method to pass in a ``.yaml`` file with the hparams you'd like to use.
-                These will be converted into a :class:`dict` and passed into your
-                :class:`CellariumModule` for use.
-            strict:
-                Whether to strictly enforce that the keys in :attr:`checkpoint_path` match the keys
-                returned by this module's state dict.
-            \**kwargs: Any extra keyword args needed to init the model. Can also be used to override saved
-                hyperparameter values.
-
-        Return:
-            :class:`CellariumModule` instance with loaded weights and hyperparameters.
-
-        Example::
-
-            # load weights without mapping ...
-            module = CellariumModule.load_from_checkpoint("path/to/checkpoint.ckpt")
-
-            # or load weights mapping all weights from GPU 1 to GPU 0 ...
-            map_location = {"cuda:1": "cuda:0"}
-            module = CellariumModule.load_from_checkpoint(
-                "path/to/checkpoint.ckpt",
-                map_location=map_location
-            )
-
-            # or load weights and hyperparameters from separate files.
-            module = CellariumModule.load_from_checkpoint(
-                "path/to/checkpoint.ckpt",
-                hparams_file="/path/to/config.yaml"
-            )
+            batch:
+                A dictionary containing the batch data.
+            batch_idx:
+                The index of the batch.
 
-            # override some of the params with new values
-            module = CellariumModule.load_from_checkpoint(
-                "path/to/checkpoint.ckpt",
-                optim_fn=torch.optim.AdamW,
-                default_lr=0.0001,
-            )
+        Returns:
+            Loss tensor or ``None`` if no loss.
         """
-        return super().load_from_checkpoint(
-            checkpoint_path=checkpoint_path,
-            map_location=map_location,
-            hparams_file=hparams_file,
-            strict=strict,
-            **kwargs,
-        )
+        if self.pipeline is None:
+            raise RuntimeError("The model is not configured. Call `configure_model` before accessing the model.")
 
-    def training_step(  # type: ignore[override]
-        self, batch: dict[str, np.ndarray | torch.Tensor], batch_idx: int
-    ) -> torch.Tensor | None:
-        args, kwargs = self.model._get_fn_args_from_batch(batch)
-        loss = self.model(*args, **kwargs)
+        output = self.pipeline(batch)
+        loss = output.get("loss")
         if loss is not None:
             # Logging to TensorBoard by default
             self.log("train_loss", loss)
         return loss
 
-    def forward(self, batch: dict[str, np.ndarray | torch.Tensor]) -> torch.Tensor | dict[str, torch.Tensor | None]:
-        """Forward pass of the model."""
-        assert isinstance(self.model, PredictMixin)
-        args, kwargs = self.model._get_fn_args_from_batch(batch)
-        return self.model.predict(*args, **kwargs)
+    def forward(self, batch: dict[str, np.ndarray | torch.Tensor]) -> dict[str, np.ndarray | torch.Tensor]:
+        """
+        Forward pass for inference step.
+
+        Args:
+            batch: A dictionary containing the batch data.
+
+        Returns:
+            A dictionary containing the batch data and inference outputs.
+        """
+        if self.pipeline is None:
+            raise RuntimeError("The model is not configured. Call `configure_model` before accessing the model.")
+
+        return self.pipeline.predict(batch)
+
+    def validation_step(self, batch: dict[str, Any], batch_idx: int) -> None:
+        """
+        Forward pass for validation step.
+
+        Args:
+            batch:
+                A dictionary containing the batch data.
+            batch_idx:
+                The index of the batch.
+
+        Returns:
+            None
+        """
+        if self.pipeline is None:
+            raise RuntimeError("The model is not configured. Call `configure_model` before accessing the model.")
+
+        self.pipeline.validate(batch)
 
-    def configure_optimizers(self) -> OptimizerLRSchedulerConfig:
+    def configure_optimizers(self) -> OptimizerLRSchedulerConfig | None:
         """Configure optimizers for the model."""
-        optim_config: OptimizerLRSchedulerConfig = {
-            "optimizer": self.optim_fn(self.model.parameters(), **self.optim_kwargs)
-        }
-        if self.scheduler_fn is not None:
-            assert self.scheduler_kwargs is not None
-            scheduler = self.scheduler_fn(optim_config["optimizer"], **self.scheduler_kwargs)
+        optim_fn = self.hparams["optim_fn"]
+        optim_kwargs = self.hparams["optim_kwargs"] or {}
+        scheduler_fn = self.hparams["scheduler_fn"]
+        scheduler_kwargs = self.hparams["scheduler_kwargs"] or {}
+
+        if optim_fn is None:
+            if optim_kwargs:
+                warnings.warn("Optimizer kwargs are provided but no optimizer is defined.", UserWarning)
+            if scheduler_fn is not None:
+                warnings.warn("Scheduler is defined but no optimizer is defined.", UserWarning)
+            return None
+
+        optim_config: OptimizerLRSchedulerConfig = {"optimizer": optim_fn(self.model.parameters(), **optim_kwargs)}
+        if scheduler_fn is not None:
+            scheduler = scheduler_fn(optim_config["optimizer"], **scheduler_kwargs)
             optim_config["lr_scheduler"] = {"scheduler": scheduler, "interval": "step"}
         return optim_config
 
     def on_train_epoch_start(self) -> None:
         """
         Calls the ``set_epoch`` method on the iterable dataset of the given dataloader.
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/data/__init__.py` & `cellarium_ml-0.0.5/cellarium/ml/data/__init__.py`

 * *Files identical despite different names*

### Comparing `cellarium-ml-0.0.3/cellarium/ml/data/dadc_dataset.py` & `cellarium_ml-0.0.5/cellarium/ml/data/dadc_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
 import math
 
 import numpy as np
 import torch
+from anndata import AnnData
 from torch.utils.data import IterableDataset
 
 from cellarium.ml.data.distributed_anndata import DistributedAnnDataCollection
 from cellarium.ml.utilities.data import AnnDataField, get_rank_and_num_replicas, get_worker_info
 
 
 class IterableDistributedAnnDataCollectionDataset(IterableDataset):
@@ -39,25 +40,25 @@
         ...     shard_size=10_000,
         ...     max_cache_size=2)
 
         >>> dataset = IterableDistributedAnnDataCollectionDataset(
         ...     dadc,
         ...     batch_keys={
         ...         "x_ng": AnnDataField(attr="X", convert_fn=densify),
-        ...         "feature_g": AnnDataField(attr="var_names"),
+        ...         "var_names_g": AnnDataField(attr="var_names"),
         ...     },
         ...     batch_size=5000,
         ...     shuffle=True,
         ...     seed=0,
         ...     drop_last=True,
         ... )
 
     Args:
         dadc:
-            DistributedAnnDataCollection from which to load the data.
+            DistributedAnnDataCollection or AnnData from which to load the data.
         batch_keys:
             Dictionary that specifies which attributes and keys of the :attr:`dadc` to return
             in the batch data and how to convert them. Keys must correspond to
             the input keys of the transforms or the model. Values must be instances of
             :class:`cellarium.ml.utilities.data.AnnDataField`.
         batch_size:
             How many samples per batch to load.
@@ -66,67 +67,80 @@
         seed:
             Random seed used to shuffle the sampler if :attr:`shuffle=True`.
         drop_last:
             If ``True``, then the sampler will drop the tail of the data
             to make it evenly divisible across the number of replicas. If ``False``,
             the sampler will add extra indices to make the data evenly divisible across
             the replicas.
+        start_idx:
+            The starting index of the dataset. If ``None``, then the dataset will start from the first index.
+        end_idx:
+            The ending index (exclusive) of the dataset. If ``None``, then the dataset will end at
+            the last index (inclusive).
         test_mode:
             If ``True``, then tracking of cache and worker informations will be enabled.
     """
 
     def __init__(
         self,
-        dadc: DistributedAnnDataCollection,
+        dadc: DistributedAnnDataCollection | AnnData,
         batch_keys: dict[str, AnnDataField],
         batch_size: int = 1,
         shuffle: bool = False,
         seed: int = 0,
         drop_last: bool = False,
+        start_idx: int | None = None,
+        end_idx: int | None = None,
         test_mode: bool = False,
     ) -> None:
         self.dadc = dadc
+        if isinstance(dadc, AnnData):
+            # mimic a DistributedAnnDataCollection
+            self.dadc.limits = [dadc.n_obs]
         self.batch_keys = batch_keys
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.seed = seed
         self.drop_last = drop_last
+        self.start_idx = 0 if start_idx is None else start_idx
+        self.end_idx = dadc.n_obs if end_idx is None else end_idx
         self.epoch = 0
         self.test_mode = test_mode
 
     def __len__(self) -> int:
         """
         Returns the number of batches per replica.
         """
         _, num_replicas = get_rank_and_num_replicas()
 
-        if self.drop_last and len(self.dadc) % num_replicas != 0:
+        n_obs = self.end_idx - self.start_idx
+        if self.drop_last and n_obs % num_replicas != 0:
             # Split to nearest available length that is evenly divisible.
             # This is to ensure each rank receives the same amount of data.
-            per_replica = len(self.dadc) // num_replicas
+            per_replica = n_obs // num_replicas
         else:
-            per_replica = math.ceil(len(self.dadc) / num_replicas)
+            per_replica = math.ceil(n_obs / num_replicas)
         return math.ceil(per_replica / float(self.batch_size))
 
     def set_epoch(self, epoch: int) -> None:
         r"""
         Sets the epoch for the iterator. When :attr:`shuffle=True`, this ensures all replicas
         use a different random ordering for each epoch.
         """
         self.epoch = epoch
 
     def __getitem__(self, idx: int | list[int] | slice) -> dict[str, np.ndarray]:
         r"""
-        Returns a dictionary containing the data from the :attr:`dadc` with keys specified by its :attr:`dadc.convert`
+        Returns a dictionary containing the data from the :attr:`dadc` with keys specified by the :attr:`batch_keys`
         at the given index ``idx``.
         """
 
         data = {}
         for key, field in self.batch_keys.items():
-            data[key] = field(self.dadc)[idx]
+            data[key] = field(self.dadc, idx)
 
         # for testing purposes
         if self.test_mode:
             rank, num_replicas = get_rank_and_num_replicas()
             worker_id, num_workers = get_worker_info()
             data["rank"] = np.array([rank])
             data["num_replicas"] = np.array([num_replicas])
@@ -289,15 +303,15 @@
 
         +----------+-------+-------+--------+
         |          |batch 0|batch 1|batch 2 |
         +==========+=======+=======+========+
         | worker 0 | (6,7) | (8,9) | (10,0) |
         +----------+-------+-------+--------+
         """
-        if self.test_mode:
+        if self.test_mode and isinstance(self.dadc, DistributedAnnDataCollection):
             # clear lru cache
             self.dadc.cache.clear()
 
         # replicas
         rank, num_replicas = get_rank_and_num_replicas()
 
         if self.drop_last and len(self.dadc) % num_replicas != 0:
@@ -319,34 +333,39 @@
         iter_start = worker_id * per_worker
         iter_end = min(iter_start + per_worker, per_replica)
 
         # indices
         if self.shuffle:
             rng = torch.Generator()
             rng.manual_seed(self.seed + self.epoch)
-            iter_limits = list(zip([0] + self.dadc.limits, self.dadc.limits))
+            limits = [idx for idx in self.dadc.limits if idx > self.start_idx and idx < self.end_idx]
+            iter_limits = list(zip([self.start_idx] + limits, limits + [self.end_idx]))
             # shuffle shards
             limit_indices = torch.randperm(len(iter_limits), generator=rng).tolist()
             indices = []
             for limit_idx in limit_indices:
                 lower, upper = iter_limits[limit_idx]
                 # shuffle cells within shards
                 indices.extend((torch.randperm(upper - lower, generator=rng) + lower).tolist())
         else:
-            indices = list(range(len(self.dadc)))
+            indices = list(range(self.start_idx, self.end_idx))
 
         if not self.drop_last:
             # add extra samples to make it evenly divisible
             padding_size = total_size - len(indices)
             if padding_size <= len(indices):
                 indices += indices[:padding_size]
             else:
                 indices += (indices * math.ceil(padding_size / len(indices)))[:padding_size]
         else:
             # remove tail of data to make it evenly divisible.
             indices = indices[:total_size]
         indices = indices[rank * per_replica : (rank + 1) * per_replica]
-        assert len(indices) == per_replica
+        if len(indices) != per_replica:
+            raise ValueError(
+                f"The number of indices must be equal to the per_replica size. "
+                f"Got {len(indices)} != {per_replica} at rank {rank}."
+            )
 
         yield from (self[indices[i : i + self.batch_size]] for i in range(iter_start, iter_end, self.batch_size))
         # Sets epoch for persistent workers
         self.set_epoch(self.epoch + 1)
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/data/distributed_anndata.py` & `cellarium_ml-0.0.5/cellarium/ml/data/distributed_anndata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import gc
 from collections.abc import Iterable, Sequence
 from contextlib import contextmanager
 
+import numpy as np
 import pandas as pd
-from anndata import AnnData
-from anndata._core.index import Index, _normalize_indices
+from anndata import AnnData, concat
+from anndata._core.index import Index, Index1D, _normalize_indices
 from anndata.experimental.multi_files._anncollection import (
     AnnCollection,
     AnnCollectionView,
     ConvertType,
 )
 from boltons.cacheutils import LRU
 from braceexpand import braceexpand
@@ -46,15 +45,15 @@
     """
     Distributed AnnData Collection View.
 
     This class is a wrapper around AnnCollectionView where adatas is a list
     of :class:`LazyAnnData` objects.
     """
 
-    def __getitem__(self, index: Index) -> DistributedAnnDataCollectionView:
+    def __getitem__(self, index: Index) -> "DistributedAnnDataCollectionView":
         oidx, vidx = _normalize_indices(index, self.obs_names, self.var_names)
         resolved_idx = self._resolve_idx(oidx, vidx)
 
         return DistributedAnnDataCollectionView(self.reference, self.convert, resolved_idx)
 
     @property
     def obs_names(self) -> pd.Index:
@@ -148,15 +147,15 @@
             and a function to be applied as a value.
         indices_strict:
             If  ``True``, arrays from the subset objects will always have the same order
             of indices as in selection used to subset.
             This parameter can be set to ``False`` if the order in the returned arrays
             is not important, for example, when using them for stochastic gradient descent.
             In this case the performance of subsetting can be a bit better.
-        obs_columns:
+        obs_columns_to_validate:
             Subset of columns to validate in the :attr:`obs` attribute.
             If ``None``, all columns are validated.
     """
 
     def __init__(
         self,
         filenames: Sequence[str] | str,
@@ -166,95 +165,110 @@
         max_cache_size: int = 1,
         cache_size_strictly_enforced: bool = True,
         label: str | None = None,
         keys: Sequence[str] | None = None,
         index_unique: str | None = None,
         convert: ConvertType | None = None,
         indices_strict: bool = True,
-        obs_columns: Sequence | None = None,
+        obs_columns_to_validate: Sequence[str] | None = None,
     ):
         self.filenames = list(braceexpand(filenames) if isinstance(filenames, str) else filenames)
         if (shard_size is None) and (last_shard_size is not None):
             raise ValueError("If `last_shard_size` is specified then `shard_size` must also be specified.")
         if limits is None:
-            assert shard_size is not None, "If `limits` is `None` then `shard_size` must be specified`"
+            if shard_size is None:
+                raise ValueError("If `limits` is `None` then `shard_size` must be specified`")
             limits = [shard_size * (i + 1) for i in range(len(self.filenames))]
             if last_shard_size is not None:
                 limits[-1] = limits[-1] - shard_size + last_shard_size
         else:
             limits = list(limits)
-        assert len(limits) == len(self.filenames)
+        if len(limits) != len(self.filenames):
+            raise ValueError(
+                f"The number of points in `limits` ({len(limits)}) must match "
+                f"the number of `filenames` ({len(self.filenames)})."
+            )
         # lru cache
         self.cache = LRU(max_cache_size)
         self.max_cache_size = max_cache_size
         self.cache_size_strictly_enforced = cache_size_strictly_enforced
         # schema
         adata0 = self.cache[self.filenames[0]] = read_h5ad_file(self.filenames[0])
-        assert len(adata0) == limits[0]
-        self.schema = AnnDataSchema(adata0, obs_columns)
+        if len(adata0) != limits[0]:
+            raise ValueError(
+                f"The number of cells in the first anndata file ({len(adata0)}) "
+                f"does not match the first limit ({limits[0]})."
+            )
+        self.obs_columns_to_validate = obs_columns_to_validate
+        self.schema = AnnDataSchema(adata0, obs_columns_to_validate)
         # lazy anndatas
         lazy_adatas = [
             LazyAnnData(filename, (start, end), self.schema, self.cache)
             for start, end, filename in zip([0] + limits, limits, self.filenames)
         ]
         # use filenames as default keys
         if keys is None:
             keys = self.filenames
-        assert len(keys) == len(self.filenames)
+        if len(keys) != len(self.filenames):
+            raise ValueError(
+                f"The number of keys ({len(keys)}) must match the number of `filenames` ({len(filenames)})."
+            )
         with lazy_getattr():
             super().__init__(
                 adatas=lazy_adatas,
                 join_obs=None,
                 join_obsm=None,
                 join_vars=None,
                 label=label,
                 keys=keys,
                 index_unique=index_unique,
                 convert=convert,
                 harmonize_dtypes=False,
                 indices_strict=indices_strict,
             )
 
-    def __getitem__(self, index: Index) -> DistributedAnnDataCollectionView:
+    def __getitem__(self, index: Index) -> AnnData:
         """
-        Return a distributed view of the collection of anndatas.
+        Materialize and gather anndata files at given indices from the list of lazy anndatas.
 
         :class:`LazyAnnData` instances corresponding to cells in the index are materialized.
         """
         oidx, vidx = _normalize_indices(index, self.obs_names, self.var_names)
-        resolved_idx = self._resolve_idx(oidx, vidx)
-        adatas_indices = [i for i, e in enumerate(resolved_idx[0]) if e is not None]
-        # TODO: materialize at the last moment?
-        self.materialize(adatas_indices)
+        adatas_oidx, oidx, vidx, reverse = self._resolve_idx(oidx, vidx)
+        adatas = self.materialize(adatas_oidx, vidx)
+        adata = concat(adatas, merge="same")
+        adata = adata if reverse is None else adata[reverse]
+        # make sure that categorical dtypes are preserved
+        adata.obs = adata.obs.astype(self.schema.attr_values["obs"].dtypes)
+        return adata
 
-        return DistributedAnnDataCollectionView(self, self.convert, resolved_idx)
-
-    def materialize(self, indices: int | Sequence[int]) -> list[AnnData]:
+    def materialize(self, adatas_oidx: list[np.ndarray | None], vidx: Index1D) -> list[AnnData]:
         """
         Buffer and return anndata files at given indices from the list of lazy anndatas.
 
         This efficiently first retrieves cached files and only then caches new files.
         """
-        if isinstance(indices, int):
-            indices = (indices,)
+        adata_idx_to_oidx = {i: oidx for i, oidx in enumerate(adatas_oidx) if oidx is not None}
+        n_adatas = len(adata_idx_to_oidx)
         if self.cache_size_strictly_enforced:
-            assert len(indices) <= self.max_cache_size, (
-                f"Expected the number of anndata files ({len(indices)}) to be "
-                f"no more than the max cache size ({self.max_cache_size})."
-            )
-        adatas = [None] * len(indices)
+            if n_adatas > self.max_cache_size:
+                raise ValueError(
+                    f"Expected the number of anndata files ({n_adatas}) to be "
+                    f"no more than the max cache size ({self.max_cache_size})."
+                )
+        adatas = [None] * n_adatas
         # first fetch cached anndata files
         # this ensures that they are not popped if they were lru
-        for i, idx in enumerate(indices):
-            if self.adatas[idx].cached:
-                adatas[i] = self.adatas[idx].adata
+        for i, (adata_idx, oidx) in enumerate(adata_idx_to_oidx.items()):
+            if self.adatas[adata_idx].cached:
+                adatas[i] = self.adatas[adata_idx].adata[oidx, vidx]
         # only then cache new anndata files
-        for i, idx in enumerate(indices):
-            if not self.adatas[idx].cached:
-                adatas[i] = self.adatas[idx].adata
+        for i, (adata_idx, oidx) in enumerate(adata_idx_to_oidx.items()):
+            if not self.adatas[adata_idx].cached:
+                adatas[i] = self.adatas[adata_idx].adata[oidx, vidx]
         return adatas
 
     def __repr__(self) -> str:
         n_obs, n_vars = self.shape
         descr = f"DistributedAnnDataCollection object with n_obs × n_vars = {self.n_obs} × {self.n_vars}"
         descr += f"\n  constructed from {len(self.filenames)} AnnData objects"
         for attr, keys in self._view_attrs_keys.items():
@@ -271,23 +285,30 @@
 
         return descr
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["cache"]
         del state["adatas"]
+        del state["obs_names"]
+        del state["schema"]
+        del state["_obs"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.cache = LRU(self.max_cache_size)
+        adata0 = self.cache[self.filenames[0]] = read_h5ad_file(self.filenames[0])
+        self.schema = AnnDataSchema(adata0, self.obs_columns_to_validate)
         self.adatas = [
             LazyAnnData(filename, (start, end), self.schema, self.cache)
             for start, end, filename in zip([0] + self.limits, self.limits, self.filenames)
         ]
+        self.obs_names = pd.Index([f"cell_{i}" for i in range(self.limits[-1])])
+        self._obs = pd.DataFrame(index=self.obs_names)
 
 
 class LazyAnnData:
     """
     Lazy :class:`~anndata.AnnData` backed by a file.
 
     Accessing attributes under :func:`lazy_getattr` context returns schema attributes.
@@ -363,18 +384,19 @@
         """Return backed anndata from the filename"""
         try:
             adata = self.cache[self.filename]
         except KeyError:
             # fetch anndata
             adata = read_h5ad_file(self.filename)
             # validate anndata
-            assert self.n_obs == adata.n_obs, (
-                "Expected n_obs for LazyAnnData object and backed anndata to match "
-                f"but found {self.n_obs} and {adata.n_obs}, respectively."
-            )
+            if self.n_obs != adata.n_obs:
+                raise ValueError(
+                    "Expected `n_obs` for LazyAnnData object and backed anndata to match "
+                    f"but found {self.n_obs} and {adata.n_obs}, respectively."
+                )
             self.schema.validate_anndata(adata)
             # cache anndata
             if len(self.cache) < self.cache.max_size:
                 self.cache[self.filename] = adata
             else:
                 self.cache[self.filename] = adata
                 # garbage collection of AnnData is not reliable
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/data/fileio.py` & `cellarium_ml-0.0.5/cellarium/ml/data/fileio.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     Example::
 
         >>> adata = read_h5ad_gcs("gs://dsp-cellarium-cas-public/test-data/test_0.h5ad")
 
     Args:
         filename: Path to the data file in Cloud Storage.
     """
-    assert filename.startswith("gs:")
+    if not filename.startswith("gs:"):
+        raise ValueError("The filename must start with 'gs:' protocol name.")
     # parse bucket and blob names from the filename
     filename = re.sub(r"^gs://?", "", filename)
     bucket_name, blob_name = filename.split("/", 1)
 
     if storage_client is None:
         storage_client = Client()
 
@@ -47,29 +48,31 @@
         >>> adata = read_h5ad_url(
         ...     "https://storage.googleapis.com/dsp-cellarium-cas-public/test-data/test_0.h5ad"
         ... )
 
     Args:
         filename: URL of the data file.
     """
-    assert any(filename.startswith(scheme) for scheme in url_schemes)
+    if not any(filename.startswith(scheme) for scheme in url_schemes):
+        raise ValueError("The filename must start with 'http:', 'https:', or 'ftp:' protocol name.")
     with urllib.request.urlopen(filename) as response:
         with tempfile.TemporaryFile() as tmp_file:
             shutil.copyfileobj(response, tmp_file)
             return read_h5ad(tmp_file)
 
 
 def read_h5ad_local(filename: str) -> AnnData:
     r"""
     Read ``.h5ad``-formatted hdf5 file from the local disk.
 
     Args:
         filename: Path to the local data file.
     """
-    assert filename.startswith("file:")
+    if not filename.startswith("file:"):
+        raise ValueError("The filename must start with 'file:' protocol name.")
     filename = re.sub(r"^file://?", "", filename)
     return read_h5ad(filename)
 
 
 def read_h5ad_file(filename: str, **kwargs) -> AnnData:
     r"""
     Read ``.h5ad``-formatted hdf5 file from a filename.
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/data/schema.py` & `cellarium_ml-0.0.5/cellarium/ml/data/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,40 +23,40 @@
         >>> adata.var["mu"] = ["a", "b", "c"]
         >>> schema = AnnDataSchema(ref_adata)
         >>> schema.validate_anndata(adata)
 
     Args:
         adata:
             Reference AnnData object.
-        obs_columns:
+        obs_columns_to_validate:
             Subset of columns to validate in the ``.obs`` attribute.
             If ``None``, all columns are validated.
     """
 
     attrs = ["obs", "obsm", "var", "varm", "varp", "var_names", "layers"]
 
-    def __init__(self, adata: AnnData, obs_columns: Sequence | None = None) -> None:
+    def __init__(self, adata: AnnData, obs_columns_to_validate: Sequence[str] | None = None) -> None:
         self.attr_values = {}
         for attr in self.attrs:
             # FIXME: some of the attributes have a reference to the anndata object itself.
             # This results in anndata object not being garbage collected.
             self.attr_values[attr] = getattr(adata, attr)
-        self.obs_columns = obs_columns
+        self.obs_columns_to_validate = obs_columns_to_validate
 
     def validate_anndata(self, adata: AnnData) -> None:
         """Validate anndata has proper attributes."""
 
         for attr in self.attrs:
             value = getattr(adata, attr)
             ref_value = self.attr_values[attr]
             if attr == "obs":
-                if self.obs_columns is not None:
+                if self.obs_columns_to_validate is not None:
                     # Subset the columns to validate
-                    ref_value = ref_value[self.obs_columns]
-                    value = value[self.obs_columns]
+                    ref_value = ref_value[self.obs_columns_to_validate]
+                    value = value[self.obs_columns_to_validate]
                 # compare the elements inside the Index object and their order
                 if not ref_value.columns.equals(value.columns):
                     raise ValueError(
                         ".obs attribute columns for anndata passed in does not match .obs attribute columns "
                         "of the reference anndata."
                     )
                 if not ref_value.dtypes.equals(value.dtypes):
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/lr_schedulers/linear_lr.py` & `cellarium_ml-0.0.5/cellarium/ml/lr_schedulers/linear_lr.py`

 * *Files identical despite different names*

### Comparing `cellarium-ml-0.0.3/cellarium/ml/models/__init__.py` & `cellarium_ml-0.0.5/cellarium/ml/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
-from cellarium.ml.models.from_cli import (
-    GeneformerFromCLI,
-    IncrementalPCAFromCLI,
-    OnePassMeanVarStdFromCLI,
-    ProbabilisticPCAFromCLI,
-    TDigestFromCLI,
-)
-from cellarium.ml.models.gather import GatherLayer
 from cellarium.ml.models.geneformer import Geneformer
 from cellarium.ml.models.incremental_pca import IncrementalPCA
 from cellarium.ml.models.logistic_regression import LogisticRegression
-from cellarium.ml.models.model import CellariumModel, PredictMixin
+from cellarium.ml.models.model import CellariumModel, PredictMixin, ValidateMixin
+from cellarium.ml.models.mu_linear import MuLinear, abcdParameter
 from cellarium.ml.models.onepass_mean_var_std import OnePassMeanVarStd
 from cellarium.ml.models.probabilistic_pca import ProbabilisticPCA
 from cellarium.ml.models.tdigest import TDigest
 
 __all__ = [
     "CellariumModel",
-    "GatherLayer",
     "Geneformer",
-    "GeneformerFromCLI",
     "IncrementalPCA",
-    "IncrementalPCAFromCLI",
     "LogisticRegression",
+    "abcdParameter",
+    "MuLinear",
     "OnePassMeanVarStd",
-    "OnePassMeanVarStdFromCLI",
     "PredictMixin",
     "ProbabilisticPCA",
-    "ProbabilisticPCAFromCLI",
     "TDigest",
-    "TDigestFromCLI",
+    "ValidateMixin",
 ]
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/models/incremental_pca.py` & `cellarium_ml-0.0.5/cellarium/ml/models/incremental_pca.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,94 +1,107 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
 import math
-from typing import Any
+from collections.abc import Sequence
 
 import lightning.pytorch as pl
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 from lightning.pytorch.strategies import DDPStrategy
 
 from cellarium.ml.models.model import CellariumModel, PredictMixin
+from cellarium.ml.utilities.testing import (
+    assert_arrays_equal,
+    assert_columns_and_array_lengths_equal,
+)
 
 
 class IncrementalPCA(CellariumModel, PredictMixin):
     """
     Distributed and Incremental PCA.
 
     **References:**
 
     1. `A Distributed and Incremental SVD Algorithm for Agglomerative Data Analysis on Large Networks (Iwen et al.)
        <https://users.math.msu.edu/users/iwenmark/Papers/distrib_inc_svd.pdf>`_.
     2. `Incremental Learning for Robust Visual Tracking (Ross et al.)
        <https://www.cs.toronto.edu/~dross/ivt/RossLimLinYang_ijcv.pdf>`_.
 
     Args:
-        g_genes:
-            Number of genes.
-        k_components:
+        var_names_g:
+            The variable names schema for the input data validation.
+        n_components:
             Number of principal components.
         svd_lowrank_niter:
             Number of iterations for the low-rank SVD algorithm.
         perform_mean_correction:
             If ``True`` then the mean correction is applied to the update step.
             If ``False`` then the data is assumed to be centered and the mean correction
             is not applied to the update step.
-        transform:
-            If not ``None`` is used to transform the input data.
     """
 
     def __init__(
         self,
-        g_genes: int,
-        k_components: int,
+        var_names_g: Sequence[str],
+        n_components: int,
         svd_lowrank_niter: int = 2,
         perform_mean_correction: bool = False,
-        transform: nn.Module | None = None,
     ) -> None:
         super().__init__()
-        self.g_genes = g_genes
-        self.k_components = k_components
+        self.var_names_g = np.array(var_names_g)
+        n_vars = len(self.var_names_g)
+        self.n_vars = n_vars
+        self.n_components = n_components
         self.svd_lowrank_niter = svd_lowrank_niter
         self.perform_mean_correction = perform_mean_correction
-        self.transform = transform
         self.V_kg: torch.Tensor
         self.S_k: torch.Tensor
         self.x_mean_g: torch.Tensor
         self.x_size: torch.Tensor
-        self.register_buffer("V_kg", torch.zeros(k_components, g_genes))
-        self.register_buffer("S_k", torch.zeros(k_components))
-        self.register_buffer("x_mean_g", torch.zeros(g_genes))
-        self.register_buffer("x_size", torch.tensor(0))
-        self._dummy_param = nn.Parameter(torch.tensor(0.0))
-
-    @staticmethod
-    def _get_fn_args_from_batch(tensor_dict: dict[str, np.ndarray | torch.Tensor]) -> tuple[tuple, dict]:
-        x = tensor_dict["X"]
-        return (x,), {}
+        self.register_buffer("V_kg", torch.empty(n_components, n_vars))
+        self.register_buffer("S_k", torch.empty(n_components))
+        self.register_buffer("x_mean_g", torch.empty(n_vars))
+        self.register_buffer("x_size", torch.empty(()))
+        self._dummy_param = nn.Parameter(torch.empty(()))
+        self.reset_parameters()
+
+    def reset_parameters(self) -> None:
+        self.V_kg.zero_()
+        self.S_k.zero_()
+        self.x_mean_g.zero_()
+        self.x_size.zero_()
+        self._dummy_param.data.zero_()
 
-    def forward(self, x_ng: torch.Tensor) -> None:
+    def forward(self, x_ng: torch.Tensor, var_names_g: np.ndarray) -> dict[str, torch.Tensor | None]:
         """
         Incrementally update partial SVD with new data.
+
+        Args:
+            x_ng:
+                Gene counts matrix.
+            var_names_g:
+                The list of the variable names in the input data.
+
+        Returns:
+            An empty dictionary.
         """
-        if self.transform is not None:
-            x_ng = self.transform(x_ng)
+        assert_columns_and_array_lengths_equal("x_ng", x_ng, "var_names_g", var_names_g)
+        assert_arrays_equal("var_names_g", var_names_g, "var_names_g", self.var_names_g)
 
-        g = self.g_genes
-        k = self.k_components
+        g = self.n_vars
+        k = self.n_components
         niter = self.svd_lowrank_niter
         self_X_size = self.x_size
         other_X_size = x_ng.size(0)
         total_X_size = self_X_size + other_X_size
         assert k <= min(other_X_size, g), (
-            f"Rank of svd_lowrank (k_components): {k}"
-            f" must be less than min(n_cells, g_genes): {min(other_X_size, g)}"
+            f"Rank of svd_lowrank (n_components): {k}" f" must be less than min(n_obs, n_vars): {min(other_X_size, g)}"
         )
 
         # compute SVD of new data
         if self.perform_mean_correction:
             self_X_mean = self.x_mean_g
             other_X_mean = x_ng.mean(dim=0)
             _, S_k, V_gk = torch.svd_lowrank(x_ng - other_X_mean, q=k, niter=niter)
@@ -111,14 +124,16 @@
         # update buffers
         self.V_kg = V_gk.T
         self.S_k = S_k
         self.x_size = total_X_size
         if self.perform_mean_correction:
             self.x_mean_g = self_X_mean * self_X_size / total_X_size + other_X_mean * other_X_size / total_X_size
 
+        return {}
+
     def on_train_start(self, trainer: pl.Trainer) -> None:
         if trainer.world_size > 1:
             assert isinstance(trainer.strategy, DDPStrategy), (
                 "Distributed and Incremental PCA requires that " "the trainer uses the DDP strategy."
             )
             assert trainer.strategy._ddp_kwargs["broadcast_buffers"] is False, (
                 "Distributed and Incremental PCA requires that " "broadcast_buffers is set to False."
@@ -140,15 +155,15 @@
         # no need to merge if only one process
         if trainer.world_size == 1:
             return
 
         assert trainer.current_epoch == 0, "Only one pass through the data is required."
 
         # parameters
-        k = self.k_components
+        k = self.n_components
         niter = self.svd_lowrank_niter
         self_X_size = self.x_size
         self_X = torch.einsum("k,kg->kg", self.S_k, self.V_kg).contiguous()
         if self.perform_mean_correction:
             self_X_mean = self.x_mean_g
 
         # initialize rank, world_size, and merging level i
@@ -212,27 +227,42 @@
 
     @property
     def explained_variance_k(self) -> torch.Tensor:
         r"""
         The amount of variance explained by each of the selected components. The variance
         estimation uses ``x_size`` degrees of freedom.
 
-        Equal to ``k_components`` largest eigenvalues of the covariance matrix of input data.
+        Equal to ``n_components`` largest eigenvalues of the covariance matrix of input data.
         """
         return self.S_k**2 / self.x_size
 
     @property
     def components_kg(self) -> torch.Tensor:
         r"""
         Principal axes in feature space, representing the directions of maximum variance
         in the data. Equivalently, the right singular vectors of the centered input data,
         parallel to its eigenvectors. The components are sorted by decreasing ``explained_variance_k``.
         """
         return self.V_kg
 
-    def predict(self, x_ng: torch.Tensor, **kwargs: Any) -> torch.Tensor:
-        r"""
+    def predict(self, x_ng: torch.Tensor, var_names_g: np.ndarray) -> dict[str, np.ndarray | torch.Tensor]:
+        """
         Centering and embedding of the input data ``x_ng`` into the principal component space.
+
+        Args:
+            x_ng:
+                Gene counts matrix.
+            var_names_g:
+                The list of the variable names in the input data.
+
+        Returns:
+            A dictionary with the following keys:
+
+            - ``x_ng``: Embedding of the input data into the principal component space.
+            - ``var_names_g``: The list of variable names for the output data.
         """
-        if self.transform is not None:
-            x_ng = self.transform(x_ng)
-        return (x_ng - self.x_mean_g) @ self.V_kg.T
+        assert_columns_and_array_lengths_equal("x_ng", x_ng, "var_names_g", var_names_g)
+        assert_arrays_equal("var_names_g", var_names_g, "var_names_g", self.var_names_g)
+
+        z_nk = (x_ng - self.x_mean_g) @ self.V_kg.T
+        var_names_k = np.array([f"PC{i + 1}" for i in range(self.n_components)])
+        return {"x_ng": z_nk, "var_names_g": var_names_k}
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/models/model.py` & `cellarium_ml-0.0.5/cellarium/ml/models/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 
     def __init__(self) -> None:
         super(torch.nn.Module, self).__setattr__("_pyro_params", OrderedDict())
         super().__init__()
 
     __call__: Callable[..., torch.Tensor | None]
 
-    @staticmethod
     @abstractmethod
-    def _get_fn_args_from_batch(tensor_dict: dict[str, np.ndarray | torch.Tensor]) -> tuple[tuple, dict]:
+    def reset_parameters(self) -> None:
         """
-        Get forward method arguments from batch.
+        Reset the model parameters and buffers that were constructed in the __init__ method.
+        Constructed means methods like ``torch.tensor``, ``torch.empty``, ``torch.zeros``,
+        ``torch.randn``, ``torch.as_tensor``, etc.
+        If the parameter or buffer was assigned (e.g. from a torch.Tensor passed to the __init__)
+        then there is no need to reset it.
         """
 
     def __getattr__(self, name: str) -> Any:
         if "_pyro_params" in self.__dict__:
             _pyro_params = self.__dict__["_pyro_params"]
             if name in _pyro_params:
                 constraint, event_dim = _pyro_params[name]
@@ -66,20 +69,23 @@
 
 class PredictMixin(metaclass=ABCMeta):
     """
     Abstract mixin class for models that can perform prediction.
     """
 
     @abstractmethod
-    def predict(self, x_ng: torch.Tensor, **kwargs: Any) -> torch.Tensor | dict[str, torch.Tensor | None]:
+    def predict(self, *args: Any, **kwargs: Any) -> dict[str, np.ndarray | torch.Tensor]:
         """
-        Perform prediction on data tensor.
+        Perform prediction.
+        """
+
 
-        Args:
-            x_ng:
-                Data tensor.
-            **kwargs:
-                Additional keyword arguments.
+class ValidateMixin(metaclass=ABCMeta):
+    """
+    Abstract mixin class for models that can perform validation.
+    """
 
-        Returns:
-            Prediction tensor or dictionary of prediction tensors.
+    @abstractmethod
+    def validate(self, *args: Any, **kwargs: Any) -> None:
+        """
+        Perform validation.
         """
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/preprocessing/highly_variable_genes.py` & `cellarium_ml-0.0.5/cellarium/ml/preprocessing/highly_variable_genes.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,17 @@
             dispersions are ignored.
         n_bins:
             Number of bins for binning the mean gene expression. Normalization is done with respect to each bin.
             If just a single gene falls into a bin, the normalized dispersion is artificially set to 1. You’ll be
             informed about this
     """
     # compute the dispersion
-    assert len(gene_names) == len(mean) == len(var), "Sizes of `gene_names`, `mean`, and `var` should be the same"
+    if not (len(gene_names) == len(mean) == len(var)):
+        raise ValueError("Sizes of `gene_names`, `mean`, and `var` should be the same")
+
     mean[mean == 0] = 1e-12  # set entries equal to zero to small value
     dispersion = var / mean
     # logarithmized mean as in Seurat
     dispersion[dispersion == 0] = np.nan
     dispersion = torch.log(dispersion)
 
     mean = torch.log1p(mean)
@@ -108,16 +110,16 @@
         disp_cut_off = dispersion_norm[n_top_genes - 1]
         gene_subset = np.nan_to_num(df["dispersions_norm"].values) >= disp_cut_off
         logging.debug(f"the {n_top_genes} top genes correspond to a " f"normalized dispersion cutoff of {disp_cut_off}")
     else:
         dispersion_norm[np.isnan(dispersion_norm)] = 0  # similar to Seurat
         gene_subset = np.logical_and.reduce(
             (
-                mean > min_mean,
-                mean < max_mean,
+                mean.numpy() > min_mean,
+                mean.numpy() < max_mean,
                 dispersion_norm > min_disp,
                 dispersion_norm < max_disp,
             )
         )
 
     df["highly_variable"] = gene_subset
     return df
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/transforms/divide_by_scale.py` & `cellarium_ml-0.0.5/cellarium/ml/transforms/divide_by_scale.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
+from collections.abc import Sequence
 
 import numpy as np
 import torch
-from numpy.typing import ArrayLike
 from torch import nn
 
 from cellarium.ml.utilities.testing import (
     assert_arrays_equal,
     assert_columns_and_array_lengths_equal,
     assert_nonnegative,
 )
@@ -21,46 +21,47 @@
     .. math::
 
         y_{ng} = \\frac{x_{ng}}{\\mathrm{scale}_g + \\mathrm{eps}}
 
     Args:
         scale_g:
             A scale for each gene.
-        feature_schema:
+        var_names_g:
             The variable names schema for the input data validation.
         eps:
             A value added to the denominator for numerical stability.
     """
 
-    def __init__(self, scale_g: torch.Tensor, feature_schema: ArrayLike, eps: float = 1e-6) -> None:
+    def __init__(self, scale_g: torch.Tensor, var_names_g: Sequence[str], eps: float = 1e-6) -> None:
         super().__init__()
         self.scale_g: torch.Tensor
         self.register_buffer("scale_g", scale_g)
-        self.feature_schema = np.array(feature_schema)
+        self.var_names_g = np.array(var_names_g)
         assert_nonnegative("eps", eps)
         self.eps = eps
 
     def forward(
         self,
         x_ng: torch.Tensor,
-        feature_g: np.ndarray | None = None,
-    ) -> torch.Tensor:
+        var_names_g: np.ndarray,
+    ) -> dict[str, torch.Tensor]:
         """
         Args:
             x_ng:
                 Gene counts.
-            feature_g:
+            var_names_g:
                 The list of the variable names in the input data. If ``None``, no validation is performed.
 
         Returns:
-            Gene counts divided by scale.
+            A dictionary with the following keys:
+
+            - ``x_ng``: The gene counts divided by the scale.
         """
-        if feature_g is not None:
-            assert_columns_and_array_lengths_equal("x_ng", x_ng, "feature_g", feature_g)
-            assert_arrays_equal("feature_g", feature_g, "feature_schema", self.feature_schema)
+        assert_columns_and_array_lengths_equal("x_ng", x_ng, "var_names_g", var_names_g)
+        assert_arrays_equal("var_names_g", var_names_g, "var_names_g", self.var_names_g)
+
+        x_ng = x_ng / (self.scale_g + self.eps)
 
-        return x_ng / (self.scale_g + self.eps)
+        return {"x_ng": x_ng}
 
     def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}(scale_g={self.scale_g}, feature_schema={self.feature_schema}, eps={self.eps})"
-        )
+        return f"{self.__class__.__name__}(scale_g={self.scale_g}, var_names_g={self.var_names_g}, eps={self.eps})"
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/transforms/filter.py` & `cellarium_ml-0.0.5/cellarium/ml/transforms/filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
+from collections.abc import Sequence
 from functools import cache
 from typing import Any
 
 import numpy as np
 import torch
-from numpy.typing import ArrayLike
 from torch import nn
 
 from cellarium.ml.utilities.testing import (
     assert_columns_and_array_lengths_equal,
 )
 
 
@@ -24,45 +24,58 @@
 
         y_{ng} = x_{ng}[:, \\mathrm{mask}_g]
 
     Args:
         filter_list: A list of features to filter by.
     """
 
-    def __init__(self, filter_list: ArrayLike) -> None:
+    def __init__(self, filter_list: Sequence[str]) -> None:
         super().__init__()
         self.filter_list = np.array(filter_list)
         if len(self.filter_list) == 0:
             raise ValueError(f"`filter_list` must not be empty. Got {self.filter_list}")
 
     @cache
-    def filter(self, feature_g: tuple) -> np.ndarray[Any, np.dtype[np.bool_]]:
+    def filter(self, var_names_g: tuple) -> np.ndarray[Any, np.dtype[np.int_]]:
         """
         Args:
-            feature_g: The list of the variable names in the input data.
+            var_names_g: The list of the variable names in the input data.
 
         Returns:
-            A boolean mask of the features to filter by.
+            An array of indices of the features in ``var_names_g`` that are in :attr:`filter_list`.
         """
-        mask = np.isin(feature_g, self.filter_list)
+        mask = np.isin(var_names_g, self.filter_list)
         if not np.any(mask):
-            raise AssertionError("No features in `feature_g` matched the `filter_list`")
-        return mask
+            raise AssertionError("No features in `var_names_g` matched the `filter_list`")
+        mask_indices = np.where(mask)[0]
+        return mask_indices
 
-    def forward(self, x_ng: torch.Tensor, feature_g: np.ndarray) -> torch.Tensor:
+    def forward(self, x_ng: torch.Tensor, var_names_g: np.ndarray) -> dict[str, torch.Tensor | np.ndarray]:
         """
+        .. note::
+
+            When used with :class:`~cellarium.ml.core.CellariumModule` or :class:`~cellarium.ml.core.CellariumPipeline`,
+            ``x_ng`` and ``var_names_g`` keys in the input dictionary will be overwritten with the filtered values.
+
         Args:
             x_ng:
                 Gene counts.
-            feature_g:
+            var_names_g:
                 The list of the variable names in the input data.
 
         Returns:
-            Filtered gene counts.
+            A dictionary with the following keys:
+
+            - ``x_ng``: Gene counts filtered by :attr:`filter_list`.
+            - ``var_names_g``: The list of the variable names in the input data filtered by :attr:`filter_list`.
         """
-        assert_columns_and_array_lengths_equal("x_ng", x_ng, "feature_g", feature_g)
+        assert_columns_and_array_lengths_equal("x_ng", x_ng, "var_names_g", var_names_g)
+
+        filter_indices = self.filter(tuple(var_names_g.tolist()))
+        ndx = torch.arange(x_ng.shape[0])
+        x_ng = x_ng[ndx[:, None], filter_indices]
+        var_names_g = var_names_g[filter_indices]
 
-        filter_mask = self.filter(tuple(feature_g.tolist()))
-        return x_ng[:, filter_mask]
+        return {"x_ng": x_ng, "var_names_g": var_names_g}
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(filter_list={self.filter_list})"
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/transforms/normalize_total.py` & `cellarium_ml-0.0.5/cellarium/ml/transforms/normalize_total.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,24 +39,32 @@
         assert_nonnegative("eps", eps)
         self.eps = eps
 
     def forward(
         self,
         x_ng: torch.Tensor,
         total_mrna_umis_n: torch.Tensor | None = None,
-    ) -> torch.Tensor:
+    ) -> dict[str, torch.Tensor]:
         """
+        .. note::
+
+            When used with :class:`~cellarium.ml.core.CellariumModule` or :class:`~cellarium.ml.core.CellariumPipeline`,
+            ``x_ng`` key in the input dictionary will be overwritten with the normalized values.
+
         Args:
             x_ng:
                 Gene counts.
             total_mrna_umis_n:
                 Total mRNA UMI counts per cell. If ``None``, it is computed from ``x_ng``.
 
         Returns:
-            Gene counts normalized to target count.
+            A dictionary with the following keys:
+
+            - ``x_ng``: The gene counts normalized to target count.
         """
         if total_mrna_umis_n is None:
             total_mrna_umis_n = x_ng.sum(dim=-1)
-        return self.target_count * x_ng / (total_mrna_umis_n[:, None] + self.eps)
+        x_ng = self.target_count * x_ng / (total_mrna_umis_n[:, None] + self.eps)
+        return {"x_ng": x_ng}
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(target_count={self.target_count}, eps={self.eps})"
```

### Comparing `cellarium-ml-0.0.3/cellarium/ml/utilities/data.py` & `cellarium_ml-0.0.5/cellarium/ml/utilities/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,23 +54,16 @@
             If ``None``, :func:`np.asarray` is used.
     """
 
     attr: str
     key: str | None = None
     convert_fn: Callable[[Any], np.ndarray] | None = None
 
-    def __call__(self, adata: AnnData | AnnCollection) -> "AnnDataField":
-        self.adata = adata
-        return self
-
-    def __getitem__(self, idx: int | list[int] | slice) -> np.ndarray:
-        if self.adata is None:
-            raise ValueError("Must call AnnDataField with an AnnData-like object first")
-
-        value = getattr(self.adata[idx], self.attr)
+    def __call__(self, adata: AnnData | AnnCollection, idx: int | list[int] | slice) -> np.ndarray:
+        value = getattr(adata[idx], self.attr)
         if self.key is not None:
             value = value[self.key]
 
         if self.convert_fn is not None:
             value = self.convert_fn(value)
         else:
             value = np.asarray(value)
@@ -98,15 +91,15 @@
     if not dist.is_available():
         num_replicas = 1
         rank = 0
     else:
         try:
             num_replicas = dist.get_world_size()
             rank = dist.get_rank()
-        except RuntimeError:
+        except (ValueError, RuntimeError):  # RuntimeError was changed to ValueError in PyTorch 2.2
             warnings.warn(
                 "Distributed package is available but the default process group has not been initialized. "
                 "Falling back to ``rank=0`` and ``num_replicas=1``.",
                 UserWarning,
             )
             num_replicas = 1
             rank = 0
@@ -146,24 +139,24 @@
     Returns:
         Dictionary with the same keys as the input dictionaries, but with values concatenated along
         the batch dimension.
     """
     keys = batch[0].keys()
     collated_batch = {}
     if len(batch) > 1:
-        assert all(keys == data.keys() for data in batch[1:]), "All dictionaries in the batch must have the same keys."
+        if not all(keys == data.keys() for data in batch[1:]):
+            raise ValueError("All dictionaries in the batch must have the same keys.")
     for key in keys:
-        if key == "obs_names":
+        if key == "obs_names_n":
             collated_batch[key] = np.concatenate([data[key] for data in batch], axis=0)
-        elif key in ["var_names", "feature_g"]:
-            # Check that all var_names are the same
+        elif key == "var_names_g":
+            # Check that all var_names_g are the same
             if len(batch) > 1:
-                assert all(
-                    np.array_equal(batch[0][key], data[key]) for data in batch[1:]
-                ), "All dictionaries in the batch must have the same var_names."
+                if not all(np.array_equal(batch[0][key], data[key]) for data in batch[1:]):
+                    raise ValueError("All dictionaries in the batch must have the same var_names_g.")
             # If so, just take the first one
             collated_batch[key] = batch[0][key]
         else:
             collated_batch[key] = torch.cat([torch.from_numpy(data[key]) for data in batch], dim=0)
     return collated_batch
```

### Comparing `cellarium-ml-0.0.3/cellarium_ml.egg-info/SOURCES.txt` & `cellarium_ml-0.0.5/cellarium_ml.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,54 +7,60 @@
 cellarium/ml/py.typed
 cellarium/ml/callbacks/__init__.py
 cellarium/ml/callbacks/prediction_writer.py
 cellarium/ml/callbacks/variance_monitor.py
 cellarium/ml/core/__init__.py
 cellarium/ml/core/datamodule.py
 cellarium/ml/core/module.py
-cellarium/ml/core/saving.py
+cellarium/ml/core/pipeline.py
 cellarium/ml/data/__init__.py
 cellarium/ml/data/dadc_dataset.py
 cellarium/ml/data/distributed_anndata.py
 cellarium/ml/data/fileio.py
 cellarium/ml/data/schema.py
+cellarium/ml/distributed/__init__.py
+cellarium/ml/distributed/gather.py
+cellarium/ml/distributions/__init__.py
+cellarium/ml/distributions/negative_binomial.py
 cellarium/ml/lr_schedulers/__init__.py
 cellarium/ml/lr_schedulers/linear_lr.py
 cellarium/ml/models/__init__.py
-cellarium/ml/models/from_cli.py
-cellarium/ml/models/gather.py
 cellarium/ml/models/geneformer.py
 cellarium/ml/models/incremental_pca.py
 cellarium/ml/models/logistic_regression.py
 cellarium/ml/models/model.py
+cellarium/ml/models/mu_linear.py
 cellarium/ml/models/onepass_mean_var_std.py
 cellarium/ml/models/probabilistic_pca.py
 cellarium/ml/models/tdigest.py
 cellarium/ml/preprocessing/__init__.py
 cellarium/ml/preprocessing/highly_variable_genes.py
 cellarium/ml/transforms/__init__.py
 cellarium/ml/transforms/divide_by_scale.py
 cellarium/ml/transforms/filter.py
 cellarium/ml/transforms/log1p.py
 cellarium/ml/transforms/normalize_total.py
 cellarium/ml/transforms/z_score.py
 cellarium/ml/utilities/__init__.py
+cellarium/ml/utilities/core.py
 cellarium/ml/utilities/data.py
 cellarium/ml/utilities/testing.py
-cellarium/ml/utilities/types.py
 cellarium_ml.egg-info/PKG-INFO
 cellarium_ml.egg-info/SOURCES.txt
 cellarium_ml.egg-info/dependency_links.txt
 cellarium_ml.egg-info/entry_points.txt
 cellarium_ml.egg-info/requires.txt
 cellarium_ml.egg-info/top_level.txt
 tests/test_cli.py
+tests/test_core.py
 tests/test_dataset.py
 tests/test_distributed_anndata.py
 tests/test_geneformer.py
+tests/test_highly_variable_genes.py
 tests/test_ipca.py
+tests/test_mup.py
 tests/test_onepass_mean_var_std.py
 tests/test_ppca.py
 tests/test_read_h5ad.py
 tests/test_schema.py
 tests/test_tdigest.py
 tests/test_transforms.py
```

### Comparing `cellarium-ml-0.0.3/pyproject.toml` & `cellarium_ml-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,38 +23,37 @@
 dependencies = [
   "anndata",
   "boltons",
   "braceexpand",
   "crick>=0.0.4",
   "google-cloud-storage",
   "jsonargparse[signatures]",
-  "lightning>=2.0.9",
+  "lightning>=2.2.0",
   "pyro-ppl",
-  "torch>=2.0.0",
+  "pytest",
+  "torch>=2.2.0",
   "transformers",
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
-lint = [
-    "black[jupyter]",
-    "ruff",
-]
-mypy = ["mypy"]
+lint = ["ruff"]
+mypy = ["mypy", "types-PyYAML"]
 test = [
-  "pytest",
   "pytest-xdist",
   "tensorboard",
+  "torchvision",
 ]
 docs = [
+  "nbsphinx",
   "Pillow",
+  "seaborn>=0.13.0",
   "sphinx",
   "sphinx_rtd_theme",
-  "sphinx-autodoc-typehints",
   "sphinx-copybutton",
 ]
 dev = ["cellarium-ml[docs,lint,mypy,test]"]
 
 [project.scripts]
 cellarium-ml = "cellarium.ml.cli:main"
 
@@ -72,16 +71,18 @@
 
 [tool.setuptools-git-versioning]
 enabled = true
 dev_template = "{tag}.post{ccount}"
 
 [tool.ruff]
 line-length = 120
-select = ["E", "F", "I", "W"]
+extend-include = ["*.ipynb"]
+target-version = "py310"
 
-[tool.black]
-line-length = 120
+[tool.ruff.lint]
+select = ["E", "F", "I", "W"]
 
 [tool.mypy]
 ignore_missing_imports = true
 explicit_package_bases = true
 check_untyped_defs = true
+warn_unreachable = true
```

### Comparing `cellarium-ml-0.0.3/tests/test_dataset.py` & `cellarium_ml-0.0.5/tests/test_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,48 +12,23 @@
 from anndata import AnnData
 
 from cellarium.ml import CellariumModule
 from cellarium.ml.data import (
     DistributedAnnDataCollection,
     IterableDistributedAnnDataCollectionDataset,
 )
-from cellarium.ml.models import CellariumModel, GatherLayer
-from cellarium.ml.utilities.data import AnnDataField, collate_fn, get_rank_and_num_replicas
+from cellarium.ml.utilities.data import AnnDataField, collate_fn
+from tests.common import BoringModel
 
 # RuntimeError: Too many open files. Communication with the workers is no longer possible.
 # Please increase the limit using `ulimit -n` in the shell or change the sharing strategy
 # by calling `torch.multiprocessing.set_sharing_strategy('file_system')` at the beginning of your code
 torch.multiprocessing.set_sharing_strategy("file_system")
 
 
-class BoringModel(CellariumModel):
-    """
-    This model appends a batch input to an :attr:`iter_data` list at each iteration.
-    Its intended use is for testing purposes where batch inputs can be inspected after
-    iteration over the dataset with ``Trainer.fit()``. Batch input would typically contain
-    feature counts, worker info, torch.distributed info, cache info, etc.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.iter_data: list = []
-        self._dummy_param = torch.nn.Parameter(torch.tensor(0.0))
-
-    @staticmethod
-    def _get_fn_args_from_batch(tensor_dict: dict[str, np.ndarray | torch.Tensor]) -> tuple[tuple, dict]:
-        return (), tensor_dict
-
-    def forward(self, **batch: torch.Tensor) -> None:
-        _, num_replicas = get_rank_and_num_replicas()
-        if num_replicas > 1:
-            for key, value in batch.items():
-                batch[key] = torch.cat(GatherLayer.apply(value), dim=0)
-        self.iter_data.append(batch)
-
-
 @pytest.fixture(params=[[3, 6, 9, 12], [4, 8, 12], [4, 8, 11]])  # limits
 def dadc(tmp_path: Path, request: pytest.FixtureRequest):
     limits = request.param
     n_cell = limits[-1]
     g_gene = 1
 
     X = np.arange(n_cell).reshape(n_cell, g_gene)
@@ -76,15 +51,15 @@
 @pytest.mark.parametrize("shuffle", [False, True], ids=["no shuffle", "shuffle"])
 @pytest.mark.parametrize("num_workers", [0, 1, 2], ids=["zero workers", "one worker", "two workers"])
 @pytest.mark.parametrize("batch_size", [1, 2, 3], ids=["batch size 1", "batch size 2", "batch size 3"])
 def test_iterable_dataset(dadc: DistributedAnnDataCollection, shuffle: bool, num_workers: int, batch_size: int):
     n_obs = len(dadc)
     dataset = IterableDistributedAnnDataCollectionDataset(
         dadc,
-        batch_keys={"X": AnnDataField("X")},
+        batch_keys={"x_ng": AnnDataField("X")},
         batch_size=batch_size,
         shuffle=shuffle,
         test_mode=True,
     )
     data_loader = torch.utils.data.DataLoader(
         dataset,
         num_workers=num_workers,
@@ -98,15 +73,15 @@
         for worker in range(num_workers):
             miss_count = max(c for c, w in zip(miss_counts, worker_ids) if w == worker)
             assert miss_count == math.ceil(len(dadc.limits) / num_workers)
     else:
         miss_count = max(miss_counts)
         assert miss_count == len(dadc.limits)
 
-    actual_idx = list(int(i) for batch in data_loader for i in batch["X"])
+    actual_idx = list(int(i) for batch in data_loader for i in batch["x_ng"])
     expected_idx = list(range(n_obs))
 
     # assert entire dataset is sampled
     assert len(expected_idx) == len(actual_idx)
     assert set(expected_idx) == set(actual_idx)
 
 
@@ -121,42 +96,42 @@
     batch_size: int,
     drop_last: bool,
 ):
     devices = int(os.environ.get("TEST_DEVICES", "1"))
     n_obs = len(dadc)
     dataset = IterableDistributedAnnDataCollectionDataset(
         dadc,
-        batch_keys={"X": AnnDataField("X")},
+        batch_keys={"x_ng": AnnDataField("X")},
         batch_size=batch_size,
         shuffle=shuffle,
         drop_last=drop_last,
         test_mode=True,
     )
     data_loader = torch.utils.data.DataLoader(
         dataset,
         num_workers=num_workers,
         collate_fn=collate_fn,
     )
 
     # fit
     model = BoringModel()
-    module = CellariumModule(model)
+    module = CellariumModule(model=model)
     trainer = pl.Trainer(
         barebones=True,
         accelerator="cpu",
         devices=devices,
         max_epochs=1,  # one pass
     )
     trainer.fit(module, data_loader)
 
     # run tests only for rank 0
     if trainer.global_rank != 0:
         return
 
-    actual_idx = list(int(i) for batch in model.iter_data for i in batch["X"])
+    actual_idx = list(int(i) for batch in model.iter_data for i in batch["x_ng"])
     expected_idx = list(range(n_obs))
 
     # assert entire dataset is sampled
     if drop_last and n_obs % devices != 0:
         expected_len = (n_obs // devices) * devices
         assert expected_len == len(actual_idx)
         assert set(actual_idx).issubset(expected_idx)
@@ -183,29 +158,29 @@
     num_workers: int,
     persistent_workers: bool,
     epochs: int,
 ):
     devices = int(os.environ.get("TEST_DEVICES", "1"))
     dataset = IterableDistributedAnnDataCollectionDataset(
         dadc,
-        batch_keys={"X": AnnDataField("X")},
+        batch_keys={"x_ng": AnnDataField("X")},
         batch_size=1,
         shuffle=True,
         test_mode=True,
     )
     data_loader = torch.utils.data.DataLoader(
         dataset,
         num_workers=num_workers,
         collate_fn=collate_fn,
         persistent_workers=persistent_workers,
     )
 
     # fit
     model = BoringModel()
-    module = CellariumModule(model)
+    module = CellariumModule(model=model)
     trainer = pl.Trainer(
         barebones=True,
         accelerator="cpu",
         devices=devices,
         max_epochs=epochs,
         strategy="ddp",
     )
```

### Comparing `cellarium-ml-0.0.3/tests/test_distributed_anndata.py` & `cellarium_ml-0.0.5/tests/test_distributed_anndata.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from anndata import AnnData
 
 from cellarium.ml.data import (
     DistributedAnnDataCollection,
     IterableDistributedAnnDataCollectionDataset,
     read_h5ad_file,
 )
-from cellarium.ml.utilities.data import AnnDataField
+from cellarium.ml.utilities.data import AnnDataField, categories_to_codes
 
 
 @pytest.fixture
 def adatas_path(tmp_path: Path):
     n_cell, n_gene = (10, 5)
     # adata0.n_obs == 2, adata1.n_obs == 3, adata2.n_obs == 5
     limits = [2, 5, 10]
@@ -32,14 +32,18 @@
     M = rng.normal(size=(n_cell, 2))
     V = rng.normal(size=(n_gene, 2))
     P = rng.normal(size=(n_gene, n_gene))
     obs = pd.DataFrame(
         {
             "A": rng.integers(0, 2, n_cell),
             "B": rng.integers(0, 2, n_cell),
+            "C": pd.Categorical(
+                np.array(["e", "f"])[np.random.randint(0, 2, n_cell)],
+                categories=["e", "f"],
+            ),
         },
         index=[f"ref_cell{i:03d}" for i in range(n_cell)],
     )
     var = pd.DataFrame(
         {
             "D": np.zeros(n_gene),
             "E": np.ones(n_gene),
@@ -56,14 +60,15 @@
         obsm={"M": M},
         varm={"V": V},
         varp={"P": P},
     )
     adata.write(os.path.join(tmp_path, "adata.h5ad"))
     for i, limit in enumerate(zip([0] + limits, limits)):
         sliced_adata = adata[slice(*limit)]
+        sliced_adata.obs["C"] = sliced_adata.obs["C"].cat.set_categories(adata.obs["C"].cat.categories)
         sliced_adata.write(os.path.join(tmp_path, f"adata.00{i}.h5ad"))
     return tmp_path
 
 
 @pytest.fixture
 def adt(adatas_path: Path):
     # single anndata
@@ -137,40 +142,43 @@
 ):
     # compare indexing single and distributed anndata
     max_cache_size = dat.max_cache_size
     cache_size_strictly_enforced = dat.cache_size_strictly_enforced
     oidx, n_adatas = row_select
 
     if cache_size_strictly_enforced and (n_adatas > max_cache_size):
-        with pytest.raises(AssertionError, match="Expected the number of anndata files"):
+        with pytest.raises(ValueError, match="Expected the number of anndata files"):
             dat_view = dat[oidx, vidx]
     else:
         adt_view = adt[oidx, vidx]
         dat_view = dat[oidx, vidx]
+        adt_view.obs["C"] = adt_view.obs["C"].cat.set_categories(adt.obs["C"].cat.categories)
         np.testing.assert_array_equal(adt_view.X, dat_view.X)
         np.testing.assert_array_equal(adt_view.var_names, dat_view.var_names)
         np.testing.assert_array_equal(adt_view.obs_names, dat_view.obs_names)
         np.testing.assert_array_equal(adt_view.layers["L"], dat_view.layers["L"])
         np.testing.assert_array_equal(adt_view.obsm["M"], dat_view.obsm["M"])
-        np.testing.assert_array_equal(adt_view.obs["A"], dat_view.obs["A"])
+        assert adt_view.obs["A"].equals(dat_view.obs["A"])
+        assert adt_view.obs["C"].equals(dat_view.obs["C"])
 
 
 def test_pickle(dat: DistributedAnnDataCollection):
-    new_dat = pickle.loads(pickle.dumps(dat))
+    new_dat: DistributedAnnDataCollection = pickle.loads(pickle.dumps(dat))
 
-    assert len(new_dat.cache) == 0
+    assert len(new_dat.cache) == 1
 
     new_dat_view, dat_view = new_dat[:2], dat[:2]
 
     np.testing.assert_array_equal(new_dat_view.X, dat_view.X)
     np.testing.assert_array_equal(new_dat_view.var_names, dat_view.var_names)
     np.testing.assert_array_equal(new_dat_view.obs_names, dat_view.obs_names)
     np.testing.assert_array_equal(new_dat_view.layers["L"], dat_view.layers["L"])
     np.testing.assert_array_equal(new_dat_view.obsm["M"], dat_view.obsm["M"])
-    np.testing.assert_array_equal(new_dat_view.obs["A"], dat_view.obs["A"])
+    assert new_dat_view.obs["A"].equals(dat_view.obs["A"])
+    assert new_dat_view.obs["C"].equals(dat_view.obs["C"])
 
 
 @pytest.mark.parametrize(
     "row_select",
     [(slice(0, 2), 1), (slice(1, 4), 2), ([1, 2, 4, 4], 2), ([6, 1, 3], 3)],
     ids=["one adata", "two adatas", "sorted two adatas", "unsorted three adatas"],
 )
@@ -183,45 +191,45 @@
     max_cache_size = dat.max_cache_size
     cache_size_strictly_enforced = dat.cache_size_strictly_enforced
     oidx, n_adatas = row_select
 
     dataset = IterableDistributedAnnDataCollectionDataset(
         dat,
         batch_keys={
-            "X": AnnDataField("X"),
+            "x_ng": AnnDataField("X"),
             "obs_names": AnnDataField("obs_names"),
         },
     )
 
     if cache_size_strictly_enforced and (n_adatas > max_cache_size):
-        with pytest.raises(AssertionError, match="Expected the number of anndata files"):
-            dataset_X = dataset[oidx]["X"]
+        with pytest.raises(ValueError, match="Expected the number of anndata files"):
+            dataset_X = dataset[oidx]["x_ng"]
     else:
         adt_X = adt[oidx].X
-        dataset_X = dataset[oidx]["X"]
+        dataset_X = dataset[oidx]["x_ng"]
         np.testing.assert_array_equal(adt_X, dataset_X)
 
         adt_obs_names = adt[oidx].obs_names
         dataset_obs_names = dataset[oidx]["obs_names"]
         np.testing.assert_array_equal(adt_obs_names, dataset_obs_names)
 
 
 def test_pickle_dataset(dat: DistributedAnnDataCollection):
     dataset = IterableDistributedAnnDataCollectionDataset(
         dat,
         batch_keys={
-            "X": AnnDataField("X"),
+            "x_ng": AnnDataField("X"),
             "obs_names": AnnDataField("obs_names"),
         },
     )
     new_dataset = pickle.loads(pickle.dumps(dataset))
 
-    assert len(new_dataset.dadc.cache) == 0
+    assert len(new_dataset.dadc.cache) == 1
 
-    np.testing.assert_array_equal(new_dataset[:2]["X"], dataset[:2]["X"])
+    np.testing.assert_array_equal(new_dataset[:2]["x_ng"], dataset[:2]["x_ng"])
     np.testing.assert_array_equal(new_dataset[:2]["obs_names"], dataset[:2]["obs_names"])
 
 
 @pytest.fixture
 def dadc(adatas_path: Path):
     # distributed anndata
     filenames = str(os.path.join(adatas_path, "adata.{000..002}.h5ad"))
@@ -235,14 +243,15 @@
 
 
 @pytest.mark.parametrize(
     "attr,key,convert_fn",
     [
         ("X", None, None),
         ("obs", "A", None),
+        ("obs", "C", categories_to_codes),
         ("obs_names", None, None),
         ("var_names", None, None),
         ("layers", "L", None),
     ],
 )
 @pytest.mark.parametrize("idx", [slice(0, 5), [0, 2, 4], 0])
 def test_anndata_field(
@@ -255,10 +264,10 @@
     expected = getattr(dadc[idx], attr)
     if key is not None:
         expected = expected[key]
     if convert_fn is not None:
         expected = convert_fn(expected)
 
     field = AnnDataField(attr, key, convert_fn)
-    actual = field(dadc)[idx]
+    actual = field(dadc, idx)
 
     np.testing.assert_array_equal(expected, actual)
```

### Comparing `cellarium-ml-0.0.3/tests/test_ipca.py` & `cellarium_ml-0.0.5/tests/test_ipca.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 import lightning.pytorch as pl
 import numpy as np
 import pytest
 import torch
 from lightning.pytorch.strategies import DDPStrategy
 
 from cellarium.ml import CellariumModule
-from cellarium.ml.models import IncrementalPCA, IncrementalPCAFromCLI
-from cellarium.ml.transforms import NormalizeTotal
+from cellarium.ml.models import IncrementalPCA
 from cellarium.ml.utilities.data import collate_fn
 from tests.common import BoringDataset
 
 
 @pytest.fixture
 def x_ng():
     n, g = 10000, 100
@@ -35,26 +34,29 @@
     n, g = x_ng.shape
     x_ng_centered = x_ng - x_ng.mean(dim=0)
     devices = int(os.environ.get("TEST_DEVICES", "1"))
     batch_size = batch_size // devices
 
     # dataloader
     train_loader = torch.utils.data.DataLoader(
-        BoringDataset((x_ng if perform_mean_correction else x_ng_centered).numpy()),
+        BoringDataset(
+            (x_ng if perform_mean_correction else x_ng_centered).numpy(),
+            np.array([f"gene_{i}" for i in range(g)]),
+        ),
         batch_size=batch_size,
         shuffle=False,
         collate_fn=collate_fn,
     )
     # model
     ipca = IncrementalPCA(
-        g_genes=g,
-        k_components=k,
+        var_names_g=[f"gene_{i}" for i in range(g)],
+        n_components=k,
         perform_mean_correction=perform_mean_correction,
     )
-    module = CellariumModule(ipca)
+    module = CellariumModule(model=ipca)
     # trainer
     strategy = DDPStrategy(broadcast_buffers=False) if devices > 1 else "auto"
     trainer = pl.Trainer(
         barebones=True,
         accelerator="cpu",
         devices=devices,
         max_epochs=1,
@@ -82,32 +84,31 @@
         (x_ng if perform_mean_correction else x_ng_centered).mean(dim=0),
         atol=1e-5,
     )
 
 
 def test_load_from_checkpoint_multi_device(tmp_path: Path):
     n, g = 3, 2
+    var_names_g = [f"gene_{i}" for i in range(g)]
     devices = int(os.environ.get("TEST_DEVICES", "1"))
     # dataloader
     train_loader = torch.utils.data.DataLoader(
-        BoringDataset(np.arange(n * g).reshape(n, g)),
+        BoringDataset(
+            np.random.randn(n, g),
+            np.array(var_names_g),
+        ),
         collate_fn=collate_fn,
     )
     # model
-    init_args = {"g_genes": g, "k_components": 1, "perform_mean_correction": True, "target_count": 10}
-    model = IncrementalPCAFromCLI(**init_args)  # type: ignore[arg-type]
-    config = {
-        "model": {
-            "model": {
-                "class_path": "cellarium.ml.models.IncrementalPCAFromCLI",
-                "init_args": init_args,
-            }
-        }
-    }
-    module = CellariumModule(model, config=config)
+    model = IncrementalPCA(
+        var_names_g=var_names_g,
+        n_components=1,
+        perform_mean_correction=True,
+    )
+    module = CellariumModule(model=model)
     # trainer
     strategy = DDPStrategy(broadcast_buffers=False) if devices > 1 else "auto"
     trainer = pl.Trainer(
         accelerator="cpu",
         strategy=strategy,  # type: ignore[arg-type]
         devices=devices,
         max_epochs=1,
@@ -119,18 +120,13 @@
     # run tests only for rank 0
     if trainer.global_rank != 0:
         return
 
     # load model from checkpoint
     ckpt_path = tmp_path / f"lightning_logs/version_0/checkpoints/epoch=0-step={math.ceil(n / devices)}.ckpt"
     assert ckpt_path.is_file()
-    loaded_model: IncrementalPCAFromCLI = CellariumModule.load_from_checkpoint(ckpt_path).model
+    loaded_model: IncrementalPCA = CellariumModule.load_from_checkpoint(ckpt_path).model
     # assert
-    assert isinstance(model.transform, torch.nn.Sequential) and len(model.transform) == 2
-    assert isinstance(loaded_model.transform, torch.nn.Sequential) and len(loaded_model.transform) == 2
-    assert isinstance(model.transform[0], NormalizeTotal)
-    assert isinstance(loaded_model.transform[0], NormalizeTotal)
-    assert model.transform[0].target_count == loaded_model.transform[0].target_count
     np.testing.assert_allclose(model.V_kg.detach(), loaded_model.V_kg.detach())
     np.testing.assert_allclose(model.S_k.detach(), loaded_model.S_k.detach())
     np.testing.assert_allclose(model.x_size.detach(), loaded_model.x_size.detach())
     np.testing.assert_allclose(model.x_mean_g.detach(), loaded_model.x_mean_g.detach())
```

### Comparing `cellarium-ml-0.0.3/tests/test_onepass_mean_var_std.py` & `cellarium_ml-0.0.5/tests/test_tdigest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
 import math
 import os
+import shutil
 from pathlib import Path
 
 import lightning.pytorch as pl
 import numpy as np
 import pytest
 import torch
 from anndata import AnnData
-from lightning.pytorch.strategies import DDPStrategy
 
 from cellarium.ml import CellariumModule
-from cellarium.ml.data import DistributedAnnDataCollection, IterableDistributedAnnDataCollectionDataset
-from cellarium.ml.models import OnePassMeanVarStd, OnePassMeanVarStdFromCLI
-from cellarium.ml.transforms import Log1p, NormalizeTotal
+from cellarium.ml.data import (
+    DistributedAnnDataCollection,
+    IterableDistributedAnnDataCollectionDataset,
+)
+from cellarium.ml.models import TDigest
+from cellarium.ml.transforms import NormalizeTotal
 from cellarium.ml.utilities.data import AnnDataField, collate_fn
 from tests.common import BoringDataset
 
 
 @pytest.fixture
 def adata():
-    n_cell, g_gene = 10, 5
+    n_cell, g_gene = 1000, 5
     rng = np.random.default_rng(1465)
-    X = rng.integers(10, size=(n_cell, g_gene))
+    X = rng.integers(100, size=(n_cell, g_gene))
     return AnnData(X, dtype=X.dtype)
 
 
 @pytest.fixture
 def dadc(adata: AnnData, tmp_path: Path):
     # save anndata files
-    limits = [2, 5, 10]
+    limits = [200, 500, 1000]
     for i, limit in enumerate(zip([0] + limits, limits)):
         sliced_adata = adata[slice(*limit)]
         sliced_adata.write(os.path.join(tmp_path, f"adata.00{i}.h5ad"))
 
     # distributed anndata
     filenames = str(os.path.join(tmp_path, "adata.{000..002}.h5ad"))
     return DistributedAnnDataCollection(
@@ -44,112 +47,110 @@
         max_cache_size=2,  # allow max_cache_size=2 for IterableDistributedAnnDataCollectionDataset
         cache_size_strictly_enforced=True,
     )
 
 
 @pytest.mark.parametrize("shuffle", [False, True])
 @pytest.mark.parametrize("num_workers", [0, 2])
-@pytest.mark.parametrize("batch_size", [1, 2, 3])
-def test_onepass_mean_var_std_multi_device(
+@pytest.mark.parametrize("batch_size", [10, 100])
+@pytest.mark.parametrize(
+    "transforms",
+    [[NormalizeTotal(target_count=10_000, eps=0)], []],
+)
+def test_tdigest_multi_device(
     adata: AnnData,
     dadc: DistributedAnnDataCollection,
     shuffle: bool,
     num_workers: int,
     batch_size: int,
+    transforms: list[torch.nn.Module],
 ):
     devices = int(os.environ.get("TEST_DEVICES", "1"))
+    batch_size = batch_size // devices
+
     # prepare dataloader
     dataset = IterableDistributedAnnDataCollectionDataset(
         dadc,
-        batch_keys={"X": AnnDataField("X")},
+        batch_keys={
+            "x_ng": AnnDataField("X"),
+            "var_names_g": AnnDataField("var_names"),
+        },
         batch_size=batch_size,
         shuffle=shuffle,
     )
     data_loader = torch.utils.data.DataLoader(
         dataset,
         num_workers=num_workers,
         collate_fn=collate_fn,
     )
-    transform = torch.nn.Sequential(NormalizeTotal(target_count=10_000), Log1p())
 
     # fit
-    model = OnePassMeanVarStd(g_genes=dadc.n_vars, transform=transform)
-    module = CellariumModule(model)
-    strategy = DDPStrategy(broadcast_buffers=False) if devices > 1 else "auto"
+    model = TDigest(var_names_g=dadc.var_names)
+    module = CellariumModule(transforms=transforms, model=model)
     trainer = pl.Trainer(
         barebones=True,
         accelerator="cpu",
         devices=devices,
         max_epochs=1,  # one pass
-        strategy=strategy,  # type: ignore[arg-type]
     )
     trainer.fit(module, train_dataloaders=data_loader)
 
     # run tests only for rank 0
     if trainer.global_rank != 0:
         return
 
-    # actual mean, var, and std
-    actual_mean = model.mean_g
-    actual_var = model.var_g
-    actual_std = model.std_g
-
-    # expected mean, var, and std
-    x = transform(torch.from_numpy(adata.X))
-    expected_mean = torch.mean(x, dim=0)
-    expected_var = torch.var(x, dim=0, unbiased=False)
-    expected_std = torch.std(x, dim=0, unbiased=False)
-
-    np.testing.assert_allclose(expected_mean, actual_mean, atol=1e-5)
-    np.testing.assert_allclose(expected_var, actual_var, atol=1e-4)
-    np.testing.assert_allclose(expected_std, actual_std, atol=1e-4)
-
+    # actual median
+    actual_median_g = model.median_g
 
-def test_load_from_checkpoint_multi_device(tmp_path: Path):
-    n, g = 3, 2
+    # expected median
+    batch = {"x_ng": torch.from_numpy(adata.X)}
+    for transform in transforms:
+        batch = transform(**batch)
+    x = batch["x_ng"]
+    for i in range(x.shape[1]):
+        mask = torch.nonzero(x[:, i])
+        expected_median = torch.median(x[mask, i])
+        actual_median = actual_median_g[i]
+        # assert within 1% accuracy
+        np.testing.assert_allclose(expected_median, actual_median, rtol=0.01)
+
+
+def test_load_from_checkpoint_multi_device():
+    # using pytest tmp_path fixture creates a directory per rank
+    # so we need to use a fixed shared directory
+    tmp_path = Path("/tmp/test_load_from_checkpoint_multi_device")
+    n, g = 4, 3
+    var_names_g = [f"gene_{i}" for i in range(g)]
     devices = int(os.environ.get("TEST_DEVICES", "1"))
     # dataloader
     train_loader = torch.utils.data.DataLoader(
-        BoringDataset(np.arange(n * g).reshape(n, g)),
+        BoringDataset(
+            np.random.randn(n, g),
+            np.array(var_names_g),
+        ),
         collate_fn=collate_fn,
     )
     # model
-    init_args = {"g_genes": g, "target_count": 10}
-    model = OnePassMeanVarStdFromCLI(**init_args)
-    config = {
-        "model": {
-            "model": {
-                "class_path": "cellarium.ml.models.OnePassMeanVarStdFromCLI",
-                "init_args": init_args,
-            }
-        }
-    }
-    module = CellariumModule(model, config=config)
+    model = TDigest(var_names_g=var_names_g)
+    module = CellariumModule(model=model)
     # trainer
-    strategy = DDPStrategy(broadcast_buffers=False) if devices > 1 else "auto"
     trainer = pl.Trainer(
         accelerator="cpu",
-        strategy=strategy,  # type: ignore[arg-type]
         devices=devices,
         max_epochs=1,
         default_root_dir=tmp_path,
     )
     # fit
     trainer.fit(module, train_dataloaders=train_loader)
 
     # run tests only for rank 0
     if trainer.global_rank != 0:
         return
 
     # load model from checkpoint
     ckpt_path = tmp_path / f"lightning_logs/version_0/checkpoints/epoch=0-step={math.ceil(n / devices)}.ckpt"
     assert ckpt_path.is_file()
-    loaded_model: OnePassMeanVarStdFromCLI = CellariumModule.load_from_checkpoint(ckpt_path).model
+    loaded_model: TDigest = CellariumModule.load_from_checkpoint(ckpt_path).model
     # assert
-    assert isinstance(model.transform, torch.nn.Sequential) and len(model.transform) == 2
-    assert isinstance(loaded_model.transform, torch.nn.Sequential) and len(loaded_model.transform) == 2
-    assert isinstance(model.transform[0], NormalizeTotal)
-    assert isinstance(loaded_model.transform[0], NormalizeTotal)
-    assert model.transform[0].target_count == loaded_model.transform[0].target_count
-    np.testing.assert_allclose(model.mean_g, loaded_model.mean_g)
-    np.testing.assert_allclose(model.var_g, loaded_model.var_g)
-    np.testing.assert_allclose(model.std_g, loaded_model.std_g)
+    np.testing.assert_allclose(model.median_g, loaded_model.median_g)
+
+    shutil.rmtree(tmp_path)
```

### Comparing `cellarium-ml-0.0.3/tests/test_ppca.py` & `cellarium_ml-0.0.5/tests/test_ppca.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
 import math
 import os
 from pathlib import Path
+from typing import Literal
 
 import lightning.pytorch as pl
 import numpy as np
 import pyro
 import pytest
 import torch
 
 from cellarium.ml import CellariumModule
 from cellarium.ml.callbacks import VarianceMonitor
-from cellarium.ml.models import ProbabilisticPCA, ProbabilisticPCAFromCLI
-from cellarium.ml.transforms import NormalizeTotal
+from cellarium.ml.models import ProbabilisticPCA
 from cellarium.ml.utilities.data import collate_fn
 from tests.common import BoringDataset
 
 
 @pytest.fixture
 def x_ng():
     n, g, k = 1000, 10, 3
@@ -30,47 +30,52 @@
     x_ng = z_nk @ w_kg + noise
     return x_ng
 
 
 @pytest.mark.parametrize("ppca_flavor", ["marginalized", "linear_vae"])
 @pytest.mark.parametrize("learn_mean", [False, True])
 @pytest.mark.parametrize("minibatch", [False, True], ids=["fullbatch", "minibatch"])
-def test_probabilistic_pca_multi_device(x_ng: np.ndarray, minibatch: bool, ppca_flavor: str, learn_mean: bool):
+def test_probabilistic_pca_multi_device(
+    x_ng: np.ndarray, minibatch: bool, ppca_flavor: Literal["marginalized", "linear_vae"], learn_mean: bool
+):
     n, g = x_ng.shape
     k = 3
     devices = int(os.environ.get("TEST_DEVICES", "1"))
     if learn_mean:
         x_mean_g = None
     else:
         x_mean_g = torch.as_tensor(x_ng.mean(axis=0))
 
     # dataloader
     batch_size = n // 2 if minibatch else n
     train_loader = torch.utils.data.DataLoader(
-        BoringDataset(x_ng),
+        BoringDataset(
+            x_ng,
+            np.array([f"gene_{i}" for i in range(g)]),
+        ),
         batch_size=batch_size,
         shuffle=False,
         collate_fn=collate_fn,
     )
     # model
     pyro.clear_param_store()
     total_var = np.var(x_ng, axis=0).sum()
     w = np.sqrt(0.5 * total_var / (g * k))
     s = np.sqrt(0.5 * total_var / g)
     ppca = ProbabilisticPCA(
-        n_cells=n,
-        g_genes=g,
-        k_components=k,
+        n_obs=n,
+        var_names_g=[f"gene_{i}" for i in range(g)],
+        n_components=k,
         ppca_flavor=ppca_flavor,
         mean_g=x_mean_g,
         W_init_scale=w,
         sigma_init_scale=s,
     )
     module = CellariumModule(
-        ppca,
+        model=ppca,
         optim_fn=torch.optim.Adam,
         optim_kwargs={"lr": 3e-2},
         scheduler_fn=torch.optim.lr_scheduler.CosineAnnealingLR,
         scheduler_kwargs={"T_max": 1000},  # one cycle
     )
     # trainer
     trainer = pl.Trainer(
@@ -88,15 +93,15 @@
     L_g, U_gg = np.linalg.eig(x_cov_gg)
 
     # total variance
     expected_total_var = np.var(x_ng, axis=0).sum()
     actual_total_var = ppca.W_variance + ppca.sigma_variance
     np.testing.assert_allclose(expected_total_var, actual_total_var, rtol=1e-3)
 
-    # variance explained be each PC
+    # variance explained by each PC
     expected_explained_var = L_g[:k]
     actual_explained_var = ppca.L_k
     np.testing.assert_allclose(expected_explained_var, actual_explained_var, rtol=1e-3)
 
     # absolute cosine similarity between expected and actual PCs
     abs_cos_sim = torch.abs(
         torch.nn.functional.cosine_similarity(
@@ -107,23 +112,27 @@
     )
     np.testing.assert_allclose(np.ones(k), abs_cos_sim, rtol=1e-3)
 
 
 def test_variance_monitor(x_ng: np.ndarray):
     n, g = x_ng.shape
     k = 3
+    var_names_g = [f"gene_{i}" for i in range(g)]
     # dataloader
     train_loader = torch.utils.data.DataLoader(
-        BoringDataset(x_ng),
+        BoringDataset(
+            x_ng,
+            np.array(var_names_g),
+        ),
         batch_size=n // 2,
         collate_fn=collate_fn,
     )
     # model
-    ppca = ProbabilisticPCA(n, g, k, "marginalized")
-    module = CellariumModule(ppca)
+    ppca = ProbabilisticPCA(n, var_names_g, k, "marginalized")
+    module = CellariumModule(model=ppca, optim_fn=torch.optim.Adam)
     # trainer
     var_monitor = VarianceMonitor(total_variance=np.var(x_ng, axis=0).sum())
     trainer = pl.Trainer(
         accelerator="cpu",
         devices=1,
         max_steps=2,
         callbacks=[var_monitor],
@@ -131,38 +140,33 @@
     )
     # fit
     trainer.fit(module, train_dataloaders=train_loader)
 
 
 def test_load_from_checkpoint_multi_device(tmp_path: Path):
     n, g = 3, 2
+    var_names_g = [f"gene_{i}" for i in range(g)]
     devices = int(os.environ.get("TEST_DEVICES", "1"))
     # dataloader
     train_loader = torch.utils.data.DataLoader(
-        BoringDataset(np.arange(n * g).reshape(n, g)),
+        BoringDataset(
+            np.random.randn(n, g).astype(np.float32),
+            np.array(var_names_g),
+        ),
         collate_fn=collate_fn,
     )
     # model
-    init_args = {
-        "n_cells": n,
-        "g_genes": g,
-        "k_components": 1,
-        "ppca_flavor": "marginalized",
-        "target_count": 10,
-    }
-    model = ProbabilisticPCAFromCLI(**init_args)  # type: ignore[arg-type]
-    config = {
-        "model": {
-            "model": {
-                "class_path": "cellarium.ml.models.ProbabilisticPCAFromCLI",
-                "init_args": init_args,
-            }
-        }
-    }
-    module = CellariumModule(model, config=config)
+    pyro.clear_param_store()
+    model = ProbabilisticPCA(
+        n_obs=n,
+        var_names_g=var_names_g,
+        n_components=1,
+        ppca_flavor="marginalized",
+    )
+    module = CellariumModule(model=model, optim_fn=torch.optim.Adam)
     # trainer
     trainer = pl.Trainer(
         accelerator="cpu",
         devices=devices,
         max_epochs=1,
         default_root_dir=tmp_path,
     )
@@ -172,17 +176,12 @@
     # run tests only for rank 0
     if trainer.global_rank != 0:
         return
 
     # load model from checkpoint
     ckpt_path = tmp_path / f"lightning_logs/version_0/checkpoints/epoch=0-step={math.ceil(n / devices)}.ckpt"
     assert ckpt_path.is_file()
-    loaded_model: ProbabilisticPCAFromCLI = CellariumModule.load_from_checkpoint(ckpt_path).model
+    loaded_model: ProbabilisticPCA = CellariumModule.load_from_checkpoint(ckpt_path).model
     # assert
-    assert isinstance(model.transform, torch.nn.Sequential) and len(model.transform) == 2
-    assert isinstance(loaded_model.transform, torch.nn.Sequential) and len(loaded_model.transform) == 2
-    assert isinstance(model.transform[0], NormalizeTotal)
-    assert isinstance(loaded_model.transform[0], NormalizeTotal)
-    assert model.transform[0].target_count == loaded_model.transform[0].target_count
     np.testing.assert_allclose(model.W_kg.detach(), loaded_model.W_kg.detach())
-    np.testing.assert_allclose(model.sigma.detach(), loaded_model.sigma.detach())
+    np.testing.assert_allclose(model.sigma.detach(), loaded_model.sigma.detach())  # type: ignore[attr-defined]
     np.testing.assert_allclose(model.mean_g.detach(), loaded_model.mean_g.detach())
```

### Comparing `cellarium-ml-0.0.3/tests/test_schema.py` & `cellarium_ml-0.0.5/tests/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     if change_obs_categories:
         adata.obs["C"] = pd.Categorical(
             np.array(["g", "h"])[np.random.randint(0, 2, n_cell)],
             categories=["g", "h"],
         )
 
     if subset_obs_columns:
-        schema = AnnDataSchema(ref_adata, obs_columns=["A", "B"])
+        schema = AnnDataSchema(ref_adata, obs_columns_to_validate=["A", "B"])
     else:
         schema = AnnDataSchema(ref_adata)
 
     if change_obs_categories and not subset_obs_columns:
         with pytest.raises(ValueError, match=".obs attribute dtypes for anndata passed in"):
             schema.validate_anndata(adata)
     else:
```

### Comparing `cellarium-ml-0.0.3/tests/test_transforms.py` & `cellarium_ml-0.0.5/tests/test_transforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
 import numpy as np
 import pytest
 import torch
 
+from cellarium.ml import CellariumPipeline
 from cellarium.ml.transforms import Filter, Log1p, NormalizeTotal, ZScore
 
 n, g, target_count = 100, 3, 10_000
 
 
 @pytest.fixture
 def x_ng():
@@ -21,58 +22,64 @@
 
 @pytest.fixture
 def log_normalize(x_ng: torch.Tensor):
     l_n1 = x_ng.sum(dim=-1, keepdim=True)
     y_ng = torch.log1p(target_count * x_ng / l_n1)
     mean_g = y_ng.mean(dim=0)
     std_g = y_ng.std(dim=0)
-    feature_schema = [f"gene_{i}" for i in range(g)]
-    transform = torch.nn.Sequential(
-        NormalizeTotal(target_count),
-        Log1p(),
-        ZScore(mean_g, std_g, feature_schema),
+    var_names_g = [f"gene_{i}" for i in range(g)]
+    transform = CellariumPipeline(
+        [
+            NormalizeTotal(target_count),
+            Log1p(),
+            ZScore(mean_g, std_g, var_names_g),
+        ]
     )
     return transform
 
 
-def test_log_normalize_shape(x_ng: torch.Tensor, log_normalize: torch.nn.Sequential):
-    new_x_ng = log_normalize(x_ng)
+def test_log_normalize_shape(x_ng: torch.Tensor, log_normalize: CellariumPipeline):
+    var_names_g = np.array([f"gene_{i}" for i in range(g)])
+    batch = {"x_ng": x_ng, "var_names_g": var_names_g}
+    new_x_ng = log_normalize(batch)["x_ng"]
     assert x_ng.shape == new_x_ng.shape
 
 
-def test_log_normalize_mean_std(x_ng: torch.Tensor, log_normalize: torch.nn.Sequential):
-    new_x_ng = log_normalize(x_ng)
+def test_log_normalize_mean_std(x_ng: torch.Tensor, log_normalize: CellariumPipeline):
+    var_names_g = np.array([f"gene_{i}" for i in range(g)])
+    batch = {"x_ng": x_ng, "var_names_g": var_names_g}
+    new_x_ng = log_normalize(batch)["x_ng"]
 
     actual_mean = new_x_ng.mean(dim=0)
     actual_std = new_x_ng.std(dim=0)
 
     np.testing.assert_allclose(0, actual_mean, atol=1e-5)
     np.testing.assert_allclose(1, actual_std, atol=1e-5)
 
 
 @pytest.mark.parametrize(
     "filter_list",
     [["gene_0"], ["gene_0", "gene_1"], ["gene_0", "gene_2"]],
 )
 def test_filter(x_ng: torch.Tensor, filter_list: list[str]):
     transform = Filter(filter_list)
-    feature_g = np.array([f"gene_{i}" for i in range(g)])
-    new_x_ng = transform(x_ng, feature_g)
+    var_names_g = np.array([f"gene_{i}" for i in range(g)])
+    new_x_ng = transform(x_ng, var_names_g)["x_ng"]
     assert new_x_ng.shape[1] == len(filter_list)
     assert new_x_ng.shape[0] == x_ng.shape[0]
 
 
 def test_filter_cache():
     filter_list = ["gene_0", "gene_1"]
     transform = Filter(filter_list)
     transform.filter.cache_clear()
 
     m = 4
     for g in range(1, 1 + m):
-        feature_g = np.array([f"gene_{i}" for i in range(g)])
+        var_names_g = np.array([f"gene_{i}" for i in range(g)])
         x_ng = torch.zeros((2, g))
         for _ in range(g):
-            transform(x_ng, feature_g)
+            transform(x_ng, var_names_g)
 
     assert transform.filter.cache_info().currsize == m
     assert transform.filter.cache_info().misses == m
     assert transform.filter.cache_info().hits == m * (m - 1) / 2
```

