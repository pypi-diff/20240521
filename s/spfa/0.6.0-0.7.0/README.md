# Comparing `tmp/spfa-0.6.0.tar.gz` & `tmp/spfa-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spfa-0.6.0.tar", max compression
+gzip compressed data, was "spfa-0.7.0.tar", max compression
```

## Comparing `spfa-0.6.0.tar` & `spfa-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      928 2023-10-02 06:21:10.442593 spfa-0.6.0/README.md
--rw-r--r--   0        0        0     1004 2023-10-10 11:51:25.837787 spfa-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      114 2023-09-29 10:06:15.200034 spfa-0.6.0/spfa/__init__.py
--rwxr-xr-x   0        0        0    20710 2023-10-10 11:51:11.189632 spfa-0.6.0/spfa/models/spFA.py
--rw-r--r--   0        0        0      355 2023-09-29 09:32:04.923069 spfa-0.6.0/spfa/plots/__init__.py
--rwxr-xr-x   0        0        0    10284 2023-10-04 13:52:30.427048 spfa-0.6.0/spfa/plots/plots.py
--rw-r--r--   0        0        0      141 2023-09-29 09:30:10.672939 spfa-0.6.0/spfa/utils/__init__.py
--rwxr-xr-x   0        0        0     2592 2023-10-10 10:46:12.761151 spfa-0.6.0/spfa/utils/utils.py
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 spfa-0.6.0/setup.py
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 spfa-0.6.0/PKG-INFO
+-rwxr-xr-x   0        0        0      928 2023-10-02 06:21:10.442593 spfa-0.7.0/README.md
+-rw-r--r--   0        0        0     1004 2024-05-21 07:34:08.223772 spfa-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-09-29 10:06:15.200034 spfa-0.7.0/spfa/__init__.py
+-rwxr-xr-x   0        0        0    34721 2024-05-21 07:33:23.426522 spfa-0.7.0/spfa/models/spFA.py
+-rw-r--r--   0        0        0      520 2024-05-21 07:33:23.426522 spfa-0.7.0/spfa/plots/__init__.py
+-rwxr-xr-x   0        0        0    20310 2024-05-21 07:33:23.426522 spfa-0.7.0/spfa/plots/plots.py
+-rwxr-xr-x   0        0        0      333 2024-05-21 07:33:23.426522 spfa-0.7.0/spfa/utils/__init__.py
+-rwxr-xr-x   0        0        0     6808 2024-05-21 07:33:23.426522 spfa-0.7.0/spfa/utils/utils.py
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 spfa-0.7.0/setup.py
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 spfa-0.7.0/PKG-INFO
```

### Comparing `spfa-0.6.0/README.md` & `spfa-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `spfa-0.6.0/pyproject.toml` & `spfa-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spFA"
-version = "0.6.0"
+version = "0.7.0"
 description = "Probabilistic factor analysis model with covariate guided factors"
 authors = ["capraz <tuemayc@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "spfa"}]
 license = "MIT"
```

### Comparing `spfa-0.6.0/setup.py` & `spfa-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           'sphinx-rtd-theme==1.0.0',
           'sphinxcontrib-napoleon==0.7',
           'nbsphinx==0.8.9'],
  'notebook': ['jupyter']}
 
 setup_kwargs = {
     'name': 'spfa',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Probabilistic factor analysis model with covariate guided factors',
     'long_description': '# spFA\n\n# Introduction\n\nHere we present semi-supervised probabilistic Factor Analysis (spFA), a multi-omics integration method, which infers a set of low dimensional latent factors that represent the main sources of variability. spFA enables the discovery of primary sources of variation while adjusting for known covariates and simultaneously disentangling variation that is shared between multiple omics modalities and specific to single modalities. The spFA method is implemented in python using the pyro framework for probabilistic programming.\n\n\n# Installation\n\nTo install `spfa` first create `Python 3.8` environment e.g. by\n\n```\nconda create --name spfa-env python=3.8\nconda activate spfa-env\n```\n\nand install the package using \n\n```\npip install spfa\n```\n\n\n\n# How to use `spfa` for multi-omics analyses\n\nA detailed manual with examples and how to use `spfa` can be found here https://tcapraz.github.io/spFA/index.html.\n\n\n',
     'author': 'capraz',
     'author_email': 'tuemayc@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `spfa-0.6.0/PKG-INFO` & `spfa-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spfa
-Version: 0.6.0
+Version: 0.7.0
 Summary: Probabilistic factor analysis model with covariate guided factors
 License: MIT
 Author: capraz
 Author-email: tuemayc@hotmail.com
 Requires-Python: >=3.8.1,<3.11.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

