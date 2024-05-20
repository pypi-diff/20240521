# Comparing `tmp/pih-rcgn-0.14.tar.gz` & `tmp/pih-rcgn-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-rcgn-0.14.tar", last modified: Wed Apr 10 02:27:02 2024, max compression
+gzip compressed data, was "pih-rcgn-0.15.tar", last modified: Mon May 20 23:13:02 2024, max compression
```

## Comparing `pih-rcgn-0.14.tar` & `pih-rcgn-0.15.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:27:02.482201 pih-rcgn-0.14/
--rw-rw-rw-   0        0        0      610 2024-04-10 02:27:02.450951 pih-rcgn-0.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:27:02.018833 pih-rcgn-0.14/RecognizeService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-rcgn-0.14/RecognizeService/__init__.py
--rw-rw-rw-   0        0        0      143 2024-02-15 01:35:08.000000 pih-rcgn-0.14/RecognizeService/__main__.py
--rw-rw-rw-   0        0        0    57769 2024-03-28 02:50:14.000000 pih-rcgn-0.14/RecognizeService/api.py
--rw-rw-rw-   0        0        0     1224 2024-02-09 14:42:12.000000 pih-rcgn-0.14/RecognizeService/collection.py
--rw-rw-rw-   0        0        0     4656 2024-04-10 02:26:25.000000 pih-rcgn-0.14/RecognizeService/const.py
--rw-rw-rw-   0        0        0    29045 2024-03-19 22:16:00.000000 pih-rcgn-0.14/RecognizeService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:27:02.416676 pih-rcgn-0.14/pih_rcgn.egg-info/
--rw-rw-rw-   0        0        0      610 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-10 02:27:01.000000 pih-rcgn-0.14/pih_rcgn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      137 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:27:02.482201 pih-rcgn-0.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:13:02.671859 pih-rcgn-0.15/
+-rw-rw-rw-   0        0        0      610 2024-05-20 23:13:02.640606 pih-rcgn-0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:13:01.945567 pih-rcgn-0.15/RecognizeService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-rcgn-0.15/RecognizeService/__init__.py
+-rw-rw-rw-   0        0        0      143 2024-02-15 01:35:08.000000 pih-rcgn-0.15/RecognizeService/__main__.py
+-rw-rw-rw-   0        0        0    57769 2024-03-28 02:50:14.000000 pih-rcgn-0.15/RecognizeService/api.py
+-rw-rw-rw-   0        0        0     1224 2024-02-09 14:42:12.000000 pih-rcgn-0.15/RecognizeService/collection.py
+-rw-rw-rw-   0        0        0     4656 2024-05-20 22:40:33.000000 pih-rcgn-0.15/RecognizeService/const.py
+-rw-rw-rw-   0        0        0    29045 2024-03-19 22:16:00.000000 pih-rcgn-0.15/RecognizeService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:13:02.593736 pih-rcgn-0.15/pih_rcgn.egg-info/
+-rw-rw-rw-   0        0        0      610 2024-05-20 23:13:01.000000 pih-rcgn-0.15/pih_rcgn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-20 23:13:01.000000 pih-rcgn-0.15/pih_rcgn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:13:01.000000 pih-rcgn-0.15/pih_rcgn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-20 23:13:01.000000 pih-rcgn-0.15/pih_rcgn.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      137 2024-05-20 23:13:01.000000 pih-rcgn-0.15/pih_rcgn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 23:13:01.000000 pih-rcgn-0.15/pih_rcgn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:13:02.687482 pih-rcgn-0.15/setup.cfg
```

### Comparing `pih-rcgn-0.14/PKG-INFO` & `pih-rcgn-0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-rcgn
-Version: 0.14
+Version: 0.15
 Summary: PIH Recognize service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

### Comparing `pih-rcgn-0.14/RecognizeService/api.py` & `pih-rcgn-0.15/RecognizeService/api.py`

 * *Files identical despite different names*

### Comparing `pih-rcgn-0.14/RecognizeService/collection.py` & `pih-rcgn-0.15/RecognizeService/collection.py`

 * *Files identical despite different names*

### Comparing `pih-rcgn-0.14/RecognizeService/const.py` & `pih-rcgn-0.15/RecognizeService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "reportlab",
         "python-Levenshtein",
         "numpy",
         "opencv-python",
         "deskew"
     )
 
-VERSION: str = "0.14"
+VERSION: str = "0.15"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Recognize service",
     host=HOST.NAME,
     host_changeable=False,
     commands=(
```

### Comparing `pih-rcgn-0.14/RecognizeService/service.py` & `pih-rcgn-0.15/RecognizeService/service.py`

 * *Files identical despite different names*

### Comparing `pih-rcgn-0.14/pih_rcgn.egg-info/PKG-INFO` & `pih-rcgn-0.15/pih_rcgn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-rcgn
-Version: 0.14
+Version: 0.15
 Summary: PIH Recognize service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

