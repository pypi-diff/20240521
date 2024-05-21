# Comparing `tmp/Nagra-0.0.4.zip` & `tmp/Nagra-0.1.0.zip`

## zipinfo {}

```diff
@@ -1,65 +1,65 @@
-Zip file size: 35053 bytes, number of entries: 63
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 13:11 Nagra-0.0.4/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 13:11 Nagra-0.0.4/Nagra.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 13:11 Nagra-0.0.4/nagra/
--rw-r--r--  2.0 unx      426 b- defN 24-Apr-03 13:11 Nagra-0.0.4/PKG-INFO
--rw-r--r--  2.0 unx    11357 b- defN 24-Feb-08 12:03 Nagra-0.0.4/LICENSE
--rw-r--r--  2.0 unx     5246 b- defN 24-Mar-25 13:37 Nagra-0.0.4/README.md
--rw-r--r--  2.0 unx     1135 b- defN 24-Mar-24 21:40 Nagra-0.0.4/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-03 13:11 Nagra-0.0.4/setup.cfg
--rw-r--r--  2.0 unx      426 b- defN 24-Apr-03 13:11 Nagra-0.0.4/Nagra.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     1659 b- defN 24-Apr-03 13:11 Nagra-0.0.4/Nagra.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       40 b- defN 24-Apr-03 13:11 Nagra-0.0.4/Nagra.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       39 b- defN 24-Apr-03 13:11 Nagra-0.0.4/Nagra.egg-info/requires.txt
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-03 13:11 Nagra-0.0.4/Nagra.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 13:11 Nagra-0.0.4/Nagra.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 13:11 Nagra-0.0.4/nagra/template/
--rw-r--r--  2.0 unx     1187 b- defN 24-Mar-29 07:30 Nagra-0.0.4/nagra/delete.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-29 07:53 Nagra-0.0.4/nagra/misc.py
--rw-r--r--  2.0 unx     3721 b- defN 24-Mar-29 07:56 Nagra-0.0.4/nagra/transaction.py
--rw-r--r--  2.0 unx      734 b- defN 24-Mar-29 07:54 Nagra-0.0.4/nagra/statement.py
--rw-r--r--  2.0 unx     9377 b- defN 24-Mar-29 08:02 Nagra-0.0.4/nagra/sexpr.py
--rw-r--r--  2.0 unx      145 b- defN 24-Apr-03 13:10 Nagra-0.0.4/nagra/__init__.py
--rw-r--r--  2.0 unx     3446 b- defN 24-Apr-02 17:02 Nagra-0.0.4/nagra/cli.py
--rw-r--r--  2.0 unx     1998 b- defN 24-Mar-29 07:53 Nagra-0.0.4/nagra/utils.py
--rw-r--r--  2.0 unx      262 b- defN 24-Feb-29 15:38 Nagra-0.0.4/nagra/exceptions.py
--rw-r--r--  2.0 unx     6095 b- defN 24-Mar-29 07:54 Nagra-0.0.4/nagra/table.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-03 11:46 Nagra-0.0.4/nagra/select.py
--rw-r--r--  2.0 unx       28 b- defN 24-Feb-05 09:54 Nagra-0.0.4/nagra/__main__.py
--rw-r--r--  2.0 unx     5264 b- defN 24-Mar-29 07:38 Nagra-0.0.4/nagra/upsert.py
--rw-r--r--  2.0 unx     3970 b- defN 24-Apr-02 17:03 Nagra-0.0.4/nagra/schema.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 13:11 Nagra-0.0.4/nagra/template/postgresql/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 13:11 Nagra-0.0.4/nagra/template/sqlite/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 13:11 Nagra-0.0.4/nagra/template/duckdb/
--rw-r--r--  2.0 unx       40 b- defN 24-Feb-12 09:55 Nagra-0.0.4/nagra/template/postgresql/drop_table.sql
--rw-r--r--  2.0 unx       99 b- defN 24-Jan-09 13:47 Nagra-0.0.4/nagra/template/postgresql/delete.sql
--rw-r--r--  2.0 unx      567 b- defN 24-Feb-19 21:55 Nagra-0.0.4/nagra/template/postgresql/select.sql
--rw-r--r--  2.0 unx      344 b- defN 24-Feb-19 22:54 Nagra-0.0.4/nagra/template/postgresql/delete-with-join.sql
--rw-r--r--  2.0 unx      120 b- defN 24-Mar-25 11:29 Nagra-0.0.4/nagra/template/postgresql/find_columns.sql
--rw-r--r--  2.0 unx      425 b- defN 24-Feb-20 14:49 Nagra-0.0.4/nagra/template/postgresql/upsert.sql
--rw-r--r--  2.0 unx      186 b- defN 24-Mar-24 17:08 Nagra-0.0.4/nagra/template/postgresql/add_column.sql
--rw-r--r--  2.0 unx      374 b- defN 23-Sep-25 20:38 Nagra-0.0.4/nagra/template/postgresql/find_foreign_keys.sql
--rw-r--r--  2.0 unx       58 b- defN 24-Mar-24 14:24 Nagra-0.0.4/nagra/template/postgresql/create_table.sql
--rw-r--r--  2.0 unx       78 b- defN 23-Sep-17 13:24 Nagra-0.0.4/nagra/template/postgresql/debug.sql
--rw-r--r--  2.0 unx      166 b- defN 23-Sep-25 20:38 Nagra-0.0.4/nagra/template/postgresql/create_unique_index.sql
--rw-r--r--  2.0 unx       32 b- defN 24-Feb-12 09:55 Nagra-0.0.4/nagra/template/sqlite/drop_table.sql
--rw-r--r--  2.0 unx       99 b- defN 24-Jan-09 13:46 Nagra-0.0.4/nagra/template/sqlite/delete.sql
--rw-r--r--  2.0 unx      570 b- defN 24-Feb-19 22:51 Nagra-0.0.4/nagra/template/sqlite/select.sql
--rw-r--r--  2.0 unx      344 b- defN 24-Feb-19 22:54 Nagra-0.0.4/nagra/template/sqlite/delete-with-join.sql
--rw-r--r--  2.0 unx      189 b- defN 24-Mar-25 11:30 Nagra-0.0.4/nagra/template/sqlite/find_columns.sql
--rw-r--r--  2.0 unx      424 b- defN 24-Mar-20 17:03 Nagra-0.0.4/nagra/template/sqlite/upsert.sql
--rw-r--r--  2.0 unx      186 b- defN 24-Mar-24 17:08 Nagra-0.0.4/nagra/template/sqlite/add_column.sql
--rw-r--r--  2.0 unx       56 b- defN 24-Mar-24 21:25 Nagra-0.0.4/nagra/template/sqlite/create_table.sql
--rw-r--r--  2.0 unx       37 b- defN 23-Nov-08 22:09 Nagra-0.0.4/nagra/template/sqlite/select_foreign_keys.sql
--rw-r--r--  2.0 unx       78 b- defN 23-Oct-27 08:20 Nagra-0.0.4/nagra/template/sqlite/debug.sql
--rw-r--r--  2.0 unx      166 b- defN 23-Oct-27 08:20 Nagra-0.0.4/nagra/template/sqlite/create_unique_index.sql
--rw-r--r--  2.0 unx       99 b- defN 24-Feb-10 17:12 Nagra-0.0.4/nagra/template/duckdb/add_foreign_key.sql
--rw-r--r--  2.0 unx       73 b- defN 23-Dec-06 21:51 Nagra-0.0.4/nagra/template/duckdb/delete.sql
--rw-r--r--  2.0 unx      579 b- defN 23-Dec-06 21:51 Nagra-0.0.4/nagra/template/duckdb/select.sql
--rw-r--r--  2.0 unx      271 b- defN 23-Dec-06 21:51 Nagra-0.0.4/nagra/template/duckdb/delete-with-join.sql
--rw-r--r--  2.0 unx      386 b- defN 23-Dec-06 22:47 Nagra-0.0.4/nagra/template/duckdb/upsert.sql
--rw-r--r--  2.0 unx      323 b- defN 23-Dec-06 22:35 Nagra-0.0.4/nagra/template/duckdb/create_table.sql
--rw-r--r--  2.0 unx       37 b- defN 23-Dec-06 21:59 Nagra-0.0.4/nagra/template/duckdb/select_foreign_keys.sql
--rw-r--r--  2.0 unx       78 b- defN 23-Dec-06 21:51 Nagra-0.0.4/nagra/template/duckdb/debug.sql
--rw-r--r--  2.0 unx      166 b- defN 23-Dec-06 21:51 Nagra-0.0.4/nagra/template/duckdb/create_unique_index.sql
-63 files, 69576 bytes uncompressed, 25273 bytes compressed:  63.7%
+Zip file size: 36609 bytes, number of entries: 63
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 17:09 Nagra-0.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 17:09 Nagra-0.1.0/Nagra.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 17:09 Nagra-0.1.0/nagra/
+-rw-r--r--  2.0 unx      426 b- defN 24-May-21 17:09 Nagra-0.1.0/PKG-INFO
+-rw-r--r--  2.0 unx    11357 b- defN 24-Feb-08 12:03 Nagra-0.1.0/LICENSE
+-rw-r--r--  2.0 unx     5246 b- defN 24-Mar-25 13:37 Nagra-0.1.0/README.md
+-rw-r--r--  2.0 unx     1148 b- defN 24-Apr-04 17:22 Nagra-0.1.0/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-May-21 17:09 Nagra-0.1.0/setup.cfg
+-rw-r--r--  2.0 unx      426 b- defN 24-May-21 17:09 Nagra-0.1.0/Nagra.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     1659 b- defN 24-May-21 17:09 Nagra-0.1.0/Nagra.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       40 b- defN 24-May-21 17:09 Nagra-0.1.0/Nagra.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-May-21 17:09 Nagra-0.1.0/Nagra.egg-info/requires.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-May-21 17:09 Nagra-0.1.0/Nagra.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 17:09 Nagra-0.1.0/Nagra.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 17:09 Nagra-0.1.0/nagra/template/
+-rw-r--r--  2.0 unx     1705 b- defN 24-May-15 17:11 Nagra-0.1.0/nagra/delete.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-29 07:53 Nagra-0.1.0/nagra/misc.py
+-rw-r--r--  2.0 unx     3808 b- defN 24-May-21 17:01 Nagra-0.1.0/nagra/transaction.py
+-rw-r--r--  2.0 unx      734 b- defN 24-Mar-29 07:54 Nagra-0.1.0/nagra/statement.py
+-rw-r--r--  2.0 unx     9615 b- defN 24-May-21 17:01 Nagra-0.1.0/nagra/sexpr.py
+-rw-r--r--  2.0 unx      145 b- defN 24-May-21 17:08 Nagra-0.1.0/nagra/__init__.py
+-rw-r--r--  2.0 unx     3439 b- defN 24-May-15 10:12 Nagra-0.1.0/nagra/cli.py
+-rw-r--r--  2.0 unx     1998 b- defN 24-Mar-29 07:53 Nagra-0.1.0/nagra/utils.py
+-rw-r--r--  2.0 unx      311 b- defN 24-May-15 10:12 Nagra-0.1.0/nagra/exceptions.py
+-rw-r--r--  2.0 unx     7816 b- defN 24-May-21 17:01 Nagra-0.1.0/nagra/table.py
+-rw-r--r--  2.0 unx     7560 b- defN 24-May-21 17:01 Nagra-0.1.0/nagra/select.py
+-rw-r--r--  2.0 unx       28 b- defN 24-Feb-05 09:54 Nagra-0.1.0/nagra/__main__.py
+-rw-r--r--  2.0 unx     6135 b- defN 24-May-15 16:55 Nagra-0.1.0/nagra/upsert.py
+-rw-r--r--  2.0 unx     4234 b- defN 24-May-21 17:01 Nagra-0.1.0/nagra/schema.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 17:09 Nagra-0.1.0/nagra/template/postgresql/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 17:09 Nagra-0.1.0/nagra/template/sqlite/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 17:09 Nagra-0.1.0/nagra/template/duckdb/
+-rw-r--r--  2.0 unx       40 b- defN 24-Feb-12 09:55 Nagra-0.1.0/nagra/template/postgresql/drop_table.sql
+-rw-r--r--  2.0 unx       99 b- defN 24-Jan-09 13:47 Nagra-0.1.0/nagra/template/postgresql/delete.sql
+-rw-r--r--  2.0 unx      567 b- defN 24-Feb-19 21:55 Nagra-0.1.0/nagra/template/postgresql/select.sql
+-rw-r--r--  2.0 unx      344 b- defN 24-Feb-19 22:54 Nagra-0.1.0/nagra/template/postgresql/delete-with-join.sql
+-rw-r--r--  2.0 unx      120 b- defN 24-Mar-25 11:29 Nagra-0.1.0/nagra/template/postgresql/find_columns.sql
+-rw-r--r--  2.0 unx      425 b- defN 24-Feb-20 14:49 Nagra-0.1.0/nagra/template/postgresql/upsert.sql
+-rw-r--r--  2.0 unx      285 b- defN 24-May-21 17:01 Nagra-0.1.0/nagra/template/postgresql/add_column.sql
+-rw-r--r--  2.0 unx      374 b- defN 23-Sep-25 20:38 Nagra-0.1.0/nagra/template/postgresql/find_foreign_keys.sql
+-rw-r--r--  2.0 unx       75 b- defN 24-May-07 14:18 Nagra-0.1.0/nagra/template/postgresql/create_table.sql
+-rw-r--r--  2.0 unx       78 b- defN 23-Sep-17 13:24 Nagra-0.1.0/nagra/template/postgresql/debug.sql
+-rw-r--r--  2.0 unx      166 b- defN 23-Sep-25 20:38 Nagra-0.1.0/nagra/template/postgresql/create_unique_index.sql
+-rw-r--r--  2.0 unx       32 b- defN 24-Feb-12 09:55 Nagra-0.1.0/nagra/template/sqlite/drop_table.sql
+-rw-r--r--  2.0 unx       99 b- defN 24-Jan-09 13:46 Nagra-0.1.0/nagra/template/sqlite/delete.sql
+-rw-r--r--  2.0 unx      570 b- defN 24-Feb-19 22:51 Nagra-0.1.0/nagra/template/sqlite/select.sql
+-rw-r--r--  2.0 unx      344 b- defN 24-Feb-19 22:54 Nagra-0.1.0/nagra/template/sqlite/delete-with-join.sql
+-rw-r--r--  2.0 unx      189 b- defN 24-Mar-25 11:30 Nagra-0.1.0/nagra/template/sqlite/find_columns.sql
+-rw-r--r--  2.0 unx      424 b- defN 24-Mar-20 17:03 Nagra-0.1.0/nagra/template/sqlite/upsert.sql
+-rw-r--r--  2.0 unx      286 b- defN 24-May-21 17:01 Nagra-0.1.0/nagra/template/sqlite/add_column.sql
+-rw-r--r--  2.0 unx       74 b- defN 24-May-07 14:18 Nagra-0.1.0/nagra/template/sqlite/create_table.sql
+-rw-r--r--  2.0 unx       37 b- defN 23-Nov-08 22:09 Nagra-0.1.0/nagra/template/sqlite/select_foreign_keys.sql
+-rw-r--r--  2.0 unx       78 b- defN 23-Oct-27 08:20 Nagra-0.1.0/nagra/template/sqlite/debug.sql
+-rw-r--r--  2.0 unx      166 b- defN 23-Oct-27 08:20 Nagra-0.1.0/nagra/template/sqlite/create_unique_index.sql
+-rw-r--r--  2.0 unx       99 b- defN 24-Feb-10 17:12 Nagra-0.1.0/nagra/template/duckdb/add_foreign_key.sql
+-rw-r--r--  2.0 unx       73 b- defN 23-Dec-06 21:51 Nagra-0.1.0/nagra/template/duckdb/delete.sql
+-rw-r--r--  2.0 unx      579 b- defN 23-Dec-06 21:51 Nagra-0.1.0/nagra/template/duckdb/select.sql
+-rw-r--r--  2.0 unx      271 b- defN 23-Dec-06 21:51 Nagra-0.1.0/nagra/template/duckdb/delete-with-join.sql
+-rw-r--r--  2.0 unx      386 b- defN 23-Dec-06 22:47 Nagra-0.1.0/nagra/template/duckdb/upsert.sql
+-rw-r--r--  2.0 unx      323 b- defN 23-Dec-06 22:35 Nagra-0.1.0/nagra/template/duckdb/create_table.sql
+-rw-r--r--  2.0 unx       37 b- defN 23-Dec-06 21:59 Nagra-0.1.0/nagra/template/duckdb/select_foreign_keys.sql
+-rw-r--r--  2.0 unx       78 b- defN 23-Dec-06 21:51 Nagra-0.1.0/nagra/template/duckdb/debug.sql
+-rw-r--r--  2.0 unx      166 b- defN 23-Dec-06 21:51 Nagra-0.1.0/nagra/template/duckdb/create_unique_index.sql
+63 files, 74808 bytes uncompressed, 26829 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,190 +1,190 @@
-Filename: Nagra-0.0.4/
+Filename: Nagra-0.1.0/
 Comment: 
 
-Filename: Nagra-0.0.4/Nagra.egg-info/
+Filename: Nagra-0.1.0/Nagra.egg-info/
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/
+Filename: Nagra-0.1.0/nagra/
 Comment: 
 
-Filename: Nagra-0.0.4/PKG-INFO
+Filename: Nagra-0.1.0/PKG-INFO
 Comment: 
 
-Filename: Nagra-0.0.4/LICENSE
+Filename: Nagra-0.1.0/LICENSE
 Comment: 
 
-Filename: Nagra-0.0.4/README.md
+Filename: Nagra-0.1.0/README.md
 Comment: 
 
-Filename: Nagra-0.0.4/setup.py
+Filename: Nagra-0.1.0/setup.py
 Comment: 
 
-Filename: Nagra-0.0.4/setup.cfg
+Filename: Nagra-0.1.0/setup.cfg
 Comment: 
 
-Filename: Nagra-0.0.4/Nagra.egg-info/PKG-INFO
+Filename: Nagra-0.1.0/Nagra.egg-info/PKG-INFO
 Comment: 
 
-Filename: Nagra-0.0.4/Nagra.egg-info/SOURCES.txt
+Filename: Nagra-0.1.0/Nagra.egg-info/SOURCES.txt
 Comment: 
 
-Filename: Nagra-0.0.4/Nagra.egg-info/entry_points.txt
+Filename: Nagra-0.1.0/Nagra.egg-info/entry_points.txt
 Comment: 
 
-Filename: Nagra-0.0.4/Nagra.egg-info/requires.txt
+Filename: Nagra-0.1.0/Nagra.egg-info/requires.txt
 Comment: 
 
-Filename: Nagra-0.0.4/Nagra.egg-info/top_level.txt
+Filename: Nagra-0.1.0/Nagra.egg-info/top_level.txt
 Comment: 
 
-Filename: Nagra-0.0.4/Nagra.egg-info/dependency_links.txt
+Filename: Nagra-0.1.0/Nagra.egg-info/dependency_links.txt
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/
+Filename: Nagra-0.1.0/nagra/template/
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/delete.py
+Filename: Nagra-0.1.0/nagra/delete.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/misc.py
+Filename: Nagra-0.1.0/nagra/misc.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/transaction.py
+Filename: Nagra-0.1.0/nagra/transaction.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/statement.py
+Filename: Nagra-0.1.0/nagra/statement.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/sexpr.py
+Filename: Nagra-0.1.0/nagra/sexpr.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/__init__.py
+Filename: Nagra-0.1.0/nagra/__init__.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/cli.py
+Filename: Nagra-0.1.0/nagra/cli.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/utils.py
+Filename: Nagra-0.1.0/nagra/utils.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/exceptions.py
+Filename: Nagra-0.1.0/nagra/exceptions.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/table.py
+Filename: Nagra-0.1.0/nagra/table.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/select.py
+Filename: Nagra-0.1.0/nagra/select.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/__main__.py
+Filename: Nagra-0.1.0/nagra/__main__.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/upsert.py
+Filename: Nagra-0.1.0/nagra/upsert.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/schema.py
+Filename: Nagra-0.1.0/nagra/schema.py
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/
+Filename: Nagra-0.1.0/nagra/template/postgresql/
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/
+Filename: Nagra-0.1.0/nagra/template/sqlite/
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/
+Filename: Nagra-0.1.0/nagra/template/duckdb/
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/drop_table.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/drop_table.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/delete.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/delete.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/select.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/select.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/delete-with-join.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/delete-with-join.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/find_columns.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/find_columns.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/upsert.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/upsert.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/add_column.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/add_column.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/find_foreign_keys.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/find_foreign_keys.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/create_table.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/create_table.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/debug.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/debug.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/postgresql/create_unique_index.sql
+Filename: Nagra-0.1.0/nagra/template/postgresql/create_unique_index.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/drop_table.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/drop_table.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/delete.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/delete.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/select.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/select.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/delete-with-join.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/delete-with-join.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/find_columns.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/find_columns.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/upsert.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/upsert.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/add_column.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/add_column.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/create_table.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/create_table.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/select_foreign_keys.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/select_foreign_keys.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/debug.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/debug.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/sqlite/create_unique_index.sql
+Filename: Nagra-0.1.0/nagra/template/sqlite/create_unique_index.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/add_foreign_key.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/add_foreign_key.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/delete.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/delete.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/select.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/select.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/delete-with-join.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/delete-with-join.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/upsert.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/upsert.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/create_table.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/create_table.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/select_foreign_keys.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/select_foreign_keys.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/debug.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/debug.sql
 Comment: 
 
-Filename: Nagra-0.0.4/nagra/template/duckdb/create_unique_index.sql
+Filename: Nagra-0.1.0/nagra/template/duckdb/create_unique_index.sql
 Comment: 
 
 Zip file comment:
```

## Comparing `Nagra-0.0.4/LICENSE` & `Nagra-0.1.0/LICENSE`

 * *Files identical despite different names*

## Comparing `Nagra-0.0.4/README.md` & `Nagra-0.1.0/README.md`

 * *Files identical despite different names*

## Comparing `Nagra-0.0.4/setup.py` & `Nagra-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "rich",
         "toml",
     ],
     packages=[
         "nagra",
     ],
     extras_require={
-        "test": ["pytest", "pandas"],
+        "test": ["pytest", "pandas", "typeguard"],
     },
     package_data={"nagra": ["template/*/*sql"]},
     entry_points={
         "console_scripts": [
             "nagra = nagra.cli:run",
         ],
     },
```

## Comparing `Nagra-0.0.4/Nagra.egg-info/SOURCES.txt` & `Nagra-0.1.0/Nagra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `Nagra-0.0.4/nagra/transaction.py` & `Nagra-0.1.0/nagra/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 
     _local = threading.local()
     _local.stack = []
 
     def __init__(self, dsn, rollback=False):
         if dsn.startswith("postgresql://"):
             import psycopg
+
             # TODO use Connection Pool
             self.flavor = "postgresql"
             self.connection = psycopg.connect(dsn)
         elif dsn.startswith("sqlite://"):
             self.flavor = "sqlite"
             filename = dsn[9:]
             self.connection = sqlite3.connect(filename)
+            self.connection.execute("PRAGMA foreign_keys = 1")
         elif dsn.startswith("duckdb://"):
             import duckdb
+
             self.flavor = "duckdb"
             filename = dsn[9:]
             self.connection = duckdb.connect(filename)
             self.connection.begin()
         else:
             raise ValueError(f"Invalid dsn string: {dsn}")
         self.cursor = self.connection.cursor()
@@ -79,16 +82,15 @@
 
     @classmethod
     @property
     def current(cls):
         try:
             return cls._local.stack[-1]
         except IndexError:
-            return None
-            # raise NoActiveTransaction()
+            return dummy_transaction
 
 
 def yield_from_cursor(cursor):
     while rows := cursor.fetchmany(1000):
         yield from rows
 
 
@@ -118,20 +120,23 @@
             while True:
                 vals = cursor.fetchone()
                 yield vals
                 if not cursor.nextset():
                     break
 
 
-class DummyTransaction:
+class DummyTransaction(Transaction):
     """
     Postgresql flavored transaction look-alike
     """
+
     flavor = "postgresql"
 
+    def __init__(self):
+        pass
 
     def execute(self, stmt, args=tuple()):
         raise NoActiveTransaction()
 
     def executemany(self, stmt, args=None):
         raise NoActiveTransaction()
```

## Comparing `Nagra-0.0.4/nagra/statement.py` & `Nagra-0.1.0/nagra/statement.py`

 * *Files identical despite different names*

## Comparing `Nagra-0.0.4/nagra/sexpr.py` & `Nagra-0.1.0/nagra/sexpr.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,28 +47,27 @@
     def __init__(self, *items):
         self.value = list_to_dict(*items)
 
     def __repr__(self):
         return f'<KWargs "{self.value}">'
 
 
-
 class Alias:
     """
     Simple wrapper that combine a value and an alias name
     """
 
     def __init__(self, value, name):
         self.value = value
         self.name = name
 
 
 def tokenize(expr):
     lexer = shlex.shlex(expr)
-    lexer.wordchars += ".!=<>:{}-"
+    lexer.wordchars += ".!=<>:{}-|"
     for i in lexer:
         yield Token.from_value(i)
 
 
 def scan(tokens, end_tk=")"):
     res = []
     for tk in tokens:
@@ -97,66 +96,64 @@
         "and": lambda *x: " AND ".join(x),
         "or": lambda *x: " OR ".join(x),
         "not": "NOT {}".format,
         "is": "{} is {}".format,
         "true": lambda: "true",
         "false": lambda: "false",
         # Arithmetic
-        "+" :lambda *xs: (' + '.join("{}" for _ in xs)).format(*xs),
-        "-": lambda *xs: (' - '.join("{}" for _ in xs)).format(*xs),
-        "*": lambda *xs: (' * '.join("{}" for _ in xs)).format(*xs),
-        "/": lambda *xs: (' / '.join("{}" for _ in xs)).format(*xs),
+        "+": lambda *xs: (" + ".join("{}" for _ in xs)).format(*xs),
+        "-": lambda *xs: (" - ".join("{}" for _ in xs)).format(*xs),
+        "*": lambda *xs: (" * ".join("{}" for _ in xs)).format(*xs),
+        "/": lambda *xs: (" / ".join("{}" for _ in xs)).format(*xs),
         # dates and time
         "strftime": "strftime({}, {})".format,
         "extract": "EXTRACT({} FROM {})".format,
         # Strings
         "like": "{} LIKE {}".format,
         "ilike": "{} ILIKE {}".format,
+        "||": lambda *xs: (" || ".join("{}" for _ in xs)).format(*xs),
         # Others
         "in": lambda x, *ys: f"{x} in (%s)" % ", ".join(map(str, ys)),
         "null": lambda: "NULL",
-
     }
 
     aggregates = {
         "min": "min({})".format,
         "max": "max({})".format,
         "sum": "sum({})".format,
         "avg": "avg({})".format,
         "every": "every({})".format,
         "count": lambda x="*": f"count({x})",
         # Sqlite specific
-        "group_concat": lambda *xs: ("group_concat(%s)") % (", ".join("{}" for _ in xs)).format(*xs),
+        "group_concat": lambda *xs: ("group_concat(%s)")
+        % (", ".join("{}" for _ in xs)).format(*xs),
         # Pg specific
         "string_agg": "string_agg({}, {})".format,
         "array_agg": "array_agg({})".format,
         "json_agg": "json_agg({})".format,
         "bool_or": "bool_or({})".format,
         "bool_and": "bool_and({})".format,
         "json_object_agg": "json_object_agg({}, {})".format,
     }
 
     def __init__(self, tokens):
         # Auto-wrap sublist into AST
-        self.tokens = [
-            tk if isinstance(tk, Token) else AST(tk)
-            for tk in tokens
-        ]
+        self.tokens = [tk if isinstance(tk, Token) else AST(tk) for tk in tokens]
 
     @classmethod
     def parse(cls, expr):
         res = tokenize(expr)
         tokens = scan(res)[0]
         if isinstance(tokens, Token):
             tokens = [tokens]
         return AST(tokens)
 
     def chain(self):
         for tk in self.tokens:
-            if isinstance (tk, Token):
+            if isinstance(tk, Token):
                 yield tk
             else:
                 yield from tk.chain()
 
     def _eval(self, env, flavor, top=False):
         head, tail = self.tokens[0], self.tokens[1:]
         args = [tk._eval(env, flavor) for tk in tail]
@@ -176,15 +173,14 @@
         args = [tk._eval_type(env) for tk in tail]
         res = head._eval_type(env, *args)
         return res
 
     def eval_type(self, env):
         return self._eval_type(env)
 
-
     def get_args(self):
         """
         Return token that should be treated as query arguments
         """
         args = list((tk.get_arg() for tk in self.chain()))
         return [a for a in args if a]
 
@@ -207,15 +203,15 @@
         if value in AST.builtins:
             return BuiltinToken(value)
         if value in AST.aggregates:
             return AggToken(value)
         if (value[0], value[-1]) == ("{", "}"):
             return ParamToken(value)
         try:
-            if '.' in value:
+            if "." in value:
                 value = float(value)
                 return FloatToken(value)
             else:
                 value = int(value)
                 return IntToken(value)
         except ValueError:
             pass
@@ -246,18 +242,18 @@
 
 class LitToken(Token):
     "Litteral Token"
 
     def _eval_type(self, env):
         return self._type
 
-
     def _eval(self, env, flavor, *args):
         return self.value
 
+
 class FloatToken(LitToken):
     "Float Token"
     _type = float
 
 
 class IntToken(LitToken):
     "Integer Token"
@@ -299,14 +295,15 @@
         # TODO handle paramtoken here?
         if self.is_relation():
             *head, tail = self.value.split(".")
             ftable, _, _ = env.table.join_on(tuple(head), env=env)
             col_type = ftable.columns[tail]
         else:
             col_type = env.table.columns[self.value]
+
         match col_type:
             # TODO validate type names int Table.__init__
             case "int" | "bigint":
                 return int
             case "varchar":
                 return str
             case "float":
@@ -315,45 +312,60 @@
                 return datetime
             case "bool":
                 return bool
             case "json":
                 return str
             case "date":
                 return date
+            case "uuid":
+                return str
             case _:
                 msg = f"Columns of type {col_type} not supported (for {self.value})"
                 raise NotImplementedError(msg)
 
 
 class OpToken(Token):
     ops = AST.builtins
 
     def _eval(self, env, flavor, *args):
         op = self.ops[self.value]
         return op(*args)
 
+    # FIXME shoud return different _eval_type based on op ?!
+
 
 class BuiltinToken(OpToken):
     num_like = "+-*/"
     bool_like = (
-        "!=", "<", ">", ">=", "<=", "=",
-        "and", "or", "not", "is", "like", "ilike",
+        "!=",
+        "<",
+        ">",
+        ">=",
+        "<=",
+        "=",
+        "and",
+        "or",
+        "not",
+        "is",
+        "like",
+        "ilike",
     )
 
     def _eval_type(self, env, *operands):
         # FIXME, probably too basic
         if self.value in self.num_like:
             if any(op == float for op in operands):
                 return float
             return int
         elif self.value in self.bool_like:
             return bool
         else:
             return str
 
+
 class AggToken(OpToken):
     ops = AST.aggregates
 
     num_like = ["sum", "avg"]
     bool_like = ["every"]
 
     def _eval_type(self, env, *operands):
```

## Comparing `Nagra-0.0.4/nagra/cli.py` & `Nagra-0.1.0/nagra/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 def run():
     # top-level parser
     parser = argparse.ArgumentParser(
         prog="nagra",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
 
-    default_db = os.environ.get('NAGRA_DB')
-    default_schema = os.environ.get('NAGRA_SCHEMA')
+    default_db = os.environ.get("NAGRA_DB")
+    default_schema = os.environ.get("NAGRA_SCHEMA")
     parser.add_argument(
         "--db",
         "-d",
         default=default_db,
         help=f"DB uri, (default: {default_db})",
     )
     parser.add_argument(
@@ -73,35 +73,40 @@
         default=default_schema,
         help=f"DB schema, (default: {default_schema})",
     )
     parser.add_argument(
         "--pivot",
         "-p",
         action="store_true",
-        help='Pivot results (one key-value table per record)',
+        help="Pivot results (one key-value table per record)",
     )
     subparsers = parser.add_subparsers(dest="command")
 
     parser_select = subparsers.add_parser("select")
     parser_select.add_argument("table")
     parser_select.add_argument("columns", nargs="*")
-    parser_select.add_argument("--where", "-W", type=str, action='append', nargs="*")
+    parser_select.add_argument("--where", "-W", type=str, action="append", nargs="*")
     parser_select.add_argument("--limit", "-L", type=int)
-    parser_select.add_argument("--orderby", "-O", type=str,
-                               action='append', nargs="*", help="Order by given columns")
+    parser_select.add_argument(
+        "--orderby",
+        "-O",
+        type=str,
+        action="append",
+        nargs="*",
+        help="Order by given columns",
+    )
     parser_select.set_defaults(func=select)
 
     parser_delete = subparsers.add_parser("delete")
     parser_delete.add_argument("table")
-    parser_delete.add_argument("--where", "-W", type=str, action='append', nargs="*")
+    parser_delete.add_argument("--where", "-W", type=str, action="append", nargs="*")
     parser_delete.set_defaults(func=delete)
 
     parser_schema = subparsers.add_parser("schema")
-    parser_schema.add_argument("--d2", action="store_true",
-                               help="Generate d2 file")
+    parser_schema.add_argument("--d2", action="store_true", help="Generate d2 file")
     parser_schema.add_argument("tables", nargs="*")
     parser_schema.set_defaults(func=schema)
 
     # Parse args
     args = parser.parse_args()
     if not args.command:
         parser.print_help()
```

## Comparing `Nagra-0.0.4/nagra/utils.py` & `Nagra-0.1.0/nagra/utils.py`

 * *Files identical despite different names*

## Comparing `Nagra-0.0.4/nagra/table.py` & `Nagra-0.1.0/nagra/table.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,118 +32,177 @@
 
 )
 ```
 
 
 """
 from functools import lru_cache
-from typing import Dict, List
+from typing import Optional, Union
 
 from nagra.schema import Schema
 from nagra.delete import Delete
 from nagra.select import Select
 from nagra.upsert import Upsert
-from nagra.transaction import Transaction, dummy_transaction
-
-
-_SQLITE_TYPE_MAP = {
-    "varchar": "TEXT",
-    "int": "INTEGER",
-    "float": "FLOAT",
-    "timestamp": "DATETIME",
+from nagra.statement import Statement
+from nagra.transaction import Transaction
+from nagra.exceptions import IncorrectTable
+
+
+_TYPE_MAP = {
+    "postgresql": {
+        "varchar": "VARCHAR",
+        "str": "VARCHAR",
+        "text": "VARCHAR",
+        "int": "INTEGER",
+        "bigint": "BIGINT",
+        "float": "FLOAT",
+        "timestamp": "TIMESTAMP",
+        "date": "DATE",
+        "bool": "BOOL",
+        "uuid": "UUID",
+        "json": "JSON",
+    },
+    "sqlite": {
+        "varchar": "TEXT",
+        "text": "TEXT",
+        "str": "TEXT",
+        "int": "INTEGER",
+        "bigint": "INTEGER",
+        "float": "FLOAT",
+        "timestamp": "DATETIME",
+        "date": "DATE",
+        "bool": "BOOL",
+        "uuid": "TEXT",
+        "json": "JSON",
+    },
 }
 
 
-
 class Table:
     def __init__(
         self,
         name: str,
-        columns: Dict,
-        natural_key: List = None,
-        foreign_keys: Dict = None,
-        not_null: List = None,
-        one2many: Dict = None,
+        columns: dict,
+        natural_key: Optional[list] = None,
+        foreign_keys: Optional[dict] = None,
+        not_null: Optional[list] = None,
+        one2many: Optional[dict] = None,
+        default: Optional[dict] = None,
         schema: Schema = Schema.default,
     ):
         self.name = name
         self.columns = columns
         self.natural_key = natural_key or list(columns)
         self.foreign_keys = foreign_keys or {}
         self.not_null = set(self.natural_key) | set(not_null or [])
         self.one2many = one2many or {}
+        self.default = default or {}
         self.schema = schema
+
+        # Detect malformed fk definitions
+        if len(self.natural_key) == 1:
+            (nk,) = self.natural_key
+            for fk, fk_table in self.foreign_keys.items():
+                if fk != nk or fk_table != name:
+                    continue
+                msg = f"Table '{name}': Foreign key '{fk}' refers to table natural key"
+                raise IncorrectTable(msg)
+
+        # Add table to schema
         self.schema.add(self.name, self)
 
     @classmethod
     def get(self, name, schema=Schema.default):
         """
         Shortcut method to Schema.default().get()
         """
         return schema.get(name)
 
     def select(self, *columns, trn=None):
-        trn = trn or Transaction.current or dummy_transaction
+        trn = trn or Transaction.current
         if not columns:
             columns = self.default_columns()
         slct = Select(self, *columns, trn=trn, env=Env(self))
         return slct
 
     def delete(self, where=None, trn=None):
-        trn = trn or Transaction.current or dummy_transaction
+        trn = trn or Transaction.current
         delete = Delete(self, trn=trn, env=Env(self))
         if where:
-            delete.where(where)
+            return delete.where(where)
         return delete
 
-    def upsert(self, *columns, trn=None, lenient=None):
+    def upsert(
+        self,
+        *columns,
+        trn: Optional[Transaction] = None,
+        lenient: Union[bool, list[str]] = False,
+    ):
         """
         Create an upsert object based on the given columns, if
         lenient is set, foreign keys wont be enforced on the given
         columns even if a value is passed on the subsequent execute or
         executemany. Example:
 
         >>> upsert = Table.get("comment").upsert("body", "blog_post.title", lenient=["blog_post"])
         >>> upsert.execute(("Nice post!", "A post title that will change soon."))
 
         If lenient is set to True all foreign keys will be treated as such.
         """
         if not columns:
             columns = self.default_columns()
-        trn = trn or Transaction.current or dummy_transaction
+        trn = trn or Transaction.current
         return Upsert(self, *columns, trn=trn, lenient=lenient)
 
-    def insert(self, *columns, trn=None, lenient=None):
+    def insert(
+        self,
+        *columns,
+        trn: Optional[Transaction] = None,
+        lenient: Union[bool, list[str]] = False,
+    ):
         """
         Provide an insert-only statement (won't raise error if
         record already exists). See `Table.upsert` for `lenient` role.
         """
-        return self.upsert(*columns, trn=trn, lenient=None).insert_only()
+        trn = trn or Transaction.current
+        return self.upsert(*columns, trn=trn, lenient=lenient).insert_only()
+
+
+    def drop(self, trn: Optional[Transaction] = None):
+        trn = trn or Transaction.current
+        stmt = Statement("drop_table", trn.flavor, name=self.name)
+        trn.execute(stmt())
+
 
-    def default_columns(self, nk_only=False):
+    def default_columns(self, nk_only: bool = False):
+        """
+        Return the list of default column for the current
+        table. Used by `Table.select` and `Table.upsert` when no
+        columns are provided.
+        """
         columns = self.natural_key if nk_only else self.columns
         for column in columns:
             if column not in self.foreign_keys:
                 yield column
                 continue
 
             ftable = self.schema.get(self.foreign_keys[column])
             yield from (f"{column}.{k}" for k in ftable.default_columns(nk_only=True))
 
-    def join(self, env):
+    def join(self, env: "Env"):
         for prefix, alias in env.refs.items():
             # Find alias of previous join in the chain
             *head, tail = prefix
             prev_table = env.refs[tuple(head)] if head else self.name
             # Identify last table & column of the chain
             ftable, alias_col, join_col = self.join_on(prefix, env)
             yield (ftable.name, alias, prev_table, alias_col, join_col)
 
     @lru_cache
-    def join_on(self, path, env):
+    def join_on(self, path: tuple[str, ...], env: "Env"):
         """
         `path` is a tuple containing names of column, each of
         which is a foreign key to another table.
 
         Returns the next table to join and the column to join on.
         """
         if len(path) == 1:
@@ -154,36 +213,36 @@
                 join_col = "id"
                 ftable = self.schema.get(table_name)
             else:
                 # not an alias we implictly join on self, based on the
                 # given column
                 join_col = head
                 alias_col = "id"
-                fname= self.foreign_keys[join_col]
+                fname = self.foreign_keys[join_col]
                 ftable = self.schema.get(fname)
             return ftable, alias_col, join_col
 
         # Recurse to find the previous table in the chain
-        prev_table, *_  = self.join_on(path[:-1], env)
+        prev_table, *_ = self.join_on(path[:-1], env)
         # Resolve last step
         return prev_table.join_on(path[-1:], env)
 
     def ctypes(self, trn):
-        if trn.flavor == "sqlite":
-            return {
-                c: _SQLITE_TYPE_MAP.get(d, d) for c, d in self.columns.items()
-            }
-        return self.columns
+        type_map = _TYPE_MAP[trn.flavor]
+        return {c: type_map[d] for c, d in self.columns.items()}
+
+    def __iter__(self):
+        return iter(self.select())
 
     def __repr__(self):
         return f"<Table {self.name}>"
 
 
 class Env:
-    def __init__(self, table, refs=None):
+    def __init__(self, table: "Table", refs: Optional[dict] = None):
         self.table = table
         self.refs = refs or {}
 
     def add_ref(self, path):
         *head, name, tail = path
         prefix = tuple([*head, name])
         table_alias = self.refs.get(prefix)
```

## Comparing `Nagra-0.0.4/nagra/select.py` & `Nagra-0.1.0/nagra/select.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import re
+from collections.abc import Iterable
 import dataclasses
-from datetime import datetime
-from typing import Optional
+from datetime import datetime, date
+from itertools import islice, repeat, takewhile
+from typing import Optional, Union, TYPE_CHECKING
 
 from nagra import Statement
 from nagra.sexpr import AST, AggToken
 
+if TYPE_CHECKING:
+    from nagra.table import Env
+    from nagra.transaction import Transaction
+    from pandas import DataFrame
 
 RE_VALID_IDENTIFIER = re.compile(r"\W|^(?=\d)")
 
+
 def clean_col(name):
-    return RE_VALID_IDENTIFIER.sub('_', name)
+    return RE_VALID_IDENTIFIER.sub("_", name)
 
 
 class Select:
-    def __init__(self, table, *columns, trn, env):
+    def __init__(self, table, *columns: str, trn: "Transaction", env: "Env"):
         self.table = table
-        self.env = env #Env(table)
+        self.env = env  # Env(table)
         self.where_asts = tuple()
         self._offset = None
         self._limit = None
         self.groupby_ast = tuple()
         self.order_ast = tuple()
         self.order_directions = tuple()
         self.columns = tuple()
@@ -28,54 +35,56 @@
         self.query_columns = tuple()
         self.trn = trn
         self._add_columns(columns)
 
     def _add_columns(self, columns):
         self.columns += columns
         self.columns_ast += tuple(AST.parse(c) for c in columns)
-        self.query_columns += tuple(a.eval(self.env, self.trn.flavor) for a in self.columns_ast)
+        self.query_columns += tuple(
+            a.eval(self.env, self.trn.flavor) for a in self.columns_ast
+        )
 
-    def clone(self, trn=None):
+    def clone(self, trn: Optional["Transaction"] = None):
         """
         Return a copy of select with updated parameters
         """
         trn = trn or self.trn
         cln = Select(self.table, *self.columns, trn=trn, env=self.env.clone())
         cln.where_asts = self.where_asts
         cln.groupby_ast = self.groupby_ast
         cln.order_ast = self.order_ast
-        cln.order_directions  = self.order_directions
+        cln.order_directions = self.order_directions
         return cln
 
-    def where(self, *conditions):
+    def where(self, *conditions: str):
         cln = self.clone()
         cln.where_asts += tuple(AST.parse(cond) for cond in conditions)
         return cln
 
-    def select(self, *columns):
+    def select(self, *columns: str):
         cln = self.clone()
         cln._add_columns(columns)
         return cln
 
     def offset(self, value):
         cln = self.clone()
         cln._offset = value
         return cln
 
     def limit(self, value):
         cln = self.clone()
         cln._limit = value
         return cln
 
-    def groupby(self, *groups):
+    def groupby(self, *groups: str):
         cln = self.clone()
         cln.groupby_ast += tuple(AST.parse(g) for g in groups)
         return cln
 
-    def orderby(self, *orders):
+    def orderby(self, *orders: str | tuple[str, str]):
         expressions = []
         directions = []
         for o in orders:
             if isinstance(o, tuple):
                 expression = o[0]
                 direction = o[1]
             else:
@@ -88,23 +97,21 @@
         directions.append(direction)
 
         cln = self.clone()
         cln.order_ast += tuple(AST.parse(e) for e in expressions)
         cln.order_directions += tuple(directions)
         return cln
 
-    def to_dataclass(self, *aliases):
+    def to_dataclass(self, *aliases: str):
         return dataclasses.make_dataclass(
             self.table.name,
-            fields=[
-                (clean_col(c), d)
-                for c, d in self.dtypes(*aliases)]
+            fields=[(clean_col(c), d) for c, d in self.dtypes(*aliases)],
         )
 
-    def dtypes(self, *aliases, with_optional=True):
+    def dtypes(self, *aliases: str, with_optional: bool = True):
         fields = []
         if aliases:
             assert len(aliases) == len(self.columns)
         else:
             aliases = self.columns
 
         # Construct fields
@@ -138,23 +145,28 @@
             if any(isinstance(tk, AggToken) for tk in a.chain()):
                 continue
             groupby_ast.append(a)
         return groupby_ast
 
     def stm(self):
         # Eval where conditions
-        where_conditions = [ast.eval(self.env, self.trn.flavor) for ast in self.where_asts]
+        where_conditions = [
+            ast.eval(self.env, self.trn.flavor) for ast in self.where_asts
+        ]
         # Eval Groupby
         groupby_ast = self.groupby_ast or self.infer_groupby()
         groupby = [a.eval(self.env, self.trn.flavor) for a in groupby_ast]
         # Eval Oder by
-        orderby = [a.eval(self.env, self.trn.flavor) + f" {d}" for a, d in zip(
-            self.order_ast,
-            self.order_directions,
-        )]
+        orderby = [
+            a.eval(self.env, self.trn.flavor) + f" {d}"
+            for a, d in zip(
+                self.order_ast,
+                self.order_directions,
+            )
+        ]
         # Create joins
         joins = self.table.join(self.env)
 
         stm = Statement(
             "select",
             table=self.table.name,
             columns=self.query_columns,
@@ -163,37 +175,60 @@
             limit=self._limit,
             offset=self._offset,
             groupby=groupby,
             orderby=orderby,
         )
         return stm()
 
-    def to_pandas(self, *args):
+    def to_pandas(self, *args, chunked:int=0) -> Union["DataFrame", Iterable["DataFrame"]]:
         """
-        Convert the rows into columns and return a df with the
-        proper column types, and the given aliases as column names.
+        Execute the query with given args and return a pandas
+        DataFrame. If chunked is bigger than 0, return an iterable
+        yielding dataframes.
         """
-        from pandas import DataFrame, Series
         names, dtypes = zip(*(self.dtypes(with_optional=False)))
-        by_col = zip(*self.execute(*args))
+        cursor = self.execute(*args)
+        if chunked <= 0:
+            return self.create_df(cursor, names, dtypes)
+
+        # Create generator
+        chunkify = (list(islice(cursor, chunked)) for _ in repeat(None))
+        # Return df as long as the generator yield non-empty list
+        return (
+            self.create_df(chunk, names, dtypes)
+            for chunk in takewhile(bool, chunkify)
+        )
+
+    @classmethod
+    def create_df(cls, cursor: Iterable[tuple], names: tuple[str, ...], dtypes: tuple):
+        """
+        Create a Dataframe, whose columns name are `names` and
+        types `dtypes`.
+        """
+        from pandas import DataFrame, Series, to_datetime
+
         df = DataFrame()
+        by_col = zip(*cursor)
         for name, dt, col in zip(names, dtypes, by_col):
             # FIXME Series(col, dtype=dt) fail on json cols!
             srs = Series(col)
-            if dt == int:
-                # Make sure we have no nan for int columns
-                srs = srs.fillna(0)
-            elif dt == datetime:
-                dt = str
-            df[name] = srs.astype(dt)
+            if dt in (datetime, date):
+                srs = to_datetime(srs)
+            else:
+                if dt == int:
+                    # Make sure we have no nan for int columns
+                    srs = srs.fillna(0)
+                srs = srs.astype(dt)
+            df[name] = srs
         return df
 
-    def to_dict(self):
+    def to_dict(self) -> Iterable[dict]:
         columns = [f.name for f in dataclasses.fields(self.to_dataclass())]
-        return [dict(zip(columns, record)) for record in self]
+        for record in self:
+            yield dict(zip(columns, record))
 
     def execute(self, *args):
         return self.trn.execute(self.stm(), args)
 
     def executemany(self, args):
         return self.trn.executemany(self.stm(), args)
```

## Comparing `Nagra-0.0.4/nagra/upsert.py` & `Nagra-0.1.0/nagra/upsert.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,86 @@
 from collections import defaultdict
 from itertools import islice
+from typing import Union, Optional, TYPE_CHECKING
+from collections.abc import Iterable
+
+try:
+    from pandas import DataFrame
+except ImportError:
+    DataFrame = None
 
 from nagra import Statement
-from nagra.sexpr import AST
 from nagra.exceptions import UnresolvedFK, ValidationError
 from nagra.utils import logger
-from nagra.transaction import ExecMany
+from nagra.transaction import ExecMany, Transaction
+
+if TYPE_CHECKING:
+    from nagra.table import Table
+
 
 class Upsert:
-    def __init__(self, table, *columns, trn, lenient=None):
+    def __init__(
+        self,
+        table: "Table",
+        *columns: str,
+        trn: Transaction,
+        lenient: Union[bool, list[str], None] = None,
+        insert_only: bool = False,
+        where: Iterable[str] = [],
+    ):
         self.table = table
         self.columns = list(columns)
-        self.columns_ast = [AST.parse(c) for c in columns]
         self.groups, self.resolve_stm = self.prepare()
-        self._insert_only = False
+        self._insert_only = insert_only
         self.lenient = lenient or []
-        self._where = None
+        self._where = list(where)
         self.trn = trn
 
+    def clone(
+        self,
+        trn: Optional["Transaction"] = None,
+        insert_only: Optional[bool] = None,
+        where: Iterable[str] = [],
+    ):
+        """
+        Return a copy of upsert with updated parameters
+        """
+        trn = trn or self.trn
+        insert_only = self._insert_only if insert_only is None else insert_only
+        where = self._where + list(where)
+        cln = Upsert(
+            self.table,
+            *self.columns,
+            trn=trn,
+            lenient=self.lenient,
+            insert_only=insert_only,
+            where=where,
+        )
+        return cln
+
+    def insert_only(self):
+        return self.clone(insert_only=True)
+
+    def where(self, *conditions: str):
+        return self.clone(where=conditions)
+
     def stm(self):
         conflict_key = ["id"] if "id" in self.groups else self.table.natural_key
         columns = self.groups
         do_update = False if self._insert_only else len(columns) > len(conflict_key)
         stm = Statement(
             "upsert",
             self.trn.flavor,
             table=self.table.name,
             columns=columns,
             conflict_key=conflict_key,
             do_update=do_update,
         )
         return stm()
 
-    def insert_only(self):
-        # TODO clone first
-        self._insert_only = True
-        return self
-
     def prepare(self):
         """
         Organise columns in groups and prepare statement to
         resolve fk based on columns expressions
         """
         groups = defaultdict(list)
         for col in self.columns:
@@ -56,26 +96,20 @@
                 continue
             cond = ["(= %s {})" % c for c in to_select]
             ftable = self.table.schema.get(self.table.foreign_keys[col])
             select = ftable.select("id").where(*cond)
             resolve_stm[col] = select.stm()
         return groups, resolve_stm
 
-    def where(self, *conditions):
-        if self._where is None:
-            self._where = []
-        self._where.extend(conditions)
-        return self
-
     def execute(self, *values):
         ids = self.executemany([values])
         if ids:
             return ids[0]
 
-    def executemany(self, records):
+    def executemany(self, records: Iterable[tuple]):
         # Transform list of records into a dataframe-like dict
         value_df = dict(zip(self.columns, zip(*records)))
         arg_df = {}
         for col, to_select in self.groups.items():
             if to_select:
                 values = list(zip(*(value_df[f"{col}.{s}"] for s in to_select)))
                 arg_df[col] = self._resolve(col, values)
@@ -104,23 +138,23 @@
                         break
 
         # If conditions are present, enforce those
         if self._where:
             self.validate(ids)
         return ids
 
-    def validate(self, ids):
+    def validate(self, ids: list[int]):
         iter_ids = iter(ids)
         while True:
             chunk = list(islice(iter_ids, 1000))
             if not chunk:
                 return
             cond = self._where + ["(in id %s)" % (" {}" * len(chunk))]
             select = self.table.select("(count)").where(*cond)
-            count, = select.execute(*chunk).fetchone()
+            (count,) = select.execute(*chunk).fetchone()
             if count != len(chunk):
                 msg = f"Validation failed! Condition is: {self._where} )"
                 raise ValidationError(msg)
 
     def _resolve(self, col, values):
         # XXX Detect situation where more than on result is found for
         # a given value (we could also enforce that we only resolve
@@ -142,10 +176,10 @@
                     f"Unable to resolve '{vals}' (for foreign key "
                     f"{col} of table {self.table.name})"
                 )
 
     def __call__(self, records):
         return self.executemany(records)
 
-    def from_pandas(self, df:"DataFrame"):
-        rows =  df[self.columns].values
+    def from_pandas(self, df: "DataFrame"):
+        rows = df[self.columns].values
         self.executemany(rows)
```

## Comparing `Nagra-0.0.4/nagra/schema.py` & `Nagra-0.1.0/nagra/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 from collections import defaultdict
 from jinja2 import Template
 from pathlib import Path
 from io import IOBase
+from typing import TYPE_CHECKING
 
 import toml
-
 from nagra.statement import Statement
 from nagra.transaction import Transaction
 
+if TYPE_CHECKING:
+    from nagra.table import Table
+
 
 D2_TPL = """
 {{table.name}}_: "{{table.name}}" {
   shape: sql_table
   {%- for col, dt in table.columns.items() %}
   {{col}}: {{dt}}
   {%- endfor %}
 }
 {%- for col, f_table in table.foreign_keys.items() %}
 {{table.name}}.{{col}} -> {{f_table}}.id : {{col}}
 {%- endfor -%}
 """
 
 
-
 class Schema:
     _default = None
 
     def __init__(self, trn=None, tables=None):
         self.tables = tables or {}
 
     @classmethod
     @property
     def default(cls):
         if not cls._default:
             cls._default = Schema()
         return cls._default
 
     @classmethod
-    def from_toml(self, toml_src):
+    def from_toml(self, toml_src: IOBase | Path | str) -> "Schema":
         schema = Schema()
         schema.load(toml_src)
         return schema
 
-    def load(self, toml_src):
+    def load(self, toml_src: IOBase | Path | str):
         # Late import to avoid import loops
         from nagra.table import Table
 
         # load table definitions
         match toml_src:
             case IOBase():
                 content = toml_src.read()
             case Path():
-                content =  toml_src.open().read()
+                content = toml_src.open().read()
             case _:
                 content = toml_src
         tables = toml.loads(content)
         # Instanciate tables
         for name, info in tables.items():
             Table(name, **info, schema=self)
 
-    def add(self, name, table):
+    def add(self, name: str, table: "Table"):
         if name in self.tables:
             raise RuntimeError(f"Table {name} already in schema!")
         self.tables[name] = table
 
     def reset(self):
         self.tables = {}
 
-    def get(self, name):
+    def get(self, name: str) -> "Table":
         """
         Return the table with name `name`
         """
         return self.tables[name]
 
     def _db_columns(self, trn=None, pg_schema="public"):
         trn = trn or Transaction.current
@@ -85,35 +87,37 @@
         # Find existing tables and columns
         db_columns = self._db_columns(trn)
 
         # Create tables
         for name, table in self.tables.items():
             if name in db_columns:
                 continue
+            ctypes = table.ctypes(trn)
             stmt = Statement(
-                "create_table",
-                trn.flavor,
-                table=name,
+                "create_table", trn.flavor, table=name, id_type=ctypes.get("id")
             )
             yield stmt()
 
         # Add columns
         for table in self.tables.values():
             ctypes = table.ctypes(trn)
             for column in table.columns:
+                if column == "id":
+                    continue
                 if column in db_columns[table.name]:
                     continue
                 stmt = Statement(
                     "add_column",
                     flavor=trn.flavor,
                     table=table.name,
                     column=column,
                     col_def=ctypes[column],
                     not_null=column in table.not_null,
-                    fk_table=table.foreign_keys.get(column)
+                    fk_table=table.foreign_keys.get(column),
+                    default=table.default.get(column),
                 )
                 yield stmt()
 
         # Add index on natural keys
         for name, table in self.tables.items():
             stmt = Statement(
                 "create_unique_index",
@@ -127,18 +131,17 @@
         """
         Create tables, indexes and foreign keys
         """
         trn = trn or Transaction.current
         for stm in self.setup_statements(trn):
             trn.execute(stm)
 
-    def drop(self, trn):
+    def drop(self, trn=None):
         trn = trn or Transaction.current
-        for name in self.tables:
-            stmt = Statement("drop_table", trn.flavor, name=name)
-            trn.execute(stmt())
+        for table in self.tables.values():
+            table.drop(trn)
 
     def generate_d2(self):
         tpl = Template(D2_TPL)
         tables = self.tables.values()
         res = "\n".join(tpl.render(table=t) for t in tables)
         return res
```

## Comparing `Nagra-0.0.4/nagra/template/postgresql/select.sql` & `Nagra-0.1.0/nagra/template/postgresql/select.sql`

 * *Files identical despite different names*

## Comparing `Nagra-0.0.4/nagra/template/sqlite/select.sql` & `Nagra-0.1.0/nagra/template/sqlite/select.sql`

 * *Files identical despite different names*

## Comparing `Nagra-0.0.4/nagra/template/duckdb/select.sql` & `Nagra-0.1.0/nagra/template/duckdb/select.sql`

 * *Files identical despite different names*

