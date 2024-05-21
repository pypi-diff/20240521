# Comparing `tmp/patchly-0.0.7.tar.gz` & `tmp/patchly-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchly-0.0.7.tar", last modified: Tue Oct 24 15:20:28 2023, max compression
+gzip compressed data, was "patchly-0.0.9.tar", last modified: Tue Jan  2 15:35:59 2024, max compression
```

## Comparing `patchly-0.0.7.tar` & `patchly-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.256316 patchly-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-24 15:20:05.000000 patchly-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-24 15:20:05.000000 patchly-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2023-10-24 15:20:28.256316 patchly-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2023-10-24 15:20:05.000000 patchly-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.252316 patchly-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:05.000000 patchly-0.0.7/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-10-24 15:20:05.000000 patchly-0.0.7/examples/inference_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-10-24 15:20:05.000000 patchly-0.0.7/examples/pytorch_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.256316 patchly-0.0.7/patchly/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24734 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/array_like.py
--rw-r--r--   0 runner    (1001) docker     (127)    19889 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.256316 patchly-0.0.7/patchly/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.256316 patchly-0.0.7/patchly/tests/test_adaptive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_adaptive/test_adaptive_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_adaptive/test_adaptive_chunk_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_adaptive/test_adaptive_grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.256316 patchly-0.0.7/patchly/tests/test_crop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_crop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_crop/test_crop_grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.256316 patchly-0.0.7/patchly/tests/test_edge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10456 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_edge/test_edge_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_edge/test_edge_chunk_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_edge/test_edge_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.256316 patchly-0.0.7/patchly/tests/test_squeeze/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_squeeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_squeeze/test_squeeze_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10604 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_squeeze/test_squeeze_chunk_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/tests/test_squeeze/test_squeeze_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2023-10-24 15:20:05.000000 patchly-0.0.7/patchly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:20:28.256316 patchly-0.0.7/patchly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2023-10-24 15:20:28.000000 patchly-0.0.7/patchly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-10-24 15:20:28.000000 patchly-0.0.7/patchly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 15:20:28.000000 patchly-0.0.7/patchly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-24 15:20:28.000000 patchly-0.0.7/patchly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-24 15:20:28.000000 patchly-0.0.7/patchly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-10-24 15:20:05.000000 patchly-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-10-24 15:20:28.260316 patchly-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:59.001598 patchly-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-02 15:35:44.000000 patchly-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-02 15:35:44.000000 patchly-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-01-02 15:35:59.001598 patchly-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-01-02 15:35:44.000000 patchly-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:58.997598 patchly-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:44.000000 patchly-0.0.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-01-02 15:35:44.000000 patchly-0.0.9/examples/inference_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-01-02 15:35:44.000000 patchly-0.0.9/examples/pytorch_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:58.997598 patchly-0.0.9/patchly/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24734 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/array_like.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19889 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:58.997598 patchly-0.0.9/patchly/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:58.997598 patchly-0.0.9/patchly/tests/test_adaptive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_adaptive/test_adaptive_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_adaptive/test_adaptive_chunk_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_adaptive/test_adaptive_grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:58.997598 patchly-0.0.9/patchly/tests/test_crop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_crop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_crop/test_crop_grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:59.001598 patchly-0.0.9/patchly/tests/test_edge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_edge/test_edge_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_edge/test_edge_chunk_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_edge/test_edge_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:59.001598 patchly-0.0.9/patchly/tests/test_squeeze/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_squeeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_squeeze/test_squeeze_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_squeeze/test_squeeze_chunk_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/tests/test_squeeze/test_squeeze_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-01-02 15:35:44.000000 patchly-0.0.9/patchly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:35:59.001598 patchly-0.0.9/patchly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-01-02 15:35:58.000000 patchly-0.0.9/patchly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-01-02 15:35:58.000000 patchly-0.0.9/patchly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 15:35:58.000000 patchly-0.0.9/patchly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-02 15:35:58.000000 patchly-0.0.9/patchly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-02 15:35:58.000000 patchly-0.0.9/patchly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-02 15:35:44.000000 patchly-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-02 15:35:59.001598 patchly-0.0.9/setup.cfg
```

### Comparing `patchly-0.0.7/LICENSE` & `patchly-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/PKG-INFO` & `patchly-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchly
-Version: 0.0.7
+Version: 0.0.9
 Summary: A grid sampler for N-dimensional images
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -34,25 +34,31 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/patchly.svg?color=green)](https://python.org)
 ![Unit Tests](https://github.com/MIC-DKFZ/patchly/actions/workflows/test_and_deploy.yml/badge.svg?branch=main)
 [![codecov](https://codecov.io/gh/MIC-DKFZ/patchly/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/patchly)
 
 
 Patchly is a grid sampler for N-dimensional images enabling inference and other processing steps on extremely large images. Especially for 3D images, it has been proven successfully to inference large images patch-wise in a sliding-window approach. Patchly does just that with a very simple interface to sample and aggregate images.
 
-## Features
+The main functionalities of Patchly consist of a Sampler, which samples patches from an image based on a grid, and an Aggregator, which assembles the patches back into the shape of the original image. There is a multitude of libraries providing similar functionality already. However, they tend to work only for a limited number of usage scenarios before becoming unusable. 
 
-Patchly supports:
-- N-dimensional images (1D, 2D, 3D, ...)
-- Sampling and aggregation of images
-- Any array-like images (Numpy, Tensor, Zarr, Dask, ...)
-- Memory-mapped images
-- Patch overlap (here referred to as patch offset)
-- All numpy padding techniques
-- Images with non-spatial dimensions (color dimension, batch dimension, etc)
-- Chunk sampling to minimize memory consumption
+Patchly is the first library providing an advanced set of features for users working with sophisticated image processing pipelines requiring patch-based processing.
+
+A complete overview of how the Sampler and Aggregator work and an in-depth explanation of the features can be found [here](OVERVIEW.md).
+
+## Feature Summary
+
+Patchly provides the following advanced features:
+- N-dimensional image handling (1D, 2D, 3D, ...)
+- Multiple border-handling strategies
+- Support for any array-like images (Numpy, Tensor, Zarr, Dask, ...)
+- Memory-mapped image support
+- Patch overlap
+- ~~Numpy padding techniques~~
+- Support for images with non-spatial dimensions (color dimension, batch dimension, ...)
+- Chunk aggregation to minimize memory consumption
 
 ## Installation
 
 You can install `patchly` via [pip](https://pypi.org/project/patchly/):
 
     pip install patchly
 
@@ -119,17 +125,17 @@
 
 ## License
 
 Distributed under the terms of the [Apache Software License 2.0](http://www.apache.org/licenses/LICENSE-2.0) license,
 "Patchly" is free and open source software
 
 # Acknowledgements
-<img src="HI_Logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/patchly/raw/main/HI_Logo.png" height="100px" />
 
-<img src="dkfz_logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/patchly/raw/main/dkfz_logo.png" height="100px" />
 
 Patchly is developed and maintained by the Applied Computer Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) 
 and the [Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at the 
 [German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
 
 
 <!--- Samplify will live forever! But so will Chunky (⊙ _ ⊙ ) -->
```

### Comparing `patchly-0.0.7/README.md` & `patchly-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,31 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/patchly.svg?color=green)](https://python.org)
 ![Unit Tests](https://github.com/MIC-DKFZ/patchly/actions/workflows/test_and_deploy.yml/badge.svg?branch=main)
 [![codecov](https://codecov.io/gh/MIC-DKFZ/patchly/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/patchly)
 
 
 Patchly is a grid sampler for N-dimensional images enabling inference and other processing steps on extremely large images. Especially for 3D images, it has been proven successfully to inference large images patch-wise in a sliding-window approach. Patchly does just that with a very simple interface to sample and aggregate images.
 
-## Features
+The main functionalities of Patchly consist of a Sampler, which samples patches from an image based on a grid, and an Aggregator, which assembles the patches back into the shape of the original image. There is a multitude of libraries providing similar functionality already. However, they tend to work only for a limited number of usage scenarios before becoming unusable. 
 
-Patchly supports:
-- N-dimensional images (1D, 2D, 3D, ...)
-- Sampling and aggregation of images
-- Any array-like images (Numpy, Tensor, Zarr, Dask, ...)
-- Memory-mapped images
-- Patch overlap (here referred to as patch offset)
-- All numpy padding techniques
-- Images with non-spatial dimensions (color dimension, batch dimension, etc)
-- Chunk sampling to minimize memory consumption
+Patchly is the first library providing an advanced set of features for users working with sophisticated image processing pipelines requiring patch-based processing.
+
+A complete overview of how the Sampler and Aggregator work and an in-depth explanation of the features can be found [here](OVERVIEW.md).
+
+## Feature Summary
+
+Patchly provides the following advanced features:
+- N-dimensional image handling (1D, 2D, 3D, ...)
+- Multiple border-handling strategies
+- Support for any array-like images (Numpy, Tensor, Zarr, Dask, ...)
+- Memory-mapped image support
+- Patch overlap
+- ~~Numpy padding techniques~~
+- Support for images with non-spatial dimensions (color dimension, batch dimension, ...)
+- Chunk aggregation to minimize memory consumption
 
 ## Installation
 
 You can install `patchly` via [pip](https://pypi.org/project/patchly/):
 
     pip install patchly
 
@@ -90,17 +96,17 @@
 
 ## License
 
 Distributed under the terms of the [Apache Software License 2.0](http://www.apache.org/licenses/LICENSE-2.0) license,
 "Patchly" is free and open source software
 
 # Acknowledgements
-<img src="HI_Logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/patchly/raw/main/HI_Logo.png" height="100px" />
 
-<img src="dkfz_logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/patchly/raw/main/dkfz_logo.png" height="100px" />
 
 Patchly is developed and maintained by the Applied Computer Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) 
 and the [Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at the 
 [German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
 
 
 <!--- Samplify will live forever! But so will Chunky (⊙ _ ⊙ ) -->
```

### Comparing `patchly-0.0.7/examples/inference_chunk.py` & `patchly-0.0.9/examples/inference_chunk.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/examples/pytorch_inference.py` & `patchly-0.0.9/examples/pytorch_inference.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/aggregator.py` & `patchly-0.0.9/patchly/aggregator.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/array_like.py` & `patchly-0.0.9/patchly/array_like.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/sampler.py` & `patchly-0.0.9/patchly/sampler.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/slicer.py` & `patchly-0.0.9/patchly/slicer.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_adaptive/test_adaptive_aggregator.py` & `patchly-0.0.9/patchly/tests/test_adaptive/test_adaptive_aggregator.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_adaptive/test_adaptive_chunk_aggregator.py` & `patchly-0.0.9/patchly/tests/test_adaptive/test_adaptive_chunk_aggregator.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_adaptive/test_adaptive_grid_sampler.py` & `patchly-0.0.9/patchly/tests/test_adaptive/test_adaptive_grid_sampler.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_crop/test_crop_grid_sampler.py` & `patchly-0.0.9/patchly/tests/test_crop/test_crop_grid_sampler.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_edge/test_edge_aggregator.py` & `patchly-0.0.9/patchly/tests/test_edge/test_edge_aggregator.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_edge/test_edge_chunk_aggregator.py` & `patchly-0.0.9/patchly/tests/test_edge/test_edge_chunk_aggregator.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_edge/test_edge_sampler.py` & `patchly-0.0.9/patchly/tests/test_edge/test_edge_sampler.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_squeeze/test_squeeze_aggregator.py` & `patchly-0.0.9/patchly/tests/test_squeeze/test_squeeze_aggregator.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_squeeze/test_squeeze_chunk_aggregator.py` & `patchly-0.0.9/patchly/tests/test_squeeze/test_squeeze_chunk_aggregator.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/tests/test_squeeze/test_squeeze_sampler.py` & `patchly-0.0.9/patchly/tests/test_squeeze/test_squeeze_sampler.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly/utils.py` & `patchly-0.0.9/patchly/utils.py`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/patchly.egg-info/PKG-INFO` & `patchly-0.0.9/patchly.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchly
-Version: 0.0.7
+Version: 0.0.9
 Summary: A grid sampler for N-dimensional images
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -34,25 +34,31 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/patchly.svg?color=green)](https://python.org)
 ![Unit Tests](https://github.com/MIC-DKFZ/patchly/actions/workflows/test_and_deploy.yml/badge.svg?branch=main)
 [![codecov](https://codecov.io/gh/MIC-DKFZ/patchly/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/patchly)
 
 
 Patchly is a grid sampler for N-dimensional images enabling inference and other processing steps on extremely large images. Especially for 3D images, it has been proven successfully to inference large images patch-wise in a sliding-window approach. Patchly does just that with a very simple interface to sample and aggregate images.
 
-## Features
+The main functionalities of Patchly consist of a Sampler, which samples patches from an image based on a grid, and an Aggregator, which assembles the patches back into the shape of the original image. There is a multitude of libraries providing similar functionality already. However, they tend to work only for a limited number of usage scenarios before becoming unusable. 
 
-Patchly supports:
-- N-dimensional images (1D, 2D, 3D, ...)
-- Sampling and aggregation of images
-- Any array-like images (Numpy, Tensor, Zarr, Dask, ...)
-- Memory-mapped images
-- Patch overlap (here referred to as patch offset)
-- All numpy padding techniques
-- Images with non-spatial dimensions (color dimension, batch dimension, etc)
-- Chunk sampling to minimize memory consumption
+Patchly is the first library providing an advanced set of features for users working with sophisticated image processing pipelines requiring patch-based processing.
+
+A complete overview of how the Sampler and Aggregator work and an in-depth explanation of the features can be found [here](OVERVIEW.md).
+
+## Feature Summary
+
+Patchly provides the following advanced features:
+- N-dimensional image handling (1D, 2D, 3D, ...)
+- Multiple border-handling strategies
+- Support for any array-like images (Numpy, Tensor, Zarr, Dask, ...)
+- Memory-mapped image support
+- Patch overlap
+- ~~Numpy padding techniques~~
+- Support for images with non-spatial dimensions (color dimension, batch dimension, ...)
+- Chunk aggregation to minimize memory consumption
 
 ## Installation
 
 You can install `patchly` via [pip](https://pypi.org/project/patchly/):
 
     pip install patchly
 
@@ -119,17 +125,17 @@
 
 ## License
 
 Distributed under the terms of the [Apache Software License 2.0](http://www.apache.org/licenses/LICENSE-2.0) license,
 "Patchly" is free and open source software
 
 # Acknowledgements
-<img src="HI_Logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/patchly/raw/main/HI_Logo.png" height="100px" />
 
-<img src="dkfz_logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/patchly/raw/main/dkfz_logo.png" height="100px" />
 
 Patchly is developed and maintained by the Applied Computer Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) 
 and the [Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at the 
 [German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
 
 
 <!--- Samplify will live forever! But so will Chunky (⊙ _ ⊙ ) -->
```

### Comparing `patchly-0.0.7/patchly.egg-info/SOURCES.txt` & `patchly-0.0.9/patchly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/pyproject.toml` & `patchly-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `patchly-0.0.7/setup.cfg` & `patchly-0.0.9/setup.cfg`

 * *Files identical despite different names*

