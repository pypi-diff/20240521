# Comparing `tmp/smart_parallelize-2.1.0.tar.gz` & `tmp/smart_parallelize-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.1.0.tar", max compression
+gzip compressed data, was "smart_parallelize-2.2.0.tar", max compression
```

## Comparing `smart_parallelize-2.1.0.tar` & `smart_parallelize-2.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      554 2024-05-13 01:37:00.192639 smart_parallelize-2.1.0/README.md
--rw-r--r--   0        0        0      317 2024-05-13 16:25:16.344655 smart_parallelize-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.1.0/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     4004 2024-05-13 16:25:05.494140 smart_parallelize-2.1.0/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0     4100 2024-05-13 16:25:38.243039 smart_parallelize-2.1.0/smart_parallelize/parallelize_DEP.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 smart_parallelize-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      554 2024-05-13 01:37:00.192639 smart_parallelize-2.2.0/README.md
+-rw-r--r--   0        0        0      317 2024-05-21 19:28:56.577104 smart_parallelize-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.2.0/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     4004 2024-05-14 17:03:12.517416 smart_parallelize-2.2.0/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0     4100 2024-05-13 16:25:38.243039 smart_parallelize-2.2.0/smart_parallelize/parallelize_DEP.py
+-rw-r--r--   0        0        0     1820 2024-05-21 19:40:46.175222 smart_parallelize-2.2.0/smart_parallelize/parallelize_native.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 smart_parallelize-2.2.0/PKG-INFO
```

### Comparing `smart_parallelize-2.1.0/README.md` & `smart_parallelize-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.1.0/smart_parallelize/parallelize.py` & `smart_parallelize-2.2.0/smart_parallelize/parallelize.py`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.1.0/smart_parallelize/parallelize_DEP.py` & `smart_parallelize-2.2.0/smart_parallelize/parallelize_DEP.py`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.1.0/PKG-INFO` & `smart_parallelize-2.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.1.0
+Version: 2.2.0
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

