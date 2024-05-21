# Comparing `tmp/moltx-1.0.2.tar.gz` & `tmp/moltx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moltx-1.0.2.tar", last modified: Mon May 13 09:51:16 2024, max compression
+gzip compressed data, was "moltx-1.0.3.tar", last modified: Tue May 21 01:34:08 2024, max compression
```

## Comparing `moltx-1.0.2.tar` & `moltx-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:51:16.638013 moltx-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 09:51:11.000000 moltx-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-13 09:51:16.638013 moltx-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-13 09:51:11.000000 moltx-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:51:16.634013 moltx-1.0.2/moltx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:51:16.638013 moltx-1.0.2/moltx/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/data/spe_safe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/data/spe_smiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/data/tks_safe.json
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/data/tks_smiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-13 09:51:11.000000 moltx-1.0.2/moltx/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:51:16.638013 moltx-1.0.2/moltx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-13 09:51:16.000000 moltx-1.0.2/moltx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-13 09:51:16.000000 moltx-1.0.2/moltx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:51:16.000000 moltx-1.0.2/moltx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 09:51:16.000000 moltx-1.0.2/moltx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 09:51:16.000000 moltx-1.0.2/moltx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 09:51:11.000000 moltx-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-13 09:51:16.638013 moltx-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:51:11.000000 moltx-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:51:16.638013 moltx-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-13 09:51:11.000000 moltx-1.0.2/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-13 09:51:11.000000 moltx-1.0.2/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-13 09:51:11.000000 moltx-1.0.2/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-13 09:51:11.000000 moltx-1.0.2/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 01:34:04.000000 moltx-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-21 01:34:08.637158 moltx-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-21 01:34:04.000000 moltx-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/moltx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/moltx/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/data/spe_safe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/data/spe_smiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/data/tks_safe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/data/tks_smiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/moltx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 01:34:04.000000 moltx-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-21 01:34:08.637158 moltx-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 01:34:04.000000 moltx-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-21 01:34:04.000000 moltx-1.0.3/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-21 01:34:04.000000 moltx-1.0.3/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-21 01:34:04.000000 moltx-1.0.3/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-21 01:34:04.000000 moltx-1.0.3/tests/test_tokenizer.py
```

### Comparing `moltx-1.0.2/LICENSE` & `moltx-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/PKG-INFO` & `moltx-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdkit~=2023.9.1
-Requires-Dist: torch~=2.2.0
+Requires-Dist: torch~=2.1.0
 
 # MolTx
 
 [![CI](https://github.com/js-ish/MolTx/actions/workflows/test.yml/badge.svg)](https://github.com/js-ish/MolTx/actions/workflows/test.yml?query=branch%3Amain)
 [![Coverage Status](https://coveralls.io/repos/github/js-ish/MolTx/badge.svg?branch=main)](https://coveralls.io/github/js-ish/MolTx?branch=main)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/moltx)
```

### Comparing `moltx-1.0.2/README.md` & `moltx-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/data/spe_safe.txt` & `moltx-1.0.3/moltx/data/spe_safe.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/data/spe_smiles.txt` & `moltx-1.0.3/moltx/data/spe_smiles.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/data/tks_safe.json` & `moltx-1.0.3/moltx/data/tks_safe.json`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/data/tks_smiles.json` & `moltx-1.0.3/moltx/data/tks_smiles.json`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/datasets.py` & `moltx-1.0.3/moltx/datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/models.py` & `moltx-1.0.3/moltx/models.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/nets.py` & `moltx-1.0.3/moltx/nets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/pipelines.py` & `moltx-1.0.3/moltx/pipelines.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx/tokenizers.py` & `moltx-1.0.3/moltx/tokenizers.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/moltx.egg-info/PKG-INFO` & `moltx-1.0.3/moltx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdkit~=2023.9.1
-Requires-Dist: torch~=2.2.0
+Requires-Dist: torch~=2.1.0
 
 # MolTx
 
 [![CI](https://github.com/js-ish/MolTx/actions/workflows/test.yml/badge.svg)](https://github.com/js-ish/MolTx/actions/workflows/test.yml?query=branch%3Amain)
 [![Coverage Status](https://coveralls.io/repos/github/js-ish/MolTx/badge.svg?branch=main)](https://coveralls.io/github/js-ish/MolTx?branch=main)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/moltx)
```

### Comparing `moltx-1.0.2/moltx.egg-info/SOURCES.txt` & `moltx-1.0.3/moltx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/setup.cfg` & `moltx-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/tests/test_datasets.py` & `moltx-1.0.3/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/tests/test_nets.py` & `moltx-1.0.3/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/tests/test_pipelines.py` & `moltx-1.0.3/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.2/tests/test_tokenizer.py` & `moltx-1.0.3/tests/test_tokenizer.py`

 * *Files identical despite different names*

