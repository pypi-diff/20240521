# Comparing `tmp/dzidb-1.0.tar.gz` & `tmp/dzidb-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dzidb-1.0.tar", last modified: Mon May 20 05:47:58 2024, max compression
+gzip compressed data, was "dzidb-1.1.tar", last modified: Tue May 21 07:45:01 2024, max compression
```

## Comparing `dzidb-1.0.tar` & `dzidb-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 05:47:58.990791 dzidb-1.0/
--rw-rw-rw-   0        0        0     1088 2024-05-20 05:14:45.000000 dzidb-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      107 2024-05-20 05:47:58.990791 dzidb-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-20 05:07:39.000000 dzidb-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-20 05:47:58.988820 dzidb-1.0/dzidb.egg-info/
--rw-rw-rw-   0        0        0      107 2024-05-20 05:47:58.000000 dzidb-1.0/dzidb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-20 05:47:58.000000 dzidb-1.0/dzidb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 05:47:58.000000 dzidb-1.0/dzidb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-20 05:47:58.000000 dzidb-1.0/dzidb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-05-20 05:47:58.000000 dzidb-1.0/dzidb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      395 2024-05-20 03:23:17.000000 dzidb-1.0/dzidb.py
--rw-rw-rw-   0        0        0       85 2024-05-20 05:47:58.992812 dzidb-1.0/setup.cfg
--rw-rw-rw-   0        0        0      346 2024-05-20 05:47:11.000000 dzidb-1.0/setup.py
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

### Comparing `dzidb-1.0/LICENSE.txt` & `dzidb-1.1/LICENSE.txt`

 * *Files identical despite different names*

