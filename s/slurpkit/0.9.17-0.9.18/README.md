# Comparing `tmp/slurpkit-0.9.17.tar.gz` & `tmp/slurpkit-0.9.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpkit-0.9.17.tar", last modified: Tue May 21 08:20:48 2024, max compression
+gzip compressed data, was "slurpkit-0.9.18.tar", last modified: Tue May 21 08:37:35 2024, max compression
```

## Comparing `slurpkit-0.9.17.tar` & `slurpkit-0.9.18.tar`

### file list

```diff
@@ -1,21 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:20:48.523866 slurpkit-0.9.17/
--rw-r--r--   0 root         (0) root         (0)      235 2024-05-21 08:20:48.523866 slurpkit-0.9.17/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1708 2024-05-21 08:19:22.000000 slurpkit-0.9.17/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 08:20:48.523866 slurpkit-0.9.17/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:20:48.523866 slurpkit-0.9.17/slurpkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      235 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:20:48.523866 slurpkit-0.9.17/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2160 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_0_run.py
--rw-rw-rw-   0 root         (0) root         (0)     3378 2024-05-16 12:22:52.000000 slurpkit-0.9.17/tests/test_1_device.py
--rw-rw-rw-   0 root         (0) root         (0)     2021 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_2_planning.py
--rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_3_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2927 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_4_scanner.py
--rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-16 12:22:52.000000 slurpkit-0.9.17/tests/test_5_scraper.py
--rw-rw-rw-   0 root         (0) root         (0)     2292 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_6_vault.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_7_user.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_8_templates.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2024-05-16 12:22:52.000000 slurpkit-0.9.17/tests/test_9_clean.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:37:35.150237 slurpkit-0.9.18/
+-rw-r--r--   0 root         (0) root         (0)     1984 2024-05-21 08:37:35.142237 slurpkit-0.9.18/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 08:37:35.150237 slurpkit-0.9.18/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-21 08:36:57.000000 slurpkit-0.9.18/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:37:35.130237 slurpkit-0.9.18/slurpit/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:37:35.134237 slurpkit-0.9.18/slurpit/apis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 08:37:18.000000 slurpkit-0.9.18/slurpit/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7053 2024-05-14 19:35:54.000000 slurpkit-0.9.18/slurpit/apis/baseapi.py
+-rw-rw-rw-   0 root         (0) root         (0)    11256 2024-05-20 10:32:39.000000 slurpkit-0.9.18/slurpit/apis/deviceapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2024-05-21 08:05:20.000000 slurpkit-0.9.18/slurpit/apis/planningapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2024-05-20 12:11:15.000000 slurpkit-0.9.18/slurpit/apis/platformapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2024-05-20 10:32:39.000000 slurpkit-0.9.18/slurpit/apis/scannerapi.py
+-rw-rw-rw-   0 root         (0) root         (0)    14816 2024-05-20 12:11:15.000000 slurpkit-0.9.18/slurpit/apis/scraperapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8150 2024-05-21 08:05:20.000000 slurpkit-0.9.18/slurpit/apis/templateapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4839 2024-05-20 10:32:39.000000 slurpkit-0.9.18/slurpit/apis/userapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4431 2024-05-20 10:32:39.000000 slurpkit-0.9.18/slurpit/apis/vaultapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:37:35.138237 slurpkit-0.9.18/slurpit/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 08:37:18.000000 slurpkit-0.9.18/slurpit/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/models/basemodel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/models/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/models/planning.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/models/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/models/scanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1932 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/models/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2024-05-12 14:26:16.000000 slurpkit-0.9.18/slurpit/models/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:37:35.142237 slurpkit-0.9.18/slurpkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1984 2024-05-21 08:37:35.000000 slurpkit-0.9.18/slurpkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      698 2024-05-21 08:37:35.000000 slurpkit-0.9.18/slurpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 08:37:35.000000 slurpkit-0.9.18/slurpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-21 08:37:35.000000 slurpkit-0.9.18/slurpkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-21 08:37:35.000000 slurpkit-0.9.18/slurpkit.egg-info/top_level.txt
```

### Comparing `slurpkit-0.9.17/README.md` & `slurpkit-0.9.18/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: slurpkit
+Version: 0.9.18
+Summary: A robust Python SDK for slurpit
+Author: PkServices
+Author-email: info@slurpit.io
+Keywords: sdk slurpit slurpkit
+Description-Content-Type: text/markdown
+Requires-Dist: pandas==2.2.2
+Requires-Dist: requests==2.31.0
+
 # Slurpit SDK
 
 The Slurpit SDK is a Python package for interacting with the Slurpit API, enabling developers to easily manage devices and planning resources. It is designed for simplicity and flexibility, offering methods for listing devices, retrieving planning data, and exporting information to CSV format.
 
 ## Installation
 
 You can install the Slurpit SDK using pip with the following command:
```

