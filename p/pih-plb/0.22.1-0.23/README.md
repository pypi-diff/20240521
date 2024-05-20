# Comparing `tmp/pih-plb-0.22.1.tar.gz` & `tmp/pih-plb-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.22.1.tar", last modified: Mon May 13 02:35:52 2024, max compression
+gzip compressed data, was "pih-plb-0.23.tar", last modified: Mon May 20 23:06:46 2024, max compression
```

## Comparing `pih-plb-0.22.1.tar` & `pih-plb-0.23.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:35:52.852900 pih-plb-0.22.1/
--rw-rw-rw-   0        0        0      295 2024-05-13 02:35:52.820628 pih-plb-0.22.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 02:35:52.382051 pih-plb-0.22.1/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.22.1/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.22.1/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    45820 2024-05-08 02:28:38.000000 pih-plb-0.22.1/PolibaseService/api.py
--rw-rw-rw-   0        0        0     3696 2024-05-08 03:54:41.000000 pih-plb-0.22.1/PolibaseService/const.py
--rw-rw-rw-   0        0        0    14991 2024-05-08 03:54:34.000000 pih-plb-0.22.1/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:35:52.789395 pih-plb-0.22.1/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      295 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-13 02:35:52.000000 pih-plb-0.22.1/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 02:35:52.852900 pih-plb-0.22.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:06:46.250868 pih-plb-0.23/
+-rw-rw-rw-   0        0        0      293 2024-05-20 23:06:46.219645 pih-plb-0.23/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:06:45.384563 pih-plb-0.23/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.23/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.23/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    45820 2024-05-08 02:28:38.000000 pih-plb-0.23/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     3700 2024-05-20 22:38:50.000000 pih-plb-0.23/PolibaseService/const.py
+-rw-rw-rw-   0        0        0    14991 2024-05-08 03:54:34.000000 pih-plb-0.23/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:06:46.156707 pih-plb-0.23/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-05-20 23:06:44.000000 pih-plb-0.23/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-20 23:06:44.000000 pih-plb-0.23/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:06:44.000000 pih-plb-0.23/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-20 23:06:44.000000 pih-plb-0.23/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 23:06:44.000000 pih-plb-0.23/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-20 23:06:44.000000 pih-plb-0.23/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:06:46.266507 pih-plb-0.23/setup.cfg
```

### Comparing `pih-plb-0.22.1/PolibaseService/api.py` & `pih-plb-0.23/PolibaseService/api.py`

 * *Files identical despite different names*

### Comparing `pih-plb-0.22.1/PolibaseService/const.py` & `pih-plb-0.23/PolibaseService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.tools import j
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Polibase"
 
-VERSION: str = "0.22.1"
+VERSION: str = "0.23"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
@@ -37,15 +37,15 @@
         "set_barcode_for_polibase_person",
         "check_polibase_person_card_registry_folder_name",
         "set_polibase_person_telephone_number",
         "get_polibase_person_operator_by_pin",
         "get_polibase_person_by_email",
         "update_person_change_date",
     ),
-    python_executable_path=CONST.UNKNOWN,
+    python_executable_path=CONST.UNKNOWN_VALUE,
     standalone_name="plb",
     use_standalone=True,
     packages=PACKAGES,
     version=VERSION
 )
 
 TEST: bool = False
```

### Comparing `pih-plb-0.22.1/PolibaseService/service.py` & `pih-plb-0.23/PolibaseService/service.py`

 * *Files identical despite different names*

