# Comparing `tmp/maestral_cocoa-1.9.3.dev1.tar.gz` & `tmp/maestral_cocoa-1.9.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral_cocoa-1.9.3.dev1.tar", last modified: Sat Apr 13 13:51:40 2024, max compression
+gzip compressed data, was "maestral_cocoa-1.9.4.dev0.tar", last modified: Tue May 21 19:33:53 2024, max compression
```

## Comparing `maestral_cocoa-1.9.3.dev1.tar` & `maestral_cocoa-1.9.4.dev0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.872508 maestral_cocoa-1.9.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-13 13:51:40.872508 maestral_cocoa-1.9.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-13 13:51:40.872508 maestral_cocoa-1.9.3.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.856508 maestral_cocoa-1.9.3.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/autostart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/bandwidth_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/dbx_location_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/gtk/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/gtk/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    19822 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.868508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48199 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/faceholder.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   842676 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/maestral.icns
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/release_notes.css
--rw-r--r--   0 runner    (1001) docker     (127)    51081 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-disconnected.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    47443 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-error.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    52917 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-idle.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    52604 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-info.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    46340 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-paused.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    50085 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-syncing.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/selective_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/selective_sync_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11846 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/settings_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/setup_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/syncissues.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.868508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.647241 maestral_cocoa-1.9.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-21 19:33:53.647241 maestral_cocoa-1.9.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 19:33:53.647241 maestral_cocoa-1.9.4.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.635241 maestral_cocoa-1.9.4.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.639241 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17717 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/bandwidth_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/dbx_location_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.643241 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.643241 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.643241 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/cocoa/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/cocoa/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.643241 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/gtk/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/gtk/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19822 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.647241 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48199 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/faceholder.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   842676 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/maestral.icns
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/release_notes.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51081 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-disconnected.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    47443 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-error.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    52917 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-idle.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    52604 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-info.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    46340 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-paused.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    50085 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-syncing.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/selective_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/selective_sync_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11846 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/settings_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/setup_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/syncissues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-21 19:33:48.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:33:53.647241 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-21 19:33:53.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-21 19:33:53.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:33:53.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-21 19:33:53.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:33:53.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-21 19:33:53.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 19:33:53.000000 maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/top_level.txt
```

### Comparing `maestral_cocoa-1.9.3.dev1/LICENSE.txt` & `maestral_cocoa-1.9.4.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/PKG-INFO` & `maestral_cocoa-1.9.4.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-cocoa
-Version: 1.9.3.dev1
+Version: 1.9.4.dev0
 Summary: Open-source Dropbox client for macOS and Linux.
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click
-Requires-Dist: maestral>=1.9.3.dev1
+Requires-Dist: maestral>=1.9.4.dev0
 Requires-Dist: markdown2
 Requires-Dist: toga==0.4.2
 Requires-Dist: rubicon-objc>=0.4.5
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
```

### Comparing `maestral_cocoa-1.9.3.dev1/pyproject.toml` & `maestral_cocoa-1.9.4.dev0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.briefcase]
 project_name = "Maestral"
 bundle = "com.samschott.maestral"
-version = "1.9.3.dev1"
+version = "1.9.4.dev0"
 url = "https://maestral.app"
 license = "MIT license"
 author = "Sam Schott"
 author_email = "sam.schott@outlook.com"
 template = "https://github.com/samschott/briefcase-macOS-Xcode-template.git"
 template_branch = "maestral-v2"
 
@@ -13,15 +13,15 @@
 formal_name = "Maestral"
 description = "An open-source Dropbox client for macOS and Linux"
 icon = "icon/maestral"
 sources = ["src/maestral_cocoa"]
 requires = [
     "chardet==5.2.0",
     "click==8.1.7",
-    "maestral==1.9.3.dev1",
+    "maestral==1.9.4.dev0",
     "markdown2==2.4.13",
     "rubicon-objc==0.4.7",
     "toga==0.4.2",
 ]
 sparkle_feed_url = "https://maestral.app/appcast.xml"
 sparkle_public_key = "RugM2eM14xHixaeHpl5uWSq7+sDZvYi52Xpz4IXpAdA="
 
@@ -29,15 +29,15 @@
 entitlement."com.apple.security.cs.disable-library-validation" = false
 requires = [
     "toga-cocoa==0.4.2",
 ]
 cleanup_paths = [
     "*/unittest",
 ]
-build = "103"
+build = "105"
 
 [tool.briefcase.app.maestral-cocoa.linux]
 supported = false
 
 [tool.black]
 line-length = 88
 target-version = ["py37", "py38", "py39", "py310", "py311"]
```

### Comparing `maestral_cocoa-1.9.3.dev1/setup.cfg` & `maestral_cocoa-1.9.4.dev0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = maestral-cocoa
-version = 1.9.3.dev1
+version = 1.9.4.dev0
 author = Sam Schott
 author_email = sam.schott@outlook.com
 license = MIT
 description = Open-source Dropbox client for macOS and Linux.
 url = https://maestral.app
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -24,15 +24,15 @@
 packages = find:
 package_dir = 
 	= src
 zip_safe = False
 setup_requires = build
 install_requires = 
 	click
-	maestral>=1.9.3.dev1
+	maestral>=1.9.4.dev0
 	markdown2
 	toga==0.4.2
 	rubicon-objc>=0.4.5
 python_requires = >=3.8
 
 [options.packages.find]
 where = src
```

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/__main__.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/__main__.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/activity.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/activity.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/app.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,17 +246,15 @@
         self.item_snooze_separator = MenuItemSeparator()
 
         self.menu_snooze = Menu(
             items=[self.item_snooze30, self.item_snooze60, self.item_snooze480]
         )
         self.item_snooze = MenuItem("Snooze Notifications", submenu=self.menu_snooze)
 
-        self.item_sync_issues = MenuItem(
-            "Show Sync Issues...", action=self.on_sync_issues_clicked
-        )
+        self.item_sync_issues = MenuItem("Show Sync Issues...")
         self.item_rebuild = MenuItem("Rebuild Index...", action=self.on_rebuild_clicked)
 
         self.item_settings = MenuItem("Preferences...", action=self.on_settings_clicked)
         self.item_updates = MenuItem(
             "Check for Updates...", action=self.updater.check_for_updates
         )
 
@@ -264,22 +262,23 @@
             self.item_quit.label = "Quit Maestral"
         else:
             self.item_quit.label = "Quit Maestral GUI"
 
         self.menu.insert(2, MenuItemSeparator())
         self.menu.insert(3, self.item_email)
         self.menu.insert(4, self.item_usage)
-        self.menu.insert(7, self.item_pause)
-        self.menu.insert(8, self.item_activity)
-        self.menu.insert(10, self.item_snooze)
-        self.menu.insert(11, self.item_sync_issues)
-        self.menu.insert(12, self.item_rebuild)
-        self.menu.insert(13, MenuItemSeparator())
-        self.menu.insert(14, self.item_settings)
-        self.menu.insert(15, self.item_updates)
+        self.menu.insert(7, self.item_sync_issues)
+        self.menu.insert(8, self.item_pause)
+        self.menu.insert(9, self.item_activity)
+        self.menu.insert(11, self.item_snooze)
+        self.menu.insert(12, self.item_sync_issues)
+        self.menu.insert(13, self.item_rebuild)
+        self.menu.insert(14, MenuItemSeparator())
+        self.menu.insert(15, self.item_settings)
+        self.menu.insert(16, self.item_updates)
 
         self.menu.on_open = self.on_menu_open
 
         # --------------- switch to idle icon -------------------
         self.set_icon(IDLE)
 
     # ==== callbacks menu items ========================================================
@@ -353,31 +352,34 @@
                 gc.collect()
             except CommunicationError:
                 super().exit()
 
     async def update_status(self, interface, *args, **kwargs) -> None:
         """Change icon according to status."""
         n_sync_errors = len(self.mdbx.sync_errors)
+        has_sync_issues = n_sync_errors > 0
         status = self.mdbx.status
         is_paused = self.mdbx.paused
 
         # update icon
-        if n_sync_errors > 0 and status == IDLE:
+        if has_sync_issues and status == IDLE:
             new_icon = SYNC_ERROR
         else:
             new_icon = status
 
         self.set_icon(new_icon)
 
         # update action texts
         if self.menu.visible:
-            if n_sync_errors > 0:
+            if has_sync_issues:
+                self.item_sync_issues.action = self.on_sync_issues_clicked
                 self.item_sync_issues.label = f"Show Sync Issues ({n_sync_errors})..."
             else:
-                self.item_sync_issues.label = "Show Sync Issues..."
+                self.item_sync_issues.action = None
+                self.item_sync_issues.label = f"No Sync Issues"
 
             self.item_pause.label = self.RESUME_TEXT if is_paused else self.PAUSE_TEXT
             self.item_usage.label = self.mdbx.get_state("account", "usage")
             self.item_email.label = self.mdbx.get_state("account", "email")
 
             self.item_status.label = status
```

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/autostart.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/autostart.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/bandwidth.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/bandwidth.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/bandwidth_gui.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/bandwidth_gui.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/dbx_location_dialog.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/dbx_location_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/dialogs.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/constants.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/cocoa/constants.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/dialogs.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/cocoa/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/factory.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/implementation/cocoa/factory.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/platform.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/platform.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/widgets.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/private/widgets.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/__init__.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/faceholder.pdf` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/faceholder.pdf`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/maestral.icns` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/maestral.icns`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-disconnected.pdf` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-disconnected.pdf`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-error.pdf` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-error.pdf`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-idle.pdf` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-idle.pdf`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-info.pdf` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-info.pdf`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-paused.pdf` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-paused.pdf`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-syncing.pdf` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/resources/systray-syncing.pdf`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/selective_sync.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/selective_sync.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/selective_sync_gui.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/selective_sync_gui.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/settings.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/settings.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/settings_gui.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/settings_gui.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/setup.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/setup.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/setup_gui.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/setup_gui.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/syncissues.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/syncissues.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/updater.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/updater.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/utils.py` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa/utils.py`

 * *Files identical despite different names*

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/PKG-INFO` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-cocoa
-Version: 1.9.3.dev1
+Version: 1.9.4.dev0
 Summary: Open-source Dropbox client for macOS and Linux.
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click
-Requires-Dist: maestral>=1.9.3.dev1
+Requires-Dist: maestral>=1.9.4.dev0
 Requires-Dist: markdown2
 Requires-Dist: toga==0.4.2
 Requires-Dist: rubicon-objc>=0.4.5
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
```

### Comparing `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/SOURCES.txt` & `maestral_cocoa-1.9.4.dev0/src/maestral_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

