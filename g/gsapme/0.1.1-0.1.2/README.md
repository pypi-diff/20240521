# Comparing `tmp/gsapme-0.1.1.tar.gz` & `tmp/gsapme-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsapme-0.1.1.tar", max compression
+gzip compressed data, was "gsapme-0.1.2.tar", max compression
```

## Comparing `gsapme-0.1.1.tar` & `gsapme-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      602 2024-04-25 19:23:14.417182 gsapme-0.1.1/README.md
--rw-r--r--   0        0        0      274 2024-05-07 18:31:10.358195 gsapme-0.1.1/gsapme/__init__.py
--rw-r--r--   0        0        0     3952 2024-05-07 18:29:01.335000 gsapme-0.1.1/gsapme/analysis.py
--rw-r--r--   0        0        0      897 2024-05-07 18:30:15.119156 gsapme-0.1.1/gsapme/covariance.py
--rw-r--r--   0        0        0      788 2024-05-07 18:29:33.413899 gsapme-0.1.1/gsapme/models.py
--rw-r--r--   0        0        0     2658 2024-05-07 18:29:16.024598 gsapme-0.1.1/gsapme/simulation.py
--rw-r--r--   0        0        0      378 2024-05-07 18:53:05.131511 gsapme-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 gsapme-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      602 2024-04-25 19:23:14.417182 gsapme-0.1.2/README.md
+-rw-r--r--   0        0        0      190 2024-05-21 17:50:07.458864 gsapme-0.1.2/gsapme/__init__.py
+-rw-r--r--   0        0        0    12670 2024-05-21 18:12:29.522215 gsapme-0.1.2/gsapme/analysis.py
+-rw-r--r--   0        0        0      897 2024-05-07 18:30:15.119156 gsapme-0.1.2/gsapme/covariance.py
+-rw-r--r--   0        0        0     2061 2024-05-14 18:54:14.042121 gsapme-0.1.2/gsapme/models.py
+-rw-r--r--   0        0        0     2658 2024-05-07 18:29:16.024598 gsapme-0.1.2/gsapme/simulation.py
+-rw-r--r--   0        0        0      405 2024-05-21 18:18:58.905819 gsapme-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 gsapme-0.1.2/PKG-INFO
```

### Comparing `gsapme-0.1.1/README.md` & `gsapme-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gsapme-0.1.1/gsapme/covariance.py` & `gsapme-0.1.2/gsapme/covariance.py`

 * *Files identical despite different names*

### Comparing `gsapme-0.1.1/gsapme/simulation.py` & `gsapme-0.1.2/gsapme/simulation.py`

 * *Files identical despite different names*

### Comparing `gsapme-0.1.1/PKG-INFO` & `gsapme-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: gsapme
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Theo Demetriades
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: copulas (>=0.11.0,<0.12.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Overview
 
 ## What does this package do?
```

