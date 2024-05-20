# Comparing `tmp/pih-zabbix-0.14.tar.gz` & `tmp/pih-zabbix-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-zabbix-0.14.tar", last modified: Mon May 13 03:55:01 2024, max compression
+gzip compressed data, was "pih-zabbix-0.15.tar", last modified: Mon May 20 23:18:08 2024, max compression
```

## Comparing `pih-zabbix-0.14.tar` & `pih-zabbix-0.15.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 03:55:01.245687 pih-zabbix-0.14/
--rw-rw-rw-   0        0        0      323 2024-05-13 03:55:01.184039 pih-zabbix-0.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 03:55:00.792146 pih-zabbix-0.14/ZabbixService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-zabbix-0.14/ZabbixService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-03-06 10:34:07.000000 pih-zabbix-0.14/ZabbixService/__main__.py
--rw-rw-rw-   0        0        0      722 2024-05-13 03:54:40.000000 pih-zabbix-0.14/ZabbixService/const.py
--rw-rw-rw-   0        0        0     3225 2024-04-09 23:32:53.000000 pih-zabbix-0.14/ZabbixService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-13 03:55:01.121564 pih-zabbix-0.14/pih_zabbix.egg-info/
--rw-rw-rw-   0        0        0      323 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 03:55:01.260687 pih-zabbix-0.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:18:08.197400 pih-zabbix-0.15/
+-rw-rw-rw-   0        0        0      323 2024-05-20 23:18:08.166151 pih-zabbix-0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:18:07.673749 pih-zabbix-0.15/ZabbixService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-zabbix-0.15/ZabbixService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-03-06 10:34:07.000000 pih-zabbix-0.15/ZabbixService/__main__.py
+-rw-rw-rw-   0        0        0      722 2024-05-20 22:40:33.000000 pih-zabbix-0.15/ZabbixService/const.py
+-rw-rw-rw-   0        0        0     3225 2024-04-09 23:32:53.000000 pih-zabbix-0.15/ZabbixService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:18:08.119278 pih-zabbix-0.15/pih_zabbix.egg-info/
+-rw-rw-rw-   0        0        0      323 2024-05-20 23:18:07.000000 pih-zabbix-0.15/pih_zabbix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-20 23:18:07.000000 pih-zabbix-0.15/pih_zabbix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:18:07.000000 pih-zabbix-0.15/pih_zabbix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 23:18:07.000000 pih-zabbix-0.15/pih_zabbix.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2024-05-20 23:18:07.000000 pih-zabbix-0.15/pih_zabbix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 23:18:07.000000 pih-zabbix-0.15/pih_zabbix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:18:08.214048 pih-zabbix-0.15/setup.cfg
```

### Comparing `pih-zabbix-0.14/ZabbixService/const.py` & `pih-zabbix-0.15/ZabbixService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Zabbix"
 
 HOST = A.CT_H.WS255
 
-VERSION: str = "0.14"
+VERSION: str = "0.15"
 
 PACKAGES: tuple[str, ...] = ("pyzabbix", "zabbix_utils")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Zabbix service",
     host=HOST.NAME,
```

### Comparing `pih-zabbix-0.14/ZabbixService/service.py` & `pih-zabbix-0.15/ZabbixService/service.py`

 * *Files identical despite different names*

