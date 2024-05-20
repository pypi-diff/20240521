# Comparing `tmp/database_mysql_local-0.0.308.tar.gz` & `tmp/database_mysql_local-0.0.309.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.308.tar", last modified: Mon May 20 11:16:53 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.309.tar", last modified: Mon May 20 18:44:04 2024, max compression
```

## Comparing `database_mysql_local-0.0.308.tar` & `database_mysql_local-0.0.309.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:16:53.489167 database_mysql_local-0.0.308/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 11:16:53.489167 database_mysql_local-0.0.308/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:16:53.481167 database_mysql_local-0.0.308/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:16:53.485167 database_mysql_local-0.0.308/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51501 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31830 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-20 11:16:18.000000 database_mysql_local-0.0.308/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:16:53.489167 database_mysql_local-0.0.308/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:16:53.489167 database_mysql_local-0.0.308/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:44:04.588518 database_mysql_local-0.0.309/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-20 18:43:35.000000 database_mysql_local-0.0.309/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51582 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31830 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-20 18:43:35.000000 database_mysql_local-0.0.309/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-20 18:43:35.000000 database_mysql_local-0.0.309/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/setup.py
```

### Comparing `database_mysql_local-0.0.308/PKG-INFO` & `database_mysql_local-0.0.309/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.308
+Version: 0.0.309
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.308/README.md` & `database_mysql_local-0.0.309/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.309/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.309/database_mysql_local/src/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 DEFAULT_SQL_SELECT_LIMIT = 100
 
 
+# TODO Move everything related to sync to separate directory called sync_data_source (preferable with it's own src and tests directories)
 class UpdateStatus(Enum):
     UPDATE_DATA_SOURCE = -1
     DONT_UPDATE = 0
     UPDATE_CIRCLEZ = 1
 
 
 # connector / cursor
```

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.309/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.309/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from user_context_remote.user_context import UserContext
 
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .table_definition import table_definition
 from .utils import (process_insert_data_dict, process_update_data_dict, get_where_params, where_skip_null_values,
                     validate_none_select_table_name, validate_single_clause_value,
-                    validate_select_table_name, detect_if_is_test_data,
+                    validate_select_table_name, detect_if_is_test_data, generate_table_name,
                     generate_view_name, generate_column_name, get_entity_type_by_table_name)
 
 
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
     The rest of the functions are helper functions or wrappers around the main functions."""
@@ -29,35 +29,35 @@
                  default_column_name: str = None, default_id_column_name: str = None,
                  default_select_clause_value: str = "*", default_where: str = None, is_test_data: bool = False) -> None:
         """Initializes the GenericCRUD class. If a connection is not provided, a new connection will be created."""
         self.default_schema_name = default_schema_name
         self.connection = Connector.connect(schema_name=default_schema_name)
         self.cursor = self.connection.cursor()
         self.default_column_name = self._deprecated_id_column(default_id_column_name, default_column_name)
-        self.default_table_name = default_table_name
+        self.default_table_name = default_table_name or generate_table_name(default_schema_name)
         self.default_view_table_name = default_view_table_name or generate_view_name(default_table_name)
         self.default_select_clause_value = default_select_clause_value
         self.default_where = default_where
         self.is_test_data = is_test_data or detect_if_is_test_data()
         self.user_context = UserContext()
 
     def _data_json_to_dict(self, data_json: dict = None) -> dict:
         if data_json is not None:
             # We let the developers migrate quietly for a week
-            if datetime.now() > datetime(2024, 5, 20):
+            if datetime.now() > datetime(2024, 5, 25):
                 self.logger.warning(
                     "GenericCRUD: data_json is deprecated and scheduled to be removed by 12/06/2024, use data_dict instead. "
                     "In general, use _dict when the the typing is dict and _json when the typing is json / str.")
 
             return data_json
 
     def _deprecated_id_column(self, id_column_name: str, column_name: str) -> str:
         if id_column_name:
             # We let the developers migrate quietly for a week
-            if datetime.now() > datetime(2024, 5, 20):
+            if datetime.now() > datetime(2024, 5, 25):
                 # TODO: print the caller filename
                 self.logger.warning(
                     "GenericCRUD: id_column_name and id_column_value are deprecated and scheduled to be removed by 12/06/2024, use column_name and column_value instead.")
             return id_column_name
         return column_name
 
     def insert(self, *, schema_name: str = None, table_name: str = None, data_dict: dict = None, data_json: dict = None,
@@ -249,15 +249,15 @@
         self.logger.debug(object=locals())
         return existing_duplicate_id
 
     def update_by_id(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> None:
-        if datetime.now() > datetime(2024, 5, 20):
+        if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning("GenericCRUD.update_by_id is deprecated, use update_by_column_and_value instead.")
         return self.update_by_column_and_value(schema_name=schema_name, table_name=table_name,
                                                column_name=column_name, column_value=column_value,
                                                id_column_name=id_column_name, id_column_value=id_column_value,
                                                data_dict=data_dict, data_json=data_json,
                                                limit=limit, order_by=order_by, commit_changes=commit_changes)
 
@@ -313,15 +313,15 @@
         self.cursor.execute(update_query, tuple(data_dict.values()) + params)
         if commit_changes:
             self.connection.commit()
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
                      column_name: str = None, column_value: Any = None,
                      id_column_name: str = None, id_column_value: Any = None) -> None:
-        if datetime.now() > datetime(2024, 5, 20):
+        if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning("GenericCRUD.delete_by_id is deprecated, use delete_by_column_and_value instead.")
         return self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
                                                column_name=column_name, column_value=column_value,
                                                id_column_name=id_column_name, id_column_value=id_column_value)
 
     def delete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
                                    column_name: str = None, column_value: Any = None,
@@ -366,16 +366,16 @@
         where = self.__where_security(where=where, view_name=view_table_name)
         self._validate_args(args=locals())
 
         # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
         # TODO: If is_test_data exists in the table and is_test_data=False, add `AND is_test_data=0` to avoid users getting test data
         #   (but the tests should be allowed to access real data)
-        if (self.is_test_data and view_table_name.replace("_view", "") ==
-                self.default_view_table_name.replace("_table", "")):
+        if (self.is_test_data and (view_table_name or "").replace("_view", "") ==
+                (self.default_view_table_name or "").replace("_table", "")):
             # test data does not appear in the view, but we still wants to access it in tests (partial solution).
             view_table_name = self.default_table_name
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
@@ -396,15 +396,15 @@
 
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
                                column_name: str = None, column_value: Any = None,
                                id_column_name: str = None, id_column_value: Any = None,
                                distinct: bool = False, order_by: str = "") -> tuple:
-        if datetime.now() > datetime(2024, 5, 20):
+        if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_one_tuple_by_id is deprecated, use select_one_tuple_by_column_and_value instead.")
         return self.select_one_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by)
 
@@ -423,15 +423,15 @@
         else:
             return tuple()  # or None?
 
     def select_one_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "") -> dict:
-        if datetime.now() > datetime(2024, 5, 20):
+        if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_one_dict_by_id is deprecated, use select_one_dict_by_column_and_value instead.")
         return self.select_one_dict_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by)
 
@@ -447,15 +447,15 @@
             column_name=column_name, column_value=column_value, distinct=distinct, order_by=order_by)
         return self.convert_to_dict(result, select_clause_value)
 
     def select_one_value_by_id(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
-        if datetime.now() > datetime(2024, 5, 20):
+        if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_one_value_by_id is deprecated, use select_one_value_by_column_and_value instead.")
         return self.select_one_value_by_column_and_value(
             select_clause_value=select_clause_value, schema_name=schema_name, view_table_name=view_table_name,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by, skip_null_values=skip_null_values)
 
@@ -513,15 +513,15 @@
             return result[0]
 
     def select_multi_value_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
-        if datetime.now() > datetime(2024, 5, 20):
+        if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_multi_value_by_id is deprecated, use select_multi_value_by_column_and_value instead.")
         return self.select_multi_value_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by,
             skip_null_values=skip_null_values)
@@ -556,15 +556,15 @@
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
     def select_multi_tuple_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
-        if datetime.now() > datetime(2024, 5, 20):
+        if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_multi_tuple_by_id is deprecated, use select_multi_tuple_by_column_and_value instead.")
         return self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
 
@@ -593,15 +593,15 @@
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
 
     def select_multi_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
-        if datetime.now() > datetime(2024, 5, 20):
+        if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_multi_dict_by_id is deprecated, use select_multi_dict_by_column_and_value instead.")
         return self.select_multi_dict_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
```

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.309/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.309/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/point.py` & `database_mysql_local-0.0.309/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.309/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.309/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# TODO Move everything related to sync to separate directory called sync_data_source (preferable with it's own src and tests directories)
 from datetime import datetime
 
 from .constants import UpdateStatus
 from .generic_crud import GenericCRUD
 
 
 # TODO: use meta logger
```

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.309/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.309/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.309/database_mysql_local/src/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,19 @@
 def get_entity_type_by_table_name(table_name: str) -> int or None:
     """Returns the entity_type_id of the table."""
     if table_name in table_definition:
         entity_type_id = table_definition[table_name].get("entity_type_id1")
         return entity_type_id
 
 
+def generate_table_name(schema_name: Optional[str]) -> Optional[str]:
+    if schema_name:
+        return schema_name + "_table"
+
+
 def generate_view_name(table_name: Optional[str]) -> Optional[str]:
     if table_name:
         return re.sub(r'(_table)$', '_view', table_name)
 
 
 def generate_column_name(table_name: Optional[str]) -> Optional[str]:
     if table_name:
```

### Comparing `database_mysql_local-0.0.308/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.309/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.308
+Version: 0.0.309
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.308/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.309/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/pyproject.toml` & `database_mysql_local-0.0.309/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.308/setup.py` & `database_mysql_local-0.0.309/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
-# TODO: we are migrating from database_mysql_local to database_mysql_local
-#  but in the meantime we want to keep both names
-old_name = "database_mysql_local"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.308',
+    version='0.0.309',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
-    packages=[package_dir, old_name],
-    package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
+    packages=[package_dir],
+    package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
```

