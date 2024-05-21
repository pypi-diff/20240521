# Comparing `tmp/fizzysearch-0.3.tar.gz` & `tmp/fizzysearch-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fizzysearch-0.3.tar", max compression
+gzip compressed data, was "fizzysearch-0.4.tar", max compression
```

## Comparing `fizzysearch-0.3.tar` & `fizzysearch-0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1152 2024-02-29 13:36:33.804542 fizzysearch-0.3/LICENSE
--rw-r--r--   0        0        0     1959 2024-05-17 02:53:44.403985 fizzysearch-0.3/README.md
--rw-r--r--   0        0        0     3063 2024-05-17 21:53:37.774091 fizzysearch-0.3/fizzysearch.py
--rw-r--r--   0        0        0      304 2024-05-17 21:54:10.410300 fizzysearch-0.3/pyproject.toml
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 fizzysearch-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1152 2024-02-29 13:36:33.804542 fizzysearch-0.4/LICENSE
+-rw-r--r--   0        0        0     1959 2024-05-17 02:53:44.403985 fizzysearch-0.4/README.md
+-rw-r--r--   0        0        0     3063 2024-05-17 21:53:37.774091 fizzysearch-0.4/fizzysearch.py
+-rw-r--r--   0        0        0      305 2024-05-21 06:41:35.412876 fizzysearch-0.4/pyproject.toml
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 fizzysearch-0.4/PKG-INFO
```

### Comparing `fizzysearch-0.3/LICENSE` & `fizzysearch-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fizzysearch-0.3/README.md` & `fizzysearch-0.4/README.md`

 * *Files identical despite different names*

### Comparing `fizzysearch-0.3/fizzysearch.py` & `fizzysearch-0.4/fizzysearch.py`

 * *Files identical despite different names*

### Comparing `fizzysearch-0.3/PKG-INFO` & `fizzysearch-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fizzysearch
-Version: 0.3
+Version: 0.4
 Summary: A SPARQL rewriter that performs enhanced searches
 Home-page: https://github.com/ISE-FIZKarlsruhe/fizzysearch
 License: MIT
 Author: Etienne Posthumus
 Author-email: ep@epoz.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

