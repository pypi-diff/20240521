# Comparing `tmp/datasiphon-0.2.5.tar.gz` & `tmp/datasiphon-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasiphon-0.2.5.tar", last modified: Tue May 21 07:52:53 2024, max compression
+gzip compressed data, was "datasiphon-0.2.6.tar", last modified: Tue May 21 09:06:35 2024, max compression
```

## Comparing `datasiphon-0.2.5.tar` & `datasiphon-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.256548 datasiphon-0.2.5/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 07:52:53.256548 datasiphon-0.2.5/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.5/README.md
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.5/pyproject.toml
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 07:52:53.256548 datasiphon-0.2.5/setup.cfg
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.255548 datasiphon-0.2.5/src/
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.256548 datasiphon-0.2.5/src/datasiphon.egg-info/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/SOURCES.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/dependency_links.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/requires.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/top_level.txt
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.256548 datasiphon-0.2.5/src/siphon/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 07:52:31.000000 datasiphon-0.2.5/src/siphon/__init__.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.5/src/siphon/base.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.5/src/siphon/nosql.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    33994 2024-05-21 07:52:31.000000 datasiphon-0.2.5/src/siphon/sql.py
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.256548 datasiphon-0.2.5/tests/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    24780 2024-05-21 07:52:31.000000 datasiphon-0.2.5/tests/test_sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.426194 datasiphon-0.2.6/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 09:06:35.426194 datasiphon-0.2.6/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.6/README.md
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.6/pyproject.toml
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 09:06:35.426194 datasiphon-0.2.6/setup.cfg
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.424194 datasiphon-0.2.6/src/
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.425194 datasiphon-0.2.6/src/datasiphon.egg-info/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/SOURCES.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/dependency_links.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/requires.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/top_level.txt
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.425194 datasiphon-0.2.6/src/siphon/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 09:06:20.000000 datasiphon-0.2.6/src/siphon/__init__.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.6/src/siphon/base.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.6/src/siphon/nosql.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    34648 2024-05-21 08:53:34.000000 datasiphon-0.2.6/src/siphon/sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.425194 datasiphon-0.2.6/tests/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    25310 2024-05-21 08:55:58.000000 datasiphon-0.2.6/tests/test_sql.py
```

### Comparing `datasiphon-0.2.5/PKG-INFO` & `datasiphon-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.5
+Version: 0.2.6
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.5/README.md` & `datasiphon-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.5/pyproject.toml` & `datasiphon-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.5/src/datasiphon.egg-info/PKG-INFO` & `datasiphon-0.2.6/src/datasiphon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.5
+Version: 0.2.6
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.5/src/siphon/nosql.py` & `datasiphon-0.2.6/src/siphon/nosql.py`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.5/src/siphon/sql.py` & `datasiphon-0.2.6/src/siphon/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -515,15 +515,15 @@
                         )
                     else:  # VSCode - Insiders bug showing this as dead code
                         FilterBuilder.check_nested(value, query_columns, filter_model, column_name)
 
 
 class PaginationBuilder:
     base_query: sa.Select
-    sql_operators_mapping = {
+    sql_operators_mapping: dict[sql_operators.OperatorType, t.Type[Operation] | str] = {
         sql_operators.eq: Eq,
         sql_operators.ne: Ne,
         sql_operators.gt: Gt,
         sql_operators.ge: Ge,
         sql_operators.lt: Lt,
         sql_operators.le: Le,
         sql_operators.or_: "or",
@@ -543,20 +543,26 @@
         for column, value in subs.items():
             if column == col_name:
                 op, value = split_substitution(value)
                 return FilterBuilder.op_mapping[op](col_name, value)
 
     @staticmethod
     def process_operation(
-        whereclause: sql_elements.BinaryExpression, substition: dict[str, dict], bindparams: dict
-    ) -> Operation:
+        whereclause: sql_elements.BinaryExpression, substition: dict[str, dict], bindparams: dict, removals: dict
+    ) -> Operation | None:
         column = PaginationBuilder.get_column_from_binary_expression(whereclause)
         if column in substition:
             operation = PaginationBuilder.find_and_generate_substitution(column, substition)
             return operation
+        if (
+            column in removals
+            and removals[column] == PaginationBuilder.sql_operators_mapping[whereclause.operator].name
+        ):
+            return None
+
         expr_value = PaginationBuilder.get_value_from_binary_expression(whereclause)
         if not isinstance(expr_value, sql_elements.BindParameter):
             raise TypeError(f"Invalid type: {type(expr_value)} for value")
         processed_expr_value = bindparams.get(column, expr_value.value)
         return PaginationBuilder.sql_operators_mapping[whereclause.operator](column, processed_expr_value)
 
     @staticmethod
@@ -648,52 +654,61 @@
                 post_processed_data[unique_col].update({operations[0].name: operations[0].value})
             else:
                 post_processed_data[unique_col].update(
                     {junction: {operation.name: operation.value} for operation in operations}
                 )
         return post_processed_data
 
-    def reconstruct_filter(self, substitution: dict[str, t.Any] = None, bindparams: dict = None) -> dict:
-        data = self.recursive_reconstruct_filter(self.base_query.whereclause, substitution, bindparams)
+    def reconstruct_filter(
+        self, substitution: dict[str, t.Any] = None, bindparams: dict = None, removals: dict = None
+    ) -> dict:
+        data = self.recursive_reconstruct_filter(self.base_query.whereclause, substitution, bindparams, removals)
         if isinstance(data, Operation):
             return {data.col: {data.name: data.value}}
         return data
 
     @staticmethod
     def recursive_reconstruct_filter(
-        whereclause: t.Any, substitution: dict[str, t.Any] = None, bindparams: dict = None
+        whereclause: t.Any, substitution: dict[str, t.Any] = None, bindparams: dict = None, removals: dict = None
     ) -> dict:
         processed_substitution = substitution or {}
         processed_bindparams = bindparams or {}
+        processed_removals = removals or {}
         if whereclause is None:
             return {}
         if isinstance(whereclause, sql_elements.BinaryExpression):
-            operation = PaginationBuilder.process_operation(whereclause, processed_substitution, processed_bindparams)
+            operation = PaginationBuilder.process_operation(
+                whereclause, processed_substitution, processed_bindparams, processed_removals
+            )
             return operation
         elif isinstance(whereclause, sql_elements.BooleanClauseList):
             operations: list[Operation | dict] = []
             result = {PaginationBuilder.sql_operators_mapping[whereclause.operator]: {}}
             for clause in whereclause.clauses:
                 operation = PaginationBuilder.recursive_reconstruct_filter(
-                    clause, processed_substitution, processed_bindparams
+                    clause, processed_substitution, processed_bindparams, processed_removals
                 )
+                if operation is None:
+                    continue
                 if operation not in operations:
                     operations.append(operation)
                 else:
                     operations[operations.index(operation)].add_values(
                         operation, junction=PaginationBuilder.sql_operators_mapping[whereclause.operator]
                     )
             post_processed_operations = PaginationBuilder.post_process_operations(
                 operations, PaginationBuilder.sql_operators_mapping[whereclause.operator]
             )
             result[PaginationBuilder.sql_operators_mapping[whereclause.operator]].update(post_processed_operations)
+            if result[PaginationBuilder.sql_operators_mapping[whereclause.operator]] == {}:
+                return {}
             return result
         elif isinstance(whereclause, sql_elements.Grouping):
             return PaginationBuilder.recursive_reconstruct_filter(
-                whereclause.element, processed_substitution, processed_bindparams
+                whereclause.element, processed_substitution, processed_bindparams, processed_removals
             )
         else:
             raise TypeError(f"Unrecognized type: {type(whereclause)}")
 
 
 class SQL(QueryBuilder):
     """
```

### Comparing `datasiphon-0.2.5/tests/test_sql.py` & `datasiphon-0.2.6/tests/test_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -647,10 +647,22 @@
                         data.table_with_time_stamp.c.name != "Peter",
                         data.table_with_time_stamp.c.created_at == "2021-01-01T12:00:00",
                     )
                 )
             ),
         )
 
+        # test reconstruct with removal
+        result = ds.sql.PaginationBuilder(second_sample_query).reconstruct_filter(
+            removals={"name": "eq"}, bindparams={"created_at": "2021-01-01T12:00:00"}
+        )
+        self.assertEqual(
+            str(ds.sql.SQL.build(data.table_with_time_stamp.select(), result)),
+            str(
+                data.table_with_time_stamp.select().where(
+                    data.table_with_time_stamp.c.created_at == "2021-01-01T12:00:00",
+                )
+            ),
+        )
 
 if __name__ == "__main__":
     unittest.main()
```

