# Comparing `tmp/qgis-plugin-dev-tools-0.6.2.tar.gz` & `tmp/qgis_plugin_dev_tools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgis-plugin-dev-tools-0.6.2.tar", last modified: Wed Sep 27 11:00:10 2023, max compression
+gzip compressed data, was "qgis_plugin_dev_tools-0.7.0.tar", last modified: Tue May 21 12:19:55 2024, max compression
```

## Comparing `qgis-plugin-dev-tools-0.6.2.tar` & `qgis_plugin_dev_tools-0.7.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.430318 qgis-plugin-dev-tools-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.430318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/changelog_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/rewrite_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/config/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/config/pyproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/publish/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12530 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/bootstrap/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/daemon_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/utils/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.430318 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2023-09-27 11:00:10.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-09-27 11:00:10.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 11:00:10.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-09-27 11:00:10.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-09-27 11:00:10.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-27 11:00:10.000000 qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 11:00:10.434318 qgis-plugin-dev-tools-0.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/test/test_read_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/test/test_read_dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/test/test_read_pyproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2023-09-27 11:00:01.000000 qgis-plugin-dev-tools-0.6.2/test/test_rewrite_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.794993 qgis_plugin_dev_tools-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.798993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.798993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/changelog_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/rewrite_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.798993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.798993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/config/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/config/pyproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/publish/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/bootstrap/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/daemon_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/utils/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-05-21 12:19:55.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-21 12:19:55.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:19:55.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-21 12:19:55.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 12:19:55.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 12:19:55.000000 qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:19:55.802993 qgis_plugin_dev_tools-0.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/test/test_read_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/test/test_read_dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/test/test_read_pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-21 12:19:45.000000 qgis_plugin_dev_tools-0.7.0/test/test_rewrite_imports.py
```

### Comparing `qgis-plugin-dev-tools-0.6.2/CHANGELOG.md` & `qgis_plugin_dev_tools-0.7.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.0] - 2024-05-21
+
+- Fix: Bundle contents by parsing pep-compliant distribution file catalog instead of possibly missing tool-specific top-level.txt
+- Feat: Allow disabling auto-loaded entrypoint plugins
+
 ## [0.6.2] - 2023-09-27
 
 - Fix: Fix issues with bundling requirements of the requirements recursively
 
 ## [0.6.1] - 2023-09-06
 
 - update author email
@@ -62,7 +67,8 @@
 [0.2.1]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.2.1
 [0.3.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.3.0
 [0.4.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.4.0
 [0.5.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.5.0
 [0.6.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.0
 [0.6.1]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.1
 [0.6.2]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.2
+[0.7.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.7.0
```

### Comparing `qgis-plugin-dev-tools-0.6.2/LICENSE` & `qgis_plugin_dev_tools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/PKG-INFO` & `qgis_plugin_dev_tools-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-dev-tools
-Version: 0.6.2
+Version: 0.7.0
 Summary: QGIS plugin development and packaging tools, which make managing runtime dependencies easy.
 Home-page: https://github.com/nlsfi/qgis-plugin-dev-tools
 Author: National Land Survey of Finland
 Author-email: os@nls.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/qgis-plugin-dev-tools/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -131,14 +131,23 @@
 * Extra plugin must have entry point in group "qgis_plugin_dev_tools"
   * See for example: [Entry point usage with setuptools]
   * Use plugin package name for entry point name
 * Extra plugin needs to be installed in the same python environment where this tool is run in
 
 Extra plugins are loaded on launch and reloaded together with the main plugin if [Plugin Reloader] is used.
 
+You can disable plugin auto-load by using `pyproject.toml` configuration (for example when using a dependency, that also provides a plugin entrypoint):
+
+```toml
+[tool.qgis_plugin_dev_tools]
+disabled_extra_plugins = [
+  "unwanted_plugin_package_name",
+]
+```
+
 ## Development of qgis-plugin-dev-tools
 
 See [development readme](./DEVELOPMENT.md).
 
 ## License & copyright
 
 Licensed under GNU GPL v3.0.
@@ -152,14 +161,19 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.0] - 2024-05-21
+
+- Fix: Bundle contents by parsing pep-compliant distribution file catalog instead of possibly missing tool-specific top-level.txt
+- Feat: Allow disabling auto-loaded entrypoint plugins
+
 ## [0.6.2] - 2023-09-27
 
 - Fix: Fix issues with bundling requirements of the requirements recursively
 
 ## [0.6.1] - 2023-09-06
 
 - update author email
@@ -214,7 +228,8 @@
 [0.2.1]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.2.1
 [0.3.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.3.0
 [0.4.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.4.0
 [0.5.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.5.0
 [0.6.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.0
 [0.6.1]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.1
 [0.6.2]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.2
+[0.7.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.7.0
```

### Comparing `qgis-plugin-dev-tools-0.6.2/README.md` & `qgis_plugin_dev_tools-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,23 @@
 * Extra plugin must have entry point in group "qgis_plugin_dev_tools"
   * See for example: [Entry point usage with setuptools]
   * Use plugin package name for entry point name
 * Extra plugin needs to be installed in the same python environment where this tool is run in
 
 Extra plugins are loaded on launch and reloaded together with the main plugin if [Plugin Reloader] is used.
 
+You can disable plugin auto-load by using `pyproject.toml` configuration (for example when using a dependency, that also provides a plugin entrypoint):
+
+```toml
+[tool.qgis_plugin_dev_tools]
+disabled_extra_plugins = [
+  "unwanted_plugin_package_name",
+]
+```
+
 ## Development of qgis-plugin-dev-tools
 
 See [development readme](./DEVELOPMENT.md).
 
 ## License & copyright
 
 Licensed under GNU GPL v3.0.
```

### Comparing `qgis-plugin-dev-tools-0.6.2/setup.cfg` & `qgis_plugin_dev_tools-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/__init__.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 import sys
 
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 
 LOGGER = logging.getLogger(__name__)
 _handler = logging.StreamHandler(sys.stdout)
 _handler.setFormatter(logging.Formatter("%(asctime)s %(levelname)-8s %(message)s"))
 LOGGER.addHandler(_handler)
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/__main__.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/__init__.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/changelog_parser.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/distribution.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/distribution.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/metadata.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/metadata.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/packaging.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/packaging.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 from pathlib import Path
 
 from qgis_plugin_dev_tools.build.rewrite_imports import (
     rewrite_imports_in_source_file,
     insert_as_first_import,
 )
 from qgis_plugin_dev_tools.config import DevToolsConfig
-from qgis_plugin_dev_tools.utils.distributions import (
-    get_distribution_top_level_package_names,
-)
+from qgis_plugin_dev_tools.utils.distributions import get_distribution_top_level_names
 
 IGNORED_FILES = shutil.ignore_patterns("__pycache__", "*.pyc", "*.pyi")
 LOGGER = logging.getLogger(__name__)
 
 VENDOR_PATH_APPEND_SCRIPT = """
 import sys
 from pathlib import Path
@@ -57,146 +55,138 @@
     )
 
 
 def copy_runtime_requirements(
     dev_tools_config: DevToolsConfig,
     build_directory_path: Path,
 ) -> None:
+    if len(dev_tools_config.runtime_distributions) == 0:
+        return
+
     plugin_package_name = dev_tools_config.plugin_package_name
+    vendor_path = build_directory_path / plugin_package_name / "_vendor"
+
+    vendor_path.mkdir(parents=True)
+    vendor_init_file = vendor_path / "__init__.py"
+    vendor_init_file.touch()
+
+    if dev_tools_config.append_distributions_to_path:
+        vendor_init_file.write_text(VENDOR_PATH_APPEND_SCRIPT)
+        insert_as_first_import(
+            build_directory_path / plugin_package_name / "__init__.py",
+            f"{plugin_package_name}._vendor",
+        )
+
+    vendored_runtime_top_level_names: list[str] = []
 
-    if len(dev_tools_config.runtime_distributions) > 0:
-        vendor_path = build_directory_path / plugin_package_name / "_vendor"
-        vendor_path.mkdir(parents=True)
-        vendor_init_file = vendor_path / "__init__.py"
-        vendor_init_file.touch()
-        if dev_tools_config.append_distributions_to_path:
-            vendor_init_file.write_text(VENDOR_PATH_APPEND_SCRIPT)
-
-    runtime_package_names = []
-    # copy dist infos (licenses etc.) and all provided top level packages
-    for dist in (
+    for vendored_distribution in (
         dev_tools_config.runtime_distributions
         + dev_tools_config.extra_runtime_distributions
     ):
-        dist_info_path = Path(dist._path)  # type: ignore
+        # if a recursively found dependency is provided by system packages,
+        # assume it does not have to be bundled (this is possibly dangerous,
+        # if build is made on a different system package set than runtime)
         if (
-            Path(sys.base_prefix) in dist_info_path.parent.parents
-            and dist in dev_tools_config.extra_runtime_distributions
+            vendored_distribution in dev_tools_config.extra_runtime_distributions
+            and Path(
+                vendored_distribution._path,  # type: ignore
+            ).is_relative_to(Path(sys.base_prefix))
         ):
-            # If QGIS Python includes the dependency, it does not have to be bundled
-            LOGGER.debug(
+            LOGGER.warning(
                 "skipping recursively found runtime requirement %s "
-                "because it is included in QGIS",
-                dist.metadata["Name"],
+                "because it is included in system packages",
+                vendored_distribution.name,
             )
             continue
 
-        dist_top_level_packages = get_distribution_top_level_package_names(dist)
-
-        LOGGER.debug(
-            "bundling runtime requirement %s",
-            dist.metadata["Name"],
-        )
-
-        # don't vendor self, but allow to vendor other packages provided
+        # don't vendor plugin package, but allow to vendor other packages provided
         # from plugin distribution. if "-e ." installs "my-plugin-name" distribution
         # containing my_plugin & my_util_package top level packages, bundling is only
         # needed for my_util_package
-        dist_top_level_packages = [
-            name for name in dist_top_level_packages if name != plugin_package_name
-        ]
-
-        runtime_package_names.extend(dist_top_level_packages)
+        dist_top_level_names = get_distribution_top_level_names(vendored_distribution)
+        dist_top_level_names.discard(plugin_package_name)
 
         LOGGER.debug(
-            "copying %s to build directory",
-            dist_info_path.resolve(),
+            "bundling runtime requirement %s with top level names %s",
+            vendored_distribution.name,
+            dist_top_level_names,
         )
-        shutil.copytree(
-            src=dist_info_path,
-            dst=build_directory_path
-            / plugin_package_name
-            / "_vendor"
-            / dist_info_path.name,
-            ignore=IGNORED_FILES,
+        _copy_distribution_files(
+            vendored_distribution,
+            dist_top_level_names,
+            vendor_path,
         )
-        for package_name in dist_top_level_packages:
-            _copy_package(
-                build_directory_path,
-                dist,
-                dist_info_path,
-                package_name,
-                plugin_package_name,
-            )
 
-    if dev_tools_config.append_distributions_to_path:
-        plugin_init_file = (build_directory_path / plugin_package_name) / "__init__.py"
-        insert_as_first_import(plugin_init_file, f"{plugin_package_name}._vendor")
-        return
+        vendored_runtime_top_level_names.extend(dist_top_level_names)
 
-    for package_name in runtime_package_names:
-        LOGGER.debug("rewriting imports for %s", package_name)
+    if not dev_tools_config.append_distributions_to_path:
+        for package_name in vendored_runtime_top_level_names:
+            LOGGER.debug("rewriting imports for %s", package_name)
 
-        py_files = list((build_directory_path / plugin_package_name).rglob("*.py"))
-        ui_files = list((build_directory_path / plugin_package_name).rglob("*.ui"))
+            py_files = list((build_directory_path / plugin_package_name).rglob("*.py"))
+            ui_files = list((build_directory_path / plugin_package_name).rglob("*.ui"))
 
-        for source_file in py_files + ui_files:
-            rewrite_imports_in_source_file(
-                source_file,
-                rewritten_package_name=package_name,
-                container_package_name=f"{plugin_package_name}._vendor",
-            )
+            for source_file in py_files + ui_files:
+                rewrite_imports_in_source_file(
+                    source_file,
+                    rewritten_package_name=package_name,
+                    container_package_name=f"{plugin_package_name}._vendor",
+                )
 
 
-def _copy_package(
-    build_directory_path: Path,
-    dist: Distribution,
-    dist_info_path: Path,
-    package_name: str,
-    plugin_package_name: str,
+def _copy_distribution_files(
+    distribution: Distribution,
+    top_level_names: set[str],
+    target_root_path: Path,
 ) -> None:
-    LOGGER.debug(
-        "bundling runtime requirement %s package %s",
-        dist.metadata["Name"],
-        package_name,
-    )
+    if (file_paths := distribution.files) is None:
+        LOGGER.warning("could not resolve %s contents to bundle", distribution.name)
+        return
+
+    # bundle metadata directory first
+    distribution_metadata_path = Path(distribution._path)  # type: ignore
     LOGGER.debug(
         "copying %s to build directory",
-        (dist_info_path.parent / package_name).resolve(),
+        distribution_metadata_path.resolve(),
+    )
+    shutil.copytree(
+        src=distribution_metadata_path,
+        dst=target_root_path / distribution_metadata_path.name,
+        ignore=IGNORED_FILES,
     )
 
-    # Full package
-    dist_src = dist_info_path.parent / package_name
-    if dist_src.exists():
+    directories_to_bundle = {
+        top_directory_name
+        for file_path in file_paths
+        if len(file_path.parts) > 1
+        and (top_directory_name := file_path.parts[0]) in top_level_names
+    }
+    files_to_bundle = {
+        file_path
+        for file_path in file_paths
+        if len(file_path.parts) == 1 and file_path.stem in top_level_names
+    }
+
+    record_root_path = distribution_metadata_path.parent
+
+    for directory_path in directories_to_bundle:
+        original_path = record_root_path / directory_path
+        new_path = target_root_path / directory_path
+
+        LOGGER.debug("copying %s to build directory", original_path.resolve())
+
         shutil.copytree(
-            src=dist_src,
-            dst=build_directory_path / plugin_package_name / "_vendor" / package_name,
+            src=original_path,
+            dst=new_path,
             ignore=IGNORED_FILES,
         )
-        return
 
-    # Single module
-    dist_src = dist_info_path.parent / f"{package_name}.py"
-    if dist_src.exists():
-        shutil.copy(
-            src=dist_src, dst=build_directory_path / plugin_package_name / "_vendor"
-        )
-        return
+    for file_path in files_to_bundle:
+        original_path = record_root_path / file_path
+        new_path = target_root_path / file_path
 
-    # pyd file
-    pyd_files = list(dist_info_path.parent.glob(f"{package_name}*.pyd"))
-    if pyd_files:
-        for dist_src in pyd_files:
-            shutil.copy(
-                src=dist_src, dst=build_directory_path / plugin_package_name / "_vendor"
-            )
-        return
-    if not package_name.startswith("_"):
-        raise ValueError(
-            f"Sources for runtime requirement {dist.metadata['Name']} "
-            f"cannot be found in {dist_info_path.parent}"
-        )
+        LOGGER.debug("copying %s to build directory", original_path.resolve())
 
-    LOGGER.warning(
-        "Could not find path %s",
-        (dist_info_path.parent / package_name).resolve(),
-    )
+        shutil.copy(
+            src=original_path,
+            dst=new_path,
+        )
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/build/rewrite_imports.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/build/rewrite_imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,38 +15,38 @@
 
     from_module: str
     to_module: str
 
     _replaced_imported_names: Dict[str, str] = field(default_factory=dict, init=False)
 
     # collect the found imported names to replace the references also
-    def visit_Import(self, node: ast.Import) -> Any:  # noqa N802
+    def visit_Import(self, node: ast.Import) -> Any:  # noqa: N802
         for alias in node.names:
             if alias.name.startswith(f"{self.from_module}.") and alias.asname is None:
                 old_module_name = alias.name
                 new_identifier_name = "vendored_" + alias.name.replace(".", "_")
                 self._replaced_imported_names[old_module_name] = new_identifier_name
                 child_module_names = old_module_name.replace(
                     f"{self.from_module}.", "", 1
                 )
                 alias.name = f"{self.to_module}.{child_module_names}"
                 alias.asname = new_identifier_name
         return node
 
     # check the attributes for an imported module name reference
-    def visit_Attribute(self, node: ast.Attribute) -> Any:  # noqa N802
+    def visit_Attribute(self, node: ast.Attribute) -> Any:  # noqa: N802
         attribute_name = ast.unparse(node)
         if attribute_name in self._replaced_imported_names:
             replaced_name = self._replaced_imported_names[attribute_name]
             return ast.Name(id=replaced_name, ctx=ast.Load())
 
         return self.generic_visit(node)
 
     # this will only handle sys.modules['something'] replace
-    def visit_Subscript(self, node: ast.Subscript) -> Any:  # noqa N802
+    def visit_Subscript(self, node: ast.Subscript) -> Any:  # noqa: N802
         if (
             ast.unparse(node.value) == "sys.modules"
             and isinstance(node.slice, ast.Constant)
             and isinstance(node.slice.value, str)
             and node.slice.value.startswith(f"{self.from_module}.")
         ):
             child_module_names = node.slice.value.replace(f"{self.from_module}.", "", 1)
@@ -65,15 +65,14 @@
     # or the name is defined in a sys.modules key as a constant
     specials = [
         f"import {rewritten_package_name}.",
         f"sys.modules['{rewritten_package_name}.",
         f'sys.modules["{rewritten_package_name}.',
     ]
     if any(special in contents for special in specials):
-
         # hold on to the original for license comments
         # since comments are lost with ast parse+unparse
         orig_file = source_file.with_name(source_file.name + "_original")
         orig_file.write_text(contents, encoding="utf-8")
         original_note = f"# parsed with ast, see original {orig_file.name}\n\n"
 
         tree = ast.parse(contents)
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/cli/__init__.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,33 +17,31 @@
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 
 import argparse
 import logging
 import sys
 from pathlib import Path
-from typing import List, Optional
+from typing import Optional
 
 from importlib_metadata import entry_points
 
 from qgis_plugin_dev_tools import LOGGER as ROOT_LOGGER
 from qgis_plugin_dev_tools.build import make_plugin_zip
 from qgis_plugin_dev_tools.config import DevToolsConfig
 from qgis_plugin_dev_tools.config.dotenv import read_dotenv_configs
 from qgis_plugin_dev_tools.publish import publish_plugin_zip_file
 from qgis_plugin_dev_tools.start import launch_development_qgis
 from qgis_plugin_dev_tools.start.config import DevelopmentModeConfig
-from qgis_plugin_dev_tools.utils.distributions import (
-    get_distribution_top_level_package_names,
-)
+from qgis_plugin_dev_tools.utils.distributions import get_distribution_top_level_names
 
 LOGGER = logging.getLogger(__name__)
 
 
-def start(dotenv_file_paths: List[Path]) -> None:
+def start(dotenv_file_paths: list[Path]) -> None:
     # TODO: allow choosing pyproject file from cli?
     dev_tools_config = DevToolsConfig.from_pyproject_config(Path("pyproject.toml"))
     # TODO: allow setting debugger flag from cli?
     # TODO: find default executable paths to allow zero-config .env?
     # TODO: rglob('metadata.txt') from cwd to allow zero-config pyproject.toml?
     dotenv_config = read_dotenv_configs(dotenv_file_paths)
     LOGGER.info(
@@ -59,21 +57,24 @@
             runtime_environment=dotenv_config.runtime_environment,
             runtime_library_paths=[Path(p) for p in sys.path],
             plugin_package_path=dev_tools_config.plugin_package_path,
             plugin_package_name=dev_tools_config.plugin_package_name,
             plugin_dependency_package_names=[
                 name
                 for dist in dev_tools_config.runtime_distributions
-                for name in get_distribution_top_level_package_names(dist)
+                for name in get_distribution_top_level_names(dist)
             ],
             debugger_library=dotenv_config.DEBUGGER_LIBRARY,
             extra_plugin_package_names=[
                 entry_point.name
                 for entry_point in entry_points_found_from_python_env
-                if entry_point.name != dev_tools_config.plugin_package_name
+                if (
+                    entry_point.name != dev_tools_config.plugin_package_name
+                    and entry_point.name not in dev_tools_config.disabled_extra_plugins
+                )
             ],
         )
     )
 
 
 def build(override_plugin_version: Optional[str]) -> None:
     # TODO: allow choosing pyproject file from cli?
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/config/__init__.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/config/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 
 from collections import ChainMap
 from enum import Enum, auto
 from importlib.util import find_spec
 from pathlib import Path
-from typing import List
 
 from importlib_metadata import Distribution, distribution
 from packaging.requirements import Requirement
 
 from qgis_plugin_dev_tools.config.pyproject import read_pyproject_config
 from qgis_plugin_dev_tools.utils.distributions import get_distribution_requirements
 
@@ -35,33 +34,35 @@
     DISTRIBUTION = auto()
 
     @staticmethod
     def from_config_value(config_value: str) -> "VersionNumberSource":
         try:
             return VersionNumberSource[config_value.upper()]
         except KeyError:
-            raise ValueError(f"{config_value=} is not a valid value")
+            raise ValueError(f"{config_value=} is not a valid value") from None
 
 
 class DevToolsConfig:
     plugin_package_name: str
     plugin_package_path: Path
-    runtime_distributions: List[Distribution]
+    runtime_distributions: list[Distribution]
     changelog_file_path: Path
     append_distributions_to_path: bool
     version_number_source: VersionNumberSource
+    disabled_extra_plugins: list[str]
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         plugin_package_name: str,
-        runtime_requires: List[str],
+        runtime_requires: list[str],
         changelog_file_path: Path,
         append_distributions_to_path: bool,
         auto_add_recursive_runtime_dependencies: bool,
-        version_number_source: VersionNumberSource = VersionNumberSource.CHANGELOG,
+        version_number_source: VersionNumberSource,
+        disabled_extra_plugins: list[str],
     ) -> None:
         plugin_package_spec = find_spec(plugin_package_name)
         if plugin_package_spec is None or plugin_package_spec.origin is None:
             raise ValueError(
                 f"could not find {plugin_package_name=} in the current environment"
             )
 
@@ -71,14 +72,15 @@
         self.runtime_distributions = [
             distribution(Requirement(spec).name) for spec in runtime_requires
         ]
         self.changelog_file_path = changelog_file_path
         self.append_distributions_to_path = append_distributions_to_path
         self.version_number_source = version_number_source
         self.extra_runtime_distributions = []
+        self.disabled_extra_plugins = disabled_extra_plugins
 
         if auto_add_recursive_runtime_dependencies:
             # Add the requirements of the distributions as well
             distributions_versions = {
                 dist.name: dist.version for dist in self.runtime_distributions
             }
             self.extra_runtime_distributions = [
@@ -105,8 +107,9 @@
             ),
             auto_add_recursive_runtime_dependencies=(
                 pyproject_config.auto_add_recursive_runtime_dependencies
             ),
             version_number_source=VersionNumberSource.from_config_value(
                 pyproject_config.version_number_source
             ),
+            disabled_extra_plugins=pyproject_config.disabled_extra_plugins,
         )
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/config/dotenv.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/config/dotenv.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,51 +15,51 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Optional
 
 from dotenv import dotenv_values
 
 LOGGER = logging.getLogger(__name__)
 
 
-class DotenvConfig:  # noqa SIM119
+class DotenvConfig:
     """
     Expected structure for the config keys in the .env.
     """
 
     QGIS_EXECUTABLE_PATH: Path
     DEBUGGER_LIBRARY: Optional[str]
     DEVELOPMENT_PROFILE_NAME: Optional[str]
-    runtime_environment: Dict[str, str]
+    runtime_environment: dict[str, str]
 
     def __init__(
         self,
         *,
-        QGIS_EXECUTABLE_PATH: str,  # noqa N803
-        DEBUGGER_LIBRARY: Optional[str] = None,  # noqa N803
-        DEVELOPMENT_PROFILE_NAME: Optional[str] = None,  # noqa N803
+        QGIS_EXECUTABLE_PATH: str,  # noqa: N803
+        DEBUGGER_LIBRARY: Optional[str] = None,  # noqa: N803
+        DEVELOPMENT_PROFILE_NAME: Optional[str] = None,  # noqa: N803
         **other_vars: str,
     ) -> None:
         self.QGIS_EXECUTABLE_PATH = Path(QGIS_EXECUTABLE_PATH)
         if not self.QGIS_EXECUTABLE_PATH.exists():
             raise ValueError(
                 f"QGIS executable {self.QGIS_EXECUTABLE_PATH.resolve()} does not exist."
             )
         self.DEBUGGER_LIBRARY = DEBUGGER_LIBRARY
         self.DEVELOPMENT_PROFILE_NAME = DEVELOPMENT_PROFILE_NAME
         self.runtime_environment = other_vars
 
 
-def read_dotenv_configs(dotenv_file_paths: List[Path]) -> DotenvConfig:
+def read_dotenv_configs(dotenv_file_paths: list[Path]) -> DotenvConfig:
     config = {}
     for dotenv_file_path in dotenv_file_paths:
         LOGGER.debug("reading config from %s", dotenv_file_path.resolve())
         config.update(dotenv_values(dotenv_file_path, verbose=False, encoding="utf-8"))
     try:
         return DotenvConfig(**{k: v for k, v in config.items() if v})
     except (KeyError, TypeError) as e:
-        raise ValueError(f"dev tools config invalid in .env: {e}")
+        raise ValueError(f"dev tools config invalid in .env: {e}") from e
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/config/pyproject.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/config/pyproject.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import List, Literal, Union
+from typing import Literal, Union
 
 import tomli
 
 LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
@@ -32,20 +32,21 @@
     """
     Expected structure for the config keys under the tool section.
     """
 
     DEV_TOOLS_SECTION_LOCATOR = "qgis_plugin_dev_tools"
 
     plugin_package_name: str
-    runtime_requires: List[str] = field(default_factory=list)
+    runtime_requires: list[str] = field(default_factory=list)
     use_dangerous_vendor_sys_path_append: bool = False
     auto_add_recursive_runtime_dependencies: bool = False
     version_number_source: Union[
         Literal["changelog"], Literal["distribution"]
     ] = "changelog"
+    disabled_extra_plugins: list[str] = field(default_factory=list)
 
     def __post_init__(self) -> None:
         if self.version_number_source not in ["changelog", "distribution"]:
             raise ValueError(
                 f"invalid value for version_number_source={self.version_number_source}"
             )
 
@@ -56,8 +57,8 @@
         config = tomli.load(pyproject_file)
         try:
             dev_tools_configuration = config.get("tool", {})[
                 PyprojectConfig.DEV_TOOLS_SECTION_LOCATOR
             ]
             return PyprojectConfig(**dev_tools_configuration)
         except (KeyError, TypeError) as e:
-            raise ValueError(f"dev tools config invalid in pyproject.toml: {e}")
+            raise ValueError(f"dev tools config invalid in pyproject.toml: {e}") from e
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/publish/__init__.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/publish/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # json rpc api spec in https://plugins.qgis.org/plugins/RPC2/
 
 import logging
 import os
 from base64 import b64encode
 from pathlib import Path
-from typing import Dict, Tuple, cast
+from typing import cast
 from uuid import uuid4
 
 import requests
 
 LOGGER = logging.getLogger(__name__)
 
+HTTP_STATUS_CODE_OK = 200
+
 
 def publish_plugin_zip_file(plugin_zip_file_path: Path) -> None:
     username = os.environ.get("QPDT_PUBLISH_USERNAME")
     password = os.environ.get("QPDT_PUBLISH_PASSWORD")
 
     if not username or not password:
         raise ValueError(
@@ -47,23 +49,23 @@
     )
 
     LOGGER.debug(
         "got response from plugin RPC api with body %s",
         response.text,
     )
 
-    if response.status_code != 200:
+    if response.status_code != HTTP_STATUS_CODE_OK:
         raise Exception(
             "QGIS plugin repository plugin upload "
             f"HTTP request failed with status {response.status_code}"
         )
     if "error" in response.json():
         raise Exception(
             "QGIS plugin repository plugin upload "
             f"request returned error response {response.json().get('error')}"
         )
 
-    plugin_id, version_id = cast(Dict[str, Tuple[int, int]], response.json()).get(
+    plugin_id, version_id = cast(dict[str, tuple[int, int]], response.json()).get(
         "result", (None, None)
     )
 
     LOGGER.info("uploaded plugin id %s & version id %s", plugin_id, version_id)
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/__init__.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,21 +28,19 @@
 
 
 def launch_development_qgis(
     development_mode_config: DevelopmentModeConfig,
 ) -> None:
     LOGGER.info("starting daemon server")
     with start_daemon_server() as (port, handle_single_request):
-
         LOGGER.info("creating a bootstrap file")
         with create_bootstrap_file(
             development_mode_config,
             port,
         ) as bootstrap_file_path:
-
             LOGGER.info("launching qgis")
             launch_qgis_with_bootstrap_script(
                 development_mode_config.qgis_executable_path,
                 bootstrap_file_path,
                 development_mode_config.profile_name,
             )
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/bootstrap/__init__.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/bootstrap/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 
 import dataclasses
 import logging
 import pickle
 import sys
+from collections.abc import Generator
 from contextlib import contextmanager
 from importlib import resources
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Generator
 
 from qgis_plugin_dev_tools.start.bootstrap.template import BootstrapConfig
 from qgis_plugin_dev_tools.start.config import DevelopmentModeConfig
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -40,18 +40,18 @@
     with TemporaryDirectory() as temp_dir:
         bootstrap_config = BootstrapConfig(
             daemon_socket_port=daemon_socket_port,
             runtime_library_paths=development_mode_configuration.runtime_library_paths,
             runtime_environment=development_mode_configuration.runtime_environment,
             plugin_package_path=development_mode_configuration.plugin_package_path,
             plugin_package_name=development_mode_configuration.plugin_package_name,
-            plugin_dependency_package_names=development_mode_configuration.plugin_dependency_package_names,  # noqa E501
+            plugin_dependency_package_names=development_mode_configuration.plugin_dependency_package_names,
             debugger_library=development_mode_configuration.debugger_library,
             bootstrap_python_executable_path=Path(sys.executable),
-            extra_plugin_package_names=development_mode_configuration.extra_plugin_package_names,  # noqa E501
+            extra_plugin_package_names=development_mode_configuration.extra_plugin_package_names,
         )
 
         LOGGER.debug("using bootstrap config:\n%s", bootstrap_config)
 
         bootstrap_template_contents = resources.read_text(
             __name__, "template.py", encoding="utf-8"
         ).replace(
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/bootstrap/template.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/bootstrap/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,93 +22,91 @@
 import functools
 import os
 import pickle
 import sys
 from dataclasses import asdict, dataclass
 from importlib.util import find_spec
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Optional
 
 # defer qgis.* imports until necessary to avoid loading those
 # for the interpreter that launches the bootstrapping, since it
 # will import the config class from this module
 
 
-def _unload_package_modules(package_names: List[str]) -> None:
+def _unload_package_modules(package_names: list[str]) -> None:
     to_clean_names = [
         module_name
         for module_name in sys.modules
         if any(
             module_name == package_name or module_name.startswith(f"{package_name}.")
             for package_name in package_names
         )
     ]
     for module_name in to_clean_names:
-        try:  # noqa SIM105
+        try:
             if hasattr(sys.modules[module_name], "qCleanupResources"):
                 sys.modules[module_name].qCleanupResources()
-        except Exception:  # noqa PIE786
+        except Exception:
             pass
-        try:  # noqa SIM105
+        with contextlib.suppress(Exception):
             del sys.modules[module_name]
-        except Exception:  # noqa PIE786
-            pass
 
 
 def _monkeypatch_plugin_module_unload_to_unload_dependencies(
-    plugin_package_name: str, plugin_dependency_package_names: List[str]
+    plugin_package_name: str, plugin_dependency_package_names: list[str]
 ) -> None:
     from qgis.core import Qgis, QgsMessageLog
 
     if len(plugin_dependency_package_names) > 0:
         QgsMessageLog.logMessage(
             f"patching plugin {plugin_package_name} unload "
             f"to unload dependencies {plugin_dependency_package_names} also",
             "Bootstrap",
             level=Qgis.Info,
         )
 
-        from qgis.utils import (  # noqa N813 (qgis naming)
+        from qgis.utils import (  # (qgis naming)
             _unloadPluginModules as _original_unload,
         )
 
         unload_plugin_dependency_modules = functools.partial(
             _unload_package_modules, plugin_dependency_package_names
         )
 
-        def _custom_unload(packageName: str) -> bool:  # noqa N803 (qgis naming)
+        def _custom_unload(packageName: str) -> bool:  # noqa: N803 (qgis naming)
             original_return = _original_unload(packageName)
             if packageName == plugin_package_name:
                 unload_plugin_dependency_modules()
             return original_return
 
         import qgis.utils as qgis_utils_module
 
         qgis_utils_module._unloadPluginModules = _custom_unload
 
 
 def _monkeypatch_plugin_reload_to_reload_extra_plugins(
-    main_plugin_package_name: str, extra_plugin_package_names: List[str]
+    main_plugin_package_name: str, extra_plugin_package_names: list[str]
 ) -> None:
     from qgis.core import Qgis, QgsMessageLog
-    from qgis.utils import loadPlugin as _original_load  # noqa N813 (qgis naming)
+    from qgis.utils import loadPlugin as _original_load  # noqa: N813 (qgis naming)
     from qgis.utils import startPlugin
-    from qgis.utils import unloadPlugin as _original_unload  # noqa N813 (qgis naming)
+    from qgis.utils import unloadPlugin as _original_unload  # noqa: N813 (qgis naming)
 
-    def _custom_unload(packageName: str) -> bool:  # noqa N803 (qgis naming)
+    def _custom_unload(packageName: str) -> bool:  # noqa: N803 (qgis naming)
         original_return = _original_unload(packageName)
 
         if packageName == main_plugin_package_name:
             for plugin_package_name in extra_plugin_package_names:
                 with contextlib.suppress(Exception):
                     _original_unload(plugin_package_name)
 
         return original_return
 
-    def _custom_load(packageName: str) -> bool:  # noqa N803 (qgis naming)
+    def _custom_load(packageName: str) -> bool:  # noqa: N803 (qgis naming)
         if packageName == main_plugin_package_name:
             for plugin_package_name in extra_plugin_package_names:
                 with contextlib.suppress(Exception):
                     _original_load(plugin_package_name)
                     startPlugin(plugin_package_name)
                     QgsMessageLog.logMessage(
                         f"activating {plugin_package_name} plugin",
@@ -120,32 +118,32 @@
 
     import qgis.utils as qgis_utils_module
 
     qgis_utils_module.unloadPlugin = _custom_unload
     qgis_utils_module.loadPlugin = _custom_load
 
 
-def _setup_runtime_library_paths(runtime_library_paths: List[Path]) -> None:
+def _setup_runtime_library_paths(runtime_library_paths: list[Path]) -> None:
     from qgis.core import Qgis, QgsMessageLog
 
     QgsMessageLog.logMessage(
         "setting dev env package paths", "Bootstrap", level=Qgis.Info
     )
     sys.path.extend(str(p) for p in runtime_library_paths)
 
 
-def _setup_runtime_environment(runtime_environment: Dict[str, str]) -> None:
+def _setup_runtime_environment(runtime_environment: dict[str, str]) -> None:
     from qgis.core import Qgis, QgsMessageLog
 
     QgsMessageLog.logMessage("setting dev env variables", "Bootstrap", level=Qgis.Info)
     os.environ.update(runtime_environment)
 
 
 def _enable_extra_plugins(
-    main_plugin_package_name: str, extra_plugin_package_names: List[str]
+    main_plugin_package_name: str, extra_plugin_package_names: list[str]
 ) -> None:
     from qgis.PyQt.QtCore import QSettings
     from qgis.utils import plugin_paths, unloadPlugin
 
     for plugin_package_name in extra_plugin_package_names:
         spec = find_spec(plugin_package_name)
         if spec is not None and spec.origin is not None:
@@ -158,15 +156,15 @@
         main_plugin_package_name, extra_plugin_package_names
     )
 
 
 def _enable_plugin(
     plugin_package_name: str,
     plugin_package_path: Path,
-    plugin_dependency_package_names: List[str],
+    plugin_dependency_package_names: list[str],
 ) -> None:
     from pyplugin_installer.installer_data import plugins as installer_plugins
     from qgis.core import Qgis, QgsMessageLog
     from qgis.PyQt.QtCore import QSettings
     from qgis.utils import (
         loadPlugin,
         plugin_paths,
@@ -236,32 +234,32 @@
 
 
 def _start_debugger(library_name: Optional[str], python_executable_path: Path) -> None:
     from qgis.core import Qgis, QgsMessageLog
 
     try:
         if library_name == "debugpy":
-            import debugpy  # noqa SC200
+            import debugpy  # noqa: SC200
 
             # at least on windows qgis resets the env and sys.executable points
             # to the qgis executable, hold on to the original python to use here
-            debugpy.configure(python=str(python_executable_path))  # noqa SC200
-            debugpy.listen(("localhost", 5678))  # noqa SC200
+            debugpy.configure(python=str(python_executable_path))  # noqa: SC200
+            debugpy.listen(("localhost", 5678))  # noqa: SC200
 
         elif library_name == "pydevd":
-            import pydevd  # noqa SC200
+            import pydevd  # noqa: SC200
 
-            pydevd.settrace(  # noqa SC200
+            pydevd.settrace(  # noqa: SC200
                 "localhost", port=5678, stdoutToServer=True, stderrToServer=True
             )
 
         else:
             return
 
-    except Exception as e:  # noqa PIE786
+    except Exception as e:
         QgsMessageLog.logMessage(
             f"failed to start {library_name} debugger: {e}",
             "Bootstrap",
             level=Qgis.Info,
         )
     else:
         QgsMessageLog.logMessage(
@@ -270,22 +268,22 @@
             level=Qgis.Info,
         )
 
 
 @dataclass
 class BootstrapConfig:
     daemon_socket_port: int
-    runtime_library_paths: List[Path]
-    runtime_environment: Dict[str, str]
+    runtime_library_paths: list[Path]
+    runtime_environment: dict[str, str]
     plugin_package_path: Path
     plugin_package_name: str
-    plugin_dependency_package_names: List[str]
+    plugin_dependency_package_names: list[str]
     debugger_library: Optional[str]
     bootstrap_python_executable_path: Path
-    extra_plugin_package_names: List[str]
+    extra_plugin_package_names: list[str]
 
     def __str__(self) -> str:
         result = ""
         for k, v in asdict(self).items():
             if isinstance(v, list):
                 result += f"  {k}=\n    " + "\n    ".join(map(str, v)) + "\n"
             else:
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/config.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Optional
 
 
 @dataclass
 class DevelopmentModeConfig:
     qgis_executable_path: Path
     profile_name: Optional[str]
-    runtime_environment: Dict[str, str]
-    runtime_library_paths: List[Path]
+    runtime_environment: dict[str, str]
+    runtime_library_paths: list[Path]
     plugin_package_path: Path
     plugin_package_name: str
-    plugin_dependency_package_names: List[str]
+    plugin_dependency_package_names: list[str]
     debugger_library: Optional[str]
-    extra_plugin_package_names: List[str]
+    extra_plugin_package_names: list[str]
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/daemon_server.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/daemon_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 #  useful, but WITHOUT ANY WARRANTY; without even the implied warranty
 #  of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 
+from collections.abc import Generator
 from contextlib import contextmanager
 from socketserver import BaseRequestHandler, TCPServer
-from typing import Callable, Generator, Tuple
+from typing import Callable
 
 DAEMON_SERVER_TIMEOUT = 60
 
 
 class SingleRequestHandlingTCPServer(TCPServer):
     timeout = DAEMON_SERVER_TIMEOUT
     is_timeout = False
 
     def handle_timeout(self) -> None:
         self.is_timeout = True
         return super().handle_timeout()
 
 
 @contextmanager
-def start_daemon_server() -> Generator[Tuple[int, Callable[[], bool]], None, None]:
+def start_daemon_server() -> Generator[tuple[int, Callable[[], bool]], None, None]:
     # TODO: add hot reload instead of closing the daemon?
     # watcher = QFileSystemWatcher([str(p) for p in Path(plugin_path).rglob('*.py')])
     # watcher.fileChanged.connect(send_something_to_socket)
 
     with SingleRequestHandlingTCPServer(("localhost", 0), BaseRequestHandler) as server:
         _, port = server.server_address
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/start/launch.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/start/launch.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools/utils/distributions.py` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools/utils/distributions.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,48 +15,70 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with qgis-plugin-dev-tools. If not, see <https://www.gnu.org/licenses/>.
 import importlib.util
 import logging
 from importlib.machinery import SourceFileLoader
-from typing import Dict, List, Optional, cast
+from typing import Optional, cast
 
 import importlib_metadata
 from importlib_metadata import Distribution, distribution
 from packaging.requirements import Requirement
 
 LOGGER = logging.getLogger(__name__)
 
 
-def get_distribution_top_level_package_names(dist: Distribution) -> List[str]:
-    return (dist.read_text("top_level.txt") or "").split()
+def get_distribution_top_level_names(dist: Distribution) -> set[str]:
+    if (file_paths := dist.files) is None:
+        LOGGER.warning("could not resolve %s top level names", dist.name)
+        return set()
+
+    return {
+        top_level_directory_name
+        for path in file_paths
+        if (
+            len(path.parts) > 1
+            and not (top_level_directory_name := path.parts[0]).endswith(
+                (".dist-info", ".egg-info")
+            )
+            and top_level_directory_name not in ("..", "__pycache__")
+        )
+    } | {
+        path.stem
+        for path in file_paths
+        if len(path.parts) == 1 and path.suffix in (".py", ".pyd")
+    }
+
 
+def get_distribution_requirements(dist: Distribution) -> dict[str, Distribution]:
+    requirement_distributions: dict[str, Distribution] = {}
 
-def get_distribution_requirements(dist: Distribution) -> Dict[str, Distribution]:
     requirements = [
         Requirement(requirement.split(" ")[0])
         for requirement in dist.requires or []
         if "extra ==" not in requirement
     ]
-    distributions = {}
     for requirement in requirements:
         try:
-            distributions[requirement.name] = distribution(requirement.name)
+            requirement_distributions[requirement.name] = distribution(requirement.name)
         except importlib_metadata.PackageNotFoundError:
             LOGGER.warning(
                 "Getting distribution for %s failed. "
                 "This may be caused by including builtin "
                 "packages as requirements.",
                 requirement.name,
             )
             spec = importlib.util.find_spec(requirement.name)
             loader = cast(Optional[SourceFileLoader], spec.loader) if spec else None
             if spec and loader and loader.is_package(requirement.name):
                 LOGGER.error("Could not find package %s", requirement.name)
             continue
 
-    sub_requirements = {}
-    for requirement in distributions.values():
-        sub_requirements.update(get_distribution_requirements(requirement))
-    distributions.update(sub_requirements)
-    return distributions
+    nested_requirement_distributions: dict[str, Distribution] = {}
+    for requirement_distribution in requirement_distributions.values():
+        nested_requirement_distributions.update(
+            get_distribution_requirements(requirement_distribution)
+        )
+    requirement_distributions.update(nested_requirement_distributions)
+
+    return requirement_distributions
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/PKG-INFO` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-dev-tools
-Version: 0.6.2
+Version: 0.7.0
 Summary: QGIS plugin development and packaging tools, which make managing runtime dependencies easy.
 Home-page: https://github.com/nlsfi/qgis-plugin-dev-tools
 Author: National Land Survey of Finland
 Author-email: os@nls.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/qgis-plugin-dev-tools/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -131,14 +131,23 @@
 * Extra plugin must have entry point in group "qgis_plugin_dev_tools"
   * See for example: [Entry point usage with setuptools]
   * Use plugin package name for entry point name
 * Extra plugin needs to be installed in the same python environment where this tool is run in
 
 Extra plugins are loaded on launch and reloaded together with the main plugin if [Plugin Reloader] is used.
 
+You can disable plugin auto-load by using `pyproject.toml` configuration (for example when using a dependency, that also provides a plugin entrypoint):
+
+```toml
+[tool.qgis_plugin_dev_tools]
+disabled_extra_plugins = [
+  "unwanted_plugin_package_name",
+]
+```
+
 ## Development of qgis-plugin-dev-tools
 
 See [development readme](./DEVELOPMENT.md).
 
 ## License & copyright
 
 Licensed under GNU GPL v3.0.
@@ -152,14 +161,19 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.0] - 2024-05-21
+
+- Fix: Bundle contents by parsing pep-compliant distribution file catalog instead of possibly missing tool-specific top-level.txt
+- Feat: Allow disabling auto-loaded entrypoint plugins
+
 ## [0.6.2] - 2023-09-27
 
 - Fix: Fix issues with bundling requirements of the requirements recursively
 
 ## [0.6.1] - 2023-09-06
 
 - update author email
@@ -214,7 +228,8 @@
 [0.2.1]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.2.1
 [0.3.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.3.0
 [0.4.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.4.0
 [0.5.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.5.0
 [0.6.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.0
 [0.6.1]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.1
 [0.6.2]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.6.2
+[0.7.0]: https://github.com/nlsfi/qgis-plugin-dev-tools/releases/tag/v0.7.0
```

### Comparing `qgis-plugin-dev-tools-0.6.2/src/qgis_plugin_dev_tools.egg-info/SOURCES.txt` & `qgis_plugin_dev_tools-0.7.0/src/qgis_plugin_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qgis-plugin-dev-tools-0.6.2/test/test_build.py` & `qgis_plugin_dev_tools-0.7.0/test/test_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import os
 import sys
 import textwrap
 import zipfile
 from pathlib import Path
-from typing import TYPE_CHECKING, Set
 
 import pytest
-
 from qgis_plugin_dev_tools.build import make_plugin_zip
-
-if TYPE_CHECKING:
-    from qgis_plugin_dev_tools.config import DevToolsConfig
+from qgis_plugin_dev_tools.config import DevToolsConfig, VersionNumberSource
 
 
 @pytest.fixture()
 def plugin_dir(tmp_path: Path) -> Path:
     plugin_dir = tmp_path / "Plugin"
     plugin_dir.mkdir()
 
@@ -56,54 +52,60 @@
     os.chdir(tmp_path.resolve())
     sys.path.append(tmp_path.resolve().as_posix())
 
     return plugin_dir
 
 
 @pytest.fixture()
-def dev_tools_config(plugin_dir: Path):
+def dev_tools_config(plugin_dir: Path) -> DevToolsConfig:
     from qgis_plugin_dev_tools.config import DevToolsConfig
 
     return DevToolsConfig(
         plugin_package_name="Plugin",
         runtime_requires=["pytest"],
         changelog_file_path=plugin_dir / "CHANGELOG.md",
         append_distributions_to_path=True,
         auto_add_recursive_runtime_dependencies=True,
+        version_number_source=VersionNumberSource.CHANGELOG,
+        disabled_extra_plugins=[],
     )
 
 
 @pytest.fixture()
-def dev_tools_config_with_duplicate_dependencies(plugin_dir: Path):
+def dev_tools_config_with_duplicate_dependencies(plugin_dir: Path) -> DevToolsConfig:
     from qgis_plugin_dev_tools.config import DevToolsConfig
 
     return DevToolsConfig(
         plugin_package_name="Plugin",
         runtime_requires=["pytest-cov"],
         changelog_file_path=plugin_dir / "CHANGELOG.md",
         append_distributions_to_path=True,
         auto_add_recursive_runtime_dependencies=True,
+        version_number_source=VersionNumberSource.CHANGELOG,
+        disabled_extra_plugins=[],
     )
 
 
 @pytest.fixture()
-def dev_tools_config_minimal(plugin_dir: Path):
+def dev_tools_config_minimal(plugin_dir: Path) -> DevToolsConfig:
     # No python path append and not recursive deps
     from qgis_plugin_dev_tools.config import DevToolsConfig
 
     return DevToolsConfig(
         plugin_package_name="Plugin",
         runtime_requires=["pytest"],
         changelog_file_path=plugin_dir / "CHANGELOG.md",
         append_distributions_to_path=False,
         auto_add_recursive_runtime_dependencies=False,
+        version_number_source=VersionNumberSource.CHANGELOG,
+        disabled_extra_plugins=[],
     )
 
 
-def test_make_zip(dev_tools_config: "DevToolsConfig", plugin_dir: Path, tmp_path: Path):
+def test_make_zip(dev_tools_config: "DevToolsConfig", tmp_path: Path):
     target_path = tmp_path / "dist"
     expected_zip = target_path / "Plugin-0.1.0.zip"
 
     make_plugin_zip(dev_tools_config, target_path)
 
     assert target_path.exists()
     assert expected_zip.exists()
@@ -127,33 +129,32 @@
         "colorama",
         "colorama-0.4.4.dist-info",
         "importlib_metadata",
         "importlib_metadata-4.11.3.dist-info",
         "iniconfig",
         "iniconfig-1.1.1.dist-info",
         "packaging",
-        "packaging-21.3.dist-info",
+        "packaging-23.2.dist-info",
         "pluggy",
         "pluggy-1.0.0.dist-info",
         "py",
         "py-1.11.0.dist-info",
-        "pyparsing-3.0.8.dist-info",
         "pytest",
         "pytest-6.2.5.dist-info",
         "toml",
         "toml-0.10.2.dist-info",
         "typing_extensions-4.2.0.dist-info",
+        "typing_extensions.py",  # no top-level.txt in .dist-info, parsed from record
         "zipp-3.8.0.dist-info",
-        "zipp.py",
+        "zipp.py",  # top-level.txt in .dist-info, includes zipp
     }
 
 
 def test_make_zip_with_duplicate_dependencies(
     dev_tools_config_with_duplicate_dependencies: "DevToolsConfig",
-    plugin_dir: Path,
     tmp_path: Path,
 ):
     target_path = tmp_path / "dist"
     expected_zip = target_path / "Plugin-0.1.0.zip"
 
     make_plugin_zip(dev_tools_config_with_duplicate_dependencies, target_path)
 
@@ -181,34 +182,34 @@
         "coverage",
         "coverage-6.3.2.dist-info",
         "importlib_metadata",
         "importlib_metadata-4.11.3.dist-info",
         "iniconfig",
         "iniconfig-1.1.1.dist-info",
         "packaging",
-        "packaging-21.3.dist-info",
+        "packaging-23.2.dist-info",
         "pluggy",
         "pluggy-1.0.0.dist-info",
         "py",
         "py-1.11.0.dist-info",
-        "pyparsing-3.0.8.dist-info",
         "pytest",
         "pytest-6.2.5.dist-info",
         "pytest_cov",
         "pytest_cov-2.12.0.dist-info",
         "toml",
         "toml-0.10.2.dist-info",
         "typing_extensions-4.2.0.dist-info",
+        "typing_extensions.py",  # no top-level.txt in .dist-info, parsed from record
         "zipp-3.8.0.dist-info",
-        "zipp.py",
+        "zipp.py",  # top-level.txt in .dist-info, includes zipp
     }
 
 
 def test_make_zip_with_minimal_config(
-    dev_tools_config_minimal: "DevToolsConfig", plugin_dir: Path, tmp_path: Path
+    dev_tools_config_minimal: "DevToolsConfig", tmp_path: Path
 ):
     target_path = tmp_path / "dist"
     expected_zip = target_path / "Plugin-test-version.zip"
 
     make_plugin_zip(
         dev_tools_config_minimal, target_path, override_plugin_version="test-version"
     )
@@ -228,15 +229,15 @@
         "__init__.py",
         "_pytest",
         "pytest",
         "pytest-6.2.5.dist-info",
     }
 
 
-def _get_file_names(zip_file: Path, prefix: str) -> Set[str]:
+def _get_file_names(zip_file: Path, prefix: str) -> set[str]:
     with zipfile.ZipFile(zip_file) as z:
         namelist = z.namelist()
         return {
             name.replace(prefix, "").split("/")[0]
             for name in namelist
             if name.startswith(prefix) and name != prefix
         }
```

### Comparing `qgis-plugin-dev-tools-0.6.2/test/test_read_distributions.py` & `qgis_plugin_dev_tools-0.7.0/test/test_read_distributions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+from typing import Any
+
 import pytest
 from importlib_metadata import distribution
 from packaging.requirements import Requirement
-
 from qgis_plugin_dev_tools.utils.distributions import get_distribution_requirements
 
 
 @pytest.fixture()
-def sample_dist():
+def sample_dist() -> Any:
     return distribution(Requirement("pytest").name)
 
 
-def test_get_distribution_requirements(sample_dist):
+def test_get_distribution_requirements(sample_dist: Any):
     requirements = get_distribution_requirements(sample_dist)
     assert sorted(requirements.keys()) == [
         "atomicwrites",
         "attrs",
         "colorama",
         "importlib-metadata",
         "iniconfig",
         "packaging",
         "pluggy",
         "py",
-        "pyparsing",
         "toml",
         "typing-extensions",
         "zipp",
     ]
```

### Comparing `qgis-plugin-dev-tools-0.6.2/test/test_read_dotenv.py` & `qgis_plugin_dev_tools-0.7.0/test/test_read_dotenv.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 import sys
-from typing import List
+from pathlib import Path
+from typing import Callable
 
 import pytest
-
 from qgis_plugin_dev_tools.config.dotenv import read_dotenv_configs
 
 
 @pytest.fixture()
-def create_dotenv_with_contents(tmp_path_factory):
-    def write_contents_from_list(contents: List[str]):
+def create_dotenv_with_contents(
+    tmp_path_factory,  # noqa: ANN001
+) -> Callable[[list[str]], Path]:
+    def write_contents_from_list(contents: list[str]) -> Path:
         dotenv_file_path = tmp_path_factory.mktemp(basename="env") / ".env"
         dotenv_file_path.write_text("\n".join(contents), encoding="utf-8")
         return dotenv_file_path
 
     return write_contents_from_list
 
 
-def test_executable_must_be_given(create_dotenv_with_contents):
+def test_executable_must_be_given(
+    create_dotenv_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_dotenv_with_contents(["QGIS_EXECUTABLE_PATH="])
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="QGIS_EXECUTABLE_PATH"):
         read_dotenv_configs([test_file])
 
 
-def test_executable_must_exist(create_dotenv_with_contents):
+def test_executable_must_exist(
+    create_dotenv_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_dotenv_with_contents(
         ["QGIS_EXECUTABLE_PATH=some-missing-binary"]
     )
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="some-missing-binary"):
         read_dotenv_configs([test_file])
 
 
-def test_optionals_can_be_missing(create_dotenv_with_contents):
+def test_optionals_can_be_missing(
+    create_dotenv_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_dotenv_with_contents([f"QGIS_EXECUTABLE_PATH={sys.executable}"])
 
     result = read_dotenv_configs([test_file])
     assert result.DEVELOPMENT_PROFILE_NAME is None
     assert result.DEBUGGER_LIBRARY is None
 
 
-def test_other_vars_saved_as_runtime_env(create_dotenv_with_contents):
+def test_other_vars_saved_as_runtime_env(
+    create_dotenv_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_dotenv_with_contents(
         [
             f"QGIS_EXECUTABLE_PATH={sys.executable}",
             "DEBUGGER_LIBRARY=something",
             "SOME_UNKNOWN_VAR=thing",
             "OTHER_UNKNOWN=1",
         ]
@@ -53,29 +63,33 @@
     result = read_dotenv_configs([test_file])
     assert result.runtime_environment == {
         "SOME_UNKNOWN_VAR": "thing",
         "OTHER_UNKNOWN": "1",
     }
 
 
-def test_empty_vars_not_saved_in_runtime_env(create_dotenv_with_contents):
+def test_empty_vars_not_saved_in_runtime_env(
+    create_dotenv_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_dotenv_with_contents(
         [
             f"QGIS_EXECUTABLE_PATH={sys.executable}",
             "DEBUGGER_LIBRARY=something",
             "SOME_UNKNOWN_VAR=thing",
             "OTHER_UNKNOWN=",
         ]
     )
 
     result = read_dotenv_configs([test_file])
     assert result.runtime_environment == {"SOME_UNKNOWN_VAR": "thing"}
 
 
-def test_multiple_files_last_overrides(create_dotenv_with_contents):
+def test_multiple_files_last_overrides(
+    create_dotenv_with_contents: Callable[[list[str]], Path]
+):
     test_file_1 = create_dotenv_with_contents(
         [
             f"QGIS_EXECUTABLE_PATH={sys.executable}",
             "DEBUGGER_LIBRARY=something",
             "SOMETHING=thing",
             "FIRST_ONLY=1",
         ]
```

### Comparing `qgis-plugin-dev-tools-0.6.2/test/test_read_pyproject.py` & `qgis_plugin_dev_tools-0.7.0/test/test_read_pyproject.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,86 @@
 from pathlib import Path
-from typing import List
+from typing import Callable
 
 import pytest
-
 from qgis_plugin_dev_tools.config.pyproject import read_pyproject_config
 
 
 @pytest.fixture()
-def create_pyproject_toml_with_contents(tmpdir):
+def create_pyproject_toml_with_contents(tmpdir: str) -> Callable[[list[str]], Path]:
     toml_file_path = Path(tmpdir) / "test.toml"
 
-    def write_contents_from_list(contents: List[str]):
+    def write_contents_from_list(contents: list[str]) -> Path:
         toml_file_path.write_text("\n".join(contents), encoding="utf-8")
         return toml_file_path
 
     return write_contents_from_list
 
 
-def test_section_missing_fails(create_pyproject_toml_with_contents):
+def test_section_missing_fails(
+    create_pyproject_toml_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_pyproject_toml_with_contents(
         [
             "[tool.not_the_expected_name]",
             'plugin_package_name = "testing"',
         ]
     )
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="config invalid"):
         read_pyproject_config(test_file)
 
 
-def test_package_name_missing_fails(create_pyproject_toml_with_contents):
+def test_package_name_missing_fails(
+    create_pyproject_toml_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_pyproject_toml_with_contents(
         [
             "[tool.qgis_plugin_dev_tools]",
             'not_the_package_name_key = "testing"',
         ]
     )
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="not_the_package_name_key"):
         read_pyproject_config(test_file)
 
 
-def test_requires_allowed_missing(create_pyproject_toml_with_contents):
+def test_requires_allowed_missing(
+    create_pyproject_toml_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_pyproject_toml_with_contents(
         [
             "[tool.qgis_plugin_dev_tools]",
             'plugin_package_name = "testing"',
         ]
     )
 
     assert read_pyproject_config(test_file).runtime_requires == []
 
 
-def test_requires_allowed_empty(create_pyproject_toml_with_contents):
+def test_requires_allowed_empty(
+    create_pyproject_toml_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_pyproject_toml_with_contents(
         [
             "[tool.qgis_plugin_dev_tools]",
             'plugin_package_name = "testing"',
             "runtime_requires = []",
         ]
     )
 
     result = read_pyproject_config(test_file)
     assert result.runtime_requires == []
     assert not result.use_dangerous_vendor_sys_path_append
     assert not result.auto_add_recursive_runtime_dependencies
 
 
-def test_section_read_to_dataclass(create_pyproject_toml_with_contents):
+def test_section_read_to_dataclass(
+    create_pyproject_toml_with_contents: Callable[[list[str]], Path]
+):
     test_file = create_pyproject_toml_with_contents(
         [
             "[tool.qgis_plugin_dev_tools]",
             'plugin_package_name = "testing"',
             'runtime_requires = ["one", "another"]',
             "use_dangerous_vendor_sys_path_append = true",
             "auto_add_recursive_runtime_dependencies = true",
```

### Comparing `qgis-plugin-dev-tools-0.6.2/test/test_rewrite_imports.py` & `qgis_plugin_dev_tools-0.7.0/test/test_rewrite_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from pathlib import Path
-from typing import List
 from xml.etree import ElementTree
 
 from qgis_plugin_dev_tools.build.rewrite_imports import rewrite_imports_in_source_file
 
 
-def _trim_first_line_comment(lines: List[str]) -> List[str]:
+def _trim_first_line_comment(lines: list[str]) -> list[str]:
     if lines[0].startswith("#"):
         return lines[1:]
     return lines
 
 
 def test_from_x_import_matching_name_not_rewritten(tmp_path: Path):
-
     file = tmp_path / "mock.py"
 
     file.write_text(
         """
     from something import xyz as xyz_alias
     from something import xyz
     """
@@ -92,15 +90,14 @@
     a = 123; import xyz_f; b = 456
     \timport xyz_g
     """.splitlines()
     )
 
 
 def test_ui_file_custom_widget_imports_are_replaced(tmp_path: Path):
-
     file = tmp_path / "mock.ui"
 
     file.write_text(
         """<?xml version="1.0" encoding="UTF-8"?>
     <ui version="4.0">
       <customwidget>
         <class>CustomTreeView</class>
```

