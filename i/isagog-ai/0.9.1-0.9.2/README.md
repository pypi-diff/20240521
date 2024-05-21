# Comparing `tmp/isagog_ai-0.9.1.tar.gz` & `tmp/isagog_ai-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.9.1.tar", max compression
+gzip compressed data, was "isagog_ai-0.9.2.tar", max compression
```

## Comparing `isagog_ai-0.9.1.tar` & `isagog_ai-0.9.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.9.1/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.9.1/isagog/client/__init__.py
--rw-r--r--   0        0        0    10041 2024-04-19 13:29:42.088830 isagog_ai-0.9.1/isagog/client/kg_client.py
--rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.9.1/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.9.1/isagog/generator/__init__.py
--rw-r--r--   0        0        0     6140 2024-05-21 08:58:37.658038 isagog_ai-0.9.1/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.9.1/isagog/model/__init__.py
--rw-r--r--   0        0        0    26840 2024-04-19 13:44:40.672961 isagog_ai-0.9.1/isagog/model/kg_model.py
--rw-r--r--   0        0        0    28060 2024-05-21 08:55:34.747544 isagog_ai-0.9.1/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.9.1/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.9.1/LICENSE
--rw-r--r--   0        0        0      588 2024-05-21 08:41:15.435406 isagog_ai-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.9.1/README.md
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.9.2/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.9.2/isagog/client/__init__.py
+-rw-r--r--   0        0        0    10041 2024-04-19 13:29:42.088830 isagog_ai-0.9.2/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.9.2/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.9.2/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     6140 2024-05-21 08:58:37.658038 isagog_ai-0.9.2/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.9.2/isagog/model/__init__.py
+-rw-r--r--   0        0        0    26840 2024-04-19 13:44:40.672961 isagog_ai-0.9.2/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    28099 2024-05-21 09:16:34.959082 isagog_ai-0.9.2/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.9.2/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.9.2/LICENSE
+-rw-r--r--   0        0        0      588 2024-05-21 09:16:34.949078 isagog_ai-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.9.2/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.9.2/PKG-INFO
```

### Comparing `isagog_ai-0.9.1/isagog/client/kg_client.py` & `isagog_ai-0.9.2/isagog/client/kg_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.1/isagog/client/nlp_client.py` & `isagog_ai-0.9.2/isagog/client/nlp_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.1/isagog/generator/sparql_generator.py` & `isagog_ai-0.9.2/isagog/generator/sparql_generator.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.1/isagog/model/kg_model.py` & `isagog_ai-0.9.2/isagog/model/kg_model.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.1/isagog/model/kg_query.py` & `isagog_ai-0.9.2/isagog/model/kg_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -749,15 +749,15 @@
 
         out = {}
 
         version = kwargs.get('version')
 
         if not version or version > "1.0.0":
             out['subject'] = self.subject
-
+        out['prefixes'] = self.prefixes
         out['clauses'] = [c.to_dict(version=version) for c in self.clauses]
         out['graph'] = self.graph
         out['limit'] = self.limit
         out['lang'] = self.lang
         if self.min_score:
             out['min_score'] = self.min_score
         return out
```

### Comparing `isagog_ai-0.9.1/LICENSE` & `isagog_ai-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.1/pyproject.toml` & `isagog_ai-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 392e 3122 0d0a 6465 7363 7269 7074 696f  9.1"..descriptio
+00000030: 392e 3222 0d0a 6465 7363 7269 7074 696f  9.2"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
```

### Comparing `isagog_ai-0.9.1/PKG-INFO` & `isagog_ai-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.9.1
+Version: 0.9.2
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

