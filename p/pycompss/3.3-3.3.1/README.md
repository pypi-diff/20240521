# Comparing `tmp/pycompss-3.3.tar.gz` & `tmp/pycompss-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompss-3.3.tar", last modified: Thu Nov  9 08:36:38 2023, max compression
+gzip compressed data, was "pycompss-3.3.1.tar", last modified: Tue May 21 15:28:28 2024, max compression
```

## Comparing `pycompss-3.3.tar` & `pycompss-3.3.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-11-09 08:36:38.018161 pycompss-3.3/
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)    11406 2023-11-09 08:36:37.000000 pycompss-3.3/LICENSE.txt
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)      156 2023-11-09 08:36:37.000000 pycompss-3.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3709 2023-11-09 08:36:38.018161 pycompss-3.3/PKG-INFO
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     2044 2023-11-09 08:36:37.000000 pycompss-3.3/README.rst
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)        4 2023-11-09 08:36:37.000000 pycompss-3.3/VERSION.txt
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     9934 2023-11-09 08:36:37.000000 pycompss-3.3/backend.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-11-09 08:36:38.018161 pycompss-3.3/pycompss.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3709 2023-11-09 08:36:37.000000 pycompss-3.3/pycompss.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      241 2023-11-09 08:36:37.000000 pycompss-3.3/pycompss.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-11-09 08:36:37.000000 pycompss-3.3/pycompss.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       11 2023-11-09 08:36:37.000000 pycompss-3.3/pycompss.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-11-09 08:36:37.000000 pycompss-3.3/pycompss.egg-info/top_level.txt
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     1535 2023-11-09 08:36:37.000000 pycompss-3.3/pycompssenv
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       38 2023-11-09 08:36:38.018161 pycompss-3.3/setup.cfg
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     4917 2023-11-09 08:36:37.000000 pycompss-3.3/setup.py
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)       37 2023-11-09 08:36:37.000000 pycompss-3.3/url
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-05-21 15:28:28.241369 pycompss-3.3.1/
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)    11406 2024-05-21 15:28:19.000000 pycompss-3.3.1/LICENSE.txt
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)      136 2024-05-21 15:28:19.000000 pycompss-3.3.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    17212 2024-05-21 15:28:28.241369 pycompss-3.3.1/PKG-INFO
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     2044 2024-05-21 15:28:19.000000 pycompss-3.3.1/README.rst
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)        6 2024-05-21 15:28:19.000000 pycompss-3.3.1/VERSION.txt
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     1535 2024-05-21 15:28:19.000000 pycompss-3.3.1/pycompssenv
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     2845 2024-05-21 15:28:19.000000 pycompss-3.3.1/pyproject.toml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       38 2024-05-21 15:28:28.241369 pycompss-3.3.1/setup.cfg
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)    17039 2024-05-21 15:28:19.000000 pycompss-3.3.1/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-05-21 15:28:28.233369 pycompss-3.3.1/src/
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-05-21 15:28:28.237369 pycompss-3.3.1/src/pycompss/
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)      843 2024-05-21 15:28:19.000000 pycompss-3.3.1/src/pycompss/__init__.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-05-21 15:28:28.237369 pycompss-3.3.1/src/pycompss.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    17212 2024-05-21 15:28:28.000000 pycompss-3.3.1/src/pycompss.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      290 2024-05-21 15:28:28.000000 pycompss-3.3.1/src/pycompss.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2024-05-21 15:28:28.000000 pycompss-3.3.1/src/pycompss.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       31 2024-05-21 15:28:28.000000 pycompss-3.3.1/src/pycompss.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        9 2024-05-21 15:28:28.000000 pycompss-3.3.1/src/pycompss.egg-info/top_level.txt
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)       37 2024-05-21 15:28:19.000000 pycompss-3.3.1/url
```

### Comparing `pycompss-3.3/LICENSE.txt` & `pycompss-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycompss-3.3/README.rst` & `pycompss-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pycompss-3.3/pycompssenv` & `pycompss-3.3.1/pycompssenv`

 * *Files identical despite different names*

