# Comparing `tmp/pih-file-0.11.tar.gz` & `tmp/pih-file-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-file-0.11.tar", last modified: Wed Apr 10 01:41:32 2024, max compression
+gzip compressed data, was "pih-file-0.12.tar", last modified: Mon May 20 22:51:24 2024, max compression
```

## Comparing `pih-file-0.11.tar` & `pih-file-0.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:41:32.907974 pih-file-0.11/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:41:32.437116 pih-file-0.11/FileWatchdogService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-file-0.11/FileWatchdogService/__init__.py
--rw-rw-rw-   0        0        0      156 2024-02-15 01:20:33.000000 pih-file-0.11/FileWatchdogService/__main__.py
--rw-rw-rw-   0        0        0      510 2024-04-10 00:01:38.000000 pih-file-0.11/FileWatchdogService/const.py
--rw-rw-rw-   0        0        0     3847 2024-03-14 22:53:57.000000 pih-file-0.11/FileWatchdogService/service.py
--rw-rw-rw-   0        0        0      298 2024-04-10 01:41:32.875697 pih-file-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:41:32.844456 pih-file-0.11/pih_file.egg-info/
--rw-rw-rw-   0        0        0      298 2024-04-10 01:41:31.000000 pih-file-0.11/pih_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:41:32.923620 pih-file-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:51:24.124245 pih-file-0.12/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:51:23.690633 pih-file-0.12/FileWatchdogService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-file-0.12/FileWatchdogService/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-02-15 01:20:33.000000 pih-file-0.12/FileWatchdogService/__main__.py
+-rw-rw-rw-   0        0        0      510 2024-05-20 22:38:29.000000 pih-file-0.12/FileWatchdogService/const.py
+-rw-rw-rw-   0        0        0     3847 2024-03-14 22:53:57.000000 pih-file-0.12/FileWatchdogService/service.py
+-rw-rw-rw-   0        0        0      298 2024-05-20 22:51:24.090892 pih-file-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:51:24.058622 pih-file-0.12/pih_file.egg-info/
+-rw-rw-rw-   0        0        0      298 2024-05-20 22:51:23.000000 pih-file-0.12/pih_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-20 22:51:23.000000 pih-file-0.12/pih_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:51:23.000000 pih-file-0.12/pih_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-20 22:51:23.000000 pih-file-0.12/pih_file.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 22:51:23.000000 pih-file-0.12/pih_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-20 22:51:23.000000 pih-file-0.12/pih_file.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:51:24.155519 pih-file-0.12/setup.cfg
```

### Comparing `pih-file-0.11/FileWatchdogService/service.py` & `pih-file-0.12/FileWatchdogService/service.py`

 * *Files identical despite different names*

