# Comparing `tmp/pih-doc-0.14.tar.gz` & `tmp/pih-doc-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-doc-0.14.tar", last modified: Mon May  6 00:47:47 2024, max compression
+gzip compressed data, was "pih-doc-0.15.tar", last modified: Mon May 20 22:49:41 2024, max compression
```

## Comparing `pih-doc-0.14.tar` & `pih-doc-0.15.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 00:47:47.935872 pih-doc-0.14/
-drwxrwxrwx   0        0        0        0 2024-05-06 00:47:47.540748 pih-doc-0.14/DocsService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.14/DocsService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.14/DocsService/__main__.py
--rw-rw-rw-   0        0        0    41563 2024-05-06 00:47:28.000000 pih-doc-0.14/DocsService/api.py
--rw-rw-rw-   0        0        0     1634 2024-05-06 00:45:54.000000 pih-doc-0.14/DocsService/const.py
--rw-rw-rw-   0        0        0     5242 2024-04-10 12:59:25.000000 pih-doc-0.14/DocsService/service.py
--rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.14/DocsService/tools.py
--rw-rw-rw-   0        0        0      595 2024-05-06 00:47:47.904767 pih-doc-0.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 00:47:47.873311 pih-doc-0.14/pih_doc.egg-info/
--rw-rw-rw-   0        0        0      595 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 00:47:47.935872 pih-doc-0.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:49:41.032484 pih-doc-0.15/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:49:40.334139 pih-doc-0.15/DocsService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.15/DocsService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.15/DocsService/__main__.py
+-rw-rw-rw-   0        0        0    41563 2024-05-06 00:47:28.000000 pih-doc-0.15/DocsService/api.py
+-rw-rw-rw-   0        0        0     1634 2024-05-20 22:38:29.000000 pih-doc-0.15/DocsService/const.py
+-rw-rw-rw-   0        0        0     5241 2024-05-20 00:00:21.000000 pih-doc-0.15/DocsService/service.py
+-rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.15/DocsService/tools.py
+-rw-rw-rw-   0        0        0      595 2024-05-20 22:49:41.001235 pih-doc-0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:49:40.966504 pih-doc-0.15/pih_doc.egg-info/
+-rw-rw-rw-   0        0        0      595 2024-05-20 22:49:39.000000 pih-doc-0.15/pih_doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-20 22:49:39.000000 pih-doc-0.15/pih_doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:49:39.000000 pih-doc-0.15/pih_doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-20 22:49:39.000000 pih-doc-0.15/pih_doc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2024-05-20 22:49:39.000000 pih-doc-0.15/pih_doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 22:49:39.000000 pih-doc-0.15/pih_doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:49:41.391857 pih-doc-0.15/setup.cfg
```

### Comparing `pih-doc-0.14/DocsService/api.py` & `pih-doc-0.15/DocsService/api.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.14/DocsService/const.py` & `pih-doc-0.15/DocsService/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     QUANTITY_COLUMN_NAME: str = "фактическое наличие"
     NAME_MAX_LENTH: int = 120
     QUANTITY_NOT_SET: str = "-"
 
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.14"
+VERSION: str = "0.15"
 
 PACKAGES: tuple[str, ...] = (
     "xlsxwriter",
     "xlrd",
     "xlutils",
     "openpyxl",
     "python-barcode",
```

### Comparing `pih-doc-0.14/DocsService/service.py` & `pih-doc-0.15/DocsService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pih import A
 from typing import Any
 from DocsService.const import SD
 
 SC = A.CT_SC
 
-ISOLATED: bool = False
+ISOLATED: bool = True
 
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
         from datetime import datetime
         import grpc
```

### Comparing `pih-doc-0.14/DocsService/tools.py` & `pih-doc-0.15/DocsService/tools.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.14/PKG-INFO` & `pih-doc-0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.14
+Version: 0.15
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

### Comparing `pih-doc-0.14/pih_doc.egg-info/PKG-INFO` & `pih-doc-0.15/pih_doc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.14
+Version: 0.15
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

