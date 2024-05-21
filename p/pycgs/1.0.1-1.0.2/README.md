# Comparing `tmp/pycgs-1.0.1.tar.gz` & `tmp/pycgs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycgs-1.0.1.tar", max compression
+gzip compressed data, was "pycgs-1.0.2.tar", max compression
```

## Comparing `pycgs-1.0.1.tar` & `pycgs-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-12-20 13:38:05.351111 pycgs-1.0.1/LICENSE
--rw-r--r--   0        0        0     1831 2024-05-20 13:14:47.762406 pycgs-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-12-28 06:21:20.171976 pycgs-1.0.1/pycgs/__init__.py
--rw-r--r--   0        0        0     3062 2024-05-20 13:00:11.369246 pycgs-1.0.1/pycgs/cgs.py
--rw-r--r--   0        0        0      158 2023-12-28 06:21:18.689937 pycgs-1.0.1/pycgs/type.py
--rw-r--r--   0        0        0      630 2024-05-20 12:41:52.701775 pycgs-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 pycgs-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-20 13:38:05.351111 pycgs-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1831 2024-05-20 13:14:47.762406 pycgs-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-12-28 06:21:20.171976 pycgs-1.0.2/pycgs/__init__.py
+-rw-r--r--   0        0        0     3074 2024-05-21 13:51:30.627343 pycgs-1.0.2/pycgs/cgs.py
+-rw-r--r--   0        0        0      158 2023-12-28 06:21:18.689937 pycgs-1.0.2/pycgs/type.py
+-rw-r--r--   0        0        0      630 2024-05-21 13:54:10.225316 pycgs-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 pycgs-1.0.2/PKG-INFO
```

### Comparing `pycgs-1.0.1/LICENSE` & `pycgs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycgs-1.0.1/README.md` & `pycgs-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pycgs-1.0.1/pycgs/cgs.py` & `pycgs-1.0.2/pycgs/cgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pycgs.type import Edge, EdgeWithWeight
 
 
 __all__ = ["foundational_cgs", "weighted_cgs"]
 
 
-def foundational_cgs(relationships: list[Edge]) -> dict[str, str]:
+def foundational_cgs(relationships: list[Edge] | set[Edge]) -> dict[str, str]:
     """
     Foundational CGS algorithm.
     """
     # Create a Directed Acyclic Graph
     cptg = nx.DiGraph()  # CPTG: Coreference-based Primary Term Graph
 
     # Add edges to the graph based on the coreference relationships
```

### Comparing `pycgs-1.0.1/pyproject.toml` & `pycgs-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycgs"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python implementation of the Coreference-based Graph Search (CGS) algorithm."
 authors = ["YANG Zijie <yangzijie@westlake.edu.cn>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `pycgs-1.0.1/PKG-INFO` & `pycgs-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycgs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python implementation of the Coreference-based Graph Search (CGS) algorithm.
 License: Apache-2.0
 Author: YANG Zijie
 Author-email: yangzijie@westlake.edu.cn
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

