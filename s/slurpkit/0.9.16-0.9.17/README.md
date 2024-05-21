# Comparing `tmp/slurpkit-0.9.16.tar.gz` & `tmp/slurpkit-0.9.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpkit-0.9.16.tar", last modified: Tue May 21 08:12:38 2024, max compression
+gzip compressed data, was "slurpkit-0.9.17.tar", last modified: Tue May 21 08:20:48 2024, max compression
```

## Comparing `slurpkit-0.9.16.tar` & `slurpkit-0.9.17.tar`

### file list

```diff
@@ -1,10 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 08:12:38.076767 slurpkit-0.9.16/
--rw-rw-rw-   0        0        0      181 2024-05-21 08:12:38.076767 slurpkit-0.9.16/PKG-INFO
--rw-rw-rw-   0        0        0     1911 2024-05-21 07:08:42.000000 slurpkit-0.9.16/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 08:12:38.077766 slurpkit-0.9.16/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-21 08:12:38.075746 slurpkit-0.9.16/slurpkit.egg-info/
--rw-rw-rw-   0        0        0      181 2024-05-21 08:12:37.000000 slurpkit-0.9.16/slurpkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2024-05-21 08:12:37.000000 slurpkit-0.9.16/slurpkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 08:12:37.000000 slurpkit-0.9.16/slurpkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-21 08:12:37.000000 slurpkit-0.9.16/slurpkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 08:12:37.000000 slurpkit-0.9.16/slurpkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:20:48.523866 slurpkit-0.9.17/
+-rw-r--r--   0 root         (0) root         (0)      235 2024-05-21 08:20:48.523866 slurpkit-0.9.17/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2024-05-21 08:19:22.000000 slurpkit-0.9.17/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 08:20:48.523866 slurpkit-0.9.17/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:20:48.523866 slurpkit-0.9.17/slurpkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      235 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 08:20:48.000000 slurpkit-0.9.17/slurpkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 08:20:48.523866 slurpkit-0.9.17/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_0_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2024-05-16 12:22:52.000000 slurpkit-0.9.17/tests/test_1_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_2_planning.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_3_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_4_scanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-16 12:22:52.000000 slurpkit-0.9.17/tests/test_5_scraper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2292 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_6_vault.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_7_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2024-05-15 18:10:44.000000 slurpkit-0.9.17/tests/test_8_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2024-05-16 12:22:52.000000 slurpkit-0.9.17/tests/test_9_clean.py
```

### Comparing `slurpkit-0.9.16/README.md` & `slurpkit-0.9.17/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-Here's a polished version of your README file for the Slurpit SDK:
-
----
-
 # Slurpit SDK
 
 The Slurpit SDK is a Python package for interacting with the Slurpit API, enabling developers to easily manage devices and planning resources. It is designed for simplicity and flexibility, offering methods for listing devices, retrieving planning data, and exporting information to CSV format.
 
 ## Installation
 
 You can install the Slurpit SDK using pip with the following command:
@@ -13,15 +9,15 @@
 ```bash
 pip install slurpkit
 ```
 
 Alternatively, if you prefer to install from source, clone the repository and run the setup script:
 
 ```bash
-git clone https://github.com/your-repo/slurpit.git
+git clone https://gitlab.com/slurpit.io/python-sdk.git
 cd slurpit
 python setup.py install
 ```
 
 ## Quick Start
 
 To use the SDK, start by importing the package and setting up the API client:
@@ -67,11 +63,7 @@
 Handle large sets of devices with pagination:
 
 ```python
 devices = api.device.get_devices(offset=100, limit=1000)
 for device in devices:
     print(device.hostname)
 ```
-
----
-
-This version enhances clarity, adds context to some sections, and provides a more structured format for ease of reading and use.
```

