# Comparing `tmp/gfloat-0.1.tar.gz` & `tmp/gfloat-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfloat-0.1.tar", last modified: Thu May  2 12:05:40 2024, max compression
+gzip compressed data, was "gfloat-0.2.tar", last modified: Tue May 21 16:54:41 2024, max compression
```

## Comparing `gfloat-0.1.tar` & `gfloat-0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/.github/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/.github/workflows/
--rw-r--r--   0 awf       (1000) awf       (1000)      924 2024-05-02 11:54:43.000000 gfloat-0.1/.github/workflows/ci.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)     3178 2024-05-02 11:54:43.000000 gfloat-0.1/.gitignore
--rw-r--r--   0 awf       (1000) awf       (1000)      645 2024-05-02 11:54:43.000000 gfloat-0.1/.pre-commit-config.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)      360 2024-05-02 11:54:43.000000 gfloat-0.1/.readthedocs.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)      103 2024-05-02 11:54:43.000000 gfloat-0.1/BUILDING.md
--rw-r--r--   0 awf       (1000) awf       (1000)     1093 2024-05-02 11:54:43.000000 gfloat-0.1/LICENSE
--rw-r--r--   0 awf       (1000) awf       (1000)     3297 2024-05-02 12:05:40.735762 gfloat-0.1/PKG-INFO
--rw-r--r--   0 awf       (1000) awf       (1000)     2540 2024-05-02 11:54:43.000000 gfloat-0.1/README.md
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/docs/
--rw-r--r--   0 awf       (1000) awf       (1000)      638 2024-01-27 16:06:55.000000 gfloat-0.1/docs/Makefile
--rw-r--r--   0 awf       (1000) awf       (1000)      799 2024-01-27 13:41:22.000000 gfloat-0.1/docs/make.bat
--rw-r--r--   0 awf       (1000) awf       (1000)        8 2024-03-22 15:17:01.000000 gfloat-0.1/docs/requirements-rtd.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       74 2024-05-01 12:01:20.000000 gfloat-0.1/docs/requirements.txt
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/docs/source/
--rw-r--r--   0 awf       (1000) awf       (1000)    12905 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/01-decode.ipynb
--rw-r--r--   0 awf       (1000) awf       (1000)    25085 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/02-value-stats.ipynb
--rw-r--r--   0 awf       (1000) awf       (1000)    97024 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/03-value-tables.ipynb
--rw-r--r--   0 awf       (1000) awf       (1000)      608 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/api.rst
--rw-r--r--   0 awf       (1000) awf       (1000)      993 2024-05-02 12:05:29.000000 gfloat-0.1/docs/source/conf.py
--rw-r--r--   0 awf       (1000) awf       (1000)      689 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/formats.rst
--rw-r--r--   0 awf       (1000) awf       (1000)     1923 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/index.rst
--rw-r--r--   0 awf       (1000) awf       (1000)      228 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/notebooks.rst
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/etc/
--rwxr-xr-x   0 awf       (1000) awf       (1000)      357 2024-05-02 11:54:43.000000 gfloat-0.1/etc/check-copyright.sh
--rw-r--r--   0 awf       (1000) awf       (1000)      474 2024-05-02 12:05:10.000000 gfloat-0.1/etc/package.sh
--rw-r--r--   0 awf       (1000) awf       (1000)      637 2024-05-02 11:54:43.000000 gfloat-0.1/etc/test-check-copyright.sh
--rw-r--r--   0 awf       (1000) awf       (1000)      993 2024-05-02 12:05:29.000000 gfloat-0.1/pyproject.toml
--rw-r--r--   0 awf       (1000) awf       (1000)       99 2024-05-02 11:54:43.000000 gfloat-0.1/requirements-test.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-03-22 15:19:02.000000 gfloat-0.1/requirements.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       38 2024-05-02 12:05:40.735762 gfloat-0.1/setup.cfg
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/src/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/src/gfloat/
--rw-r--r--   0 awf       (1000) awf       (1000)      482 2024-05-01 12:01:20.000000 gfloat-0.1/src/gfloat/__init__.py
--rw-r--r--   0 awf       (1000) awf       (1000)     3161 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/block.py
--rw-r--r--   0 awf       (1000) awf       (1000)     2815 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/decode.py
--rw-r--r--   0 awf       (1000) awf       (1000)     4989 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/formats.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/printing.py
--rw-r--r--   0 awf       (1000) awf       (1000)     6556 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/round.py
--rw-r--r--   0 awf       (1000) awf       (1000)    11911 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/types.py
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/src/gfloat.egg-info/
--rw-r--r--   0 awf       (1000) awf       (1000)     3297 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/PKG-INFO
--rw-r--r--   0 awf       (1000) awf       (1000)      948 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/SOURCES.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        1 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/dependency_links.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       79 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/requires.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/top_level.txt
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/test/
--rw-r--r--   0 awf       (1000) awf       (1000)      528 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_block.py
--rw-r--r--   0 awf       (1000) awf       (1000)     7580 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_decode.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1242 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_encode.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1006 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_finfo.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1039 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_printing.py
--rw-r--r--   0 awf       (1000) awf       (1000)     6222 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_round.py
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.380962 gfloat-0.2/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/.github/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/.github/workflows/
+-rw-r--r--   0 awf       (1000) awf       (1000)      876 2024-05-19 10:37:30.000000 gfloat-0.2/.github/workflows/ci.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)     3178 2024-05-02 11:54:43.000000 gfloat-0.2/.gitignore
+-rw-r--r--   0 awf       (1000) awf       (1000)      630 2024-05-19 10:37:30.000000 gfloat-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)      239 2024-05-19 10:37:30.000000 gfloat-0.2/.readthedocs.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)      168 2024-05-19 10:37:30.000000 gfloat-0.2/BUILDING.md
+-rw-r--r--   0 awf       (1000) awf       (1000)     1093 2024-05-02 11:54:43.000000 gfloat-0.2/LICENSE
+-rw-r--r--   0 awf       (1000) awf       (1000)     3052 2024-05-21 16:54:41.380962 gfloat-0.2/PKG-INFO
+-rw-r--r--   0 awf       (1000) awf       (1000)     2605 2024-05-19 10:37:30.000000 gfloat-0.2/README.md
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/docs/
+-rw-r--r--   0 awf       (1000) awf       (1000)      638 2024-01-27 16:06:55.000000 gfloat-0.2/docs/Makefile
+-rw-r--r--   0 awf       (1000) awf       (1000)      799 2024-01-27 13:41:22.000000 gfloat-0.2/docs/make.bat
+-rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-05-19 10:37:30.000000 gfloat-0.2/docs/requirements-rtd.txt
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/docs/source/
+-rw-r--r--   0 awf       (1000) awf       (1000)    12905 2024-05-02 11:54:43.000000 gfloat-0.2/docs/source/01-decode.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)    25062 2024-05-19 10:37:30.000000 gfloat-0.2/docs/source/02-value-stats.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)    97024 2024-05-02 11:54:43.000000 gfloat-0.2/docs/source/03-value-tables.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)      741 2024-05-21 15:10:25.000000 gfloat-0.2/docs/source/api.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)     1262 2024-05-21 16:54:36.000000 gfloat-0.2/docs/source/conf.py
+-rw-r--r--   0 awf       (1000) awf       (1000)      945 2024-05-21 15:10:25.000000 gfloat-0.2/docs/source/formats.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)     1923 2024-05-02 11:54:43.000000 gfloat-0.2/docs/source/index.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)      228 2024-05-02 11:54:43.000000 gfloat-0.2/docs/source/notebooks.rst
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/etc/
+-rwxr-xr-x   0 awf       (1000) awf       (1000)      357 2024-05-02 11:54:43.000000 gfloat-0.2/etc/check-copyright.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)      474 2024-05-21 15:13:46.000000 gfloat-0.2/etc/package.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)      637 2024-05-02 11:54:43.000000 gfloat-0.2/etc/test-check-copyright.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)     1051 2024-05-21 16:54:36.000000 gfloat-0.2/pyproject.toml
+-rw-r--r--   0 awf       (1000) awf       (1000)      304 2024-05-21 15:10:25.000000 gfloat-0.2/requirements-dev.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-03-22 15:19:02.000000 gfloat-0.2/requirements.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)       38 2024-05-21 16:54:41.380962 gfloat-0.2/setup.cfg
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/src/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.370962 gfloat-0.2/src/gfloat/
+-rw-r--r--   0 awf       (1000) awf       (1000)      543 2024-05-21 15:10:25.000000 gfloat-0.2/src/gfloat/__init__.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     5616 2024-05-21 15:10:25.000000 gfloat-0.2/src/gfloat/block.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     2815 2024-05-02 11:54:43.000000 gfloat-0.2/src/gfloat/decode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     5235 2024-05-21 15:10:25.000000 gfloat-0.2/src/gfloat/formats.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-05-02 11:54:43.000000 gfloat-0.2/src/gfloat/printing.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     6556 2024-05-02 11:54:43.000000 gfloat-0.2/src/gfloat/round.py
+-rw-r--r--   0 awf       (1000) awf       (1000)    11982 2024-05-21 15:10:25.000000 gfloat-0.2/src/gfloat/types.py
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.380962 gfloat-0.2/src/gfloat.egg-info/
+-rw-r--r--   0 awf       (1000) awf       (1000)     3052 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/PKG-INFO
+-rw-r--r--   0 awf       (1000) awf       (1000)      951 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/SOURCES.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        1 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/dependency_links.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/requires.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-05-21 16:54:41.000000 gfloat-0.2/src/gfloat.egg-info/top_level.txt
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-21 16:54:41.380962 gfloat-0.2/test/
+-rw-r--r--   0 awf       (1000) awf       (1000)      866 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_block.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     7553 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_decode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1224 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_encode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1006 2024-05-02 11:54:43.000000 gfloat-0.2/test/test_finfo.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     2100 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_microxcaling.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1039 2024-05-02 11:54:43.000000 gfloat-0.2/test/test_printing.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     6200 2024-05-21 15:10:25.000000 gfloat-0.2/test/test_round.py
```

### Comparing `gfloat-0.1/.github/workflows/ci.yaml` & `gfloat-0.2/.github/workflows/ci.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -16,16 +16,15 @@
         with:
           python-version: "3.9"
           cache: "pip"
 
       - name: Install requirements
         run: |
           pip install -U pip
-          pip install .[test]
-          pip install -r docs/requirements.txt
+          pip install .[dev]
 
       - name: Log installed environment
         run: |
           python3 -m pip freeze
 
       - name: Pre-commit all files
         run: |
```

### Comparing `gfloat-0.1/.gitignore` & `gfloat-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/.pre-commit-config.yaml` & `gfloat-0.2/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -7,22 +7,21 @@
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 
 -   repo: https://github.com/psf/black
     rev: 24.4.0
     hooks:
-    - id: black
+    - id: black-jupyter
 
 -   repo: local
     hooks:
     - id: etc/check-copyright.sh
       name: check copyright
       entry: etc/check-copyright.sh
       language: script
       exclude: |
-            (?x)^(
-                docs/Makefile|
-                docs/make.bat|
-                .*\.md|
-                (.*/|)requirements.*\.txt
-            )$
+            (?x)(
+                ^docs/Makefile$|
+                ^docs/make.bat$|
+                (/|)requirements.*\.txt$
+            )
```

### Comparing `gfloat-0.1/LICENSE` & `gfloat-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/PKG-INFO` & `gfloat-0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 Metadata-Version: 2.1
 Name: gfloat
-Version: 0.1
+Version: 0.2
 Summary: Generic floating point handling in Python
 Author-email: Andrew Fitzgibbon <awf@fitzgibbon.ie>
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pandas; extra == "test"
-Requires-Dist: ipykernel; extra == "test"
-Requires-Dist: black[jupyter]; extra == "test"
-Requires-Dist: ml_dtypes; extra == "test"
-Requires-Dist: mypy; extra == "test"
-Requires-Dist: pre-commit; extra == "test"
+
+<!-- Copyright (c) 2024 Graphcore Ltd. All rights reserved. -->
 
 # gfloat: Generic floating-point types in Python
 
 An implementation of generic floating point encode/decode logic,
 handling various current and proposed floating point types:
 
  - [IEEE 754](https://en.wikipedia.org/wiki/IEEE_754): Binary16, Binary32
```

### Comparing `gfloat-0.1/README.md` & `gfloat-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<!-- Copyright (c) 2024 Graphcore Ltd. All rights reserved. -->
+
 # gfloat: Generic floating-point types in Python
 
 An implementation of generic floating point encode/decode logic,
 handling various current and proposed floating point types:
 
  - [IEEE 754](https://en.wikipedia.org/wiki/IEEE_754): Binary16, Binary32
  - [OCP Float8](https://www.opencompute.org/documents/ocp-8-bit-floating-point-specification-ofp8-revision-1-0-2023-06-20-pdf): E5M2, E4M3
```

### Comparing `gfloat-0.1/docs/Makefile` & `gfloat-0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/docs/make.bat` & `gfloat-0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/docs/source/01-decode.ipynb` & `gfloat-0.2/docs/source/01-decode.ipynb`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/docs/source/02-value-stats.ipynb` & `gfloat-0.2/docs/source/02-value-stats.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975117952699475%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(75, 'df = pandas.DataFrame(stats)')], delete: [76, 75]}}, "*

 * *            "3: {'source': {delete: [0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.12.3'}}"}*

```diff
@@ -106,16 +106,15 @@
                 "\n",
                 "formats_to_check = (\n",
                 "    tiny_formats\n",
                 "    + fp8_formats\n",
                 "    + [format_info_bfloat16, format_info_ocp_int8, format_info_ocp_e8m0]\n",
                 ")\n",
                 "stats = [collect_stats(fi) for fi in formats_to_check]\n",
-                "df = pandas.DataFrame(stats)\n",
-                "\n"
+                "df = pandas.DataFrame(stats)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Emit HTML table"
@@ -384,15 +383,14 @@
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "\n",
                 "# Special rendering for float values - if they don't render nicely in 10.5g,\n",
                 "# use float_pow2str\n",
                 "def render_float(v):\n",
                 "    s = f\"{v:8.5g}\"\n",
                 "    if not \"e\" in s and float(s) == v:\n",
                 "        return s\n",
                 "    else:\n",
@@ -426,13 +424,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.14"
+            "version": "3.12.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `gfloat-0.1/docs/source/03-value-tables.ipynb` & `gfloat-0.2/docs/source/03-value-tables.ipynb`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/docs/source/api.rst` & `gfloat-0.2/docs/source/api.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 .. Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
 API
 ===
 
 .. module:: gfloat
 
-Functions
----------
+Scalar Functions
+----------------
 
 .. autofunction:: decode_float
 .. autofunction:: round_float
 .. autofunction:: encode_float
 
+Block format functions
+----------------------
+
 .. autofunction:: decode_block
 .. autofunction:: encode_block
+.. autofunction:: quantize_block
+
+.. autofunction:: compute_scale_amax
+
 
 Classes
 -------
 
 .. autoclass:: FormatInfo()
    :members:
 .. autoclass:: FloatClass()
```

### Comparing `gfloat-0.1/docs/source/conf.py` & `gfloat-0.2/docs/source/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Configuration file for the Sphinx documentation builder.
 
 # -- Project information
 
 project = "GFloat"
 copyright = "2024, Graphcore Ltd"
 author = "Andrew Fitzgibbon"
-release = "0.1"  # Set version in package.sh
-version = "0.1"  # Set version in package.sh
+release = "0.2"  # Set version in package.sh
+version = "0.2"  # Set version in package.sh
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.duration",
     "sphinx.ext.doctest",
     "sphinx.ext.autodoc",
@@ -20,14 +20,24 @@
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx.ext.napoleon",
     "sphinx_paramlinks",
     "myst_nb",
 ]
 
+autodoc_typehints = "none"  # We have them in the parameter descriptors
+autodoc_typehints_format = "short"
+python_use_unqualified_type_names = True
+
+autodoc_type_aliases = {
+    "Iterable": "Iterable",
+    "npt.ArrayLike": "ArrayLike",
+    "npt.NDArray": "NDArray",
+}
+
 autodoc_default_options = {
     "member-order": "bysource",
 }
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "sphinx": ("https://www.sphinx-doc.org/en/master/", None),
```

### Comparing `gfloat-0.1/docs/source/formats.rst` & `gfloat-0.2/docs/source/formats.rst`

 * *Files 15% similar despite different names*

```diff
@@ -27,7 +27,17 @@
 .. autodata:: format_info_ocp_e8m0
 .. autodata:: format_info_ocp_int8
 
 IEEE WG P3109 Formats
 ---------------------
 
 .. autofunction:: format_info_p3109
+
+Block Formats
+---------------------
+
+.. autodata:: format_info_mxfp8_e5m2
+.. autodata:: format_info_mxfp8_e4m3
+.. autodata:: format_info_mxfp6_e3m2
+.. autodata:: format_info_mxfp6_e2m3
+.. autodata:: format_info_mxfp4_e2m1
+.. autodata:: format_info_mxint8
```

### Comparing `gfloat-0.1/docs/source/index.rst` & `gfloat-0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/etc/test-check-copyright.sh` & `gfloat-0.2/etc/test-check-copyright.sh`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/pyproject.toml` & `gfloat-0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,30 +6,35 @@
 
 [tool.setuptools]
 packages = ['gfloat']
 package-dir = {"" = "src"}
 
 [project]
 name =  "gfloat"
-version = "0.1" # Set version in package.sh
+version = "0.2" # Set version in package.sh
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
-dynamic = ["dependencies", "optional-dependencies"]
+dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 # version = {attr = "gfloat.VERSION"} # Wow: https://github.com/pypa/setuptools/issues/1724
 dependencies = {file = ["requirements.txt"]}
-optional-dependencies = {test = {file = ["requirements-test.txt"]}}
+# optional-dependencies = {dev = {file = ["requirements-dev.txt"]}}
 
 [tool.black]
 line-length = 88
 fast = true
+
+[tool.mypy]
+[[tool.mypy.overrides]]
+module = "mx.*"
+ignore_missing_imports = true
```

### Comparing `gfloat-0.1/src/gfloat/decode.py` & `gfloat-0.2/src/gfloat/decode.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/src/gfloat/formats.py` & `gfloat-0.2/src/gfloat/formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,141 +1,141 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
 from .block import BlockFormatInfo
 from .types import FormatInfo
 
 #: FormatInfo for IEEE-754 Binary32 format
 format_info_binary32 = FormatInfo(
-    name="binary32",
+    name="format_info_binary32",
     k=32,
     precision=24,
     emax=127,
     has_nz=True,
     has_infs=True,
     num_high_nans=2**23 - 1,
     has_subnormals=True,
     is_signed=True,
     is_twos_complement=False,
 )
 
 #: FormatInfo for IEEE-754 Binary16 format
 format_info_binary16 = FormatInfo(
-    name="binary16",
+    name="format_info_binary16",
     k=16,
     precision=11,
     emax=15,
     has_nz=True,
     has_infs=True,
     num_high_nans=2**10 - 1,
     has_subnormals=True,
     is_signed=True,
     is_twos_complement=False,
 )
 
 #: FormatInfo for Google BFloat16 format
 format_info_bfloat16 = FormatInfo(
-    name="bfloat16",
+    name="format_info_bfloat16",
     k=16,
     precision=8,
     emax=127,
     has_nz=True,
     has_infs=True,
     num_high_nans=2**7 - 1,
     has_subnormals=True,
     is_signed=True,
     is_twos_complement=False,
 )
 
 #: FormatInfo for OCP E5M2 format
 format_info_ocp_e5m2 = FormatInfo(
-    name="ocp_e5m2",
+    name="format_info_ocp_e5m2",
     k=8,
     precision=3,
     emax=15,
     has_nz=True,
     has_infs=True,
     num_high_nans=2**2 - 1,
     has_subnormals=True,
     is_signed=True,
     is_twos_complement=False,
 )
 
 #: FormatInfo for OCP E4M3 format
 format_info_ocp_e4m3 = FormatInfo(
-    name="ocp_e4m3",
+    name="format_info_ocp_e4m3",
     k=8,
     precision=4,
     emax=8,
     has_nz=True,
     has_infs=False,
     num_high_nans=1,
     has_subnormals=True,
     is_signed=True,
     is_twos_complement=False,
 )
 
 #: FormatInfo for OCP MX E2M3 format
 format_info_ocp_e2m3 = FormatInfo(
-    name="ocp_e2m3",
+    name="format_info_ocp_e2m3",
     k=6,
     precision=4,
     emax=2,
     has_nz=True,
     has_infs=False,
     num_high_nans=0,
     has_subnormals=True,
     is_signed=True,
     is_twos_complement=False,
 )
 
 #: FormatInfo for OCP MX E3M2 format
 format_info_ocp_e3m2 = FormatInfo(
-    name="ocp_e3m2",
+    name="format_info_ocp_e3m2",
     k=6,
     precision=3,
     emax=4,
     has_nz=True,
     has_infs=False,
     num_high_nans=0,
     has_subnormals=True,
     is_signed=True,
     is_twos_complement=False,
 )
 
 #: FormatInfo for OCP MX E2M1 format
 format_info_ocp_e2m1 = FormatInfo(
-    name="ocp_e2m1",
+    name="format_info_ocp_e2m1",
     k=4,
     precision=2,
     emax=2,
     has_nz=True,
     has_infs=False,
     num_high_nans=0,
     has_subnormals=True,
     is_signed=True,
     is_twos_complement=False,
 )
 
 #: FormatInfo for OCP MX E8M0 format
 format_info_ocp_e8m0 = FormatInfo(
-    name="ocp_e8m0",
+    name="format_info_ocp_e8m0",
     k=8,
     precision=1,
     emax=127,
     has_nz=False,
     has_infs=False,
     num_high_nans=1,
     has_subnormals=False,
     is_signed=False,
     is_twos_complement=False,
 )
 
 #: FormatInfo for OCP MX INT8 format
 format_info_ocp_int8 = FormatInfo(
-    name="ocp_int8",
+    name="format_info_ocp_int8",
     k=8,
     precision=8,
     emax=0,
     has_nz=False,
     has_infs=False,
     num_high_nans=0,
     has_subnormals=True,
@@ -206,19 +206,19 @@
     format_info_binary32,
 ]
 
 # ------
 # Block formats
 
 format_info_mxfp8_e5m2 = BlockFormatInfo(
-    "ocp_mxfp8_e5m2", format_info_ocp_e5m2, 32, format_info_ocp_e8m0
+    "format_info_mxfp8_e5m2", format_info_ocp_e5m2, 32, format_info_ocp_e8m0
 )
 
 format_info_mxfp8_e4m3 = BlockFormatInfo(
-    "ocp_mxfp8_e4m3", format_info_ocp_e4m3, 32, format_info_ocp_e8m0
+    "format_info_mxfp8_e4m3", format_info_ocp_e4m3, 32, format_info_ocp_e8m0
 )
 
 format_info_mxfp6_e3m2 = BlockFormatInfo(
     "format_info_mxfp6_e3m2", format_info_ocp_e3m2, 32, format_info_ocp_e8m0
 )
 
 format_info_mxfp6_e2m3 = BlockFormatInfo(
@@ -229,15 +229,19 @@
     "format_info_mxfp4_e2m1", format_info_ocp_e2m1, 32, format_info_ocp_e8m0
 )
 
 format_info_mxfp4_e2m1 = BlockFormatInfo(
     "format_info_mxfp4_e2m1", format_info_ocp_e2m1, 32, format_info_ocp_e8m0
 )
 
+format_info_mxint8 = BlockFormatInfo(
+    "format_info_mxint8", format_info_ocp_int8, 32, format_info_ocp_e8m0
+)
+
 all_block_formats = [
     format_info_mxfp8_e5m2,
     format_info_mxfp8_e4m3,
     format_info_mxfp6_e3m2,
     format_info_mxfp6_e2m3,
     format_info_mxfp4_e2m1,
-    format_info_mxfp4_e2m1,
+    format_info_mxint8,
 ]
```

### Comparing `gfloat-0.1/src/gfloat/printing.py` & `gfloat-0.2/src/gfloat/printing.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/src/gfloat/round.py` & `gfloat-0.2/src/gfloat/round.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/src/gfloat/types.py` & `gfloat-0.2/src/gfloat/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,9 +396,13 @@
     @property
     def is_all_subnormal(self) -> bool:
         """
         Are all encoded values subnormal?
         """
         return (self.expBits == 0) and self.has_subnormals
 
+    @property
+    def __name__(self) -> str:
+        return self.name
+
     def __str__(self) -> str:
         return f"{self.name}"
```

### Comparing `gfloat-0.1/src/gfloat.egg-info/PKG-INFO` & `gfloat-0.2/src/gfloat.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 Metadata-Version: 2.1
 Name: gfloat
-Version: 0.1
+Version: 0.2
 Summary: Generic floating point handling in Python
 Author-email: Andrew Fitzgibbon <awf@fitzgibbon.ie>
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pandas; extra == "test"
-Requires-Dist: ipykernel; extra == "test"
-Requires-Dist: black[jupyter]; extra == "test"
-Requires-Dist: ml_dtypes; extra == "test"
-Requires-Dist: mypy; extra == "test"
-Requires-Dist: pre-commit; extra == "test"
+
+<!-- Copyright (c) 2024 Graphcore Ltd. All rights reserved. -->
 
 # gfloat: Generic floating-point types in Python
 
 An implementation of generic floating point encode/decode logic,
 handling various current and proposed floating point types:
 
  - [IEEE 754](https://en.wikipedia.org/wiki/IEEE_754): Binary16, Binary32
```

### Comparing `gfloat-0.1/src/gfloat.egg-info/SOURCES.txt` & `gfloat-0.2/src/gfloat.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 BUILDING.md
 LICENSE
 README.md
 pyproject.toml
-requirements-test.txt
+requirements-dev.txt
 requirements.txt
 .github/workflows/ci.yaml
 docs/Makefile
 docs/make.bat
 docs/requirements-rtd.txt
-docs/requirements.txt
 docs/source/01-decode.ipynb
 docs/source/02-value-stats.ipynb
 docs/source/03-value-tables.ipynb
 docs/source/api.rst
 docs/source/conf.py
 docs/source/formats.rst
 docs/source/index.rst
@@ -35,9 +34,10 @@
 src/gfloat.egg-info/dependency_links.txt
 src/gfloat.egg-info/requires.txt
 src/gfloat.egg-info/top_level.txt
 test/test_block.py
 test/test_decode.py
 test/test_encode.py
 test/test_finfo.py
+test/test_microxcaling.py
 test/test_printing.py
 test/test_round.py
```

### Comparing `gfloat-0.1/test/test_decode.py` & `gfloat-0.2/test/test_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,23 +179,23 @@
     assert dec(0x01) == fi.smallest
     assert dec(0x7F) == fi.max
     assert dec(0x80) == -2.0
     assert dec(0x80) == fi.min
     assert dec(0xFF) == -fi.smallest
 
 
-@pytest.mark.parametrize("fi", p3109_formats, ids=str)
+@pytest.mark.parametrize("fi", p3109_formats)
 def test_specials(fi: FormatInfo) -> None:
     assert fi.code_of_nan == 0x80
     assert fi.code_of_zero == 0x00
     assert fi.code_of_posinf == 0x7F
     assert fi.code_of_neginf == 0xFF
 
 
-@pytest.mark.parametrize("fi", all_formats, ids=str)
+@pytest.mark.parametrize("fi", all_formats)
 def test_specials_decode(fi: FormatInfo) -> None:
     dec = lambda v: decode_float(fi, v).fval
 
     if fi.has_zero:
         assert dec(fi.code_of_zero) == 0
 
     if fi.num_nans > 0:
@@ -236,15 +236,15 @@
 
 @pytest.mark.parametrize("v", [-1, 0x10000])
 def test_except(v: int) -> None:
     with pytest.raises(ValueError):
         decode_float(format_info_binary16, v)
 
 
-@pytest.mark.parametrize("fi", [fi for fi in all_formats if fi.bits <= 8], ids=str)
+@pytest.mark.parametrize("fi", [fi for fi in all_formats if fi.bits <= 8])
 def test_dense(fi: FormatInfo) -> None:
     fvs = [decode_float(fi, i) for i in range(0, 2**fi.bits)]
 
     vals = np.array([fv.fval for fv in fvs])
 
     assert np.min(vals[np.isfinite(vals)]) == fi.min
     assert np.max(vals[np.isfinite(vals)]) == fi.max
```

### Comparing `gfloat-0.1/test/test_encode.py` & `gfloat-0.2/test/test_encode.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pytest
 
 from gfloat import decode_float, encode_float
 from gfloat.formats import *
 
 
-@pytest.mark.parametrize("fi", all_formats, ids=str)
+@pytest.mark.parametrize("fi", all_formats)
 def test_encode(fi: FormatInfo) -> None:
     dec = lambda v: decode_float(fi, v).fval
 
     if fi.bits <= 8:
         step = 1
     elif fi.bits <= 16:
         step = 13
@@ -23,15 +23,15 @@
         fv = decode_float(fi, i)
         ival = encode_float(fi, fv.fval)
         assert (i == ival) or np.isnan(fv.fval)
         fv2 = decode_float(fi, ival)
         np.testing.assert_equal(fv2.fval, fv.fval)
 
 
-@pytest.mark.parametrize("fi", all_formats, ids=str)
+@pytest.mark.parametrize("fi", all_formats)
 def test_encode_edges(fi: FormatInfo) -> None:
     assert encode_float(fi, fi.max) == fi.code_of_max
 
     assert encode_float(fi, fi.max * 1.25) == (
         fi.code_of_posinf
         if fi.has_infs
         else fi.code_of_nan if fi.num_nans > 0 else fi.code_of_max
```

### Comparing `gfloat-0.1/test/test_finfo.py` & `gfloat-0.2/test/test_finfo.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/test/test_printing.py` & `gfloat-0.2/test/test_printing.py`

 * *Files identical despite different names*

### Comparing `gfloat-0.1/test/test_round.py` & `gfloat-0.2/test/test_round.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 @pytest.mark.parametrize(
     "fi",
     [
         format_info_ocp_e5m2,
         format_info_ocp_e4m3,
         *p3109_formats,
     ],
-    ids=str,
 )
 def test_round(fi: FormatInfo) -> None:
     """
     Test rounding from values between exact binary8 values
     For integer code point i, let
       v0 = the float value at i
       v1 = the float value at i+1, i.e. nextUp(v0)
@@ -180,15 +179,15 @@
     for v in np.arange(289).astype(float):
         val = round_float(fi, v)
 
         mlval = _mlround(v, mldtype)
         np.testing.assert_equal(val, mlval)
 
 
-@pytest.mark.parametrize("fi", all_formats, ids=str)
+@pytest.mark.parametrize("fi", all_formats)
 def test_round_roundtrip(fi: FormatInfo) -> None:
     if fi.bits <= 8:
         step = 1
     elif fi.bits <= 16:
         step = 13
     elif fi.bits <= 32:
         step = 73013
```

