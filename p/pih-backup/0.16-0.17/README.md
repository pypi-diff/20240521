# Comparing `tmp/pih-backup-0.16.tar.gz` & `tmp/pih-backup-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-backup-0.16.tar", last modified: Mon May 13 02:48:41 2024, max compression
+gzip compressed data, was "pih-backup-0.17.tar", last modified: Mon May 20 22:46:44 2024, max compression
```

## Comparing `pih-backup-0.16.tar` & `pih-backup-0.17.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:48:41.564010 pih-backup-0.16/
-drwxrwxrwx   0        0        0        0 2024-05-13 02:48:41.202563 pih-backup-0.16/BackupService/
--rw-rw-rw-   0        0        0      140 2024-02-10 11:56:01.000000 pih-backup-0.16/BackupService/__main__.py
--rw-rw-rw-   0        0        0     5478 2024-04-09 23:53:55.000000 pih-backup-0.16/BackupService/api.py
--rw-rw-rw-   0        0        0     1676 2024-05-03 03:32:44.000000 pih-backup-0.16/BackupService/const.py
--rw-rw-rw-   0        0        0     4929 2024-05-03 03:53:43.000000 pih-backup-0.16/BackupService/service.py
--rw-rw-rw-   0        0        0      269 2024-05-13 02:48:41.532764 pih-backup-0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 02:48:41.501517 pih-backup-0.16/pih_backup.egg-info/
--rw-rw-rw-   0        0        0      269 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 02:48:41.579645 pih-backup-0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:45.078036 pih-backup-0.17/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:44.715474 pih-backup-0.17/BackupService/
+-rw-rw-rw-   0        0        0      140 2024-02-10 11:56:01.000000 pih-backup-0.17/BackupService/__main__.py
+-rw-rw-rw-   0        0        0     5478 2024-04-09 23:53:55.000000 pih-backup-0.17/BackupService/api.py
+-rw-rw-rw-   0        0        0     1676 2024-05-20 22:38:29.000000 pih-backup-0.17/BackupService/const.py
+-rw-rw-rw-   0        0        0     4929 2024-05-03 03:53:43.000000 pih-backup-0.17/BackupService/service.py
+-rw-rw-rw-   0        0        0      269 2024-05-20 22:46:45.045729 pih-backup-0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:45.014486 pih-backup-0.17/pih_backup.egg-info/
+-rw-rw-rw-   0        0        0      269 2024-05-20 22:46:44.000000 pih-backup-0.17/pih_backup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-05-20 22:46:44.000000 pih-backup-0.17/pih_backup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:46:44.000000 pih-backup-0.17/pih_backup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 22:46:44.000000 pih-backup-0.17/pih_backup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 22:46:44.000000 pih-backup-0.17/pih_backup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 22:46:44.000000 pih-backup-0.17/pih_backup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:46:45.093678 pih-backup-0.17/setup.cfg
```

### Comparing `pih-backup-0.16/BackupService/api.py` & `pih-backup-0.17/BackupService/api.py`

 * *Files identical despite different names*

### Comparing `pih-backup-0.16/BackupService/const.py` & `pih-backup-0.17/BackupService/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pih import A
 from pih.collections import RobocopyJobDescription
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Backup"
 
-VERSION: str = "0.16"
+VERSION: str = "0.17"
 
 
 JOB_CONFIG_ALIAS: str = "job_config"
 
 
 class ROBOCOPY:
```

### Comparing `pih-backup-0.16/BackupService/service.py` & `pih-backup-0.17/BackupService/service.py`

 * *Files identical despite different names*

