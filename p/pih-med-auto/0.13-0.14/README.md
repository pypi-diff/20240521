# Comparing `tmp/pih-med_auto-0.13.tar.gz` & `tmp/pih-med_auto-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-med_auto-0.13.tar", last modified: Wed Apr 10 01:46:38 2024, max compression
+gzip compressed data, was "pih-med_auto-0.14.tar", last modified: Mon May 20 22:59:59 2024, max compression
```

## Comparing `pih-med_auto-0.13.tar` & `pih-med_auto-0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:46:38.825724 pih-med_auto-0.13/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:46:37.436566 pih-med_auto-0.13/MedicalAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-med_auto-0.13/MedicalAutomationService/__init__.py
--rw-rw-rw-   0        0        0      161 2024-02-15 02:15:00.000000 pih-med_auto-0.13/MedicalAutomationService/__main__.py
--rw-rw-rw-   0        0        0      586 2024-04-10 00:33:12.000000 pih-med_auto-0.13/MedicalAutomationService/const.py
--rw-rw-rw-   0        0        0    20992 2024-04-10 00:31:50.000000 pih-med_auto-0.13/MedicalAutomationService/service.py
--rw-rw-rw-   0        0        0      307 2024-04-10 01:46:38.763241 pih-med_auto-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:46:38.669443 pih-med_auto-0.13/pih_med_auto.egg-info/
--rw-rw-rw-   0        0        0      307 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:46:38.825724 pih-med_auto-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:59:59.347239 pih-med_auto-0.14/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:59:58.874313 pih-med_auto-0.14/MedicalAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-med_auto-0.14/MedicalAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-02-15 02:15:00.000000 pih-med_auto-0.14/MedicalAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      586 2024-05-20 22:38:29.000000 pih-med_auto-0.14/MedicalAutomationService/const.py
+-rw-rw-rw-   0        0        0    20992 2024-04-10 00:31:50.000000 pih-med_auto-0.14/MedicalAutomationService/service.py
+-rw-rw-rw-   0        0        0      307 2024-05-20 22:59:59.315990 pih-med_auto-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:59:59.269117 pih-med_auto-0.14/pih_med_auto.egg-info/
+-rw-rw-rw-   0        0        0      307 2024-05-20 22:59:58.000000 pih-med_auto-0.14/pih_med_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-05-20 22:59:58.000000 pih-med_auto-0.14/pih_med_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:59:58.000000 pih-med_auto-0.14/pih_med_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-20 22:59:58.000000 pih-med_auto-0.14/pih_med_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 22:59:58.000000 pih-med_auto-0.14/pih_med_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-20 22:59:58.000000 pih-med_auto-0.14/pih_med_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:59:59.362862 pih-med_auto-0.14/setup.cfg
```

### Comparing `pih-med_auto-0.13/MedicalAutomationService/const.py` & `pih-med_auto-0.14/MedicalAutomationService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.collections.service import ServiceDescription
 
 NAME: str = "MedicalAutomation"
 
 HOST = A.CT_H.BACKUP_WORKER
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 PACKAGES: tuple[str, ...] = (
     A.PTH_FCD_DIST.NAME(A.CT_SR.MOBILE_HELPER.standalone_name),  # type: ignore
 )
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-med_auto-0.13/MedicalAutomationService/service.py` & `pih-med_auto-0.14/MedicalAutomationService/service.py`

 * *Files identical despite different names*

