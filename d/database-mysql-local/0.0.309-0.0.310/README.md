# Comparing `tmp/database_mysql_local-0.0.309.tar.gz` & `tmp/database_mysql_local-0.0.310.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.309.tar", last modified: Mon May 20 18:44:04 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.310.tar", last modified: Mon May 20 22:40:44 2024, max compression
```

## Comparing `database_mysql_local-0.0.309.tar` & `database_mysql_local-0.0.310.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:44:04.588518 database_mysql_local-0.0.309/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-20 18:43:35.000000 database_mysql_local-0.0.309/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51582 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31830 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-20 18:43:35.000000 database_mysql_local-0.0.309/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-20 18:43:35.000000 database_mysql_local-0.0.309/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 18:44:04.000000 database_mysql_local-0.0.309/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:44:04.596518 database_mysql_local-0.0.309/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-20 18:43:09.000000 database_mysql_local-0.0.309/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:40:44.875030 database_mysql_local-0.0.310/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51577 2024-05-20 22:40:14.000000 database_mysql_local-0.0.310/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31830 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-20 22:40:14.000000 database_mysql_local-0.0.310/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-20 22:40:14.000000 database_mysql_local-0.0.310/setup.py
```

### Comparing `database_mysql_local-0.0.309/PKG-INFO` & `database_mysql_local-0.0.310/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.309
+Version: 0.0.310
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
-Author-email: info@circles.life
+Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python>=8.3.0
 Requires-Dist: url-remote>=0.0.80
```

### Comparing `database_mysql_local-0.0.309/README.md` & `database_mysql_local-0.0.310/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.310/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.310/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.310/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.310/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         self._validate_args(args=locals())
 
         # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
         # TODO: If is_test_data exists in the table and is_test_data=False, add `AND is_test_data=0` to avoid users getting test data
         #   (but the tests should be allowed to access real data)
         if (self.is_test_data and (view_table_name or "").replace("_view", "") ==
-                (self.default_view_table_name or "").replace("_table", "")):
+                (self.default_table_name or "").replace("_table", "")):
             # test data does not appear in the view, but we still wants to access it in tests (partial solution).
             view_table_name = self.default_table_name
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
```

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.310/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.310/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/point.py` & `database_mysql_local-0.0.310/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.310/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.310/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.310/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.310/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.310/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.310/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.309
+Version: 0.0.310
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
-Author-email: info@circles.life
+Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python>=8.3.0
 Requires-Dist: url-remote>=0.0.80
```

### Comparing `database_mysql_local-0.0.309/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.310/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/pyproject.toml` & `database_mysql_local-0.0.310/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.309/setup.py` & `database_mysql_local-0.0.310/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.309',
+    version='0.0.310',
     author="Circles",
-    author_email="info@circles.life",
+    author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
     long_description_content_type='text/markdown',
     classifiers=[
```

