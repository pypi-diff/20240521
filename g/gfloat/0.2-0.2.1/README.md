# Comparing `tmp/gfloat-0.2.tar.gz` & `tmp/gfloat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfloat-0.2.tar", last modified: Tue May 21 16:54:41 2024, max compression
+gzip compressed data, was "gfloat-0.2.1.tar", last modified: Tue May 21 20:53:36 2024, max compression
```

## Comparing `gfloat-0.2.tar` & `gfloat-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.380962 gfloat-0.2/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/.github/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/.github/workflows/
--rw-r--r--   0 awf       (1000) awf       (1000)      876 2024-05-19 10:37:30.000000 gfloat-0.2/.github/workflows/ci.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)     3178 2024-05-02 11:54:43.000000 gfloat-0.2/.gitignore
--rw-r--r--   0 awf       (1000) awf       (1000)      630 2024-05-19 10:37:30.000000 gfloat-0.2/.pre-commit-config.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)      239 2024-05-19 10:37:30.000000 gfloat-0.2/.readthedocs.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)      168 2024-05-19 10:37:30.000000 gfloat-0.2/BUILDING.md
--rw-r--r--   0 awf       (1000) awf       (1000)     1093 2024-05-02 11:54:43.000000 gfloat-0.2/LICENSE
--rw-r--r--   0 awf       (1000) awf       (1000)     3052 2024-05-21 16:54:41.380962 gfloat-0.2/PKG-INFO
--rw-r--r--   0 awf       (1000) awf       (1000)     2605 2024-05-19 10:37:30.000000 gfloat-0.2/README.md
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/docs/
--rw-r--r--   0 awf       (1000) awf       (1000)      638 2024-01-27 16:06:55.000000 gfloat-0.2/docs/Makefile
--rw-r--r--   0 awf       (1000) awf       (1000)      799 2024-01-27 13:41:22.000000 gfloat-0.2/docs/make.bat
--rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-05-19 10:37:30.000000 gfloat-0.2/docs/requirements-rtd.txt
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/docs/source/
--rw-r--r--   0 awf       (1000) awf       (1000)    12905 2024-05-02 11:54:43.000000 gfloat-0.2/docs/source/01-decode.ipynb
--rw-r--r--   0 awf       (1000) awf       (1000)    25062 2024-05-19 10:37:30.000000 gfloat-0.2/docs/source/02-value-stats.ipynb
--rw-r--r--   0 awf       (1000) awf       (1000)    97024 2024-05-02 11:54:43.000000 gfloat-0.2/docs/source/03-value-tables.ipynb
--rw-r--r--   0 awf       (1000) awf       (1000)      741 2024-05-21 15:10:25.000000 gfloat-0.2/docs/source/api.rst
--rw-r--r--   0 awf       (1000) awf       (1000)     1262 2024-05-21 16:54:36.000000 gfloat-0.2/docs/source/conf.py
--rw-r--r--   0 awf       (1000) awf       (1000)      945 2024-05-21 15:10:25.000000 gfloat-0.2/docs/source/formats.rst
--rw-r--r--   0 awf       (1000) awf       (1000)     1923 2024-05-02 11:54:43.000000 gfloat-0.2/docs/source/index.rst
--rw-r--r--   0 awf       (1000) awf       (1000)      228 2024-05-02 11:54:43.000000 gfloat-0.2/docs/source/notebooks.rst
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/etc/
--rwxr-xr-x   0 awf       (1000) awf       (1000)      357 2024-05-02 11:54:43.000000 gfloat-0.2/etc/check-copyright.sh
--rw-r--r--   0 awf       (1000) awf       (1000)      474 2024-05-21 15:13:46.000000 gfloat-0.2/etc/package.sh
--rw-r--r--   0 awf       (1000) awf       (1000)      637 2024-05-02 11:54:43.000000 gfloat-0.2/etc/test-check-copyright.sh
--rw-r--r--   0 awf       (1000) awf       (1000)     1051 2024-05-21 16:54:36.000000 gfloat-0.2/pyproject.toml
--rw-r--r--   0 awf       (1000) awf       (1000)      304 2024-05-21 15:10:25.000000 gfloat-0.2/requirements-dev.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-03-22 15:19:02.000000 gfloat-0.2/requirements.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       38 2024-05-21 16:54:41.380962 gfloat-0.2/setup.cfg
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/src/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/src/gfloat/
--rw-r--r--   0 awf       (1000) awf       (1000)      543 2024-05-21 15:10:25.000000 gfloat-0.2/src/gfloat/__init__.py
--rw-r--r--   0 awf       (1000) awf       (1000)     5616 2024-05-21 15:10:25.000000 gfloat-0.2/src/gfloat/block.py
--rw-r--r--   0 awf       (1000) awf       (1000)     2815 2024-05-02 11:54:43.000000 gfloat-0.2/src/gfloat/decode.py
--rw-r--r--   0 awf       (1000) awf       (1000)     5235 2024-05-21 15:10:25.000000 gfloat-0.2/src/gfloat/formats.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-05-02 11:54:43.000000 gfloat-0.2/src/gfloat/printing.py
--rw-r--r--   0 awf       (1000) awf       (1000)     6556 2024-05-02 11:54:43.000000 gfloat-0.2/src/gfloat/round.py
--rw-r--r--   0 awf       (1000) awf       (1000)    11982 2024-05-21 15:10:25.000000 gfloat-0.2/src/gfloat/types.py
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.380962 gfloat-0.2/src/gfloat.egg-info/
--rw-r--r--   0 awf       (1000) awf       (1000)     3052 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/PKG-INFO
--rw-r--r--   0 awf       (1000) awf       (1000)      951 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/SOURCES.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        1 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/dependency_links.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/requires.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/top_level.txt
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.380962 gfloat-0.2/test/
--rw-r--r--   0 awf       (1000) awf       (1000)      866 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_block.py
--rw-r--r--   0 awf       (1000) awf       (1000)     7553 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_decode.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1224 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_encode.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1006 2024-05-02 11:54:43.000000 gfloat-0.2/test/test_finfo.py
--rw-r--r--   0 awf       (1000) awf       (1000)     2100 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_microxcaling.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1039 2024-05-02 11:54:43.000000 gfloat-0.2/test/test_printing.py
--rw-r--r--   0 awf       (1000) awf       (1000)     6200 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_round.py
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.295811 gfloat-0.2.1/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.285811 gfloat-0.2.1/.github/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.285811 gfloat-0.2.1/.github/workflows/
+-rw-r--r--   0 awf       (1000) awf       (1000)      923 2024-05-21 20:46:19.000000 gfloat-0.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)     3178 2024-05-02 11:54:43.000000 gfloat-0.2.1/.gitignore
+-rw-r--r--   0 awf       (1000) awf       (1000)      630 2024-05-19 10:37:30.000000 gfloat-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)      239 2024-05-19 10:37:30.000000 gfloat-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)      168 2024-05-19 10:37:30.000000 gfloat-0.2.1/BUILDING.md
+-rw-r--r--   0 awf       (1000) awf       (1000)     1093 2024-05-02 11:54:43.000000 gfloat-0.2.1/LICENSE
+-rw-r--r--   0 awf       (1000) awf       (1000)     3618 2024-05-21 20:53:36.295811 gfloat-0.2.1/PKG-INFO
+-rw-r--r--   0 awf       (1000) awf       (1000)     2605 2024-05-19 10:37:30.000000 gfloat-0.2.1/README.md
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.285811 gfloat-0.2.1/docs/
+-rw-r--r--   0 awf       (1000) awf       (1000)      638 2024-01-27 16:06:55.000000 gfloat-0.2.1/docs/Makefile
+-rw-r--r--   0 awf       (1000) awf       (1000)      799 2024-01-27 13:41:22.000000 gfloat-0.2.1/docs/make.bat
+-rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-05-21 20:14:58.000000 gfloat-0.2.1/docs/requirements-rtd.txt
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.285811 gfloat-0.2.1/docs/source/
+-rw-r--r--   0 awf       (1000) awf       (1000)    12905 2024-05-21 20:14:49.000000 gfloat-0.2.1/docs/source/01-decode.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)    25062 2024-05-19 10:37:30.000000 gfloat-0.2.1/docs/source/02-value-stats.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)    97024 2024-05-21 20:12:50.000000 gfloat-0.2.1/docs/source/03-value-tables.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)      741 2024-05-21 15:10:25.000000 gfloat-0.2.1/docs/source/api.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)     1266 2024-05-21 20:53:30.000000 gfloat-0.2.1/docs/source/conf.py
+-rw-r--r--   0 awf       (1000) awf       (1000)      945 2024-05-21 15:10:25.000000 gfloat-0.2.1/docs/source/formats.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)     1923 2024-05-02 11:54:43.000000 gfloat-0.2.1/docs/source/index.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)      228 2024-05-02 11:54:43.000000 gfloat-0.2.1/docs/source/notebooks.rst
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.285811 gfloat-0.2.1/etc/
+-rwxr-xr-x   0 awf       (1000) awf       (1000)      357 2024-05-02 11:54:43.000000 gfloat-0.2.1/etc/check-copyright.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)      641 2024-05-21 20:16:23.000000 gfloat-0.2.1/etc/package.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)      637 2024-05-02 11:54:43.000000 gfloat-0.2.1/etc/test-check-copyright.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)     1076 2024-05-21 20:53:30.000000 gfloat-0.2.1/pyproject.toml
+-rw-r--r--   0 awf       (1000) awf       (1000)      307 2024-05-21 20:46:19.000000 gfloat-0.2.1/requirements-dev.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)      150 2024-05-21 20:45:34.000000 gfloat-0.2.1/requirements-test.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-03-22 15:19:02.000000 gfloat-0.2.1/requirements.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)       38 2024-05-21 20:53:36.295811 gfloat-0.2.1/setup.cfg
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.285811 gfloat-0.2.1/src/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.295811 gfloat-0.2.1/src/gfloat/
+-rw-r--r--   0 awf       (1000) awf       (1000)      543 2024-05-21 20:47:45.000000 gfloat-0.2.1/src/gfloat/__init__.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     5616 2024-05-21 15:10:25.000000 gfloat-0.2.1/src/gfloat/block.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     2815 2024-05-02 11:54:43.000000 gfloat-0.2.1/src/gfloat/decode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     5235 2024-05-21 20:14:49.000000 gfloat-0.2.1/src/gfloat/formats.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-05-02 11:54:43.000000 gfloat-0.2.1/src/gfloat/printing.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     6556 2024-05-02 11:54:43.000000 gfloat-0.2.1/src/gfloat/round.py
+-rw-r--r--   0 awf       (1000) awf       (1000)    11982 2024-05-21 15:10:25.000000 gfloat-0.2.1/src/gfloat/types.py
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.295811 gfloat-0.2.1/src/gfloat.egg-info/
+-rw-r--r--   0 awf       (1000) awf       (1000)     3618 2024-05-21 20:53:36.000000 gfloat-0.2.1/src/gfloat.egg-info/PKG-INFO
+-rw-r--r--   0 awf       (1000) awf       (1000)      973 2024-05-21 20:53:36.000000 gfloat-0.2.1/src/gfloat.egg-info/SOURCES.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        1 2024-05-21 20:53:36.000000 gfloat-0.2.1/src/gfloat.egg-info/dependency_links.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)      154 2024-05-21 20:53:36.000000 gfloat-0.2.1/src/gfloat.egg-info/requires.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-05-21 20:53:36.000000 gfloat-0.2.1/src/gfloat.egg-info/top_level.txt
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 20:53:36.295811 gfloat-0.2.1/test/
+-rw-r--r--   0 awf       (1000) awf       (1000)      866 2024-05-21 15:10:25.000000 gfloat-0.2.1/test/test_block.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     7553 2024-05-21 15:10:25.000000 gfloat-0.2.1/test/test_decode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1224 2024-05-21 15:10:25.000000 gfloat-0.2.1/test/test_encode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1006 2024-05-02 11:54:43.000000 gfloat-0.2.1/test/test_finfo.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     2100 2024-05-21 15:10:25.000000 gfloat-0.2.1/test/test_microxcaling.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1039 2024-05-02 11:54:43.000000 gfloat-0.2.1/test/test_printing.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     6200 2024-05-21 15:10:25.000000 gfloat-0.2.1/test/test_round.py
```

### Comparing `gfloat-0.2/.github/workflows/ci.yaml` & `gfloat-0.2.1/.github/workflows/ci.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
           python-version: "3.9"
           cache: "pip"
 
       - name: Install requirements
         run: |
           pip install -U pip
           pip install .[dev]
+          pip install -r requirements-test.txt
 
       - name: Log installed environment
         run: |
           python3 -m pip freeze
 
       - name: Pre-commit all files
         run: |
```

### Comparing `gfloat-0.2/.gitignore` & `gfloat-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/.pre-commit-config.yaml` & `gfloat-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/LICENSE` & `gfloat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/PKG-INFO` & `gfloat-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: gfloat
-Version: 0.2
-Summary: Generic floating point handling in Python
-Author-email: Andrew Fitzgibbon <awf@fitzgibbon.ie>
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.8.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-
 <!-- Copyright (c) 2024 Graphcore Ltd. All rights reserved. -->
 
 # gfloat: Generic floating-point types in Python
 
 An implementation of generic floating point encode/decode logic,
 handling various current and proposed floating point types:
```

### Comparing `gfloat-0.2/docs/Makefile` & `gfloat-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/docs/make.bat` & `gfloat-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/docs/source/01-decode.ipynb` & `gfloat-0.2.1/docs/source/01-decode.ipynb`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/docs/source/02-value-stats.ipynb` & `gfloat-0.2.1/docs/source/02-value-stats.ipynb`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/docs/source/03-value-tables.ipynb` & `gfloat-0.2.1/docs/source/03-value-tables.ipynb`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/docs/source/api.rst` & `gfloat-0.2.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/docs/source/conf.py` & `gfloat-0.2.1/docs/source/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Configuration file for the Sphinx documentation builder.
 
 # -- Project information
 
 project = "GFloat"
 copyright = "2024, Graphcore Ltd"
 author = "Andrew Fitzgibbon"
-release = "0.2"  # Set version in package.sh
-version = "0.2"  # Set version in package.sh
+release = "0.2.1"  # Set version in package.sh
+version = "0.2.1"  # Set version in package.sh
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.duration",
     "sphinx.ext.doctest",
     "sphinx.ext.autodoc",
```

### Comparing `gfloat-0.2/docs/source/formats.rst` & `gfloat-0.2.1/docs/source/formats.rst`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/docs/source/index.rst` & `gfloat-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/etc/test-check-copyright.sh` & `gfloat-0.2.1/etc/test-check-copyright.sh`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/pyproject.toml` & `gfloat-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 
 [tool.setuptools]
 packages = ['gfloat']
 package-dir = {"" = "src"}
 
 [project]
 name =  "gfloat"
-version = "0.2" # Set version in package.sh
+version = "0.2.1" # Set version in package.sh
 authors = [
     {name = "Andrew Fitzgibbon", email = "awf@fitzgibbon.ie"},
 ]
 description = "Generic floating point handling in Python"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
 ]
 requires-python = ">=3.8.1"
-dynamic = ["dependencies"]
+dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools.dynamic]
 # version = {attr = "gfloat.VERSION"} # Wow: https://github.com/pypa/setuptools/issues/1724
 dependencies = {file = ["requirements.txt"]}
-# optional-dependencies = {dev = {file = ["requirements-dev.txt"]}}
+optional-dependencies = {dev = {file = ["requirements-dev.txt"]}}
 
 [tool.black]
 line-length = 88
 fast = true
 
 [tool.mypy]
 [[tool.mypy.overrides]]
```

### Comparing `gfloat-0.2/src/gfloat/__init__.py` & `gfloat-0.2.1/src/gfloat/__init__.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/src/gfloat/block.py` & `gfloat-0.2.1/src/gfloat/block.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/src/gfloat/decode.py` & `gfloat-0.2.1/src/gfloat/decode.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/src/gfloat/formats.py` & `gfloat-0.2.1/src/gfloat/formats.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/src/gfloat/printing.py` & `gfloat-0.2.1/src/gfloat/printing.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/src/gfloat/round.py` & `gfloat-0.2.1/src/gfloat/round.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/src/gfloat/types.py` & `gfloat-0.2.1/src/gfloat/types.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/src/gfloat.egg-info/SOURCES.txt` & `gfloat-0.2.1/src/gfloat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 .readthedocs.yaml
 BUILDING.md
 LICENSE
 README.md
 pyproject.toml
 requirements-dev.txt
+requirements-test.txt
 requirements.txt
 .github/workflows/ci.yaml
 docs/Makefile
 docs/make.bat
 docs/requirements-rtd.txt
 docs/source/01-decode.ipynb
 docs/source/02-value-stats.ipynb
```

### Comparing `gfloat-0.2/test/test_block.py` & `gfloat-0.2.1/test/test_block.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/test/test_decode.py` & `gfloat-0.2.1/test/test_decode.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/test/test_encode.py` & `gfloat-0.2.1/test/test_encode.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/test/test_finfo.py` & `gfloat-0.2.1/test/test_finfo.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/test/test_microxcaling.py` & `gfloat-0.2.1/test/test_microxcaling.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/test/test_printing.py` & `gfloat-0.2.1/test/test_printing.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.2/test/test_round.py` & `gfloat-0.2.1/test/test_round.py`

 * *Files identical despite different names*

