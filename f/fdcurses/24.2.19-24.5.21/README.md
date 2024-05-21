# Comparing `tmp/fdcurses-24.2.19.tar.gz` & `tmp/fdcurses-24.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdcurses-24.2.19.tar", last modified: Mon Feb 19 18:46:01 2024, max compression
+gzip compressed data, was "fdcurses-24.5.21.tar", last modified: Tue May 21 17:50:48 2024, max compression
```

## Comparing `fdcurses-24.2.19.tar` & `fdcurses-24.5.21.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-02-19 18:46:01.986363 fdcurses-24.2.19/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-22 14:20:09.000000 fdcurses-24.2.19/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17388 2024-02-19 18:46:01.985363 fdcurses-24.2.19/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16520 2024-02-19 18:44:38.000000 fdcurses-24.2.19/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-02-19 18:46:01.970363 fdcurses-24.2.19/fdcurses/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    81791 2024-02-19 18:35:21.000000 fdcurses-24.2.19/fdcurses/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-02-19 18:46:01.980363 fdcurses-24.2.19/fdcurses/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      262 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/data/cwmacros_fd.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      716 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/data/fd_preferences.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4560 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/data/icon.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      305 2023-02-05 05:52:56.000000 fdcurses-24.2.19/fdcurses/data/k6gte-fdcurses.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3569 2023-02-05 05:48:58.000000 fdcurses-24.2.19/fdcurses/data/k6gte.fdcurses-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1146 2023-02-05 05:48:27.000000 fdcurses-24.2.19/fdcurses/data/k6gte.fdcurses-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2012 2023-02-05 05:48:44.000000 fdcurses-24.2.19/fdcurses/data/k6gte.fdcurses-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12729 2023-02-05 05:33:14.000000 fdcurses-24.2.19/fdcurses/data/k6gte.fdcurses.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2707 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/data/secname.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      606 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/data/secpartial.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1409 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/data/secstate.json
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-02-19 18:46:01.983363 fdcurses-24.2.19/fdcurses/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8990 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1676 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14004 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6535 2023-02-06 14:22:55.000000 fdcurses-24.2.19/fdcurses/lib/edittextfield.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4192 2023-03-01 18:55:09.000000 fdcurses-24.2.19/fdcurses/lib/groupsettings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13838 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11955 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/lib/server_database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10397 2023-03-01 18:38:35.000000 fdcurses-24.2.19/fdcurses/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-02-19 18:41:37.000000 fdcurses-24.2.19/fdcurses/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5183 2023-02-05 05:13:02.000000 fdcurses-24.2.19/fdcurses/lib/wsjtx_listener.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-02-19 18:46:01.985363 fdcurses-24.2.19/fdcurses.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17388 2024-02-19 18:46:01.000000 fdcurses-24.2.19/fdcurses.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1047 2024-02-19 18:46:01.000000 fdcurses-24.2.19/fdcurses.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-02-19 18:46:01.000000 fdcurses-24.2.19/fdcurses.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2024-02-19 18:46:01.000000 fdcurses-24.2.19/fdcurses.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       29 2024-02-19 18:46:01.000000 fdcurses-24.2.19/fdcurses.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       27 2024-02-19 18:46:01.000000 fdcurses-24.2.19/fdcurses.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1118 2024-02-19 18:41:37.000000 fdcurses-24.2.19/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-02-19 18:46:01.986363 fdcurses-24.2.19/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-02-19 18:46:01.984363 fdcurses-24.2.19/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      796 2022-04-10 14:31:06.000000 fdcurses-24.2.19/testing/inject-udp.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      945 2022-04-10 14:31:06.000000 fdcurses-24.2.19/testing/inject_multicast.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)      521 2023-03-01 18:52:45.000000 fdcurses-24.2.19/testing/multicast_listener.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2023-03-01 18:52:34.000000 fdcurses-24.2.19/testing/simulant.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 17:50:48.479999 fdcurses-24.5.21/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-05-21 17:03:09.000000 fdcurses-24.5.21/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17600 2024-05-21 17:50:48.478999 fdcurses-24.5.21/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16732 2024-05-21 17:49:49.000000 fdcurses-24.5.21/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 17:50:48.460999 fdcurses-24.5.21/fdcurses/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    83270 2024-05-21 17:40:44.000000 fdcurses-24.5.21/fdcurses/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 17:50:48.469999 fdcurses-24.5.21/fdcurses/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      262 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/cwmacros_fd.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      716 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/fd_preferences.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4560 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/icon.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      305 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/k6gte-fdcurses.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3569 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/k6gte.fdcurses-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1146 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/k6gte.fdcurses-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2012 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/k6gte.fdcurses-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12729 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/k6gte.fdcurses.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2707 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/secname.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      606 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/secpartial.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1409 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/data/secstate.json
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 17:50:48.476999 fdcurses-24.5.21/fdcurses/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     9916 2024-05-21 17:08:03.000000 fdcurses-24.5.21/fdcurses/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1676 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14004 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6535 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/lib/edittextfield.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4192 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/lib/groupsettings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13838 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11955 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/lib/server_database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10686 2024-05-21 17:30:55.000000 fdcurses-24.5.21/fdcurses/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-05-21 17:42:51.000000 fdcurses-24.5.21/fdcurses/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5183 2024-05-21 17:03:09.000000 fdcurses-24.5.21/fdcurses/lib/wsjtx_listener.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 17:50:48.478999 fdcurses-24.5.21/fdcurses.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17600 2024-05-21 17:50:48.000000 fdcurses-24.5.21/fdcurses.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1047 2024-05-21 17:50:48.000000 fdcurses-24.5.21/fdcurses.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-05-21 17:50:48.000000 fdcurses-24.5.21/fdcurses.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2024-05-21 17:50:48.000000 fdcurses-24.5.21/fdcurses.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       29 2024-05-21 17:50:48.000000 fdcurses-24.5.21/fdcurses.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       27 2024-05-21 17:50:48.000000 fdcurses-24.5.21/fdcurses.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1118 2024-05-21 17:42:51.000000 fdcurses-24.5.21/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-05-21 17:50:48.479999 fdcurses-24.5.21/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 17:50:48.477999 fdcurses-24.5.21/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      796 2024-05-21 17:03:09.000000 fdcurses-24.5.21/testing/inject-udp.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      945 2024-05-21 17:03:09.000000 fdcurses-24.5.21/testing/inject_multicast.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)      521 2024-05-21 17:03:09.000000 fdcurses-24.5.21/testing/multicast_listener.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2024-05-21 17:03:09.000000 fdcurses-24.5.21/testing/simulant.py
```

### Comparing `fdcurses-24.2.19/LICENSE` & `fdcurses-24.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/PKG-INFO` & `fdcurses-24.5.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdcurses
-Version: 24.2.19
+Version: 24.5.21
 Summary: ARRL Field Day logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger-Curses
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger-Curses/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -46,14 +46,15 @@
 fdcurses
 ```
 
 ![Alt text](https://github.com/mbridak/FieldDayLogger-Curses/raw/master/pics/logger.png)
 
 # Recent changes
 
+- [24.5.21] Add sending CW macros via CAT(rigctld).
 - [24.2.19] Fixed deprecation changes to work on Python 3.9+
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23-2-6] Removed import of tkinter, replaced with pyperclip. Safer access to dict strings in settings. Removed inverse video characters, hard on the eyes.
 - [23-2-5] Fixed crash when too many SCP matches happen.
 - [23-2-5] Safer dict key access.
 - [23-2-4] Repackaged for PyPi. Updated RAC sections.
 Added an aggregation server for group/club logging.
@@ -114,14 +115,16 @@
 I had to remap that to Shift+F11 in the terminal preference shortcuts.
 It also wanted to show a menu each time you pressed F10.
 That can be suppressed in the terminals preferences general section.
 
 If you're using cwdaemon you can change the cw sending speed by pressing + or -.
 You can abort CW output by pressing `ESC`.
 
+If you do not have a K1EL winkeyer or work-a-like, and you are using rigctld for CAT control. You can select CAT to send CW as long as your radio supports it.
+
 #### Callsign lookups
 
 An option of callsign lookups for gridsquare and op name is offered by one of three services: QRZ, HamDB or HamQTH. The use of these can be turned on or off by editing the JSON preference file. The lookup happens in it's own thread and is kicked off after the cursor leaves the call field. If the look up is successful, you'll see the status line at the bottom change giving you name, grid, bearing and distance to contact.
 
 ![lookup result](https://github.com/mbridak/FieldDayLogger-Curses/raw/master/pics/lookup-result.png)
 
 #### WSJT-X FT8
```

### Comparing `fdcurses-24.2.19/README.md` & `fdcurses-24.5.21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 fdcurses
 ```
 
 ![Alt text](https://github.com/mbridak/FieldDayLogger-Curses/raw/master/pics/logger.png)
 
 # Recent changes
 
+- [24.5.21] Add sending CW macros via CAT(rigctld).
 - [24.2.19] Fixed deprecation changes to work on Python 3.9+
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23-2-6] Removed import of tkinter, replaced with pyperclip. Safer access to dict strings in settings. Removed inverse video characters, hard on the eyes.
 - [23-2-5] Fixed crash when too many SCP matches happen.
 - [23-2-5] Safer dict key access.
 - [23-2-4] Repackaged for PyPi. Updated RAC sections.
 Added an aggregation server for group/club logging.
@@ -92,14 +93,16 @@
 I had to remap that to Shift+F11 in the terminal preference shortcuts.
 It also wanted to show a menu each time you pressed F10.
 That can be suppressed in the terminals preferences general section.
 
 If you're using cwdaemon you can change the cw sending speed by pressing + or -.
 You can abort CW output by pressing `ESC`.
 
+If you do not have a K1EL winkeyer or work-a-like, and you are using rigctld for CAT control. You can select CAT to send CW as long as your radio supports it.
+
 #### Callsign lookups
 
 An option of callsign lookups for gridsquare and op name is offered by one of three services: QRZ, HamDB or HamQTH. The use of these can be turned on or off by editing the JSON preference file. The lookup happens in it's own thread and is kicked off after the cursor leaves the call field. If the look up is successful, you'll see the status line at the bottom change giving you name, grid, bearing and distance to contact.
 
 ![lookup result](https://github.com/mbridak/FieldDayLogger-Curses/raw/master/pics/lookup-result.png)
 
 #### WSJT-X FT8
```

### Comparing `fdcurses-24.2.19/fdcurses/__main__.py` & `fdcurses-24.5.21/fdcurses/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -839,37 +839,73 @@
     return macro
 
 
 def check_function_keys(key):
     """Sends a CW macro if a function key was pressed."""
     if cw:
         if key == curses.KEY_F1 and "F1" in fkeys:
-            cw.sendcw(process_macro(fkeys["F1"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F1"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F1"][1]))
         elif key == curses.KEY_F2 and "F2" in fkeys:
-            cw.sendcw(process_macro(fkeys["F2"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F2"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F2"][1]))
         elif key == curses.KEY_F3 and "F3" in fkeys:
-            cw.sendcw(process_macro(fkeys["F3"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F3"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F3"][1]))
         elif key == curses.KEY_F4 and "F4" in fkeys:
-            cw.sendcw(process_macro(fkeys["F4"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F4"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F4"][1]))
         elif key == curses.KEY_F5 and "F5" in fkeys:
-            cw.sendcw(process_macro(fkeys["F5"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F5"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F5"][1]))
         elif key == curses.KEY_F6 and "F6" in fkeys:
-            cw.sendcw(process_macro(fkeys["F6"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F6"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F6"][1]))
         elif key == curses.KEY_F7 and "F7" in fkeys:
-            cw.sendcw(process_macro(fkeys["F7"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F7"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F7"][1]))
         elif key == curses.KEY_F8 and "F8" in fkeys:
-            cw.sendcw(process_macro(fkeys["F8"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F8"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F8"][1]))
         elif key == curses.KEY_F9 and "F9" in fkeys:
-            cw.sendcw(process_macro(fkeys["F9"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F9"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F9"][1]))
         elif key == curses.KEY_F10 and "F10" in fkeys:
-            cw.sendcw(process_macro(fkeys["F10"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F10"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F10"][1]))
         elif key == curses.KEY_F11 and "F11" in fkeys:
-            cw.sendcw(process_macro(fkeys["F11"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F11"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F11"][1]))
         elif key == curses.KEY_F12 and "F12" in fkeys:
-            cw.sendcw(process_macro(fkeys["F12"][1]))
+            if cw.servertype == 3:
+                cat_control.sendcw(process_macro(fkeys["F12"][1]))
+            else:
+                cw.sendcw(process_macro(fkeys["F12"][1]))
         elif key == 43 and cw.servertype == 1:
             cw.speed += 1
             cw.sendcw(f"\x1b2{cw.speed}")
             statusline()
         elif key == 45 and cw.servertype == 1:
             cw.speed -= 1
             if cw.speed < 5:
```

### Comparing `fdcurses-24.2.19/fdcurses/data/MASTER.SCP` & `fdcurses-24.5.21/fdcurses/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/fd_preferences.json` & `fdcurses-24.5.21/fdcurses/data/fd_preferences.json`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/icon.svg` & `fdcurses-24.5.21/fdcurses/data/icon.svg`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/k6gte.fdcurses-128.png` & `fdcurses-24.5.21/fdcurses/data/k6gte.fdcurses-128.png`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/k6gte.fdcurses-32.png` & `fdcurses-24.5.21/fdcurses/data/k6gte.fdcurses-32.png`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/k6gte.fdcurses-64.png` & `fdcurses-24.5.21/fdcurses/data/k6gte.fdcurses-64.png`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/k6gte.fdcurses.svg` & `fdcurses-24.5.21/fdcurses/data/k6gte.fdcurses.svg`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/secname.json` & `fdcurses-24.5.21/fdcurses/data/secname.json`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/secpartial.json` & `fdcurses-24.5.21/fdcurses/data/secpartial.json`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/data/secstate.json` & `fdcurses-24.5.21/fdcurses/data/secstate.json`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/lib/cat_interface.py` & `fdcurses-24.5.21/fdcurses/lib/cat_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CAT interface abstraction"""
+
 import logging
 import socket
 import xmlrpc.client
 
 
 class CAT:
     """CAT control rigctld or flrig"""
@@ -59,14 +60,42 @@
             logging.debug("Connected to rigctrld")
             self.online = True
         except ConnectionRefusedError as exception:
             self.rigctrlsocket = None
             self.online = False
             logging.debug("%s", exception)
 
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
             logging.debug("%s", vfo)
         if self.interface == "rigctld":
```

### Comparing `fdcurses-24.2.19/fdcurses/lib/cwinterface.py` & `fdcurses-24.5.21/fdcurses/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/lib/database.py` & `fdcurses-24.5.21/fdcurses/lib/database.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/lib/edittextfield.py` & `fdcurses-24.5.21/fdcurses/lib/edittextfield.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/lib/groupsettings.py` & `fdcurses-24.5.21/fdcurses/lib/groupsettings.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/lib/lookup.py` & `fdcurses-24.5.21/fdcurses/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/lib/server_database.py` & `fdcurses-24.5.21/fdcurses/lib/server_database.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses/lib/settings.py` & `fdcurses-24.5.21/fdcurses/lib/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """SettingsScreen class"""
+
 # pylint: disable=invalid-name
 # pylint: disable=too-many-function-args
 
 import curses
 import time
 
 try:
@@ -41,15 +42,15 @@
         "                                 CLOUDLOG",
         " Use Cloudlog: [ ]",
         " Cloudlog API:",
         " Cloudlog URL:",
         " Cloudlog StationID:",
         "",
         "                     CW                               BONUSES",
-        "      cwdaemon: [ ]  PyWinkeyer [ ]                Alt-Power: [ ]",
+        "      cwdaemon: [ ]  PyWinkeyer [ ]  CAT [ ]       Alt-Power: [ ]",
         " CW Host:                      CW Port:",
     ]
 
     def __init__(self, preference):
         """setup settings screen"""
         self.preference = preference
         self.input_field_focus = 0
@@ -110,17 +111,20 @@
         self.altpower = EditTextField(self.screen, 19, 64, 1, curses.A_UNDERLINE)
         self.altpower.set_bool(True)
         self.altpower.set_state(bool(preference.get("altpower")))
         self.cwdaemon = EditTextField(self.screen, 19, 18, 1, curses.A_UNDERLINE)
         self.cwdaemon.set_bool(True)
         self.pywinkeyer = EditTextField(self.screen, 19, 34, 1, curses.A_UNDERLINE)
         self.pywinkeyer.set_bool(True)
+        self.cat4cw = EditTextField(self.screen, 19, 43, 1, curses.A_UNDERLINE)
+        self.cat4cw.set_bool(True)
         cwd = preference.get("cwtype")
         self.cwdaemon.set_state(bool(cwd == 1))
         self.pywinkeyer.set_state(bool(cwd == 2))
+        self.cat4cw.set_state(bool(cwd == 3))
         self.CW_IP = EditTextField(self.screen, 20, 11, 20, curses.A_UNDERLINE)
         self.CW_IP.lowercase(True)
         self.CW_IP.set_text(preference.get("CW_IP", "127.0.0.1"))
         self.CW_port = EditTextField(self.screen, 20, 41, 5, curses.A_UNDERLINE)
         self.CW_port.set_text(str(preference.get("CW_port")))
         # self.notathome = EditTextField(self.screen, 19, 50, 1, curses.A_UNDERLINE)
         # self.notathome.set_bool(True)
@@ -147,14 +151,15 @@
             self.CAT_port,
             self.cloudlog,
             self.cloudlogapi,
             self.cloudlogurl,
             self.cloudlogstationid,
             self.cwdaemon,
             self.pywinkeyer,
+            self.cat4cw,
             self.altpower,
             self.CW_IP,
             self.CW_port,
         ]
 
         self._display_menu()
 
@@ -220,14 +225,16 @@
                     self.preference["CW_port"] = int(self.CW_port.text())
                 except ValueError:
                     self.preference["CW_port"] = 0
                 if self.cwdaemon.get_state() is True:
                     self.preference["cwtype"] = 1
                 if self.pywinkeyer.get_state() is True:
                     self.preference["cwtype"] = 2
+                if self.cat4cw.get_state() is True:
+                    self.preference["cwtype"] = 3
                 self.screen.erase()
                 return self.preference
             self.input_fields[self.input_field_focus].getchar(c)
             time.sleep(0.01)
 
     def close(self):
         """not useful yet"""
```

### Comparing `fdcurses-24.2.19/fdcurses/lib/wsjtx_listener.py` & `fdcurses-24.5.21/fdcurses/lib/wsjtx_listener.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/fdcurses.egg-info/PKG-INFO` & `fdcurses-24.5.21/fdcurses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdcurses
-Version: 24.2.19
+Version: 24.5.21
 Summary: ARRL Field Day logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger-Curses
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger-Curses/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -46,14 +46,15 @@
 fdcurses
 ```
 
 ![Alt text](https://github.com/mbridak/FieldDayLogger-Curses/raw/master/pics/logger.png)
 
 # Recent changes
 
+- [24.5.21] Add sending CW macros via CAT(rigctld).
 - [24.2.19] Fixed deprecation changes to work on Python 3.9+
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23-2-6] Removed import of tkinter, replaced with pyperclip. Safer access to dict strings in settings. Removed inverse video characters, hard on the eyes.
 - [23-2-5] Fixed crash when too many SCP matches happen.
 - [23-2-5] Safer dict key access.
 - [23-2-4] Repackaged for PyPi. Updated RAC sections.
 Added an aggregation server for group/club logging.
@@ -114,14 +115,16 @@
 I had to remap that to Shift+F11 in the terminal preference shortcuts.
 It also wanted to show a menu each time you pressed F10.
 That can be suppressed in the terminals preferences general section.
 
 If you're using cwdaemon you can change the cw sending speed by pressing + or -.
 You can abort CW output by pressing `ESC`.
 
+If you do not have a K1EL winkeyer or work-a-like, and you are using rigctld for CAT control. You can select CAT to send CW as long as your radio supports it.
+
 #### Callsign lookups
 
 An option of callsign lookups for gridsquare and op name is offered by one of three services: QRZ, HamDB or HamQTH. The use of these can be turned on or off by editing the JSON preference file. The lookup happens in it's own thread and is kicked off after the cursor leaves the call field. If the look up is successful, you'll see the status line at the bottom change giving you name, grid, bearing and distance to contact.
 
 ![lookup result](https://github.com/mbridak/FieldDayLogger-Curses/raw/master/pics/lookup-result.png)
 
 #### WSJT-X FT8
```

### Comparing `fdcurses-24.2.19/fdcurses.egg-info/SOURCES.txt` & `fdcurses-24.5.21/fdcurses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/pyproject.toml` & `fdcurses-24.5.21/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdcurses" 
-version = "24.2.19"
+version = "24.5.21"
 description = "ARRL Field Day logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `fdcurses-24.2.19/testing/inject-udp.py` & `fdcurses-24.5.21/testing/inject-udp.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/testing/inject_multicast.py` & `fdcurses-24.5.21/testing/inject_multicast.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/testing/multicast_listener.py` & `fdcurses-24.5.21/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `fdcurses-24.2.19/testing/simulant.py` & `fdcurses-24.5.21/testing/simulant.py`

 * *Files identical despite different names*

