# Comparing `tmp/pynrw-1.4.1.tar.gz` & `tmp/pynrw-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrw-1.4.1.tar", last modified: Sat May 18 14:54:13 2024, max compression
+gzip compressed data, was "pynrw-1.4.2.tar", last modified: Tue May 21 00:25:30 2024, max compression
```

## Comparing `pynrw-1.4.1.tar` & `pynrw-1.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:54:13.842595 pynrw-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-18 14:54:04.000000 pynrw-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-18 14:54:13.842595 pynrw-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-05-18 14:54:04.000000 pynrw-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:54:13.834595 pynrw-1.4.1/nrw/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:54:13.838595 pynrw-1.4.1/nrw/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/algorithms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/algorithms/_searching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/algorithms/_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/algorithms/_traversal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:54:13.838595 pynrw-1.4.1/nrw/database/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/_query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/_query_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/msaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/msaccess.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/mysql.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/database/sqlite.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:54:13.842595 pynrw-1.4.1/nrw/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_comparable_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/datastructures/_vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:54:13.842595 pynrw-1.4.1/nrw/network/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/network/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/network/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/network/_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15286 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/network/_server.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:54:04.000000 pynrw-1.4.1/nrw/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:54:13.842595 pynrw-1.4.1/pynrw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-18 14:54:13.000000 pynrw-1.4.1/pynrw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-18 14:54:13.000000 pynrw-1.4.1/pynrw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:54:13.000000 pynrw-1.4.1/pynrw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-18 14:54:13.000000 pynrw-1.4.1/pynrw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 14:54:13.000000 pynrw-1.4.1/pynrw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-18 14:54:04.000000 pynrw-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-18 14:54:04.000000 pynrw-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:54:13.842595 pynrw-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.750676 pynrw-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-21 00:25:15.000000 pynrw-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-21 00:25:30.750676 pynrw-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-21 00:25:15.000000 pynrw-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.746676 pynrw-1.4.2/nrw/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.746676 pynrw-1.4.2/nrw/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/_searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/_traversal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.746676 pynrw-1.4.2/nrw/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/_query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/msaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/msaccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/sqlite.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.750676 pynrw-1.4.2/nrw/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_comparable_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.750676 pynrw-1.4.2/nrw/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.750676 pynrw-1.4.2/pynrw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-21 00:25:15.000000 pynrw-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-21 00:25:15.000000 pynrw-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 00:25:30.750676 pynrw-1.4.2/setup.cfg
```

### Comparing `pynrw-1.4.1/LICENSE` & `pynrw-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/PKG-INFO` & `pynrw-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.4.1
+Version: 1.4.2
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Project-URL: Source, https://github.com/realshouzy/pynrw
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -36,15 +36,15 @@
 [![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-This package implements the datastructures and database classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
+This package implements the datastructures, database and network classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
 
 **Dieses Package dient alleine zu Bildungszwecken und sollte nicht in Produktion genutzt werden!**
 
 ## Installation
 
 ```bash
 pip install pynrw
```

### Comparing `pynrw-1.4.1/README.md` & `pynrw-1.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-This package implements the datastructures and database classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
+This package implements the datastructures, database and network classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
 
 **Dieses Package dient alleine zu Bildungszwecken und sollte nicht in Produktion genutzt werden!**
 
 ## Installation
 
 ```bash
 pip install pynrw
```

### Comparing `pynrw-1.4.1/nrw/algorithms/__init__.py` & `pynrw-1.4.2/nrw/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/algorithms/__init__.pyi` & `pynrw-1.4.2/nrw/algorithms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/algorithms/_searching.py` & `pynrw-1.4.2/nrw/algorithms/_searching.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/algorithms/_sorting.py` & `pynrw-1.4.2/nrw/algorithms/_sorting.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/algorithms/_traversal.py` & `pynrw-1.4.2/nrw/algorithms/_traversal.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/database/_query_result.py` & `pynrw-1.4.2/nrw/database/_query_result.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/database/_query_result.pyi` & `pynrw-1.4.2/nrw/database/_query_result.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/database/msaccess.py` & `pynrw-1.4.2/nrw/database/msaccess.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/database/msaccess.pyi` & `pynrw-1.4.2/nrw/database/msaccess.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/database/mysql.py` & `pynrw-1.4.2/nrw/database/mysql.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/database/mysql.pyi` & `pynrw-1.4.2/nrw/database/mysql.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/database/sqlite.py` & `pynrw-1.4.2/nrw/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/database/sqlite.pyi` & `pynrw-1.4.2/nrw/database/sqlite.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/__init__.py` & `pynrw-1.4.2/nrw/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/__init__.pyi` & `pynrw-1.4.2/nrw/datastructures/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_binary_search_tree.py` & `pynrw-1.4.2/nrw/datastructures/_binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_binary_tree.py` & `pynrw-1.4.2/nrw/datastructures/_binary_tree.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_comparable_content.py` & `pynrw-1.4.2/nrw/datastructures/_comparable_content.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_edge.py` & `pynrw-1.4.2/nrw/datastructures/_edge.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_graph.py` & `pynrw-1.4.2/nrw/datastructures/_graph.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_list.py` & `pynrw-1.4.2/nrw/datastructures/_list.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_queue.py` & `pynrw-1.4.2/nrw/datastructures/_queue.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_stack.py` & `pynrw-1.4.2/nrw/datastructures/_stack.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_utils.py` & `pynrw-1.4.2/nrw/datastructures/_utils.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/datastructures/_vertex.py` & `pynrw-1.4.2/nrw/datastructures/_vertex.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/network/__init__.pyi` & `pynrw-1.4.2/nrw/network/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/network/_client.py` & `pynrw-1.4.2/nrw/network/_client.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/network/_connection.py` & `pynrw-1.4.2/nrw/network/_connection.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/nrw/network/_server.py` & `pynrw-1.4.2/nrw/network/_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,52 +32,47 @@
         server: Server,
     ) -> None:
         super().__init__()
         self._server: weakref.ProxyType[Server] = weakref.proxy(
             server,
             self._on_server_shutdown,
         )
-        self._active: bool = False
-        self._server_socket: socket.socket | None = None
-        with suppress(Exception):
-            self._server_socket = socket.socket(
+        try:
+            self._server_socket: socket.socket | None = socket.socket(
                 socket.AF_INET,
                 socket.SOCK_STREAM,
             )
             self._server_socket.bind(("127.0.0.1", port))
             self._server_socket.listen()
             self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            self._active = True
+            self._active: bool = True
             self.start()
+        except Exception:  # pylint: disable=W0718
+            self._active = False
+            self._server_socket = None
 
     def _on_server_shutdown(
         self,
         server: Server,  # noqa: ARG002 # pylint: disable=W0613
     ) -> None:
         self.close()
 
     @override
     def run(self) -> None:
         while self._active:
-            with suppress(OSError):
-                try:
-                    client_socket, (client_ip, client_port) = (
-                        self._server_socket.accept()
-                    )
-                    self._server._add_new_client_message_handler(client_socket)
-                    self._server.process_new_connection(client_ip, client_port)
-                except ReferenceError:
-                    self.close()
+            with suppress(OSError, ReferenceError):
+                client_socket, (client_ip, client_port) = self._server_socket.accept()
+                self._server._add_new_client_message_handler(client_socket)
+                self._server.process_new_connection(client_ip, client_port)
 
     def close(self) -> None:
-        if self._active:
-            self._active = False
-            if self._server_socket is not None:
-                with suppress(OSError):
-                    self._server_socket.close()
+        self._active = False
+        if self._server_socket is not None:
+            with suppress(OSError):
+                self._server_socket.close()
 
 
 class _ClientSocketWrapper:
     __slots__: Final[tuple[str, str, str]] = (
         "_client_socket",
         "_to_client",
         "_from_client",
@@ -163,30 +158,28 @@
     @override
     def run(self) -> None:
         message: str | None = None
         while self._active:
             message = self._socket_wrapper.receive()
             client_ip: str | None = self._socket_wrapper.client_ip
             client_port: int = self._socket_wrapper.client_port
-            try:
+            with suppress(ReferenceError):
                 if message is not None:
                     self._server.process_message(client_ip, client_port, message)
                 else:
                     message_handler: _ClientMessageHandler | None = (
                         self._server._find_client_message_handler(
                             client_ip,
                             client_port,
                         )
                     )
                     if message_handler is not None:
                         message_handler.close()
                         self._server._remove_client_message_handler(message_handler)
                         self._server.process_closing_connection(client_ip, client_port)
-            except ReferenceError:
-                self.close()
 
     def send(self, message: str) -> None:
         if self._active:
             self._socket_wrapper.send(message)
 
     def close(self) -> None:
         if self._active:
@@ -281,15 +274,18 @@
         return self._connection_handler._active
 
     def is_connected_to(self, client_ip: str, client_port: int) -> bool:
         """Die Anfrage liefert den Wert `True`, wenn der Server mit dem durch
         `client_ip` und `client_port` spezifizierten Client aktuell verbunden ist.
         Ansonsten liefert die Methode den Wert `False`.
         """
-        return self._find_client_message_handler(client_ip, client_port) is not None
+        message_handler: _ClientMessageHandler | None = (
+            self._find_client_message_handler(client_ip, client_port)
+        )
+        return message_handler is not None and message_handler._active
 
     def send(self, client_ip: str, client_port: int, message: str) -> None:
         """Die Nachricht `message` wird - um einen Zeilentrenner erweitert - an den
         durch `client_ip` und `client_port` spezifizierten Client gesendet. Schlägt der
         Versand fehl, geschieht nichts.
         """
         message_handler: _ClientMessageHandler | None = (
@@ -337,16 +333,16 @@
                     self._message_handlers.content
                 )
                 assert message_handler is not None
                 self.process_closing_connection(
                     message_handler.client_ip,
                     message_handler.client_port,
                 )
+                message_handler.close()
                 self._message_handlers.remove()
-                self._message_handlers.next()
 
     @abstractmethod
     def process_new_connection(
         self,
         client_ip: str,
         client_port: int,
     ) -> None:
```

### Comparing `pynrw-1.4.1/pynrw.egg-info/PKG-INFO` & `pynrw-1.4.2/pynrw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.4.1
+Version: 1.4.2
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Project-URL: Source, https://github.com/realshouzy/pynrw
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -36,15 +36,15 @@
 [![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-This package implements the datastructures and database classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
+This package implements the datastructures, database and network classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
 
 **Dieses Package dient alleine zu Bildungszwecken und sollte nicht in Produktion genutzt werden!**
 
 ## Installation
 
 ```bash
 pip install pynrw
```

### Comparing `pynrw-1.4.1/pynrw.egg-info/SOURCES.txt` & `pynrw-1.4.2/pynrw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.1/pyproject.toml` & `pynrw-1.4.2/pyproject.toml`

 * *Files identical despite different names*

