# Comparing `tmp/pg_upsert-0.0.4.tar.gz` & `tmp/pg_upsert-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_upsert-0.0.4.tar", last modified: Tue May 21 18:37:59 2024, max compression
+gzip compressed data, was "pg_upsert-0.0.5.tar", last modified: Tue May 21 18:40:41 2024, max compression
```

## Comparing `pg_upsert-0.0.4.tar` & `pg_upsert-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/pg_upsert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/pg_upsert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81556 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/pg_upsert/pg_upsert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/pg_upsert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:40:41.362310 pg_upsert-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 18:40:28.000000 pg_upsert-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-05-21 18:40:41.358310 pg_upsert-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-21 18:40:28.000000 pg_upsert-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:40:41.358310 pg_upsert-0.0.5/pg_upsert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:40:28.000000 pg_upsert-0.0.5/pg_upsert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81556 2024-05-21 18:40:28.000000 pg_upsert-0.0.5/pg_upsert/pg_upsert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:40:41.358310 pg_upsert-0.0.5/pg_upsert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-05-21 18:40:41.000000 pg_upsert-0.0.5/pg_upsert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-21 18:40:41.000000 pg_upsert-0.0.5/pg_upsert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:40:41.000000 pg_upsert-0.0.5/pg_upsert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 18:40:41.000000 pg_upsert-0.0.5/pg_upsert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 18:40:41.000000 pg_upsert-0.0.5/pg_upsert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 18:40:28.000000 pg_upsert-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:40:41.362310 pg_upsert-0.0.5/setup.cfg
```

### Comparing `pg_upsert-0.0.4/LICENSE` & `pg_upsert-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_upsert-0.0.4/PKG-INFO` & `pg_upsert-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg_upsert
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for upserting data into postgres.
 Author-email: Caleb Grant <grantcaleb22@gmail.com>
 Project-URL: Homepage, https://github.com/geocoug/pg_upsert
 Project-URL: Issues, https://github.com/geocoug/pg_upsert/issues
 Keywords: postgresql,postgres,dbms,etl,upsert,database
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -307,15 +307,15 @@
     update staging.books set book_title = 'The Great Novel 2' where book_id = 'B001';
     ```
 
 5. Run the script again, but this time set `interactive=True` in the `upsert` function call in `load_data.py`.
 
     The script will display GUI dialogs during the upsert process to show which rows will be added and which rows will be updated. The user can chose to confirm, skip, or cancel the upsert process at any time. The script will not commit any changes to the database until all of the upserts have been completed successfully.
 
-    ![screenshot](./screenshot.png)
+    ![screenshot](https://github.com/geocoug/pg_upsert/blob/main/screenshot.png)
 
 6. Let's modify the `staging.books` table to include a row with a missing value in the `book_title` and `Mystery` value in the `genre` column to see what happens.
 
     ```sql
    insert into staging.books (book_id, book_title, genre, notes)
    values ('B003', null, 'Mystery', 'A book with no name!');
     ```
```

### Comparing `pg_upsert-0.0.4/README.md` & `pg_upsert-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
     update staging.books set book_title = 'The Great Novel 2' where book_id = 'B001';
     ```
 
 5. Run the script again, but this time set `interactive=True` in the `upsert` function call in `load_data.py`.
 
     The script will display GUI dialogs during the upsert process to show which rows will be added and which rows will be updated. The user can chose to confirm, skip, or cancel the upsert process at any time. The script will not commit any changes to the database until all of the upserts have been completed successfully.
 
-    ![screenshot](./screenshot.png)
+    ![screenshot](https://github.com/geocoug/pg_upsert/blob/main/screenshot.png)
 
 6. Let's modify the `staging.books` table to include a row with a missing value in the `book_title` and `Mystery` value in the `genre` column to see what happens.
 
     ```sql
    insert into staging.books (book_id, book_title, genre, notes)
    values ('B003', null, 'Mystery', 'A book with no name!');
     ```
```

### Comparing `pg_upsert-0.0.4/pg_upsert/pg_upsert.py` & `pg_upsert-0.0.5/pg_upsert/pg_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import polars as pl
 import psycopg2
 from psycopg2.extras import DictCursor
 from psycopg2.sql import SQL, Composable, Identifier, Literal
 from tabulate import tabulate
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 description_long = """
 Check data in a staging table or set of staging tables, then update and insert (upsert)
 rows of a base table or base tables from the staging table(s) of the same name.
 Initial table checks include not-null, primary key, and foreign key checks.
 If any of these checks fail, the program will exit with an error message.
 If all checks pass, the program will display the number of rows to be inserted
```

### Comparing `pg_upsert-0.0.4/pg_upsert.egg-info/PKG-INFO` & `pg_upsert-0.0.5/pg_upsert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg_upsert
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for upserting data into postgres.
 Author-email: Caleb Grant <grantcaleb22@gmail.com>
 Project-URL: Homepage, https://github.com/geocoug/pg_upsert
 Project-URL: Issues, https://github.com/geocoug/pg_upsert/issues
 Keywords: postgresql,postgres,dbms,etl,upsert,database
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -307,15 +307,15 @@
     update staging.books set book_title = 'The Great Novel 2' where book_id = 'B001';
     ```
 
 5. Run the script again, but this time set `interactive=True` in the `upsert` function call in `load_data.py`.
 
     The script will display GUI dialogs during the upsert process to show which rows will be added and which rows will be updated. The user can chose to confirm, skip, or cancel the upsert process at any time. The script will not commit any changes to the database until all of the upserts have been completed successfully.
 
-    ![screenshot](./screenshot.png)
+    ![screenshot](https://github.com/geocoug/pg_upsert/blob/main/screenshot.png)
 
 6. Let's modify the `staging.books` table to include a row with a missing value in the `book_title` and `Mystery` value in the `genre` column to see what happens.
 
     ```sql
    insert into staging.books (book_id, book_title, genre, notes)
    values ('B003', null, 'Mystery', 'A book with no name!');
     ```
```

### Comparing `pg_upsert-0.0.4/pyproject.toml` & `pg_upsert-0.0.5/pyproject.toml`

 * *Files identical despite different names*

