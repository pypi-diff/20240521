# Comparing `tmp/pih-ad-0.17.tar.gz` & `tmp/pih-ad-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ad-0.17.tar", last modified: Sat May 18 23:46:56 2024, max compression
+gzip compressed data, was "pih-ad-0.18.tar", last modified: Mon May 20 22:46:39 2024, max compression
```

## Comparing `pih-ad-0.17.tar` & `pih-ad-0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 23:46:56.208669 pih-ad-0.17/
-drwxrwxrwx   0        0        0        0 2024-05-18 23:46:55.752679 pih-ad-0.17/ActiveDirectoryService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-ad-0.17/ActiveDirectoryService/__init__.py
--rw-rw-rw-   0        0        0      157 2024-02-10 00:14:06.000000 pih-ad-0.17/ActiveDirectoryService/__main__.py
--rw-rw-rw-   0        0        0    18268 2024-05-18 23:42:52.000000 pih-ad-0.17/ActiveDirectoryService/api.py
--rw-rw-rw-   0        0        0     1580 2024-05-18 23:43:40.000000 pih-ad-0.17/ActiveDirectoryService/const.py
--rw-rw-rw-   0        0        0    15696 2024-05-18 23:46:38.000000 pih-ad-0.17/ActiveDirectoryService/service.py
--rw-rw-rw-   0        0        0      340 2024-05-18 23:46:56.161835 pih-ad-0.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 23:46:56.083679 pih-ad-0.17/pih_ad.egg-info/
--rw-rw-rw-   0        0        0      340 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 23:46:56.224304 pih-ad-0.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:39.539450 pih-ad-0.18/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:38.982827 pih-ad-0.18/ActiveDirectoryService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-ad-0.18/ActiveDirectoryService/__init__.py
+-rw-rw-rw-   0        0        0      157 2024-02-10 00:14:06.000000 pih-ad-0.18/ActiveDirectoryService/__main__.py
+-rw-rw-rw-   0        0        0    18268 2024-05-18 23:42:52.000000 pih-ad-0.18/ActiveDirectoryService/api.py
+-rw-rw-rw-   0        0        0     1580 2024-05-20 22:32:29.000000 pih-ad-0.18/ActiveDirectoryService/const.py
+-rw-rw-rw-   0        0        0    15696 2024-05-18 23:46:38.000000 pih-ad-0.18/ActiveDirectoryService/service.py
+-rw-rw-rw-   0        0        0      340 2024-05-20 22:46:39.508201 pih-ad-0.18/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:39.461328 pih-ad-0.18/pih_ad.egg-info/
+-rw-rw-rw-   0        0        0      340 2024-05-20 22:46:37.000000 pih-ad-0.18/pih_ad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-20 22:46:38.000000 pih-ad-0.18/pih_ad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:46:38.000000 pih-ad-0.18/pih_ad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-20 22:46:38.000000 pih-ad-0.18/pih_ad.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-05-20 22:46:38.000000 pih-ad-0.18/pih_ad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-20 22:46:38.000000 pih-ad-0.18/pih_ad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:46:39.555081 pih-ad-0.18/setup.cfg
```

### Comparing `pih-ad-0.17/ActiveDirectoryService/api.py` & `pih-ad-0.18/ActiveDirectoryService/api.py`

 * *Files identical despite different names*

### Comparing `pih-ad-0.17/ActiveDirectoryService/const.py` & `pih-ad-0.18/ActiveDirectoryService/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "ActiveDirectory"
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.17"
+VERSION: str = "0.18"
 
 PACKAGES: tuple[str, ...] = ("pyad", "pywin32", "wmi")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Active directory service",
     host=HOST.NAME,
```

### Comparing `pih-ad-0.17/ActiveDirectoryService/service.py` & `pih-ad-0.18/ActiveDirectoryService/service.py`

 * *Files identical despite different names*

