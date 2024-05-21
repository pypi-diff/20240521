# Comparing `tmp/pg_upsert-0.0.3.tar.gz` & `tmp/pg_upsert-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_upsert-0.0.3.tar", last modified: Mon May 20 22:57:08 2024, max compression
+gzip compressed data, was "pg_upsert-0.0.4.tar", last modified: Tue May 21 18:37:59 2024, max compression
```

## Comparing `pg_upsert-0.0.3.tar` & `pg_upsert-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/pg_upsert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/pg_upsert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81474 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/pg_upsert/pg_upsert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/pg_upsert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/pg_upsert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/pg_upsert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81556 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/pg_upsert/pg_upsert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/pg_upsert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 18:37:59.000000 pg_upsert-0.0.4/pg_upsert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 18:37:47.000000 pg_upsert-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:37:59.724758 pg_upsert-0.0.4/setup.cfg
```

### Comparing `pg_upsert-0.0.3/LICENSE` & `pg_upsert-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_upsert-0.0.3/pg_upsert/pg_upsert.py` & `pg_upsert-0.0.4/pg_upsert/pg_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 import polars as pl
 import psycopg2
 from psycopg2.extras import DictCursor
 from psycopg2.sql import SQL, Composable, Identifier, Literal
 from tabulate import tabulate
 
+__version__ = "0.0.4"
+
 description_long = """
 Check data in a staging table or set of staging tables, then update and insert (upsert)
 rows of a base table or base tables from the staging table(s) of the same name.
 Initial table checks include not-null, primary key, and foreign key checks.
 If any of these checks fail, the program will exit with an error message.
 If all checks pass, the program will display the number of rows to be inserted
 and updated, and ask for confirmation before proceeding. If the user confirms, the
@@ -1982,15 +1984,14 @@
                 stg_schema=Identifier(stg_schema),
                 table=Identifier(table),
                 pk_col_list=SQL(pk_col_list),
                 base_schema=Identifier(base_schema),
             ),
         )
         # Prompt user to examine new data and continue or quit.
-        # new_df = db.dataframe("select * from ups_newrows;")
         new_curs = db.execute("select * from ups_newrows;")
         new_cols = [col.name for col in new_curs.description]
         new_rowcount = new_curs.rowcount
         new_data = new_curs.fetchall()
 
         # if not new_df.is_empty():
         if new_rowcount > 0:
@@ -2069,14 +2070,19 @@
     """Command line interface for the upsert function."""
     parser = argparse.ArgumentParser(
         description=description_short,
         epilog=description_long,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument(
+        "--version",
+        action="version",
+        version=f"%(prog)s {__version__}",
+    )
+    parser.add_argument(
         "-q",
         "--quiet",
         action="store_true",
         help="suppress all console output",
     )
     parser.add_argument(
         "-d",
```

