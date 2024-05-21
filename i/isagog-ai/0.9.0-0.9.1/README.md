# Comparing `tmp/isagog_ai-0.9.0.tar.gz` & `tmp/isagog_ai-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.9.0.tar", max compression
+gzip compressed data, was "isagog_ai-0.9.1.tar", max compression
```

## Comparing `isagog_ai-0.9.0.tar` & `isagog_ai-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.9.0/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.9.0/isagog/client/__init__.py
--rw-r--r--   0        0        0    10041 2024-04-19 13:29:42.088830 isagog_ai-0.9.0/isagog/client/kg_client.py
--rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.9.0/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.9.0/isagog/generator/__init__.py
--rw-r--r--   0        0        0     5975 2024-05-21 07:41:53.092059 isagog_ai-0.9.0/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.9.0/isagog/model/__init__.py
--rw-r--r--   0        0        0    26840 2024-04-19 13:44:40.672961 isagog_ai-0.9.0/isagog/model/kg_model.py
--rw-r--r--   0        0        0    28011 2024-05-21 07:37:08.000395 isagog_ai-0.9.0/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.9.0/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.9.0/LICENSE
--rw-r--r--   0        0        0      588 2024-05-21 07:33:17.226879 isagog_ai-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.9.0/README.md
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.9.1/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.9.1/isagog/client/__init__.py
+-rw-r--r--   0        0        0    10041 2024-04-19 13:29:42.088830 isagog_ai-0.9.1/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.9.1/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.9.1/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     6140 2024-05-21 08:58:37.658038 isagog_ai-0.9.1/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.9.1/isagog/model/__init__.py
+-rw-r--r--   0        0        0    26840 2024-04-19 13:44:40.672961 isagog_ai-0.9.1/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    28060 2024-05-21 08:55:34.747544 isagog_ai-0.9.1/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.9.1/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.9.1/LICENSE
+-rw-r--r--   0        0        0      588 2024-05-21 08:41:15.435406 isagog_ai-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.9.1/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.9.1/PKG-INFO
```

### Comparing `isagog_ai-0.9.0/isagog/client/kg_client.py` & `isagog_ai-0.9.1/isagog/client/kg_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.0/isagog/client/nlp_client.py` & `isagog_ai-0.9.1/isagog/client/nlp_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.0/isagog/generator/sparql_generator.py` & `isagog_ai-0.9.1/isagog/generator/sparql_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 SPARQL query generator
 (c) Isagog S.r.l. 2024, MIT License
 """
 from io import StringIO
 
 from isagog.model.kg_model import Assertion
 from isagog.model.kg_query import UnarySelectQuery, AtomicClause, Comparison, Variable, \
-    ConjunctiveClause, DisjunctiveClause, _SCOREVAR, SelectQuery
+    ConjunctiveClause, DisjunctiveClause, _SCOREVAR, SelectQuery, META_PROPERTIES
 from isagog.model.kg_query import Generator, Clause
 
 
 class SPARQLGenerator(Generator):
     """
     SPARQL query generator
     """
@@ -20,14 +20,17 @@
         if isinstance(clause, AtomicClause):
             """
             Generates the sparql triple clause
             """
             if not clause.is_defined():
                 raise ValueError(f"Clause not defined {clause.subject} {clause.property} {clause.argument}")
 
+            if str(clause.property) == META_PROPERTIES.IN.value:
+                return f"FILTER ({clause.subject} IN ({clause.argument})) .\n"
+
             clause_str = ""
 
             match Comparison(clause.method):
                 case Comparison.EXACT | Comparison.ANY:
                     clause_str += clause.n3()  # f"{self.subject} {self.property} {self.argument}"
                 case Comparison.REGEX:
                     tmp_var = Variable()  # self._temp_var()
```

### Comparing `isagog_ai-0.9.0/isagog/model/kg_model.py` & `isagog_ai-0.9.1/isagog/model/kg_model.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.0/isagog/model/kg_query.py` & `isagog_ai-0.9.1/isagog/model/kg_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 # don't change this for the sake of back compatibility
 _SUBJVAR = 'i'
 _KINDVAR = 'k'
 _SCOREVAR = 'score'
 
 
+class META_PROPERTIES(Enum):
+    IN = "IN"
+
+
 def is_uri(string: str) -> bool:
     parsed = urlparse(string)
     return bool(parsed.scheme) and bool(parsed.netloc)
 
 
 def is_variable(string: str) -> bool:
     return string.startswith('?')
```

### Comparing `isagog_ai-0.9.0/LICENSE` & `isagog_ai-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.0/pyproject.toml` & `isagog_ai-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 392e 3022 0d0a 6465 7363 7269 7074 696f  9.0"..descriptio
+00000030: 392e 3122 0d0a 6465 7363 7269 7074 696f  9.1"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
```

### Comparing `isagog_ai-0.9.0/PKG-INFO` & `isagog_ai-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.9.0
+Version: 0.9.1
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

