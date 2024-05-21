# Comparing `tmp/altqq-0.0.5.tar.gz` & `tmp/altqq-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altqq-0.0.5.tar", max compression
+gzip compressed data, was "altqq-0.0.6.tar", max compression
```

## Comparing `altqq-0.0.5.tar` & `altqq-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2024-03-25 15:49:01.433272 altqq-0.0.5/LICENSE
--rw-r--r--   0        0        0     2519 2024-03-25 15:49:01.433272 altqq-0.0.5/README.md
--rw-r--r--   0        0        0     1556 2024-03-25 15:49:01.433272 altqq-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2055 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/__init__.py
--rw-r--r--   0        0        0     1794 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/structs.py
--rw-r--r--   0        0        0       36 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/translators/__init__.py
--rw-r--r--   0        0        0      911 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/translators/common.py
--rw-r--r--   0        0        0     1118 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/translators/mysql.py
--rw-r--r--   0        0        0     1474 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/translators/plain_text.py
--rw-r--r--   0        0        0     3246 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/translators/psycopg.py
--rw-r--r--   0        0        0     2909 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/translators/pyodbc.py
--rw-r--r--   0        0        0      353 2024-03-25 15:49:01.433272 altqq-0.0.5/src/altqq/types.py
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 altqq-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-21 09:25:44.699553 altqq-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2519 2024-05-21 09:25:44.703553 altqq-0.0.6/README.md
+-rw-r--r--   0        0        0     1556 2024-05-21 09:25:44.703553 altqq-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2091 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/structs.py
+-rw-r--r--   0        0        0       36 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/translators/__init__.py
+-rw-r--r--   0        0        0     1537 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/translators/common.py
+-rw-r--r--   0        0        0     1118 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/translators/mysql.py
+-rw-r--r--   0        0        0     1852 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/translators/plain_text.py
+-rw-r--r--   0        0        0     3544 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/translators/psycopg.py
+-rw-r--r--   0        0        0     3206 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/translators/pyodbc.py
+-rw-r--r--   0        0        0      459 2024-05-21 09:25:44.703553 altqq-0.0.6/src/altqq/types.py
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 altqq-0.0.6/PKG-INFO
```

### Comparing `altqq-0.0.5/LICENSE` & `altqq-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `altqq-0.0.5/README.md` & `altqq-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `altqq-0.0.5/pyproject.toml` & `altqq-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ignore = ["D107"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.poetry]
 name = "altqq"
-version = "0.0.5"
+version = "0.0.6"
 description = "Alternative Queries: Typed and Reusable Handcrafted SQL"
 authors = ["baluyotraf <baluyotraf@outlook.com>"]
 maintainers = ["baluyotraf <baluyotraf@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/baluyotraf/altqq"
 homepage = "https://altqq.baluyotraf.com"
```

### Comparing `altqq-0.0.5/src/altqq/__init__.py` & `altqq-0.0.6/src/altqq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Main entry point for the altqq library."""
 
 from altqq.structs import Calculated, Query
 from altqq.translators.mysql import MySQLQuery, MySQLTranslator
 from altqq.translators.plain_text import PlainTextTranslator
 from altqq.translators.psycopg import PsycopgQuery, PsycopgTranslator
 from altqq.translators.pyodbc import PyODBCQuery, PyODBCTranslator
-from altqq.types import NonParameter
+from altqq.types import ListParameter, NonParameter
 
 __all__ = [
     "Query",
     "Calculated",
     "NonParameter",
+    "ListParameter",
     "to_pyodbc",
     "to_psycopg",
     "to_mysql",
     "to_plain_text",
 ]
```

### Comparing `altqq-0.0.5/src/altqq/translators/common.py` & `altqq-0.0.6/src/altqq/translators/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Translator related functions not belonging to other areas."""
 
 import typing
-from typing import Any
+from typing import Any, Set, cast
 
 from typing_extensions import Annotated
 
 from altqq.structs import Query
 from altqq.types import QueryValueTypes
 
 
@@ -17,22 +17,43 @@
 
     Returns:
         bool: True if a subclass, else False.
     """
     return isinstance(value, Query)
 
 
-def is_parameter(cls: type) -> bool:
-    """Checks if a type is a parameter type.
+ANNOTATED_TYPES: Set[QueryValueTypes] = {
+    QueryValueTypes.NON_PARAMETER,
+    QueryValueTypes.LIST_PARAMETER,
+}
+
+
+def get_parameter_type(cls: type) -> QueryValueTypes:
+    """Extracts the value type based on the typing.
 
     Args:
         cls (type): Type to check.
 
     Returns:
-        bool: True if parameter, else False.
+        QueryValueTypes: Role of the value in the query
     """
     if typing.get_origin(cls) == Annotated:
         # Pyright can't match the __metadata__ attribute to Annotated
-        if QueryValueTypes.NON_PARAMETER in cls.__metadata__:  # type: ignore
-            return True
+        for metadata in cls.__metadata__:  # type: ignore
+            if metadata in ANNOTATED_TYPES:
+                return cast(QueryValueTypes, metadata)
+
+    return QueryValueTypes.PARAMETER
+
+
+def create_list_markers(marker: str, n: int) -> str:
+    """Creates list markers for list parameter types.
 
-    return False
+    Args:
+        marker (str): Parameter marker used by the translation
+        n (int): Number of parameters in the list
+
+    Returns:
+        str: String to represent the list
+    """
+    comma_separated = ",".join(marker for _ in range(n))
+    return f"({comma_separated})"
```

### Comparing `altqq-0.0.5/src/altqq/translators/mysql.py` & `altqq-0.0.6/src/altqq/translators/mysql.py`

 * *Files identical despite different names*

### Comparing `altqq-0.0.5/src/altqq/translators/plain_text.py` & `altqq-0.0.6/src/altqq/translators/plain_text.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 """Module for converting Query objects to plain text SQL."""
 
 import dataclasses as dc
 from typing import Any
 
 from altqq.structs import Query
-from altqq.translators.common import is_parameter, is_query_instance
-from altqq.types import T
+from altqq.translators import common
+from altqq.types import QueryValueTypes, T
 
 
 class PlainTextTranslator:
     """Converts a `Query` to a plain text SQL."""
 
-    def _resolve_value(self, query: Query, field: dc.Field[T]) -> Any:
-        value = getattr(query, field.name)
-        if is_query_instance(value):
-            return self.__call__(value)
-
-        if is_parameter(field.type):
-            return value
-
+    def _resolve_parameters(self, value: Any) -> str:
         # Numeric types are not escaped
         if isinstance(value, (int, float)):
-            return value
+            return str(value)
 
         # None is written as NULL
         if value is None:
             return "NULL"
 
         # All other types fall down to strings and are escaped
         return f"'{value}'"
 
+    def _resolve_value(self, query: Query, field: dc.Field[T]) -> str:
+        value = getattr(query, field.name)
+        if common.is_query_instance(value):
+            return self.__call__(value)
+
+        field_type = common.get_parameter_type(field.type)
+        if field_type == QueryValueTypes.NON_PARAMETER:
+            return value
+        elif field_type == QueryValueTypes.LIST_PARAMETER:
+            comma_separated = ",".join(self._resolve_parameters(p) for p in value)
+            return f"({comma_separated})"
+        else:
+            return self._resolve_parameters(value)
+
     def __call__(self, query: Query) -> str:
         """Converts a `Query` to a plain text SQL.
 
         The conversion to plain text also handles some of the data types. None
         is converted to `NULL`, numeric values are written as they are and
         string values and other object types are escaped using `'`.
```

### Comparing `altqq-0.0.5/src/altqq/translators/psycopg.py` & `altqq-0.0.6/src/altqq/translators/psycopg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module for converting Query objects for Psycopg execution."""
 
 import dataclasses as dc
 from string import Formatter
 from typing import Any, Iterable, List, Mapping, Sequence, Tuple, Union
 
 from altqq.structs import Query
-from altqq.translators.common import is_parameter, is_query_instance
-from altqq.types import T
+from altqq.translators import common
+from altqq.types import QueryValueTypes, T
 
 
 @dc.dataclass
 class PsycopgStatement:
     """Represents a generated Psycopg statement."""
 
     statement: Any
@@ -64,24 +64,31 @@
         self.parameter_values.extend(field.parameters)
         return field.statement
 
 
 class PsycopgTranslator:
     """Converts a `Query` to its corresponding `PsycopgQuery` object."""
 
+    MARKER = "%s"
+
     def _resolve_value(self, query: Query, field: dc.Field[T]) -> PsycopgStatement:
         value = getattr(query, field.name)
-        if is_query_instance(value):
+        if common.is_query_instance(value):
             qq = self._convert_query(value)
             return PsycopgStatement(qq.query, qq.parameters)
 
-        if is_parameter(field.type):
+        field_type = common.get_parameter_type(field.type)
+        if field_type == QueryValueTypes.NON_PARAMETER:
             return PsycopgStatement(value.replace("%", "%%"), ())
-
-        return PsycopgStatement("%s", (value,))
+        elif field_type == QueryValueTypes.LIST_PARAMETER:
+            return PsycopgStatement(
+                common.create_list_markers(self.MARKER, len(value)), value
+            )
+        else:
+            return PsycopgStatement(self.MARKER, (value,))
 
     def _convert_query(self, query: Query) -> PsycopgQuery:
         formatter = PsycopgFormatter()
         fields = dc.fields(query)
         format_dict = {f.name: self._resolve_value(query, f) for f in fields}
 
         return PsycopgQuery(
```

### Comparing `altqq-0.0.5/src/altqq/translators/pyodbc.py` & `altqq-0.0.6/src/altqq/translators/pyodbc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module for converting Query objects for PyODBC execution."""
 
 import dataclasses as dc
 from string import Formatter
 from typing import Any, Iterable, List, Mapping, Sequence, Union
 
 from altqq.structs import Query
-from altqq.translators.common import is_parameter, is_query_instance
-from altqq.types import T
+from altqq.translators import common
+from altqq.types import QueryValueTypes, T
 
 
 @dc.dataclass
 class PyODBCStatement:
     """Represents a generated PyODBC statement."""
 
     statement: Any
@@ -64,24 +64,31 @@
         self.parameter_values.extend(field.parameters)
         return field.statement
 
 
 class PyODBCTranslator:
     """Converts a `Query` to its corresponding `PyODBCQuery` object."""
 
+    MARKER = "?"
+
     def _resolve_value(self, query: Query, field: dc.Field[T]) -> PyODBCStatement:
         value = getattr(query, field.name)
-        if is_query_instance(value):
+        if common.is_query_instance(value):
             qq = self.__call__(value)
             return PyODBCStatement(qq.query, qq.parameters)
 
-        if is_parameter(field.type):
+        field_type = common.get_parameter_type(field.type)
+        if field_type == QueryValueTypes.NON_PARAMETER:
             return PyODBCStatement(value, ())
-
-        return PyODBCStatement("?", [value])
+        elif field_type == QueryValueTypes.LIST_PARAMETER:
+            return PyODBCStatement(
+                common.create_list_markers(self.MARKER, len(value)), value
+            )
+        else:
+            return PyODBCStatement(self.MARKER, [value])
 
     def __call__(self, query: Query) -> PyODBCQuery:
         """Converts a `Query` to its corresponding `PyODBCQuery` object.
 
         Args:
         query (Query): Query to translate to PyODBC
```

### Comparing `altqq-0.0.5/PKG-INFO` & `altqq-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altqq
-Version: 0.0.5
+Version: 0.0.6
 Summary: Alternative Queries: Typed and Reusable Handcrafted SQL
 Home-page: https://altqq.baluyotraf.com
 License: MIT
 Keywords: database,SQL
 Author: baluyotraf
 Author-email: baluyotraf@outlook.com
 Maintainer: baluyotraf
```

