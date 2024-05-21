# Comparing `tmp/jpegtran-0.0.1.tar.gz` & `tmp/jpegtran-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpegtran-0.0.1.tar", last modified: Tue May 21 06:52:25 2024, max compression
+gzip compressed data, was "jpegtran-0.0.2.tar", last modified: Tue May 21 06:57:04 2024, max compression
```

## Comparing `jpegtran-0.0.1.tar` & `jpegtran-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jw        (1000) jw        (1000)        0 2024-05-21 06:52:25.939360 jpegtran-0.0.1/
--rw-r--r--   0 jw        (1000) jw        (1000)     1065 2024-05-21 04:02:50.000000 jpegtran-0.0.1/LICENSE
--rw-r--r--   0 jw        (1000) jw        (1000)      501 2024-05-21 06:52:25.939360 jpegtran-0.0.1/PKG-INFO
--rw-r--r--   0 jw        (1000) jw        (1000)        0 2024-05-21 06:32:28.000000 jpegtran-0.0.1/README.md
--rw-r--r--   0 jw        (1000) jw        (1000)      500 2024-05-21 06:52:16.000000 jpegtran-0.0.1/pyproject.toml
--rw-r--r--   0 jw        (1000) jw        (1000)       38 2024-05-21 06:52:25.939360 jpegtran-0.0.1/setup.cfg
-drwxr-xr-x   0 jw        (1000) jw        (1000)        0 2024-05-21 06:52:25.939360 jpegtran-0.0.1/src/
-drwxr-xr-x   0 jw        (1000) jw        (1000)        0 2024-05-21 06:52:25.939360 jpegtran-0.0.1/src/jpeg/
--rw-r--r--   0 jw        (1000) jw        (1000)     4804 2024-05-21 06:40:39.000000 jpegtran-0.0.1/src/jpeg/__init__.py
-drwxr-xr-x   0 jw        (1000) jw        (1000)        0 2024-05-21 06:52:25.939360 jpegtran-0.0.1/src/jpegtran.egg-info/
--rw-r--r--   0 jw        (1000) jw        (1000)      501 2024-05-21 06:52:25.000000 jpegtran-0.0.1/src/jpegtran.egg-info/PKG-INFO
--rw-r--r--   0 jw        (1000) jw        (1000)      197 2024-05-21 06:52:25.000000 jpegtran-0.0.1/src/jpegtran.egg-info/SOURCES.txt
--rw-r--r--   0 jw        (1000) jw        (1000)        1 2024-05-21 06:52:25.000000 jpegtran-0.0.1/src/jpegtran.egg-info/dependency_links.txt
--rw-r--r--   0 jw        (1000) jw        (1000)        5 2024-05-21 06:52:25.000000 jpegtran-0.0.1/src/jpegtran.egg-info/top_level.txt
+drwxr-xr-x   0 jw        (1000) jw        (1000)        0 2024-05-21 06:57:04.958415 jpegtran-0.0.2/
+-rw-r--r--   0 jw        (1000) jw        (1000)     1065 2024-05-21 04:02:50.000000 jpegtran-0.0.2/LICENSE
+-rw-r--r--   0 jw        (1000) jw        (1000)      695 2024-05-21 06:57:04.958415 jpegtran-0.0.2/PKG-INFO
+-rw-r--r--   0 jw        (1000) jw        (1000)      208 2024-05-21 06:56:40.000000 jpegtran-0.0.2/README.md
+-rw-r--r--   0 jw        (1000) jw        (1000)      500 2024-05-21 06:56:52.000000 jpegtran-0.0.2/pyproject.toml
+-rw-r--r--   0 jw        (1000) jw        (1000)       38 2024-05-21 06:57:04.958415 jpegtran-0.0.2/setup.cfg
+drwxr-xr-x   0 jw        (1000) jw        (1000)        0 2024-05-21 06:57:04.958415 jpegtran-0.0.2/src/
+drwxr-xr-x   0 jw        (1000) jw        (1000)        0 2024-05-21 06:57:04.958415 jpegtran-0.0.2/src/jpeg/
+-rw-r--r--   0 jw        (1000) jw        (1000)     4804 2024-05-21 06:40:39.000000 jpegtran-0.0.2/src/jpeg/__init__.py
+drwxr-xr-x   0 jw        (1000) jw        (1000)        0 2024-05-21 06:57:04.958415 jpegtran-0.0.2/src/jpegtran.egg-info/
+-rw-r--r--   0 jw        (1000) jw        (1000)      695 2024-05-21 06:57:04.000000 jpegtran-0.0.2/src/jpegtran.egg-info/PKG-INFO
+-rw-r--r--   0 jw        (1000) jw        (1000)      197 2024-05-21 06:57:04.000000 jpegtran-0.0.2/src/jpegtran.egg-info/SOURCES.txt
+-rw-r--r--   0 jw        (1000) jw        (1000)        1 2024-05-21 06:57:04.000000 jpegtran-0.0.2/src/jpegtran.egg-info/dependency_links.txt
+-rw-r--r--   0 jw        (1000) jw        (1000)        5 2024-05-21 06:57:04.000000 jpegtran-0.0.2/src/jpegtran.egg-info/top_level.txt
```

### Comparing `jpegtran-0.0.1/LICENSE` & `jpegtran-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jpegtran-0.0.1/src/jpeg/__init__.py` & `jpegtran-0.0.2/src/jpeg/__init__.py`

 * *Files identical despite different names*

