# Comparing `tmp/datasiphon-0.2.7.tar.gz` & `tmp/datasiphon-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasiphon-0.2.7.tar", last modified: Tue May 21 09:41:13 2024, max compression
+gzip compressed data, was "datasiphon-0.2.8.tar", last modified: Tue May 21 10:35:57 2024, max compression
```

## Comparing `datasiphon-0.2.7.tar` & `datasiphon-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.491800 datasiphon-0.2.7/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 09:41:13.491800 datasiphon-0.2.7/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.7/README.md
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.7/pyproject.toml
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 09:41:13.491800 datasiphon-0.2.7/setup.cfg
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.489800 datasiphon-0.2.7/src/
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.491800 datasiphon-0.2.7/src/datasiphon.egg-info/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/SOURCES.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/dependency_links.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/requires.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/top_level.txt
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.491800 datasiphon-0.2.7/src/siphon/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 09:12:01.000000 datasiphon-0.2.7/src/siphon/__init__.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.7/src/siphon/base.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.7/src/siphon/nosql.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    36863 2024-05-21 09:40:16.000000 datasiphon-0.2.7/src/siphon/sql.py
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.491800 datasiphon-0.2.7/tests/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    28132 2024-05-21 09:40:32.000000 datasiphon-0.2.7/tests/test_sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.502215 datasiphon-0.2.8/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 10:35:57.502215 datasiphon-0.2.8/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.8/README.md
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.8/pyproject.toml
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 10:35:57.502215 datasiphon-0.2.8/setup.cfg
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.500214 datasiphon-0.2.8/src/
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.501215 datasiphon-0.2.8/src/datasiphon.egg-info/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/SOURCES.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/dependency_links.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/requires.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 10:35:57.000000 datasiphon-0.2.8/src/datasiphon.egg-info/top_level.txt
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.501215 datasiphon-0.2.8/src/siphon/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 10:35:14.000000 datasiphon-0.2.8/src/siphon/__init__.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.8/src/siphon/base.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.8/src/siphon/nosql.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    38269 2024-05-21 10:35:18.000000 datasiphon-0.2.8/src/siphon/sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 10:35:57.501215 datasiphon-0.2.8/tests/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    28784 2024-05-21 10:35:16.000000 datasiphon-0.2.8/tests/test_sql.py
```

### Comparing `datasiphon-0.2.7/PKG-INFO` & `datasiphon-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.7
+Version: 0.2.8
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.7/README.md` & `datasiphon-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.7/pyproject.toml` & `datasiphon-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.7/src/datasiphon.egg-info/PKG-INFO` & `datasiphon-0.2.8/src/datasiphon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.7
+Version: 0.2.8
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.7/src/siphon/nosql.py` & `datasiphon-0.2.8/src/siphon/nosql.py`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.7/src/siphon/sql.py` & `datasiphon-0.2.8/src/siphon/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,14 +513,40 @@
                         raise FilterFormatError(
                             f"Invalid filter: {data} - expected one of (and, or) or operator for column: {current_key}, got: {column_name}"
                         )
                     else:  # VSCode - Insiders bug showing this as dead code
                         FilterBuilder.check_nested(value, query_columns, filter_model, column_name)
 
 
+@dataclass(init=False)
+class Substitution:
+    operation: str | None
+    column: str
+    value: t.Any
+    used: bool = False
+
+    def __init__(self, column: str, value: t.Any, operation: str = None):
+        self.column = column
+        self.value = value
+        self.operation = operation
+
+    def __eq__(self, other: "Substitution") -> bool:
+        if isinstance(other, Operation):
+            return self.column == other.col
+        if not isinstance(other, Substitution):
+            return False
+        return self.column == other.column
+
+    def to_op(self, original_op: str) -> Operation:
+        self.used = True
+        if self.operation is None:
+            self.operation = original_op
+        return FilterBuilder.op_mapping[self.operation](self.column, self.value)
+
+
 class PaginationBuilder:
     base_query: sa.Select
     sql_operators_mapping: dict[sql_operators.OperatorType, t.Type[Operation] | str] = {
         sql_operators.eq: Eq,
         sql_operators.ne: Ne,
         sql_operators.gt: Gt,
         sql_operators.ge: Ge,
@@ -536,31 +562,23 @@
         sql_operators.asc_op: 1,
     }
 
     def __init__(self, base_query: sa.Select):
         self.base_query = base_query
 
     @staticmethod
-    def find_and_generate_substitution(col_name: str, subs: dict[str, dict]) -> Operation:
-        def split_substitution(value: dict[str, t.Any]) -> tuple[str, t.Any]:
-            return list(value.keys())[0], list(value.values())[0]
-
-        for column, value in subs.items():
-            if column == col_name:
-                op, value = split_substitution(value)
-                return FilterBuilder.op_mapping[op](col_name, value)
-
-    @staticmethod
     def process_operation(
-        whereclause: sql_elements.BinaryExpression, substition: dict[str, dict], bindparams: dict, removals: dict
+        whereclause: sql_elements.BinaryExpression, substition: list[Substitution], bindparams: dict, removals: dict
     ) -> Operation | None:
         column = PaginationBuilder.get_column_from_binary_expression(whereclause)
-        if column in substition:
-            operation = PaginationBuilder.find_and_generate_substitution(column, substition)
-            return operation
+        for item in substition:
+            if item.used:
+                continue
+            if item.column == column:
+                return item.to_op(PaginationBuilder.sql_operators_mapping[whereclause.operator].name)
         if (
             column in removals
             and removals[column] == PaginationBuilder.sql_operators_mapping[whereclause.operator].name
         ):
             return None
 
         expr_value = PaginationBuilder.get_value_from_binary_expression(whereclause)
@@ -661,30 +679,50 @@
             else:
                 post_processed_data[unique_col].update(
                     {junction: {operation.name: operation.value} for operation in operations}
                 )
         return post_processed_data
 
     def reconstruct_filter(
-        self, substitution: dict[str, t.Any] = None, bindparams: dict = None, removals: dict = None
+        self, substitution: list[Substitution] = None, bindparams: dict = None, removals: dict = None
     ) -> dict:
+        """
+        Reconstruct the filter into a nested dictionary from query - parsable by this package
+
+        :param substitution: The substitutions to apply if the substitutions are not used, they are added to the result
+        :param bindparams: The bindparams to apply - from prepared statement NOTE warning: if bindparams are used and not provided
+        `None` value will be used in reconstructed filter
+        :param removals: The removals to apply - remove columns from the filter
+
+        :return: The reconstructed filter
+        """
         data = self.recursive_reconstruct_filter(self.base_query.whereclause, substitution, bindparams, removals)
+        if data is None:
+            data = {}
         if isinstance(data, Operation):
-            return {data.col: {data.name: data.value}}
+            data = {data.col: {data.name: data.value}}
+        if substitution is not None:
+            for item in substitution:
+                if not item.used:
+                    if item.operation is None:
+                        raise ValueError(
+                            f"Column not used in filter and operation for substitution not provided: {item}"
+                        )
+                    data[item.column] = {item.operation: item.value}
         return data
 
     @staticmethod
     def recursive_reconstruct_filter(
-        whereclause: t.Any, substitution: dict[str, t.Any] = None, bindparams: dict = None, removals: dict = None
+        whereclause: t.Any, substitution: list[Substitution] = None, bindparams: dict = None, removals: dict = None
     ) -> dict:
-        processed_substitution = substitution or {}
+        processed_substitution = substitution or []
         processed_bindparams = bindparams or {}
         processed_removals = removals or {}
         if whereclause is None:
-            return {}
+            return None
         if isinstance(whereclause, sql_elements.BinaryExpression):
             operation = PaginationBuilder.process_operation(
                 whereclause, processed_substitution, processed_bindparams, processed_removals
             )
             return operation
         elif isinstance(whereclause, sql_elements.BooleanClauseList):
             operations: list[Operation | dict] = []
@@ -702,15 +740,15 @@
                         operation, junction=PaginationBuilder.sql_operators_mapping[whereclause.operator]
                     )
             post_processed_operations = PaginationBuilder.post_process_operations(
                 operations, PaginationBuilder.sql_operators_mapping[whereclause.operator]
             )
             result[PaginationBuilder.sql_operators_mapping[whereclause.operator]].update(post_processed_operations)
             if result[PaginationBuilder.sql_operators_mapping[whereclause.operator]] == {}:
-                return {}
+                return None
             return result
         elif isinstance(whereclause, sql_elements.Grouping):
             return PaginationBuilder.recursive_reconstruct_filter(
                 whereclause.element, processed_substitution, processed_bindparams, processed_removals
             )
         else:
             raise TypeError(f"Unrecognized type: {type(whereclause)}")
```

### Comparing `datasiphon-0.2.7/tests/test_sql.py` & `datasiphon-0.2.8/tests/test_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -633,28 +633,42 @@
                     )
                 )
             ),
         )
 
         # test reconstruct with substitution
         result = ds.sql.PaginationBuilder(second_sample_query).reconstruct_filter(
-            substitution={"name": {"ne": "Peter"}}, bindparams={"created_at": "2021-01-01T12:00:00"}
+            substitution=[ds.sql.Substitution("name", "Peter", "ne")], bindparams={"created_at": "2021-01-01T12:00:00"}
         )
         self.assertEqual(
             str(ds.sql.SQL.build(data.table_with_time_stamp.select(), result)),
             str(
                 data.table_with_time_stamp.select().where(
                     sa.and_(
                         data.table_with_time_stamp.c.name != "Peter",
                         data.table_with_time_stamp.c.created_at == "2021-01-01T12:00:00",
                     )
                 )
             ),
         )
 
+        # test substition on non filtered query - should add filter
+        sample_query_add = data.table_with_time_stamp.select()
+        result = ds.sql.PaginationBuilder(sample_query_add).reconstruct_filter(
+            substitution=[ds.sql.Substitution("name", "Peter", "eq")], bindparams={"created_at": "2021-01-01T12:00:00"}
+        )
+        self.assertEqual(
+            str(ds.sql.SQL.build(data.table_with_time_stamp.select(), result)),
+            str(
+                data.table_with_time_stamp.select().where(
+                    data.table_with_time_stamp.c.name == "Peter",
+                )
+            ),
+        )
+
         # test reconstruct with removal
         result = ds.sql.PaginationBuilder(second_sample_query).reconstruct_filter(
             removals={"name": "eq"}, bindparams={"created_at": "2021-01-01T12:00:00"}
         )
         self.assertEqual(
             str(ds.sql.SQL.build(data.table_with_time_stamp.select(), result)),
             str(
```

