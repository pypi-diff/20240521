# Comparing `tmp/datasiphon-0.2.6.tar.gz` & `tmp/datasiphon-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasiphon-0.2.6.tar", last modified: Tue May 21 09:06:35 2024, max compression
+gzip compressed data, was "datasiphon-0.2.7.tar", last modified: Tue May 21 09:41:13 2024, max compression
```

## Comparing `datasiphon-0.2.6.tar` & `datasiphon-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.426194 datasiphon-0.2.6/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 09:06:35.426194 datasiphon-0.2.6/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.6/README.md
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.6/pyproject.toml
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 09:06:35.426194 datasiphon-0.2.6/setup.cfg
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.424194 datasiphon-0.2.6/src/
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.425194 datasiphon-0.2.6/src/datasiphon.egg-info/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/SOURCES.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/dependency_links.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/requires.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 09:06:35.000000 datasiphon-0.2.6/src/datasiphon.egg-info/top_level.txt
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.425194 datasiphon-0.2.6/src/siphon/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 09:06:20.000000 datasiphon-0.2.6/src/siphon/__init__.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.6/src/siphon/base.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.6/src/siphon/nosql.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    34648 2024-05-21 08:53:34.000000 datasiphon-0.2.6/src/siphon/sql.py
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:06:35.425194 datasiphon-0.2.6/tests/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    25310 2024-05-21 08:55:58.000000 datasiphon-0.2.6/tests/test_sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.491800 datasiphon-0.2.7/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 09:41:13.491800 datasiphon-0.2.7/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.7/README.md
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.7/pyproject.toml
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 09:41:13.491800 datasiphon-0.2.7/setup.cfg
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.489800 datasiphon-0.2.7/src/
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.491800 datasiphon-0.2.7/src/datasiphon.egg-info/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/SOURCES.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/dependency_links.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/requires.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 09:41:13.000000 datasiphon-0.2.7/src/datasiphon.egg-info/top_level.txt
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.491800 datasiphon-0.2.7/src/siphon/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 09:12:01.000000 datasiphon-0.2.7/src/siphon/__init__.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.7/src/siphon/base.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.7/src/siphon/nosql.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    36863 2024-05-21 09:40:16.000000 datasiphon-0.2.7/src/siphon/sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 09:41:13.491800 datasiphon-0.2.7/tests/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    28132 2024-05-21 09:40:32.000000 datasiphon-0.2.7/tests/test_sql.py
```

### Comparing `datasiphon-0.2.6/PKG-INFO` & `datasiphon-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.6
+Version: 0.2.7
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.6/README.md` & `datasiphon-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.6/pyproject.toml` & `datasiphon-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.6/src/datasiphon.egg-info/PKG-INFO` & `datasiphon-0.2.7/src/datasiphon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.6
+Version: 0.2.7
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.6/src/siphon/nosql.py` & `datasiphon-0.2.7/src/siphon/nosql.py`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.6/src/siphon/sql.py` & `datasiphon-0.2.7/src/siphon/sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -527,14 +527,18 @@
         sql_operators.lt: Lt,
         sql_operators.le: Le,
         sql_operators.or_: "or",
         sql_operators.and_: "and",
         sql_operators.in_op: In_,
         sql_operators.not_in_op: Nin,
     }
+    sql_order_mapping: dict[sql_operators.OperatorType, int] = {
+        sql_operators.desc_op: 0,
+        sql_operators.asc_op: 1,
+    }
 
     def __init__(self, base_query: sa.Select):
         self.base_query = base_query
 
     @staticmethod
     def find_and_generate_substitution(col_name: str, subs: dict[str, dict]) -> Operation:
         def split_substitution(value: dict[str, t.Any]) -> tuple[str, t.Any]:
@@ -607,14 +611,16 @@
                     column = self.get_column_from_binary_expression(clause)
                     if column in pagination_columns and clause.operator in [sql_operators.eq, sql_operators.ne]:
                         return False
                     if self.base_query.whereclause.operator == sql_operators.and_:
                         if column not in pagination_columns and clause.operator not in [
                             sql_operators.eq,
                             sql_operators.ne,
+                            sql_operators.in_op,
+                            sql_operators.not_in_op,
                         ]:
                             return False
                 else:
                     return False
         else:
             raise TypeError(f"Unrecognized type: {type(self.base_query.whereclause)}")
         return True
@@ -705,14 +711,56 @@
         elif isinstance(whereclause, sql_elements.Grouping):
             return PaginationBuilder.recursive_reconstruct_filter(
                 whereclause.element, processed_substitution, processed_bindparams, processed_removals
             )
         else:
             raise TypeError(f"Unrecognized type: {type(whereclause)}")
 
+    def retrieve_order_by(self, count: int = 1) -> tuple[int, str] | None:
+        clauses = self.base_query._order_by_clauses
+        if len(clauses) == 0:
+            return None
+        processed_clauses = []
+        for clause in clauses:
+            processed_clauses.append(self.recusively_process_order_by(clause))
+            if len(processed_clauses) == count:
+                break
+        return processed_clauses
+
+    @staticmethod
+    def recusively_process_order_by(item: t.Any) -> tuple[int, str] | None:
+        if isinstance(item, sql_elements._label_reference):
+            return PaginationBuilder.recusively_process_order_by(item.element)
+        if isinstance(item, sql_elements.UnaryExpression):
+            return (PaginationBuilder.sql_order_mapping[item.modifier], item.element.name)
+        if isinstance(item, sa.Column):
+            # default is ascending
+            return (1, item.name)
+        raise TypeError(f"Unrecognized type: {type(item)}")
+
+    def retrieve_filtered_column(self, column_name: str) -> Operation | None:
+        whereclause = self.base_query.whereclause
+        if whereclause is None:
+            return None
+        if isinstance(whereclause, sql_elements.BinaryExpression):
+            if column_name in [
+                self.get_column_from_binary_expression(whereclause),
+                self.get_column_from_binary_expression(whereclause),
+            ]:
+                return self.process_operation(whereclause, {}, {}, {})
+        elif isinstance(whereclause, sql_elements.BooleanClauseList):
+            for clause in whereclause.clauses:
+                if isinstance(clause, sql_elements.BinaryExpression):
+                    if column_name in [
+                        self.get_column_from_binary_expression(clause),
+                        self.get_column_from_binary_expression(clause),
+                    ]:
+                        return self.process_operation(clause, {}, {}, {})
+        return None
+
 
 class SQL(QueryBuilder):
     """
     SQL query builder
     """
 
     __sql_kwargs__ = {"order_by": list[str], "limit": bool, "offset": bool}
```

### Comparing `datasiphon-0.2.6/tests/test_sql.py` & `datasiphon-0.2.7/tests/test_sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -660,9 +660,65 @@
             str(
                 data.table_with_time_stamp.select().where(
                     data.table_with_time_stamp.c.created_at == "2021-01-01T12:00:00",
                 )
             ),
         )
 
+        # test retrieve order_by
+        sample_query = data.table_with_time_stamp.select().order_by(data.table_with_time_stamp.c.created_at.desc())
+        result = ds.sql.PaginationBuilder(sample_query).retrieve_order_by()
+        self.assertEqual(len(result), 1)
+        self.assertEqual(result[0], (0, "created_at"))
+
+        # test order by with different approach
+        sample_query = data.table_with_time_stamp.select().order_by(sa.desc(data.table_with_time_stamp.c.created_at))
+        result = ds.sql.PaginationBuilder(sample_query).retrieve_order_by()
+        self.assertEqual(len(result), 1)
+        self.assertEqual(result[0], (0, "created_at"))
+
+        # test without providing direction
+        sample_query = data.table_with_time_stamp.select().order_by(data.table_with_time_stamp.c.created_at)
+        result = ds.sql.PaginationBuilder(sample_query).retrieve_order_by()
+        self.assertEqual(len(result), 1)
+        self.assertEqual(result[0], (1, "created_at"))
+
+        # test on label
+        sample_query = sa.select(
+            data.table_with_time_stamp.c.name.label("name_label"),
+        ).order_by(sa.desc(data.table_with_time_stamp.c.name.label("name_label")))
+        result = ds.sql.PaginationBuilder(sample_query).retrieve_order_by()
+        self.assertEqual(len(result), 1)
+        self.assertEqual(result[0], (0, "name_label"))
+
+        # test retrieve operation on filtered column
+        # test none
+        sample_query = data.table_with_time_stamp.select().where(data.table_with_time_stamp.c.name == None)
+        result = ds.sql.PaginationBuilder(sample_query).retrieve_filtered_column("created_at")
+        self.assertEqual(result, None)
+
+        # test single
+        sample_query = data.table_with_time_stamp.select().where(data.table_with_time_stamp.c.name == "John")
+        result = ds.sql.PaginationBuilder(sample_query).retrieve_filtered_column("name")
+        self.assertIsInstance(result, ds.sql.Operation)
+        self.assertEqual(result.col, "name")
+        self.assertEqual(result.name, "eq")
+
+        # test on more complex query
+        sample_query = data.table_with_time_stamp.select().where(
+            sa.and_(
+                data.table_with_time_stamp.c.name >= "John",
+                data.table_with_time_stamp.c.created_at < "2021-01-01T12:00:00",
+            )
+        )
+        result = ds.sql.PaginationBuilder(sample_query).retrieve_filtered_column("name")
+        self.assertIsInstance(result, ds.sql.Operation)
+        self.assertEqual(result.col, "name")
+        self.assertEqual(result.name, "ge")
+        result = ds.sql.PaginationBuilder(sample_query).retrieve_filtered_column("created_at")
+        self.assertIsInstance(result, ds.sql.Operation)
+        self.assertEqual(result.col, "created_at")
+        self.assertEqual(result.name, "lt")
+
+
 if __name__ == "__main__":
     unittest.main()
```

