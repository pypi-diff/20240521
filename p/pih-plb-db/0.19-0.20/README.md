# Comparing `tmp/pih-plb_db-0.19.tar.gz` & `tmp/pih-plb_db-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.19.tar", last modified: Mon May 13 02:49:17 2024, max compression
+gzip compressed data, was "pih-plb_db-0.20.tar", last modified: Mon May 20 23:11:58 2024, max compression
```

## Comparing `pih-plb_db-0.19.tar` & `pih-plb_db-0.20.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:49:17.877786 pih-plb_db-0.19/
--rw-rw-rw-   0        0        0      280 2024-05-13 02:49:17.846535 pih-plb_db-0.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 02:49:15.804259 pih-plb_db-0.19/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.19/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.19/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0    10548 2024-04-23 00:05:41.000000 pih-plb_db-0.19/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0     1046 2024-04-22 22:35:45.000000 pih-plb_db-0.19/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.19/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:49:17.815289 pih-plb_db-0.19/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      280 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 02:49:17.893409 pih-plb_db-0.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:11:58.464148 pih-plb_db-0.20/
+-rw-rw-rw-   0        0        0      280 2024-05-20 23:11:58.429873 pih-plb_db-0.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:11:57.721544 pih-plb_db-0.20/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.20/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.20/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0    10898 2024-05-20 22:38:27.000000 pih-plb_db-0.20/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0     1052 2024-05-20 22:38:38.000000 pih-plb_db-0.20/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.20/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:11:58.398626 pih-plb_db-0.20/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:11:58.466147 pih-plb_db-0.20/setup.cfg
```

### Comparing `pih-plb_db-0.19/PolibaseDatabaseService/api.py` & `pih-plb_db-0.20/PolibaseDatabaseService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,29 +156,36 @@
         )
         password_parameter: str = j(
             (
                 "-p",
                 esc(A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD")),
             )
         )
+        compression_level: int | None = A.S.get(
+            A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
+        )
         os.system(
             js(
                 (
                     archiver_program_path,
                     (
                         (
                             js(
                                 (
                                     j(("a -t", ARCHIVE_TYPE)),
-                                    j(
-                                        (
-                                            "-mx",
-                                            A.S.get(
-                                                A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
-                                            ),
+                                    (
+                                        None
+                                        if n(compression_level)
+                                        else j(
+                                            (
+                                                "-mx",
+                                                A.S.get(
+                                                    A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
+                                                ),
+                                            )
                                         )
                                     ),
                                     password_parameter,
                                 )
                             )
                         )
                         if n(archive_creation_parameters)
```

### Comparing `pih-plb_db-0.19/PolibaseDatabaseService/const.py` & `pih-plb_db-0.20/PolibaseDatabaseService/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = A.CT_H.POLIBASE
 
-VERSION: str = "0.19"
+VERSION: str = "0.20"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
     description="Polibase database service",
     commands=("create_polibase_database_backup",),
     version=VERSION,
     use_standalone=True,
     standalone_name="plb_db",
     run_from_system_account=True,
-    python_executable_path=CONST.UNKNOWN,
+    python_executable_path=CONST.UNKNOWN_VALUE,
 )
 
 TEST_NAME: str = "test"
 STUB_DIRECTORY_NAME: str = "stub"
 #
 POLIBASE_NAME: str = "Polibase"
 ARCHIVE_TYPE: str = A.CT_F_E.ARCHIVE
```

### Comparing `pih-plb_db-0.19/PolibaseDatabaseService/service.py` & `pih-plb_db-0.20/PolibaseDatabaseService/service.py`

 * *Files identical despite different names*

