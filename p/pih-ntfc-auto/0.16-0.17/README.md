# Comparing `tmp/pih-ntfc_auto-0.16.tar.gz` & `tmp/pih-ntfc_auto-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ntfc_auto-0.16.tar", last modified: Mon May 13 01:54:05 2024, max compression
+gzip compressed data, was "pih-ntfc_auto-0.17.tar", last modified: Mon May 20 23:04:44 2024, max compression
```

## Comparing `pih-ntfc_auto-0.16.tar` & `pih-ntfc_auto-0.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 01:54:06.048929 pih-ntfc_auto-0.16/
-drwxrwxrwx   0        0        0        0 2024-05-13 01:54:05.515769 pih-ntfc_auto-0.16/NotificationAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-ntfc_auto-0.16/NotificationAutomationService/__init__.py
--rw-rw-rw-   0        0        0      164 2024-04-15 23:57:16.000000 pih-ntfc_auto-0.16/NotificationAutomationService/__main__.py
--rw-rw-rw-   0        0        0     1615 2024-04-15 23:57:45.000000 pih-ntfc_auto-0.16/NotificationAutomationService/api.py
--rw-rw-rw-   0        0        0      424 2024-05-13 01:49:33.000000 pih-ntfc_auto-0.16/NotificationAutomationService/const.py
--rw-rw-rw-   0        0        0    20480 2024-04-26 00:53:58.000000 pih-ntfc_auto-0.16/NotificationAutomationService/service.py
--rw-rw-rw-   0        0        0      289 2024-05-13 01:54:06.017683 pih-ntfc_auto-0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 01:54:05.970808 pih-ntfc_auto-0.16/pih_ntfc_auto.egg-info/
--rw-rw-rw-   0        0        0      289 2024-05-13 01:54:04.000000 pih-ntfc_auto-0.16/pih_ntfc_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-05-13 01:54:05.000000 pih-ntfc_auto-0.16/pih_ntfc_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 01:54:04.000000 pih-ntfc_auto-0.16/pih_ntfc_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-13 01:54:04.000000 pih-ntfc_auto-0.16/pih_ntfc_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-13 01:54:04.000000 pih-ntfc_auto-0.16/pih_ntfc_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-05-13 01:54:04.000000 pih-ntfc_auto-0.16/pih_ntfc_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 01:54:06.077580 pih-ntfc_auto-0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:04:44.899460 pih-ntfc_auto-0.17/
+drwxrwxrwx   0        0        0        0 2024-05-20 23:04:44.442188 pih-ntfc_auto-0.17/NotificationAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-ntfc_auto-0.17/NotificationAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      164 2024-04-15 23:57:16.000000 pih-ntfc_auto-0.17/NotificationAutomationService/__main__.py
+-rw-rw-rw-   0        0        0     1615 2024-04-15 23:57:45.000000 pih-ntfc_auto-0.17/NotificationAutomationService/api.py
+-rw-rw-rw-   0        0        0      424 2024-05-20 22:38:29.000000 pih-ntfc_auto-0.17/NotificationAutomationService/const.py
+-rw-rw-rw-   0        0        0    20480 2024-04-26 00:53:58.000000 pih-ntfc_auto-0.17/NotificationAutomationService/service.py
+-rw-rw-rw-   0        0        0      289 2024-05-20 23:04:44.883834 pih-ntfc_auto-0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:04:44.852587 pih-ntfc_auto-0.17/pih_ntfc_auto.egg-info/
+-rw-rw-rw-   0        0        0      289 2024-05-20 23:04:43.000000 pih-ntfc_auto-0.17/pih_ntfc_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-05-20 23:04:44.000000 pih-ntfc_auto-0.17/pih_ntfc_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:04:43.000000 pih-ntfc_auto-0.17/pih_ntfc_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-20 23:04:43.000000 pih-ntfc_auto-0.17/pih_ntfc_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 23:04:43.000000 pih-ntfc_auto-0.17/pih_ntfc_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-05-20 23:04:43.000000 pih-ntfc_auto-0.17/pih_ntfc_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:04:44.930708 pih-ntfc_auto-0.17/setup.cfg
```

### Comparing `pih-ntfc_auto-0.16/NotificationAutomationService/api.py` & `pih-ntfc_auto-0.17/NotificationAutomationService/api.py`

 * *Files identical despite different names*

### Comparing `pih-ntfc_auto-0.16/NotificationAutomationService/service.py` & `pih-ntfc_auto-0.17/NotificationAutomationService/service.py`

 * *Files identical despite different names*

