# Comparing `tmp/remla24_team7_app-0.0.2.tar.gz` & `tmp/remla24_team7_app-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla24_team7_app-0.0.2.tar", last modified: Tue May 21 20:13:54 2024, max compression
+gzip compressed data, was "remla24_team7_app-0.1.0.tar", max compression
```

## Comparing `remla24_team7_app-0.0.2.tar` & `remla24_team7_app-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,4 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:13:54.070653 remla24_team7_app-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-21 20:13:54.070653 remla24_team7_app-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-21 20:13:36.000000 remla24_team7_app-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 20:13:36.000000 remla24_team7_app-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:13:54.070653 remla24_team7_app-0.0.2/remla24_team7_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:13:36.000000 remla24_team7_app-0.0.2/remla24_team7_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-21 20:13:36.000000 remla24_team7_app-0.0.2/remla24_team7_app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:13:54.070653 remla24_team7_app-0.0.2/remla24_team7_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-21 20:13:54.000000 remla24_team7_app-0.0.2/remla24_team7_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-21 20:13:54.000000 remla24_team7_app-0.0.2/remla24_team7_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:13:54.000000 remla24_team7_app-0.0.2/remla24_team7_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 20:13:54.000000 remla24_team7_app-0.0.2/remla24_team7_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:13:54.070653 remla24_team7_app-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-21 20:13:37.000000 remla24_team7_app-0.0.2/setup.py
+-rw-r--r--   0        0        0      450 2024-05-13 18:43:54.992406 remla24_team7_app-0.1.0/README.md
+-rw-r--r--   0        0        0      317 2024-05-13 18:43:54.992406 remla24_team7_app-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      729 2024-05-13 18:43:54.992406 remla24_team7_app-0.1.0/remla24_team7_app/app.py
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 remla24_team7_app-0.1.0/PKG-INFO
```

### Comparing `remla24_team7_app-0.0.2/remla24_team7_app/app.py` & `remla24_team7_app-0.1.0/remla24_team7_app/app.py`

 * *Files identical despite different names*

