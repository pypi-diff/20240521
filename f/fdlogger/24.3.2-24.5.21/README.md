# Comparing `tmp/fdlogger-24.3.2.tar.gz` & `tmp/fdlogger-24.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdlogger-24.3.2.tar", last modified: Sun Mar  3 01:48:47 2024, max compression
+gzip compressed data, was "fdlogger-24.5.21.tar", last modified: Tue May 21 16:58:51 2024, max compression
```

## Comparing `fdlogger-24.3.2.tar` & `fdlogger-24.5.21.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-03-03 01:48:47.758259 fdlogger-24.3.2/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-07-24 04:24:05.000000 fdlogger-24.3.2/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22568 2024-03-03 01:48:47.757259 fdlogger-24.3.2/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21685 2024-02-22 22:32:15.000000 fdlogger-24.3.2/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-03-03 01:48:47.702258 fdlogger-24.3.2/fdlogger/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   110725 2024-03-03 01:44:51.000000 fdlogger-24.3.2/fdlogger/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-03-03 01:48:47.731258 fdlogger-24.3.2/fdlogger/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3051 2023-06-26 06:12:26.000000 fdlogger-24.3.2/fdlogger/data/arrl_sect.dat
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-06-01 02:37:05.000000 fdlogger-24.3.2/fdlogger/data/cwmacros_fd.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2023-02-01 18:15:34.000000 fdlogger-24.3.2/fdlogger/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2023-06-01 02:37:17.000000 fdlogger-24.3.2/fdlogger/data/fd_preferences.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2023-02-01 14:59:00.000000 fdlogger-24.3.2/fdlogger/data/k6gte-fieldday.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   108154 2023-06-18 20:12:09.000000 fdlogger-24.3.2/fdlogger/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-02-22 22:32:15.000000 fdlogger-24.3.2/fdlogger/data/opon.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30785 2023-02-02 20:14:22.000000 fdlogger-24.3.2/fdlogger/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2023-02-01 18:15:34.000000 fdlogger-24.3.2/fdlogger/data/startup.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-03-03 01:48:47.742259 fdlogger-24.3.2/fdlogger/icon/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/cloud_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/cloud_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/cloud_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/gear16x16.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/k6gte-fdlogger.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2023-02-19 21:29:22.000000 fdlogger-24.3.2/fdlogger/icon/logo.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/radio.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/icon/radio_red.png
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-03-03 01:48:47.755259 fdlogger-24.3.2/fdlogger/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-24.3.2/fdlogger/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10234 2023-02-02 20:57:22.000000 fdlogger-24.3.2/fdlogger/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2023-02-02 20:57:35.000000 fdlogger-24.3.2/fdlogger/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13600 2023-06-09 20:05:46.000000 fdlogger-24.3.2/fdlogger/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2024-02-22 22:32:15.000000 fdlogger-24.3.2/fdlogger/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2023-02-03 16:08:03.000000 fdlogger-24.3.2/fdlogger/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4949 2024-02-22 22:32:15.000000 fdlogger-24.3.2/fdlogger/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6707 2023-04-08 23:33:07.000000 fdlogger-24.3.2/fdlogger/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2024-03-03 01:48:19.000000 fdlogger-24.3.2/fdlogger/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2023-02-02 20:14:22.000000 fdlogger-24.3.2/fdlogger/lib/versiontest.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-03-03 01:48:47.757259 fdlogger-24.3.2/fdlogger.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22568 2024-03-03 01:48:47.000000 fdlogger-24.3.2/fdlogger.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1218 2024-03-03 01:48:47.000000 fdlogger-24.3.2/fdlogger.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-03-03 01:48:47.000000 fdlogger-24.3.2/fdlogger.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2024-03-03 01:48:47.000000 fdlogger-24.3.2/fdlogger.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2024-03-03 01:48:47.000000 fdlogger-24.3.2/fdlogger.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2024-03-03 01:48:47.000000 fdlogger-24.3.2/fdlogger.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1179 2024-03-03 01:48:19.000000 fdlogger-24.3.2/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-03-03 01:48:47.758259 fdlogger-24.3.2/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-03-03 01:48:47.756259 fdlogger-24.3.2/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2022-09-14 17:33:52.000000 fdlogger-24.3.2/testing/inject_multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2022-07-24 04:24:05.000000 fdlogger-24.3.2/testing/inject_udp.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 fdlogger-24.3.2/testing/multicast_listener.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2023-06-09 19:22:31.000000 fdlogger-24.3.2/testing/simulant.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.910135 fdlogger-24.5.21/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-05-21 16:05:29.000000 fdlogger-24.5.21/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22907 2024-05-21 16:58:51.909135 fdlogger-24.5.21/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22023 2024-05-21 16:50:55.000000 fdlogger-24.5.21/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.884135 fdlogger-24.5.21/fdlogger/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   113266 2024-05-21 16:43:49.000000 fdlogger-24.5.21/fdlogger/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.893135 fdlogger-24.5.21/fdlogger/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3051 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/arrl_sect.dat
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/cwmacros_fd.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/fd_preferences.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/k6gte-fieldday.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   108154 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/opon.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    31170 2024-05-21 16:29:04.000000 fdlogger-24.5.21/fdlogger/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/startup.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.897135 fdlogger-24.5.21/fdlogger/icon/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/cloud_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/cloud_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/cloud_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/gear16x16.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/k6gte-fdlogger.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/logo.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/radio.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/radio_red.png
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.902135 fdlogger-24.5.21/fdlogger/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11160 2024-05-21 16:07:31.000000 fdlogger-24.5.21/fdlogger/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13600 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4949 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6922 2024-05-21 16:35:17.000000 fdlogger-24.5.21/fdlogger/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-05-21 16:45:04.000000 fdlogger-24.5.21/fdlogger/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/versiontest.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.908135 fdlogger-24.5.21/fdlogger.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22907 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1218 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       40 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1180 2024-05-21 16:45:04.000000 fdlogger-24.5.21/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-05-21 16:58:51.910135 fdlogger-24.5.21/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.905135 fdlogger-24.5.21/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2024-05-21 16:05:29.000000 fdlogger-24.5.21/testing/inject_multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2024-05-21 16:05:29.000000 fdlogger-24.5.21/testing/inject_udp.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2024-05-21 16:05:29.000000 fdlogger-24.5.21/testing/multicast_listener.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2024-05-21 16:05:29.000000 fdlogger-24.5.21/testing/simulant.py
```

### Comparing `fdlogger-24.3.2/LICENSE` & `fdlogger-24.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/PKG-INFO` & `fdlogger-24.5.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 24.3.2
+Version: 24.5.21
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -65,14 +65,15 @@
   - [Editing an existing contact](#editing-an-existing-contact)
   - [Super Check Partial](#super-check-partial)
   - [Section partial check](#section-partial-check)
   - [DUP checking](#dup-checking)
   - [Autofill](#autofill)
   - [CW Macros](#cw-macros)
   - [CW Macros (Run vs S\&P)](#cw-macros-run-vs-sp)
+  - [CW Macros without a winkeyer](#cw-macros-without-a-winkeyer)
   - [CWDAEMON speed changes](#cwdaemon-speed-changes)
   - [When the event is over](#when-the-event-is-over)
   - [Group / Club logging](#group--club-logging)
     - [Server configuration](#server-configuration)
     - [Client configuration for groups](#client-configuration-for-groups)
     - [Chat Window](#chat-window)
     - [How to know the server is there](#how-to-know-the-server-is-there)
@@ -97,14 +98,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [24.5.21] Add sending CW via CAT(rigctld)
 - [24.2.21] Added OPON.
 - [24.2.19] Corrected the datetime.utcnow() deprecation to work on Python 3.9+
 - [24.2.11] Trapped a KeyError in get_state()
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23.11.9] Merged from @wvolz fixing crash related to tuning to a non ham band.
 - [23.6.25] Fixed missing Canadian sections.
 - [23.6.24] Fix 6M CW default frequency. Wierdness with VFO fixed.
@@ -316,14 +318,20 @@
 of the screen.
 
 ![Picture showing buttons](https://github.com/mbridak/FieldDayLogger/raw/main/pics/run_sp.png)
 
 This can also be used to reload the macros if you edit them while the program
 is running.
 
+## CW Macros without a winkeyer
+
+You can send CW macros if you don't have a k1el winkeyer or workalike as long as you
+use rigctld for CAT control and your radio supports it. In the settings dialog under
+the CW tab, choose CAT.
+
 ## CWDAEMON speed changes
 
 If you use cwdaemon for your cw macro sending, you can press the PageUp and
 PageDown keys on your keyboard to increase/decrease the cw sending speed.
 You can press `ESC` to abort CW output.
 
 ## When the event is over
```

### Comparing `fdlogger-24.3.2/README.md` & `fdlogger-24.5.21/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
   - [Editing an existing contact](#editing-an-existing-contact)
   - [Super Check Partial](#super-check-partial)
   - [Section partial check](#section-partial-check)
   - [DUP checking](#dup-checking)
   - [Autofill](#autofill)
   - [CW Macros](#cw-macros)
   - [CW Macros (Run vs S\&P)](#cw-macros-run-vs-sp)
+  - [CW Macros without a winkeyer](#cw-macros-without-a-winkeyer)
   - [CWDAEMON speed changes](#cwdaemon-speed-changes)
   - [When the event is over](#when-the-event-is-over)
   - [Group / Club logging](#group--club-logging)
     - [Server configuration](#server-configuration)
     - [Client configuration for groups](#client-configuration-for-groups)
     - [Chat Window](#chat-window)
     - [How to know the server is there](#how-to-know-the-server-is-there)
@@ -74,14 +75,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [24.5.21] Add sending CW via CAT(rigctld)
 - [24.2.21] Added OPON.
 - [24.2.19] Corrected the datetime.utcnow() deprecation to work on Python 3.9+
 - [24.2.11] Trapped a KeyError in get_state()
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23.11.9] Merged from @wvolz fixing crash related to tuning to a non ham band.
 - [23.6.25] Fixed missing Canadian sections.
 - [23.6.24] Fix 6M CW default frequency. Wierdness with VFO fixed.
@@ -293,14 +295,20 @@
 of the screen.
 
 ![Picture showing buttons](https://github.com/mbridak/FieldDayLogger/raw/main/pics/run_sp.png)
 
 This can also be used to reload the macros if you edit them while the program
 is running.
 
+## CW Macros without a winkeyer
+
+You can send CW macros if you don't have a k1el winkeyer or workalike as long as you
+use rigctld for CAT control and your radio supports it. In the settings dialog under
+the CW tab, choose CAT.
+
 ## CWDAEMON speed changes
 
 If you use cwdaemon for your cw macro sending, you can press the PageUp and
 PageDown keys on your keyboard to increase/decrease the cw sending speed.
 You can press `ESC` to abort CW output.
 
 ## When the event is over
```

### Comparing `fdlogger-24.3.2/fdlogger/__main__.py` & `fdlogger-24.5.21/fdlogger/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1211,103 +1211,157 @@
 
     def sendf1(self):
         """send f1"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F1.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F1.text()
-            self.cw.sendcw(f"{self.process_macro(self.F1.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F1.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F1.toolTip())} ")
 
     def sendf2(self):
         """send f2"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F2.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F2.text()
-            self.cw.sendcw(f"{self.process_macro(self.F2.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F2.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F2.toolTip())} ")
 
     def sendf3(self):
         """send f3"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F3.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F3.text()
-            self.cw.sendcw(f"{self.process_macro(self.F3.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F3.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F3.toolTip())} ")
 
     def sendf4(self):
         """send f4"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F4.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F4.text()
-            self.cw.sendcw(f"{self.process_macro(self.F4.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F4.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F4.toolTip())} ")
 
     def sendf5(self):
         """send f5"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F5.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F5.text()
-            self.cw.sendcw(f"{self.process_macro(self.F5.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F5.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F5.toolTip())} ")
 
     def sendf6(self):
         """send f6"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F6.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F6.text()
-            self.cw.sendcw(f"{self.process_macro(self.F6.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F6.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F6.toolTip())} ")
 
     def sendf7(self):
         """send f7"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F7.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F7.text()
-            self.cw.sendcw(f"{self.process_macro(self.F7.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F7.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F7.toolTip())} ")
 
     def sendf8(self):
         """send f8"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F8.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F8.text()
-            self.cw.sendcw(f"{self.process_macro(self.F8.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F8.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F8.toolTip())} ")
 
     def sendf9(self):
         """send f9"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F9.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F9.text()
-            self.cw.sendcw(f"{self.process_macro(self.F9.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(f"{self.process_macro(self.F9.toolTip())} ")
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F9.toolTip())} ")
 
     def sendf10(self):
         """send f10"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F10.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F10.text()
-            self.cw.sendcw(f"{self.process_macro(self.F10.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(
+                        f"{self.process_macro(self.F10.toolTip())} "
+                    )
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F10.toolTip())} ")
 
     def sendf11(self):
         """send f11"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F11.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F11.text()
-            self.cw.sendcw(f"{self.process_macro(self.F11.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(
+                        f"{self.process_macro(self.F11.toolTip())} "
+                    )
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F11.toolTip())} ")
 
     def sendf12(self):
         """send f12"""
         if self.cw is not None:
             self.infoline.setText(f"Sending {self.process_macro(self.F12.toolTip())}")
             if self.preference.get("send_n1mm_packets"):
                 self.n1mm.radio_info["FunctionKeyCaption"] = self.F12.text()
-            self.cw.sendcw(f"{self.process_macro(self.F12.toolTip())} ")
+            if self.cw.servertype == 3:
+                if self.cat_control is not None:
+                    self.cat_control.sendcw(
+                        f"{self.process_macro(self.F12.toolTip())} "
+                    )
+            else:
+                self.cw.sendcw(f"{self.process_macro(self.F12.toolTip())} ")
 
     def clearinputs(self):
         """clear text entry fields"""
         self.callsign_entry.clear()
         self.class_entry.clear()
         self.section_entry.clear()
         self.callsign_entry.setFocus()
```

### Comparing `fdlogger-24.3.2/fdlogger/data/JetBrainsMono-Regular.ttf` & `fdlogger-24.5.21/fdlogger/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/data/MASTER.SCP` & `fdlogger-24.5.21/fdlogger/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/data/arrl_sect.dat` & `fdlogger-24.5.21/fdlogger/data/arrl_sect.dat`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/data/dialog.ui` & `fdlogger-24.5.21/fdlogger/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/data/fd_preferences.json` & `fdlogger-24.5.21/fdlogger/data/fd_preferences.json`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/data/main.ui` & `fdlogger-24.5.21/fdlogger/data/main.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/data/opon.ui` & `fdlogger-24.5.21/fdlogger/data/opon.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/data/settings.ui` & `fdlogger-24.5.21/fdlogger/data/settings.ui`

 * *Files 1% similar despite different names*

#### Comparing `fdlogger-24.3.2/fdlogger/data/settings.ui` & `fdlogger-24.5.21/fdlogger/data/settings.ui`

```diff
@@ -516,56 +516,56 @@
             </layout>
           </widget>
           <widget class="QWidget" name="tab">
             <attribute name="title">
               <string>CW</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_6">
-              <item row="0" column="0">
-                <widget class="QLabel" name="label_10">
+              <item row="1" column="0">
+                <widget class="QLabel" name="label_11">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                     </font>
                   </property>
                   <property name="text">
-                    <string>CW_Address:</string>
+                    <string>CW_Port:</string>
                   </property>
                   <property name="alignment">
                     <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_11">
+              <item row="0" column="1" colspan="3">
+                <widget class="QLineEdit" name="cwip_field">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                     </font>
                   </property>
                   <property name="text">
-                    <string>CW_Port:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                    <string>localhost</string>
                   </property>
                 </widget>
               </item>
-              <item row="2" column="0" alignment="Qt::AlignHCenter">
-                <widget class="QRadioButton" name="usecwdaemon_radioButton">
+              <item row="1" column="1" colspan="3">
+                <widget class="QLineEdit" name="cwport_field">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                     </font>
                   </property>
+                  <property name="inputMethodHints">
+                    <set>Qt::ImhDigitsOnly</set>
+                  </property>
                   <property name="text">
-                    <string>cwdaemon</string>
+                    <string>6789</string>
                   </property>
                 </widget>
               </item>
               <item row="2" column="1" alignment="Qt::AlignHCenter">
                 <widget class="QRadioButton" name="usepywinkeyer_radioButton">
                   <property name="font">
                     <font>
@@ -574,53 +574,66 @@
                     </font>
                   </property>
                   <property name="text">
                     <string>PyWinkeyer</string>
                   </property>
                 </widget>
               </item>
-              <item row="2" column="2" alignment="Qt::AlignHCenter">
-                <widget class="QRadioButton" name="radioButton_5">
+              <item row="2" column="0" alignment="Qt::AlignHCenter">
+                <widget class="QRadioButton" name="usecwdaemon_radioButton">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                     </font>
                   </property>
                   <property name="text">
-                    <string>None</string>
+                    <string>cwdaemon</string>
                   </property>
                 </widget>
               </item>
-              <item row="1" column="1" colspan="2">
-                <widget class="QLineEdit" name="cwport_field">
+              <item row="0" column="0">
+                <widget class="QLabel" name="label_10">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                     </font>
                   </property>
-                  <property name="inputMethodHints">
-                    <set>Qt::ImhDigitsOnly</set>
+                  <property name="text">
+                    <string>CW_Address:</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                  </property>
+                </widget>
+              </item>
+              <item row="2" column="3" alignment="Qt::AlignHCenter">
+                <widget class="QRadioButton" name="radioButton_5">
+                  <property name="font">
+                    <font>
+                      <family>JetBrains Mono</family>
+                      <pointsize>12</pointsize>
+                    </font>
                   </property>
                   <property name="text">
-                    <string>6789</string>
+                    <string>None</string>
                   </property>
                 </widget>
               </item>
-              <item row="0" column="1" colspan="2">
-                <widget class="QLineEdit" name="cwip_field">
+              <item row="2" column="2">
+                <widget class="QRadioButton" name="usecat4cw_radioButton">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                     </font>
                   </property>
                   <property name="text">
-                    <string>localhost</string>
+                    <string>CAT</string>
                   </property>
                 </widget>
               </item>
             </layout>
           </widget>
           <widget class="QWidget" name="tab_5">
             <attribute name="title">
```

### Comparing `fdlogger-24.3.2/fdlogger/data/startup.ui` & `fdlogger-24.5.21/fdlogger/data/startup.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/cloud_green.png` & `fdlogger-24.5.21/fdlogger/icon/cloud_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/cloud_grey.png` & `fdlogger-24.5.21/fdlogger/icon/cloud_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/gear16x16.png` & `fdlogger-24.5.21/fdlogger/icon/gear16x16.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/k6gte-fdlogger.png` & `fdlogger-24.5.21/fdlogger/icon/k6gte-fdlogger.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/logo.png` & `fdlogger-24.5.21/fdlogger/icon/logo.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/radio.svg` & `fdlogger-24.5.21/fdlogger/icon/radio.svg`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/radio_green.png` & `fdlogger-24.5.21/fdlogger/icon/radio_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/radio_grey.png` & `fdlogger-24.5.21/fdlogger/icon/radio_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/icon/radio_red.png` & `fdlogger-24.5.21/fdlogger/icon/radio_red.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/lib/cat_interface.py` & `fdlogger-24.5.21/fdlogger/lib/cat_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CAT interface abstraction"""
+
 import logging
 import socket
 import xmlrpc.client
 
 
 class CAT:
     """CAT control rigctld or flrig"""
@@ -60,14 +61,42 @@
             self.logger.debug("Connected to rigctrld")
             self.online = True
         except ConnectionRefusedError as exception:
             self.rigctrlsocket = None
             self.online = False
             self.logger.debug("%s", exception)
 
+    def sendcw(self, texttosend):
+        """..."""
+        self.logger.debug(f"{texttosend=} {self.interface=}")
+        if self.interface == "flrig":
+            ...
+            return
+        if self.interface == "rigctld":
+            self.sendcwrigctl(texttosend)
+
+    def sendcwrigctl(self, texttosend):
+        """..."""
+        if self.rigctrlsocket:
+            try:
+                self.online = True
+                self.rigctrlsocket.send(bytes(f"b{texttosend}\n", "utf-8"))
+                _ = self.rigctrlsocket.recv(1024).decode().strip()
+                return True
+            except socket.error as exception:
+                self.online = False
+                self.logger.debug("setvfo_rigctld: %s", f"{exception}")
+                self.rigctrlsocket = None
+                return False
+        self.__initialize_rigctrld()
+        return False
+
+    def sendcwxmlrpc(self, texttosend):
+        """..."""
+
     def get_vfo(self) -> str:
         """Poll the radio for current vfo using the interface"""
         vfo = ""
         if self.interface == "flrig":
             vfo = self.__getvfo_flrig()
             self.logger.debug("%s", vfo)
         if self.interface == "rigctld":
```

### Comparing `fdlogger-24.3.2/fdlogger/lib/cwinterface.py` & `fdlogger-24.5.21/fdlogger/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/lib/database.py` & `fdlogger-24.5.21/fdlogger/lib/database.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/lib/lookup.py` & `fdlogger-24.5.21/fdlogger/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/lib/n1mm.py` & `fdlogger-24.5.21/fdlogger/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger/lib/settings.py` & `fdlogger-24.5.21/fdlogger/lib/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
             self.cwport_field.setText(str(self.preference.get("cwport", "")))
             self.usecwdaemon_radioButton.setChecked(
                 bool(self.preference.get("cwtype") == 1)
             )
             self.usepywinkeyer_radioButton.setChecked(
                 bool(self.preference.get("cwtype") == 2)
             )
+            self.usecat4cw_radioButton.setChecked(
+                bool(self.preference.get("cwtype") == 3)
+            )
             self.connect_to_server.setChecked(bool(self.preference.get("useserver")))
             self.multicast_group.setText(
                 str(self.preference.get("multicast_group", ""))
             )
             self.multicast_port.setText(str(self.preference.get("multicast_port", "")))
             self.interface_ip.setText(str(self.preference.get("interface_ip", "")))
 
@@ -106,14 +109,16 @@
         self.preference["cwip"] = self.cwip_field.text()
         self.preference["cwport"] = int(self.cwport_field.text())
         self.preference["cwtype"] = 0
         if self.usecwdaemon_radioButton.isChecked():
             self.preference["cwtype"] = 1
         if self.usepywinkeyer_radioButton.isChecked():
             self.preference["cwtype"] = 2
+        if self.usecat4cw_radioButton.isChecked():
+            self.preference["cwtype"] = 3
         self.preference["useserver"] = self.connect_to_server.isChecked()
         self.preference["multicast_group"] = self.multicast_group.text()
         self.preference["multicast_port"] = self.multicast_port.text()
         self.preference["interface_ip"] = self.interface_ip.text()
 
         self.preference["send_n1mm_packets"] = self.send_n1mm_packets.isChecked()
         self.preference["n1mm_station_name"] = self.n1mm_station_name.text()
```

### Comparing `fdlogger-24.3.2/fdlogger/lib/versiontest.py` & `fdlogger-24.5.21/fdlogger/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/fdlogger.egg-info/PKG-INFO` & `fdlogger-24.5.21/fdlogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 24.3.2
+Version: 24.5.21
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -65,14 +65,15 @@
   - [Editing an existing contact](#editing-an-existing-contact)
   - [Super Check Partial](#super-check-partial)
   - [Section partial check](#section-partial-check)
   - [DUP checking](#dup-checking)
   - [Autofill](#autofill)
   - [CW Macros](#cw-macros)
   - [CW Macros (Run vs S\&P)](#cw-macros-run-vs-sp)
+  - [CW Macros without a winkeyer](#cw-macros-without-a-winkeyer)
   - [CWDAEMON speed changes](#cwdaemon-speed-changes)
   - [When the event is over](#when-the-event-is-over)
   - [Group / Club logging](#group--club-logging)
     - [Server configuration](#server-configuration)
     - [Client configuration for groups](#client-configuration-for-groups)
     - [Chat Window](#chat-window)
     - [How to know the server is there](#how-to-know-the-server-is-there)
@@ -97,14 +98,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [24.5.21] Add sending CW via CAT(rigctld)
 - [24.2.21] Added OPON.
 - [24.2.19] Corrected the datetime.utcnow() deprecation to work on Python 3.9+
 - [24.2.11] Trapped a KeyError in get_state()
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23.11.9] Merged from @wvolz fixing crash related to tuning to a non ham band.
 - [23.6.25] Fixed missing Canadian sections.
 - [23.6.24] Fix 6M CW default frequency. Wierdness with VFO fixed.
@@ -316,14 +318,20 @@
 of the screen.
 
 ![Picture showing buttons](https://github.com/mbridak/FieldDayLogger/raw/main/pics/run_sp.png)
 
 This can also be used to reload the macros if you edit them while the program
 is running.
 
+## CW Macros without a winkeyer
+
+You can send CW macros if you don't have a k1el winkeyer or workalike as long as you
+use rigctld for CAT control and your radio supports it. In the settings dialog under
+the CW tab, choose CAT.
+
 ## CWDAEMON speed changes
 
 If you use cwdaemon for your cw macro sending, you can press the PageUp and
 PageDown keys on your keyboard to increase/decrease the cw sending speed.
 You can press `ESC` to abort CW output.
 
 ## When the event is over
```

### Comparing `fdlogger-24.3.2/fdlogger.egg-info/SOURCES.txt` & `fdlogger-24.5.21/fdlogger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/pyproject.toml` & `fdlogger-24.5.21/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdlogger" 
-version = "24.3.2"
+version = "24.5.21"
 description = "ARRL Field Day logger GUI"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `fdlogger-24.3.2/testing/inject_multicast.py` & `fdlogger-24.5.21/testing/inject_multicast.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/testing/inject_udp.py` & `fdlogger-24.5.21/testing/inject_udp.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/testing/multicast_listener.py` & `fdlogger-24.5.21/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.3.2/testing/simulant.py` & `fdlogger-24.5.21/testing/simulant.py`

 * *Files identical despite different names*

