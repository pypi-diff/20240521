# Comparing `tmp/pih-plb_auto-0.13.tar.gz` & `tmp/pih-plb_auto-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_auto-0.13.tar", last modified: Mon Apr 15 00:54:28 2024, max compression
+gzip compressed data, was "pih-plb_auto-0.14.tar", last modified: Mon May 20 23:10:39 2024, max compression
```

## Comparing `pih-plb_auto-0.13.tar` & `pih-plb_auto-0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 00:54:28.600739 pih-plb_auto-0.13/
--rw-rw-rw-   0        0        0      284 2024-04-15 00:54:28.568457 pih-plb_auto-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 00:54:27.800594 pih-plb_auto-0.13/PolibaseAutomationService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb_auto-0.13/PolibaseAutomationService/__init__.py
--rw-rw-rw-   0        0        0      160 2024-04-15 00:41:11.000000 pih-plb_auto-0.13/PolibaseAutomationService/__main__.py
--rw-rw-rw-   0        0        0      518 2024-04-15 00:44:38.000000 pih-plb_auto-0.13/PolibaseAutomationService/const.py
--rw-rw-rw-   0        0        0    13597 2024-04-15 00:41:11.000000 pih-plb_auto-0.13/PolibaseAutomationService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 00:54:28.505680 pih-plb_auto-0.13/pih_plb_auto.egg-info/
--rw-rw-rw-   0        0        0      284 2024-04-15 00:54:27.000000 pih-plb_auto-0.13/pih_plb_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2024-04-15 00:54:27.000000 pih-plb_auto-0.13/pih_plb_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 00:54:27.000000 pih-plb_auto-0.13/pih_plb_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-15 00:54:27.000000 pih-plb_auto-0.13/pih_plb_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-15 00:54:27.000000 pih-plb_auto-0.13/pih_plb_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-15 00:54:27.000000 pih-plb_auto-0.13/pih_plb_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 00:54:28.616404 pih-plb_auto-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:10:40.022584 pih-plb_auto-0.14/
+-rw-rw-rw-   0        0        0      284 2024-05-20 23:10:39.991370 pih-plb_auto-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:10:39.567373 pih-plb_auto-0.14/PolibaseAutomationService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb_auto-0.14/PolibaseAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      160 2024-04-15 00:41:11.000000 pih-plb_auto-0.14/PolibaseAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      524 2024-05-20 22:38:29.000000 pih-plb_auto-0.14/PolibaseAutomationService/const.py
+-rw-rw-rw-   0        0        0    13597 2024-04-15 00:41:11.000000 pih-plb_auto-0.14/PolibaseAutomationService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:10:39.960085 pih-plb_auto-0.14/pih_plb_auto.egg-info/
+-rw-rw-rw-   0        0        0      284 2024-05-20 23:10:39.000000 pih-plb_auto-0.14/pih_plb_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-05-20 23:10:39.000000 pih-plb_auto-0.14/pih_plb_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:10:39.000000 pih-plb_auto-0.14/pih_plb_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-05-20 23:10:39.000000 pih-plb_auto-0.14/pih_plb_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 23:10:39.000000 pih-plb_auto-0.14/pih_plb_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-20 23:10:39.000000 pih-plb_auto-0.14/pih_plb_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:10:40.022584 pih-plb_auto-0.14/setup.cfg
```

### Comparing `pih-plb_auto-0.13/PolibaseAutomationService/const.py` & `pih-plb_auto-0.14/PolibaseAutomationService/const.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from pih.collections.service import ServiceDescription
 from pih.consts.hosts import Hosts
 from pih.consts import CONST
 
 NAME: str = "PolibaseAutomation"
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 HOST = Hosts.POLIBASE
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Polibase automation service",
     host=HOST.NAME,
-    python_executable_path=CONST.UNKNOWN,
+    python_executable_path=CONST.UNKNOWN_VALUE,
     run_from_system_account=True,
     standalone_name="plb_auto",
     use_standalone=True,
     version=VERSION,
 )
```

### Comparing `pih-plb_auto-0.13/PolibaseAutomationService/service.py` & `pih-plb_auto-0.14/PolibaseAutomationService/service.py`

 * *Files identical despite different names*

