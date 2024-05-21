# Comparing `tmp/rtd-cli-0.0.1.tar.gz` & `tmp/rtd-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtd-cli-0.0.1.tar", last modified: Tue May 21 20:33:58 2024, max compression
+gzip compressed data, was "rtd-cli-0.0.2.tar", last modified: Tue May 21 20:38:54 2024, max compression
```

## Comparing `rtd-cli-0.0.1.tar` & `rtd-cli-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:33:57.999798 rtd-cli-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 20:33:57.999798 rtd-cli-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 20:33:48.000000 rtd-cli-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:33:57.999798 rtd-cli-0.0.1/rtd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:33:48.000000 rtd-cli-0.0.1/rtd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-21 20:33:48.000000 rtd-cli-0.0.1/rtd/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:33:57.999798 rtd-cli-0.0.1/rtd_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 20:33:57.000000 rtd-cli-0.0.1/rtd_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 20:33:57.000000 rtd-cli-0.0.1/rtd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:33:57.000000 rtd-cli-0.0.1/rtd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 20:33:57.000000 rtd-cli-0.0.1/rtd_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 20:33:57.000000 rtd-cli-0.0.1/rtd_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 20:33:57.000000 rtd-cli-0.0.1/rtd_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:33:57.999798 rtd-cli-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 20:33:48.000000 rtd-cli-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:54.781307 rtd-cli-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-21 20:38:54.781307 rtd-cli-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 20:38:44.000000 rtd-cli-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:54.777307 rtd-cli-0.0.2/rtd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:44.000000 rtd-cli-0.0.2/rtd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-21 20:38:44.000000 rtd-cli-0.0.2/rtd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:54.781307 rtd-cli-0.0.2/rtd_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:38:54.781307 rtd-cli-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-21 20:38:44.000000 rtd-cli-0.0.2/setup.py
```

### Comparing `rtd-cli-0.0.1/README.md` & `rtd-cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rtd-cli-0.0.1/rtd/main.py` & `rtd-cli-0.0.2/rtd/main.py`

 * *Files identical despite different names*

