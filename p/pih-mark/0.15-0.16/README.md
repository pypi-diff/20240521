# Comparing `tmp/pih-mark-0.15.tar.gz` & `tmp/pih-mark-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mark-0.15.tar", last modified: Thu May 16 00:21:19 2024, max compression
+gzip compressed data, was "pih-mark-0.16.tar", last modified: Mon May 20 22:59:28 2024, max compression
```

## Comparing `pih-mark-0.15.tar` & `pih-mark-0.16.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 00:21:19.255083 pih-mark-0.15/
-drwxrwxrwx   0        0        0        0 2024-05-16 00:21:18.702099 pih-mark-0.15/MarkService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mark-0.15/MarkService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-13 23:54:48.000000 pih-mark-0.15/MarkService/__main__.py
--rw-rw-rw-   0        0        0    38590 2024-05-16 00:20:37.000000 pih-mark-0.15/MarkService/api.py
--rw-rw-rw-   0        0        0     1626 2024-02-09 14:42:12.000000 pih-mark-0.15/MarkService/api_test.py
--rw-rw-rw-   0        0        0     1815 2024-05-16 00:20:47.000000 pih-mark-0.15/MarkService/const.py
--rw-rw-rw-   0        0        0     6242 2024-05-15 22:57:47.000000 pih-mark-0.15/MarkService/service.py
--rw-rw-rw-   0        0        0      315 2024-05-16 00:21:19.176962 pih-mark-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 00:21:19.129042 pih-mark-0.15/pih_mark.egg-info/
--rw-rw-rw-   0        0        0      315 2024-05-16 00:21:17.000000 pih-mark-0.15/pih_mark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2024-05-16 00:21:17.000000 pih-mark-0.15/pih_mark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 00:21:17.000000 pih-mark-0.15/pih_mark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-16 00:21:17.000000 pih-mark-0.15/pih_mark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-05-16 00:21:17.000000 pih-mark-0.15/pih_mark.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 00:21:17.000000 pih-mark-0.15/pih_mark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 00:21:19.270715 pih-mark-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:59:28.641987 pih-mark-0.16/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:59:28.128881 pih-mark-0.16/MarkService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mark-0.16/MarkService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-13 23:54:48.000000 pih-mark-0.16/MarkService/__main__.py
+-rw-rw-rw-   0        0        0    38590 2024-05-16 00:20:37.000000 pih-mark-0.16/MarkService/api.py
+-rw-rw-rw-   0        0        0     1626 2024-02-09 14:42:12.000000 pih-mark-0.16/MarkService/api_test.py
+-rw-rw-rw-   0        0        0     1815 2024-05-20 22:38:29.000000 pih-mark-0.16/MarkService/const.py
+-rw-rw-rw-   0        0        0     6242 2024-05-20 00:17:10.000000 pih-mark-0.16/MarkService/service.py
+-rw-rw-rw-   0        0        0      315 2024-05-20 22:59:28.610740 pih-mark-0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:59:28.563859 pih-mark-0.16/pih_mark.egg-info/
+-rw-rw-rw-   0        0        0      315 2024-05-20 22:59:27.000000 pih-mark-0.16/pih_mark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2024-05-20 22:59:27.000000 pih-mark-0.16/pih_mark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:59:27.000000 pih-mark-0.16/pih_mark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-20 22:59:27.000000 pih-mark-0.16/pih_mark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-05-20 22:59:27.000000 pih-mark-0.16/pih_mark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 22:59:27.000000 pih-mark-0.16/pih_mark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:59:28.657614 pih-mark-0.16/setup.cfg
```

### Comparing `pih-mark-0.15/MarkService/api.py` & `pih-mark-0.16/MarkService/api.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.15/MarkService/api_test.py` & `pih-mark-0.16/MarkService/api_test.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.15/MarkService/const.py` & `pih-mark-0.16/MarkService/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Mark"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.15"
+VERSION: str = "0.16"
 
 PACKAGES: tuple[str, ...] = ("pymssql", "schedule")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Orion service",
     host=HOST.NAME,
```

### Comparing `pih-mark-0.15/MarkService/service.py` & `pih-mark-0.16/MarkService/service.py`

 * *Files identical despite different names*

