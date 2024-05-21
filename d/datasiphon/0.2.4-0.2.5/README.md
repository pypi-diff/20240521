# Comparing `tmp/datasiphon-0.2.4.tar.gz` & `tmp/datasiphon-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasiphon-0.2.4.tar", last modified: Mon May 20 10:07:02 2024, max compression
+gzip compressed data, was "datasiphon-0.2.5.tar", last modified: Tue May 21 07:52:53 2024, max compression
```

## Comparing `datasiphon-0.2.4.tar` & `datasiphon-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.612306 datasiphon-0.2.4/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-20 10:07:02.612306 datasiphon-0.2.4/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.4/README.md
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.4/pyproject.toml
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-20 10:07:02.612306 datasiphon-0.2.4/setup.cfg
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.611307 datasiphon-0.2.4/src/
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.612306 datasiphon-0.2.4/src/datasiphon.egg-info/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/SOURCES.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/dependency_links.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/requires.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/top_level.txt
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.612306 datasiphon-0.2.4/src/siphon/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-20 10:06:35.000000 datasiphon-0.2.4/src/siphon/__init__.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1127 2024-05-07 09:15:29.000000 datasiphon-0.2.4/src/siphon/base.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.4/src/siphon/nosql.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    24289 2024-05-20 09:58:29.000000 datasiphon-0.2.4/src/siphon/sql.py
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.612306 datasiphon-0.2.4/tests/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    21235 2024-05-20 10:04:47.000000 datasiphon-0.2.4/tests/test_sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.256548 datasiphon-0.2.5/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 07:52:53.256548 datasiphon-0.2.5/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.5/README.md
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.5/pyproject.toml
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-21 07:52:53.256548 datasiphon-0.2.5/setup.cfg
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.255548 datasiphon-0.2.5/src/
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.256548 datasiphon-0.2.5/src/datasiphon.egg-info/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/SOURCES.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/dependency_links.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/requires.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-21 07:52:53.000000 datasiphon-0.2.5/src/datasiphon.egg-info/top_level.txt
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.256548 datasiphon-0.2.5/src/siphon/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-21 07:52:31.000000 datasiphon-0.2.5/src/siphon/__init__.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      397 2024-05-21 07:52:31.000000 datasiphon-0.2.5/src/siphon/base.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.5/src/siphon/nosql.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    33994 2024-05-21 07:52:31.000000 datasiphon-0.2.5/src/siphon/sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-21 07:52:53.256548 datasiphon-0.2.5/tests/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    24780 2024-05-21 07:52:31.000000 datasiphon-0.2.5/tests/test_sql.py
```

### Comparing `datasiphon-0.2.4/PKG-INFO` & `datasiphon-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.4
+Version: 0.2.5
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.4/README.md` & `datasiphon-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.4/pyproject.toml` & `datasiphon-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.4/src/datasiphon.egg-info/PKG-INFO` & `datasiphon-0.2.5/src/datasiphon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.4
+Version: 0.2.5
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.4/src/siphon/nosql.py` & `datasiphon-0.2.5/src/siphon/nosql.py`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.4/src/siphon/sql.py` & `datasiphon-0.2.5/src/siphon/sql.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import typing as t
 from pydantic import BaseModel, model_validator, ValidationError
 from pydantic.fields import FieldInfo
 import re
 from copy import copy
 from sqlalchemy.sql.base import ReadOnlyColumnCollection
 import datetime as dt
+from dataclasses import dataclass
+from collections import OrderedDict
 
 
 class SqlOrderFilter(BaseModel):
     direction: str = None
     column: str = None
 
     @model_validator(mode="after")
@@ -169,16 +171,192 @@
             return type_
         elif type_ == dt.datetime:
             return dt.datetime.fromisoformat
         else:
             raise ValueError(f"Unparsable type: {type_}")
 
 
+@dataclass(init=False)
+class Operation:
+    name: str
+    col: str
+    value: t.Any
+
+    def __init__(self, col: str, value: t.Any):
+        self.col = col
+        self.value = value
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        pass
+
+    def __eq__(self, other: "Operation") -> bool:
+        if not isinstance(other, Operation):
+            return False
+        return self.col == other.col and self.name == other.name
+
+    def add_values(self, other: "Operation", **kw) -> None:
+        pass
+
+    def preprocess(self) -> "Operation":
+        return self
+
+
+class Eq(Operation):
+    name: str = "eq"
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column == process_type_func(value)
+
+    def add_values(self, other: "Eq", **kw) -> None:
+        if isinstance(self.value, list):
+            self.value.append(other.value)
+        else:
+            self.value = [self.value, other.value]
+
+    def preprocess(self) -> "Operation":
+        if isinstance(self.value, list):
+            return In_(self.col, self.value)
+        return self
+
+
+class Ne(Operation):
+    name: str = "ne"
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column != process_type_func(value)
+
+    def add_values(self, other: "Ne", **kw) -> None:
+        if isinstance(self.value, list):
+            self.value.append(other.value)
+        else:
+            self.value = [self.value, other.value]
+
+    def preprocess(self) -> "Operation":
+        if isinstance(self.value, list):
+            return Nin(self.col, self.value)
+        return self
+
+
+class Gt(Operation):
+    name: str = "gt"
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column > process_type_func(value)
+
+    def add_values(self, other: "Gt", junction: str = "and", **kw) -> None:
+        match junction:
+            case "and":
+                self.value = max(self.value, other.value)
+            case "or":
+                self.value = min(self.value, other.value)
+
+
+class Ge(Operation):
+    name: str = "ge"
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column >= process_type_func(value)
+
+    def add_values(self, other: "Ge", junction: str = "and", **kw) -> None:
+        match junction:
+            case "and":
+                self.value = max(self.value, other.value)
+            case "or":
+                self.value = min(self.value, other.value)
+
+
+class Lt(Operation):
+    name: str = "lt"
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column < process_type_func(value)
+
+    def add_values(self, other: "Lt", junction: str = "and", **kw) -> None:
+        match junction:
+            case "and":
+                self.value = min(self.value, other.value)
+            case "or":
+                self.value = max(self.value, other.value)
+
+
+class Le(Operation):
+    name: str = "le"
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column <= process_type_func(value)
+
+    def add_values(self, other: "Le", junction: str = "and", **kw) -> None:
+        match junction:
+            case "and":
+                self.value = min(self.value, other.value)
+            case "or":
+                self.value = max(self.value, other.value)
+
+
+class In_(Operation):
+    name: str = "in_"
+    value: list[t.Any]
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        # last chance to sanitize the value
+        if not isinstance(value, (list, tuple)):
+            value = [process_type_func(value)]
+        else:
+            value = [column.type.python_type(item) for item in value]
+        return column.in_(value)
+
+    def add_values(self, other: "In_", **kw) -> None:
+        self.value.extend(other.value)
+
+
+class Nin(Operation):
+    name: str = "nin"
+    value: list[t.Any]
+
+    @staticmethod
+    def generate(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        # last chance to sanitize the value
+        if not isinstance(value, (list, tuple)):
+            value = [process_type_func(value)]
+        else:
+            value = [column.type.python_type(item) for item in value]
+        return ~column.in_(value)
+
+    def add_values(self, other: "Nin", **kw) -> None:
+        self.value.extend(other.value)
+
+
 class FilterBuilder:
     junctionMapping = {"and": sa.and_, "or": sa.or_}
+    op_mapping: dict[str, Operation] = {
+        "eq": Eq,
+        "ne": Ne,
+        "gt": Gt,
+        "ge": Ge,
+        "lt": Lt,
+        "le": Le,
+        "in_": In_,
+        "nin": Nin,
+    }
 
     """
     Class for processing incoming filter (parsed by qstion package), no initial fields,
     but storing all incoming fields in extra field
     """
 
     @staticmethod
@@ -203,15 +381,15 @@
 
     @staticmethod
     def construct_column_clause(column: sa.Column, data: dict) -> sa.ColumnElement:
         current_clause = []
         for key, value in data.items():
             match key:
                 case str() as op if op in SQL.OPS:
-                    current_clause.append(SQL._op(op)(column, value))
+                    current_clause.append(FilterBuilder.op_mapping[op].generate(column, value))
                 case str() as junction if junction in ["and", "or"]:
                     clause_result = FilterBuilder.construct_column_clause(column, value)
                     if len(clause_result) == 1:
                         current_clause.append(clause_result[0])
                     else:
                         current_clause.append(FilterBuilder.junctionMapping[junction](*clause_result))
         return current_clause
@@ -335,14 +513,192 @@
                         raise FilterFormatError(
                             f"Invalid filter: {data} - expected one of (and, or) or operator for column: {current_key}, got: {column_name}"
                         )
                     else:  # VSCode - Insiders bug showing this as dead code
                         FilterBuilder.check_nested(value, query_columns, filter_model, column_name)
 
 
+class PaginationBuilder:
+    base_query: sa.Select
+    sql_operators_mapping = {
+        sql_operators.eq: Eq,
+        sql_operators.ne: Ne,
+        sql_operators.gt: Gt,
+        sql_operators.ge: Ge,
+        sql_operators.lt: Lt,
+        sql_operators.le: Le,
+        sql_operators.or_: "or",
+        sql_operators.and_: "and",
+        sql_operators.in_op: In_,
+        sql_operators.not_in_op: Nin,
+    }
+
+    def __init__(self, base_query: sa.Select):
+        self.base_query = base_query
+
+    @staticmethod
+    def find_and_generate_substitution(col_name: str, subs: dict[str, dict]) -> Operation:
+        def split_substitution(value: dict[str, t.Any]) -> tuple[str, t.Any]:
+            return list(value.keys())[0], list(value.values())[0]
+
+        for column, value in subs.items():
+            if column == col_name:
+                op, value = split_substitution(value)
+                return FilterBuilder.op_mapping[op](col_name, value)
+
+    @staticmethod
+    def process_operation(
+        whereclause: sql_elements.BinaryExpression, substition: dict[str, dict], bindparams: dict
+    ) -> Operation:
+        column = PaginationBuilder.get_column_from_binary_expression(whereclause)
+        if column in substition:
+            operation = PaginationBuilder.find_and_generate_substitution(column, substition)
+            return operation
+        expr_value = PaginationBuilder.get_value_from_binary_expression(whereclause)
+        if not isinstance(expr_value, sql_elements.BindParameter):
+            raise TypeError(f"Invalid type: {type(expr_value)} for value")
+        processed_expr_value = bindparams.get(column, expr_value.value)
+        return PaginationBuilder.sql_operators_mapping[whereclause.operator](column, processed_expr_value)
+
+    @staticmethod
+    def get_column_from_binary_expression(binary_expression: sql_elements.BinaryExpression) -> str:
+        if isinstance(binary_expression.left, sa.Column):
+            return binary_expression.left.name
+        elif isinstance(binary_expression.right, sa.Column):
+            return binary_expression.right.name
+        else:
+            return None
+
+    @staticmethod
+    def get_value_from_binary_expression(binary_expression: sql_elements.BinaryExpression) -> t.Any:
+        if isinstance(binary_expression.left, sa.Column):
+            return binary_expression.right
+        elif isinstance(binary_expression.right, sa.Column):
+            return binary_expression.left
+        else:
+            return None
+
+    def is_query_paginable(self, pagination_columns: list[str]) -> bool:
+        """
+        Check if a query is paginable
+
+        :param query: The query to check
+
+        :return: Whether the query is paginable
+        """
+
+        if self.base_query.whereclause is None:
+            return True
+        if isinstance(self.base_query.whereclause, sql_elements.BinaryExpression):
+            column = self.get_column_from_binary_expression(self.base_query.whereclause)
+            if column in pagination_columns and self.base_query.whereclause.operator in [
+                sql_operators.eq,
+                sql_operators.ne,
+            ]:
+                return False
+        elif isinstance(self.base_query.whereclause, sql_elements.BooleanClauseList):
+            for clause in self.base_query.whereclause.clauses:
+                if isinstance(clause, sql_elements.BinaryExpression):
+                    column = self.get_column_from_binary_expression(clause)
+                    if column in pagination_columns and clause.operator in [sql_operators.eq, sql_operators.ne]:
+                        return False
+                    if self.base_query.whereclause.operator == sql_operators.and_:
+                        if column not in pagination_columns and clause.operator not in [
+                            sql_operators.eq,
+                            sql_operators.ne,
+                        ]:
+                            return False
+                else:
+                    return False
+        else:
+            raise TypeError(f"Unrecognized type: {type(self.base_query.whereclause)}")
+        return True
+
+    @staticmethod
+    def post_process_operations(operations: list[Operation], junction: str) -> dict:
+        preprocessed_operations = [
+            operation.preprocess() if isinstance(operation, Operation) else operation for operation in operations
+        ]
+        post_processed_data = OrderedDict()
+        post_processed_operations = []
+        while preprocessed_operations:
+            current_operation = preprocessed_operations.pop(0)
+            if not isinstance(current_operation, Operation):
+                post_processed_data.update(current_operation)
+                continue
+            remove_indices = []
+            post_processed_data[current_operation.col] = {}
+            for item_index, item in enumerate(preprocessed_operations):
+                if item == current_operation:
+                    current_operation.add_values(item, junction=junction)
+                    remove_indices.append(item_index)
+            for index in remove_indices:
+                preprocessed_operations.pop(index)
+            post_processed_operations.append(current_operation)
+        # group operations by column - cannot use set bcs order matters
+        unique_columns = []
+        for operation in post_processed_operations:
+            if operation.col not in unique_columns:
+                unique_columns.append(operation.col)
+        grouped_operations = {
+            column: [operation for operation in post_processed_operations if operation.col == column]
+            for column in unique_columns
+        }
+        for unique_col, operations in grouped_operations.items():
+            if len(operations) == 1:
+                post_processed_data[unique_col].update({operations[0].name: operations[0].value})
+            else:
+                post_processed_data[unique_col].update(
+                    {junction: {operation.name: operation.value} for operation in operations}
+                )
+        return post_processed_data
+
+    def reconstruct_filter(self, substitution: dict[str, t.Any] = None, bindparams: dict = None) -> dict:
+        data = self.recursive_reconstruct_filter(self.base_query.whereclause, substitution, bindparams)
+        if isinstance(data, Operation):
+            return {data.col: {data.name: data.value}}
+        return data
+
+    @staticmethod
+    def recursive_reconstruct_filter(
+        whereclause: t.Any, substitution: dict[str, t.Any] = None, bindparams: dict = None
+    ) -> dict:
+        processed_substitution = substitution or {}
+        processed_bindparams = bindparams or {}
+        if whereclause is None:
+            return {}
+        if isinstance(whereclause, sql_elements.BinaryExpression):
+            operation = PaginationBuilder.process_operation(whereclause, processed_substitution, processed_bindparams)
+            return operation
+        elif isinstance(whereclause, sql_elements.BooleanClauseList):
+            operations: list[Operation | dict] = []
+            result = {PaginationBuilder.sql_operators_mapping[whereclause.operator]: {}}
+            for clause in whereclause.clauses:
+                operation = PaginationBuilder.recursive_reconstruct_filter(
+                    clause, processed_substitution, processed_bindparams
+                )
+                if operation not in operations:
+                    operations.append(operation)
+                else:
+                    operations[operations.index(operation)].add_values(
+                        operation, junction=PaginationBuilder.sql_operators_mapping[whereclause.operator]
+                    )
+            post_processed_operations = PaginationBuilder.post_process_operations(
+                operations, PaginationBuilder.sql_operators_mapping[whereclause.operator]
+            )
+            result[PaginationBuilder.sql_operators_mapping[whereclause.operator]].update(post_processed_operations)
+            return result
+        elif isinstance(whereclause, sql_elements.Grouping):
+            return PaginationBuilder.recursive_reconstruct_filter(
+                whereclause.element, processed_substitution, processed_bindparams
+            )
+        else:
+            raise TypeError(f"Unrecognized type: {type(whereclause)}")
+
+
 class SQL(QueryBuilder):
     """
     SQL query builder
     """
 
     __sql_kwargs__ = {"order_by": list[str], "limit": bool, "offset": bool}
 
@@ -418,106 +774,14 @@
         FilterBuilder.check_values(qs_filter, column_collection, filter_model)
         filter_data = FilterBuilder.construct_clause(qs_filter, column_collection)
         query = query.where(*filter_data)
         keyword_data = FilterBuilder.extract_keywords(qs_filter)
         query = keyword_data.apply_on_query(query)
         return query
 
-    @staticmethod
-    def is_query_paginable(query: sa.Select, pagination_columns: list[str]) -> bool:
-        """
-        Check if a query is paginable
-
-        :param query: The query to check
-
-        :return: Whether the query is paginable
-        """
-
-        def get_column_from_binary_expression(binary_expression: sql_elements.BinaryExpression) -> str:
-            if isinstance(binary_expression.left, sa.Column):
-                return binary_expression.left.name
-            elif isinstance(binary_expression.right, sa.Column):
-                return binary_expression.right.name
-            else:
-                return None
-
-        if query.whereclause is None:
-            return True
-        if isinstance(query.whereclause, sql_elements.BinaryExpression):
-            column = get_column_from_binary_expression(query.whereclause)
-            if column in pagination_columns and query.whereclause.operator in [sql_operators.eq, sql_operators.ne]:
-                return False
-        elif isinstance(query.whereclause, sql_elements.BooleanClauseList):
-            for clause in query.whereclause.clauses:
-                if isinstance(clause, sql_elements.BinaryExpression):
-                    column = get_column_from_binary_expression(clause)
-                    if column in pagination_columns and clause.operator in [sql_operators.eq, sql_operators.ne]:
-                        return False
-                    if query.whereclause.operator == sql_operators.and_:
-                        if column not in pagination_columns and clause.operator not in [
-                            sql_operators.eq,
-                            sql_operators.ne,
-                        ]:
-                            return False
-                else:
-                    return False
-        else:
-            raise TypeError(f"Unrecognized type: {type(query.whereclause)}")
-        return True
-
-    @staticmethod
-    def eq(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
-        return column == process_type_func(value)
-
-    @staticmethod
-    def ne(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
-        return column != process_type_func(value)
-
-    @staticmethod
-    def gt(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
-        return column > process_type_func(value)
-
-    @staticmethod
-    def ge(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
-        return column >= process_type_func(value)
-
-    @staticmethod
-    def lt(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
-        return column < process_type_func(value)
-
-    @staticmethod
-    def le(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
-        return column <= process_type_func(value)
-
-    @staticmethod
-    def in_(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
-        # last chance to sanitize the value
-        if not isinstance(value, (list, tuple)):
-            value = [process_type_func(value)]
-        else:
-            value = [column.type.python_type(item) for item in value]
-        return column.in_(value)
-
-    @staticmethod
-    def nin(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
-        # last chance to sanitize the value
-        if not isinstance(value, (list, tuple)):
-            value = [process_type_func(value)]
-        else:
-            value = [column.type.python_type(item) for item in value]
-        return ~column.in_(value)
-
     @classmethod
     def _kw(cls, kw: str, stm: sa.Select, value: t.Any) -> sa.Select:
         return getattr(cls, kw)(stm, value)
 
     @staticmethod
     def order_by(stm: sa.Select, values: list[SqlOrderFilter]) -> sa.Select:
         """
```

