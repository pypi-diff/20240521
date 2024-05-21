# Comparing `tmp/isagog_ai-0.8.7.tar.gz` & `tmp/isagog_ai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.8.7.tar", max compression
+gzip compressed data, was "isagog_ai-0.9.0.tar", max compression
```

## Comparing `isagog_ai-0.8.7.tar` & `isagog_ai-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.7/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.7/isagog/client/__init__.py
--rw-r--r--   0        0        0    10041 2024-04-19 13:29:42.088830 isagog_ai-0.8.7/isagog/client/kg_client.py
--rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.8.7/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.7/isagog/generator/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.7/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.7/isagog/model/__init__.py
--rw-r--r--   0        0        0    26840 2024-04-19 13:44:40.672961 isagog_ai-0.8.7/isagog/model/kg_model.py
--rw-r--r--   0        0        0    27831 2024-04-19 12:58:02.607269 isagog_ai-0.8.7/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.7/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.7/LICENSE
--rw-r--r--   0        0        0      588 2024-04-19 11:39:02.614851 isagog_ai-0.8.7/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.7/README.md
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.9.0/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.9.0/isagog/client/__init__.py
+-rw-r--r--   0        0        0    10041 2024-04-19 13:29:42.088830 isagog_ai-0.9.0/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.9.0/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.9.0/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     5975 2024-05-21 07:41:53.092059 isagog_ai-0.9.0/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.9.0/isagog/model/__init__.py
+-rw-r--r--   0        0        0    26840 2024-04-19 13:44:40.672961 isagog_ai-0.9.0/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    28011 2024-05-21 07:37:08.000395 isagog_ai-0.9.0/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.9.0/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.9.0/LICENSE
+-rw-r--r--   0        0        0      588 2024-05-21 07:33:17.226879 isagog_ai-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.9.0/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.9.0/PKG-INFO
```

### Comparing `isagog_ai-0.8.7/isagog/client/kg_client.py` & `isagog_ai-0.9.0/isagog/client/kg_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.7/isagog/client/nlp_client.py` & `isagog_ai-0.9.0/isagog/client/nlp_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.7/isagog/generator/sparql_generator.py` & `isagog_ai-0.9.0/isagog/generator/sparql_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,18 @@
         """
 
         if not isinstance(query, UnarySelectQuery):
             raise TypeError("Can only generate_query from UnarySelectQuery")
 
         strio = StringIO()
         for (name, uri) in query.prefixes:
-            strio.write(f"PREFIX {name}: <{uri}#>\n")
+            if uri.endswith("#") or uri.endswith("/"):
+                strio.write(f"PREFIX {name}: <{uri}>\n")
+            else:
+                strio.write(f"PREFIX {name}: <{uri}#>\n")
 
         strio.write("SELECT distinct ")  # {query.subject}")
         for rv in query.project_vars():
             strio.write(f" {rv} ")
         if query.is_scored():
             strio.write(f" ?{_SCOREVAR} ")
         strio.write(" WHERE {\n")
```

### Comparing `isagog_ai-0.8.7/isagog/model/kg_model.py` & `isagog_ai-0.9.0/isagog/model/kg_model.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.7/isagog/model/kg_query.py` & `isagog_ai-0.9.0/isagog/model/kg_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,17 @@
             for c in clauses:
                 self.clauses.append(c)
         self.graph = graph
         self.limit = limit
         self.lang = lang
         self.min_score = min_score
 
+    def add_prefix(self, prefix: str, uri: str):
+        self.prefixes.append((prefix, uri))
+
     def add(self, clauses: Clause | list[Clause], **kwargs):
         if isinstance(clauses, list):
             match kwargs.get('type', 'conjunction'):
                 case 'conjunction':
                     list_clause = ConjunctiveClause(clauses, optional=kwargs.get('optional', False))
                 case 'union':
                     list_clause = DisjunctiveClause(subject=kwargs.get('subject'), clauses=clauses)
@@ -695,14 +698,16 @@
     def from_dict(self, data: dict):
         """
            Openapi spec:  components.schemas.Clause
         """
         try:
             for key, val in data.items():
                 match key:
+                    case 'prefixes':
+                        self.prefixes = val
                     case 'subject':
                         self.subject = self._new_id(val)
                     case 'kind' | 'kinds':  # backward compatibility w 0.7
                         self.add_kinds(val)
                     case 'clauses':
                         for clause_data in val:
                             match clause_data.get('type'):
```

### Comparing `isagog_ai-0.8.7/LICENSE` & `isagog_ai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.7/pyproject.toml` & `isagog_ai-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 382e 3722 0d0a 6465 7363 7269 7074 696f  8.7"..descriptio
+00000030: 392e 3022 0d0a 6465 7363 7269 7074 696f  9.0"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
@@ -18,18 +18,18 @@
 00000110: 2022 6973 6167 6f67 2f6d 6f64 656c 227d   "isagog/model"}
 00000120: 0d0a 2020 2020 2020 2020 2020 205d 0d0a  ..           ]..
 00000130: 0d0a 0d0a 5b74 6f6f 6c2e 706f 6574 7279  ....[tool.poetry
 00000140: 2e64 6570 656e 6465 6e63 6965 735d 0d0a  .dependencies]..
 00000150: 7079 7468 6f6e 203d 2022 5e33 2e31 3022  python = "^3.10"
 00000160: 0d0a 7264 666c 6962 203d 2022 5e37 2e30  ..rdflib = "^7.0
 00000170: 2e30 220d 0a72 6571 7565 7374 7320 3d20  .0"..requests = 
-00000180: 225e 322e 3238 2e32 220d 0a75 726c 6c69  "^2.28.2"..urlli
+00000180: 225e 322e 3332 2e31 220d 0a75 726c 6c69  "^2.32.1"..urlli
 00000190: 6233 203d 2022 5e32 2e30 2e36 220d 0a74  b3 = "^2.0.6"..t
 000001a0: 6f6d 6c20 3d20 225e 302e 3130 2e32 220d  oml = "^0.10.2".
-000001b0: 0a70 7974 6573 7420 3d20 225e 382e 312e  .pytest = "^8.1.
+000001b0: 0a70 7974 6573 7420 3d20 225e 382e 322e  .pytest = "^8.2.
 000001c0: 3122 0d0a 7079 7468 6f6e 2d64 6f74 656e  1"..python-doten
 000001d0: 7620 3d20 225e 312e 302e 3022 0d0a 6874  v = "^1.0.0"..ht
 000001e0: 7470 7820 3d20 225e 302e 3237 2e30 220d  tpx = "^0.27.0".
 000001f0: 0a0d 0a0d 0a5b 6275 696c 642d 7379 7374  .....[build-syst
 00000200: 656d 5d0d 0a72 6571 7569 7265 7320 3d20  em]..requires = 
 00000210: 5b22 706f 6574 7279 2d63 6f72 6522 5d0d  ["poetry-core"].
 00000220: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
```

### Comparing `isagog_ai-0.8.7/PKG-INFO` & `isagog_ai-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.8.7
+Version: 0.9.0
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: pytest (>=8.1.1,<9.0.0)
+Requires-Dist: pytest (>=8.2.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.32.1,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: urllib3 (>=2.0.6,<3.0.0)
 Description-Content-Type: text/markdown
 
 # isagog-ai-cli
 Client for isagog ai services
```

