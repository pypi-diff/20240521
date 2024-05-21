# Comparing `tmp/dzidb-1.0.8.tar.gz` & `tmp/dzidb-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dzidb-1.0.8.tar", last modified: Tue May 21 10:06:17 2024, max compression
+gzip compressed data, was "dzidb-1.1.tar", last modified: Tue May 21 07:45:01 2024, max compression
```

## Comparing `dzidb-1.0.8.tar` & `dzidb-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 10:06:17.250493 dzidb-1.0.8/
--rw-rw-rw-   0        0        0     1088 2024-05-20 06:49:44.000000 dzidb-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      208 2024-05-21 10:06:17.250493 dzidb-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-20 06:49:44.000000 dzidb-1.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-21 10:06:17.249495 dzidb-1.0.8/dzidb.egg-info/
--rw-rw-rw-   0        0        0      208 2024-05-21 10:06:17.000000 dzidb-1.0.8/dzidb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-05-21 10:06:17.000000 dzidb-1.0.8/dzidb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 10:06:17.000000 dzidb-1.0.8/dzidb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 10:06:17.000000 dzidb-1.0.8/dzidb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 10:06:17.000000 dzidb-1.0.8/dzidb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-21 10:06:17.255498 dzidb-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      348 2024-05-21 10:06:13.000000 dzidb-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:45:01.650020 dzidb-1.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-20 06:49:44.000000 dzidb-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      206 2024-05-21 07:45:01.650020 dzidb-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-05-20 06:49:44.000000 dzidb-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-21 07:45:01.648025 dzidb-1.1/dzidb.egg-info/
+-rw-rw-rw-   0        0        0      206 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3245 2024-05-21 07:23:52.000000 dzidb-1.1/dzidb.py
+-rw-rw-rw-   0        0        0       85 2024-05-21 07:45:01.651016 dzidb-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      346 2024-05-21 07:39:01.000000 dzidb-1.1/setup.py
```

### Comparing `dzidb-1.0.8/LICENSE.txt` & `dzidb-1.1/LICENSE.txt`

 * *Files identical despite different names*

