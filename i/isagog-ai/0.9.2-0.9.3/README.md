# Comparing `tmp/isagog_ai-0.9.2.tar.gz` & `tmp/isagog_ai-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.9.2.tar", max compression
+gzip compressed data, was "isagog_ai-0.9.3.tar", max compression
```

## Comparing `isagog_ai-0.9.2.tar` & `isagog_ai-0.9.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.9.2/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.9.2/isagog/client/__init__.py
--rw-r--r--   0        0        0    10041 2024-04-19 13:29:42.088830 isagog_ai-0.9.2/isagog/client/kg_client.py
--rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.9.2/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.9.2/isagog/generator/__init__.py
--rw-r--r--   0        0        0     6140 2024-05-21 08:58:37.658038 isagog_ai-0.9.2/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.9.2/isagog/model/__init__.py
--rw-r--r--   0        0        0    26840 2024-04-19 13:44:40.672961 isagog_ai-0.9.2/isagog/model/kg_model.py
--rw-r--r--   0        0        0    28099 2024-05-21 09:16:34.959082 isagog_ai-0.9.2/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.9.2/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.9.2/LICENSE
--rw-r--r--   0        0        0      588 2024-05-21 09:16:34.949078 isagog_ai-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.9.2/README.md
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.9.3/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.9.3/isagog/client/__init__.py
+-rw-r--r--   0        0        0    10041 2024-04-19 13:29:42.088830 isagog_ai-0.9.3/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.9.3/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.9.3/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     6143 2024-05-21 12:46:12.375292 isagog_ai-0.9.3/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.9.3/isagog/model/__init__.py
+-rw-r--r--   0        0        0    26840 2024-04-19 13:44:40.672961 isagog_ai-0.9.3/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    28814 2024-05-21 13:31:29.745368 isagog_ai-0.9.3/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.9.3/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.9.3/LICENSE
+-rw-r--r--   0        0        0      588 2024-05-21 13:16:07.311372 isagog_ai-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.9.3/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.9.3/PKG-INFO
```

### Comparing `isagog_ai-0.9.2/isagog/client/kg_client.py` & `isagog_ai-0.9.3/isagog/client/kg_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.2/isagog/client/nlp_client.py` & `isagog_ai-0.9.3/isagog/client/nlp_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.2/isagog/generator/sparql_generator.py` & `isagog_ai-0.9.3/isagog/generator/sparql_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             return clause_str
         elif isinstance(clause, ConjunctiveClause):
             strio = StringIO()
             if len(clause.clauses) > 1:
                 if clause.optional:
                     strio.write("OPTIONAL")
                 strio.write("\t{\n")
-                for sub_clause in clause.clauses[1:]:
+                for sub_clause in clause.clauses: #[1:]:
                     strio.write("\t\t\t" + self.generate_clause(sub_clause))  # sub_clause.to_sparql())
                 strio.write("\t\t}\n")
                 # strio.write("\t}\n")
             else:
                 strio.write("\t\t\t" + self.generate_clause(clause.clauses[0]))  # clause.clauses[0].to_sparql())
 
             return strio.getvalue()
```

### Comparing `isagog_ai-0.9.2/isagog/model/kg_model.py` & `isagog_ai-0.9.3/isagog/model/kg_model.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.2/isagog/model/kg_query.py` & `isagog_ai-0.9.3/isagog/model/kg_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -537,27 +537,34 @@
         # clause_obj.from_dict(kwargs)
         self.add(atomic_clause)
         return self
 
     def project_clauses(self) -> list[AtomicClause]:
         return [c for c in self.clauses if isinstance(c, AtomicClause) and c.project]
 
-    def project_vars(self) -> set[str]:
-        """
-        Selects all the projectes arguments
-        """
-        _vars = []
-        for c in self.clauses:
+    def _project_vars(self, c: Clause, _vars: list[str]):
+        if isinstance(c, AtomicClause) and c.project:
             if isinstance(c, AtomicClause) and c.project:
                 if c.variable and not c.argument:
                     _vars.append(c.variable)
                 elif isinstance(c.argument, Variable):
                     _vars.append(c.argument)
                 if isinstance(c.subject, Variable):
                     _vars.append(c.subject)
+        elif isinstance(c, ConjunctiveClause) or isinstance(c, DisjunctiveClause):
+            for c in c.clauses:
+                self._project_vars(c, _vars)
+
+    def project_vars(self) -> set[str]:
+        """
+        Selects all the projectes arguments
+        """
+        _vars = []
+        for c in self.clauses:
+            self._project_vars(c, _vars)
         return set(_vars)
 
     def has_return_vars(self) -> bool:
         return len(self.project_vars()) > 0
 
     def generate(self, generator: Generator) -> str:
         return generator.generate_query(self)
@@ -620,18 +627,27 @@
         if kinds:
             self.add(AtomicClause(subject=self.subject,
                                   property=RDF_TYPE,
                                   argument=Variable(_KINDVAR),
                                   project=True))
             self.add_kinds(kinds)
 
+    def _fix_subject(self, clause: Clause):
+        if isinstance(clause, AtomicClause) and clause.subject is None:
+            clause.subject = self.subject
+        elif isinstance(clause, ConjunctiveClause) or isinstance(clause, DisjunctiveClause):
+            for c in clause.clauses:
+                self._fix_subject(c)
+
     def add(self, clauses: Clause | list[Clause], **kwargs):
         if isinstance(clauses, Clause):
-            if clauses.subject is None:
-                clauses.subject = self.subject
+            self._fix_subject(clauses)
+        elif isinstance(clauses, list):
+            for c in clauses:
+                self._fix_subject(c)
         super().add(clauses, **kwargs)
 
     def clause(self,
                property: Identifier | str,
                subject: Identifier | Variable | str = None,
                argument: str | int | float | Value | Identifier | Variable = None,
                variable: Variable | str = None,
```

### Comparing `isagog_ai-0.9.2/LICENSE` & `isagog_ai-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.9.2/pyproject.toml` & `isagog_ai-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 392e 3222 0d0a 6465 7363 7269 7074 696f  9.2"..descriptio
+00000030: 392e 3322 0d0a 6465 7363 7269 7074 696f  9.3"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
```

### Comparing `isagog_ai-0.9.2/PKG-INFO` & `isagog_ai-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.9.2
+Version: 0.9.3
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

