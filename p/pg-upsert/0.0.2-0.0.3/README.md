# Comparing `tmp/pg_upsert-0.0.2.tar.gz` & `tmp/pg_upsert-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_upsert-0.0.2.tar", last modified: Fri Dec 29 00:59:57 2023, max compression
+gzip compressed data, was "pg_upsert-0.0.3.tar", last modified: Mon May 20 22:57:08 2024, max compression
```

## Comparing `pg_upsert-0.0.2.tar` & `pg_upsert-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 00:59:57.129236 pg_upsert-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-29 00:59:17.000000 pg_upsert-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-12-29 00:59:57.129236 pg_upsert-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2023-12-29 00:59:17.000000 pg_upsert-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 00:59:57.125236 pg_upsert-0.0.2/pg_upsert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 00:59:17.000000 pg_upsert-0.0.2/pg_upsert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81253 2023-12-29 00:59:17.000000 pg_upsert-0.0.2/pg_upsert/pg_upsert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 00:59:57.129236 pg_upsert-0.0.2/pg_upsert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-12-29 00:59:57.000000 pg_upsert-0.0.2/pg_upsert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-29 00:59:57.000000 pg_upsert-0.0.2/pg_upsert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 00:59:57.000000 pg_upsert-0.0.2/pg_upsert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-29 00:59:57.000000 pg_upsert-0.0.2/pg_upsert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-29 00:59:17.000000 pg_upsert-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 00:59:57.129236 pg_upsert-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/pg_upsert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/pg_upsert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81474 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/pg_upsert/pg_upsert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/pg_upsert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 22:57:08.000000 pg_upsert-0.0.3/pg_upsert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-20 22:56:43.000000 pg_upsert-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:57:08.514114 pg_upsert-0.0.3/setup.cfg
```

### Comparing `pg_upsert-0.0.2/LICENSE` & `pg_upsert-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_upsert-0.0.2/PKG-INFO` & `pg_upsert-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: pg_upsert
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for upserting data into postgres.
 Author-email: Caleb Grant <grantcaleb22@gmail.com>
 Project-URL: Homepage, https://github.com/geocoug/pg_upsert
 Project-URL: Issues, https://github.com/geocoug/pg_upsert/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psycopg2-binary>=2.9.7
+Requires-Dist: polars>=0.19.3
+Requires-Dist: tabulate>=0.9.0
 
 # pg_upsert
 
 [![ci/cd](https://github.com/geocoug/pg_upsert/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/geocoug/pg_upsert/actions/workflows/ci-cd.yml)
 
-Check data in a staging table or set of staging tables, then interactively update and insert (upsert) rows of a base table or base tables from the staging table(s) of the same name. Initial table checks include not-null, primary key, and foreign key checks. If any of these checks fail, the program will exit with an error message. If all checks pass, the program will display the number of rows to be inserted and updated, and ask for confirmation before proceeding. If the user confirms, the program will perform the upserts and display the number of rows inserted and updated. If the user does not confirm, the program will exit without performing any upserts.
+**pg_upsert** is a Python package that provides a method to *interactively* update and insert (upsert) rows of a base table or base tables from the staging table(s) of the same name. The package is designed to work exclusively with PostgreSQL databases.
+
+The program will perform initial table checks in the form of not-null, primary key, and foreign key checks. If any of these checks fail, the program will exit with an error message. If all checks pass, the program will display the number of rows to be inserted and updated, and ask for confirmation before proceeding. If the user confirms, the program will perform the upserts and display the number of rows inserted and updated. If the user does not confirm, the program will exit without performing any upserts.
 
 ## Installation
 
 1. Create a virtual environment
 
     ```sh
     python -m venv .venv
@@ -74,54 +79,30 @@
   -m METHOD, --method METHOD
                         method to use for upsert
 ```
 
 ### Python
 
 ```py
-import logging
-from pathlib import Path
-
 from pg_upsert import upsert
 
-logfile = Path("pg_upsert.log")
-if logfile.exists():
-    logfile.unlink()
-
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[
-        logging.FileHandler(logfile),
-        logging.StreamHandler(),
-    ],
-)
-
-tables = [
-    "customers",
-    "purchase_orders",
-]
-
-exclude_cols = [
-    "alias",
-]
 
 upsert(
     host="localhost",
     database="dbname",
     user="postgres",
-    # passwd=,  # if not provided, will prompt for password
-    tables=tables,
+    # passwd=,                                  # if not provided, will prompt for password
+    tables=["customers", "purchase_orders"],
     stg_schema="staging",
     base_schema="public",
-    upsert_method="upsert",  # "upsert" | "update" | "insert", default: "upsert"
-    commit=False,  # optional, default=False
-    interactive=False,  # optional, default=False
-    exclude_cols=exclude_cols,  # optional
-    exclude_null_check_columns=exclude_cols,  # optional
+    upsert_method="upsert",                     # "upsert" | "update" | "insert", default: "upsert"
+    commit=False,                               # optional, default=False
+    interactive=True,                           # optional, default=False
+    exclude_cols=["alias"],                     # optional
+    exclude_null_check_columns=["alias"],       # optional
 )
 ```
 
 ### Docker
 
 ```sh
 docker run --rm -v $(pwd):/app ghcr.io/geocoug/pg_upsert [-h] [-q] [-d] [-l LOGFILE] [-e EXCLUDE_COLUMNS] [-n NULL_COLUMNS] [-c] [-i] [-m METHOD] HOST DATABASE USER STAGING_SCHEMA BASE_SCHEMA TABLE [TABLE ...]
```

### Comparing `pg_upsert-0.0.2/README.md` & `pg_upsert-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # pg_upsert
 
 [![ci/cd](https://github.com/geocoug/pg_upsert/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/geocoug/pg_upsert/actions/workflows/ci-cd.yml)
 
-Check data in a staging table or set of staging tables, then interactively update and insert (upsert) rows of a base table or base tables from the staging table(s) of the same name. Initial table checks include not-null, primary key, and foreign key checks. If any of these checks fail, the program will exit with an error message. If all checks pass, the program will display the number of rows to be inserted and updated, and ask for confirmation before proceeding. If the user confirms, the program will perform the upserts and display the number of rows inserted and updated. If the user does not confirm, the program will exit without performing any upserts.
+**pg_upsert** is a Python package that provides a method to *interactively* update and insert (upsert) rows of a base table or base tables from the staging table(s) of the same name. The package is designed to work exclusively with PostgreSQL databases.
+
+The program will perform initial table checks in the form of not-null, primary key, and foreign key checks. If any of these checks fail, the program will exit with an error message. If all checks pass, the program will display the number of rows to be inserted and updated, and ask for confirmation before proceeding. If the user confirms, the program will perform the upserts and display the number of rows inserted and updated. If the user does not confirm, the program will exit without performing any upserts.
 
 ## Installation
 
 1. Create a virtual environment
 
     ```sh
     python -m venv .venv
@@ -56,54 +58,30 @@
   -m METHOD, --method METHOD
                         method to use for upsert
 ```
 
 ### Python
 
 ```py
-import logging
-from pathlib import Path
-
 from pg_upsert import upsert
 
-logfile = Path("pg_upsert.log")
-if logfile.exists():
-    logfile.unlink()
-
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[
-        logging.FileHandler(logfile),
-        logging.StreamHandler(),
-    ],
-)
-
-tables = [
-    "customers",
-    "purchase_orders",
-]
-
-exclude_cols = [
-    "alias",
-]
 
 upsert(
     host="localhost",
     database="dbname",
     user="postgres",
-    # passwd=,  # if not provided, will prompt for password
-    tables=tables,
+    # passwd=,                                  # if not provided, will prompt for password
+    tables=["customers", "purchase_orders"],
     stg_schema="staging",
     base_schema="public",
-    upsert_method="upsert",  # "upsert" | "update" | "insert", default: "upsert"
-    commit=False,  # optional, default=False
-    interactive=False,  # optional, default=False
-    exclude_cols=exclude_cols,  # optional
-    exclude_null_check_columns=exclude_cols,  # optional
+    upsert_method="upsert",                     # "upsert" | "update" | "insert", default: "upsert"
+    commit=False,                               # optional, default=False
+    interactive=True,                           # optional, default=False
+    exclude_cols=["alias"],                     # optional
+    exclude_null_check_columns=["alias"],       # optional
 )
 ```
 
 ### Docker
 
 ```sh
 docker run --rm -v $(pwd):/app ghcr.io/geocoug/pg_upsert [-h] [-q] [-d] [-l LOGFILE] [-e EXCLUDE_COLUMNS] [-n NULL_COLUMNS] [-c] [-i] [-m METHOD] HOST DATABASE USER STAGING_SCHEMA BASE_SCHEMA TABLE [TABLE ...]
```

### Comparing `pg_upsert-0.0.2/pg_upsert/pg_upsert.py` & `pg_upsert-0.0.3/pg_upsert/pg_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,29 +44,27 @@
         database: str,
         user: str,
         **kwargs,
     ) -> None:
         self.host = host
         self.database = database
         self.user = user
-        if "passwd" in kwargs and kwargs["passwd"] is not None:
+        if ("passwd" in kwargs and kwargs["passwd"] is not None) or (
+            "password" in kwargs and kwargs["password"] is not None
+        ):
             self.passwd = kwargs["passwd"]
         else:
             self.passwd = self.get_password()
         self.port = 5432
         self.in_transaction = False
         self.encoding = "UTF8"
         self.conn = None
 
     def __repr__(self: PostgresDB) -> str:
-        return "PostgreSQL(host={!r}, database={!r}, user={!r})".format(
-            self.host,
-            self.database,
-            self.user,
-        )
+        return f"{self.__class__.__name__}(host={self.host}, database={self.database}, user={self.user})"  # noqa: E501
 
     def __del__(self: PostgresDB) -> None:
         """Delete the instance."""
         self.close()
 
     def get_password(self):
         return getpass.getpass(
@@ -145,17 +143,19 @@
 
         def dict_row():
             """Convert a data row to a dictionary."""
             row = curs.fetchone()
             if row:
                 if self.encoding:
                     r = [
-                        c.decode(self.encoding, "backslashreplace")
-                        if isinstance(c, bytes)
-                        else c
+                        (
+                            c.decode(self.encoding, "backslashreplace")
+                            if isinstance(c, bytes)
+                            else c
+                        )
                         for c in row
                     ]
                 else:
                     r = row
                 return dict(zip(headers, r, strict=True))
             return None
 
@@ -537,17 +537,19 @@
     nrows = range(len(rowset))
     ncols = range(len(column_headers))
     hdrwidths = [len(column_headers[j]) for j in ncols]
     if len(rowset) > 0:
         datawidthtbl = [
             [
                 len(
-                    rowset[i][j]
-                    if isinstance(rowset[i][j], str)
-                    else str(rowset[i][j]),
+                    (
+                        rowset[i][j]
+                        if isinstance(rowset[i][j], str)
+                        else str(rowset[i][j])
+                    ),
                 )
                 for i in nrows
             ]
             for j in ncols
         ]
         datawidths = [max(cwidths) for cwidths in datawidthtbl]
     else:
@@ -997,16 +999,18 @@
             and table_name = {table}
             and is_nullable = 'NO'
             and column_default is null and column_name not in ({exclude_null_checks});
         """,
         ).format(
             base_schema=Literal(base_schema),
             table=Literal(table),
-            exclude_null_checks=SQL(",").join(
-                Literal(col) for col in exclude_null_checks.split(",")
+            exclude_null_checks=(
+                SQL(",").join(Literal(col) for col in exclude_null_checks.split(","))
+                if exclude_null_checks
+                else Literal("")
             ),
         ),
     )
 
     # Process all non-nullable columns.
     while True:
         df = db.dataframe(
@@ -2180,15 +2184,15 @@
     timer = datetime.now()
     logging.debug(f"Starting upsert at {timer.strftime('%Y-%m-%d %H:%M:%S')}")
 
     db = PostgresDB(
         host=host,
         database=database,
         user=user,
-        passwd=kwargs["passwd"] if "passwd" in kwargs else None,
+        passwd=kwargs.get("passwd", None),
     )
     logging.debug(f"Connected to {db}")
 
     validate_schemas(base_schema, stg_schema)
     for table in tables:
         validate_table(base_schema, stg_schema, table)
```

### Comparing `pg_upsert-0.0.2/pg_upsert.egg-info/PKG-INFO` & `pg_upsert-0.0.3/pg_upsert.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: pg_upsert
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for upserting data into postgres.
 Author-email: Caleb Grant <grantcaleb22@gmail.com>
 Project-URL: Homepage, https://github.com/geocoug/pg_upsert
 Project-URL: Issues, https://github.com/geocoug/pg_upsert/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psycopg2-binary>=2.9.7
+Requires-Dist: polars>=0.19.3
+Requires-Dist: tabulate>=0.9.0
 
 # pg_upsert
 
 [![ci/cd](https://github.com/geocoug/pg_upsert/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/geocoug/pg_upsert/actions/workflows/ci-cd.yml)
 
-Check data in a staging table or set of staging tables, then interactively update and insert (upsert) rows of a base table or base tables from the staging table(s) of the same name. Initial table checks include not-null, primary key, and foreign key checks. If any of these checks fail, the program will exit with an error message. If all checks pass, the program will display the number of rows to be inserted and updated, and ask for confirmation before proceeding. If the user confirms, the program will perform the upserts and display the number of rows inserted and updated. If the user does not confirm, the program will exit without performing any upserts.
+**pg_upsert** is a Python package that provides a method to *interactively* update and insert (upsert) rows of a base table or base tables from the staging table(s) of the same name. The package is designed to work exclusively with PostgreSQL databases.
+
+The program will perform initial table checks in the form of not-null, primary key, and foreign key checks. If any of these checks fail, the program will exit with an error message. If all checks pass, the program will display the number of rows to be inserted and updated, and ask for confirmation before proceeding. If the user confirms, the program will perform the upserts and display the number of rows inserted and updated. If the user does not confirm, the program will exit without performing any upserts.
 
 ## Installation
 
 1. Create a virtual environment
 
     ```sh
     python -m venv .venv
@@ -74,54 +79,30 @@
   -m METHOD, --method METHOD
                         method to use for upsert
 ```
 
 ### Python
 
 ```py
-import logging
-from pathlib import Path
-
 from pg_upsert import upsert
 
-logfile = Path("pg_upsert.log")
-if logfile.exists():
-    logfile.unlink()
-
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[
-        logging.FileHandler(logfile),
-        logging.StreamHandler(),
-    ],
-)
-
-tables = [
-    "customers",
-    "purchase_orders",
-]
-
-exclude_cols = [
-    "alias",
-]
 
 upsert(
     host="localhost",
     database="dbname",
     user="postgres",
-    # passwd=,  # if not provided, will prompt for password
-    tables=tables,
+    # passwd=,                                  # if not provided, will prompt for password
+    tables=["customers", "purchase_orders"],
     stg_schema="staging",
     base_schema="public",
-    upsert_method="upsert",  # "upsert" | "update" | "insert", default: "upsert"
-    commit=False,  # optional, default=False
-    interactive=False,  # optional, default=False
-    exclude_cols=exclude_cols,  # optional
-    exclude_null_check_columns=exclude_cols,  # optional
+    upsert_method="upsert",                     # "upsert" | "update" | "insert", default: "upsert"
+    commit=False,                               # optional, default=False
+    interactive=True,                           # optional, default=False
+    exclude_cols=["alias"],                     # optional
+    exclude_null_check_columns=["alias"],       # optional
 )
 ```
 
 ### Docker
 
 ```sh
 docker run --rm -v $(pwd):/app ghcr.io/geocoug/pg_upsert [-h] [-q] [-d] [-l LOGFILE] [-e EXCLUDE_COLUMNS] [-n NULL_COLUMNS] [-c] [-i] [-m METHOD] HOST DATABASE USER STAGING_SCHEMA BASE_SCHEMA TABLE [TABLE ...]
```

### Comparing `pg_upsert-0.0.2/pyproject.toml` & `pg_upsert-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 [project]
 name = "pg_upsert"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "Caleb Grant", email = "grantcaleb22@gmail.com" }]
 description = "A Python library for upserting data into postgres."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: Database",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python :: 3",
 ]
+dependencies = [
+    "psycopg2-binary >= 2.9.7",
+    "polars >= 0.19.3",
+    "tabulate >= 0.9.0",
+]
 
 [project.urls]
 Homepage = "https://github.com/geocoug/pg_upsert"
 Issues = "https://github.com/geocoug/pg_upsert/issues"
```

