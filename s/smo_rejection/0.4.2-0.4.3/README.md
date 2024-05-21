# Comparing `tmp/smo_rejection-0.4.2.tar.gz` & `tmp/smo_rejection-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smo_rejection-0.4.2.tar", max compression
+gzip compressed data, was "smo_rejection-0.4.3.tar", max compression
```

## Comparing `smo_rejection-0.4.2.tar` & `smo_rejection-0.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      283 2024-05-20 07:59:33.308864 smo_rejection-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    16387 2024-05-20 07:59:33.306860 smo_rejection-0.4.2/README.md
--rw-r--r--   0        0        0      301 2024-05-20 07:59:33.316861 smo_rejection-0.4.2/smo_rejection/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-18 10:29:03.257241 smo_rejection-0.4.2/smo_rejection/exception.py
--rw-r--r--   0        0        0     1628 2024-05-18 10:29:03.257241 smo_rejection-0.4.2/smo_rejection/models.py
--rw-r--r--   0        0        0     4236 2024-05-20 07:59:33.326861 smo_rejection-0.4.2/smo_rejection/pdf_export.py
--rw-r--r--   0        0        0     4419 2024-05-18 10:29:03.257241 smo_rejection-0.4.2/smo_rejection/processing.py
--rw-r--r--   0        0        0     4307 2024-05-18 10:29:03.258245 smo_rejection-0.4.2/smo_rejection/simulation.py
--rw-r--r--   0        0        0     2471 2024-05-18 10:29:03.258245 smo_rejection-0.4.2/smo_rejection/utils.py
--rw-r--r--   0        0        0     4797 2024-05-20 07:59:33.329863 smo_rejection-0.4.2/smo_rejection/xml_export.py
--rw-r--r--   0        0        0    16485 1970-01-01 00:00:00.000000 smo_rejection-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      283 2024-05-20 15:05:06.949138 smo_rejection-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    16387 2024-05-20 07:59:33.306860 smo_rejection-0.4.3/README.md
+-rw-r--r--   0        0        0      496 2024-05-20 15:04:59.554803 smo_rejection-0.4.3/smo_rejection/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-18 10:29:03.257241 smo_rejection-0.4.3/smo_rejection/exception.py
+-rw-r--r--   0        0        0     1628 2024-05-18 10:29:03.257241 smo_rejection-0.4.3/smo_rejection/models.py
+-rw-r--r--   0        0        0     4236 2024-05-20 07:59:33.326861 smo_rejection-0.4.3/smo_rejection/pdf_export.py
+-rw-r--r--   0        0        0     4419 2024-05-18 10:29:03.257241 smo_rejection-0.4.3/smo_rejection/processing.py
+-rw-r--r--   0        0        0     4307 2024-05-18 10:29:03.258245 smo_rejection-0.4.3/smo_rejection/simulation.py
+-rw-r--r--   0        0        0     2471 2024-05-18 10:29:03.258245 smo_rejection-0.4.3/smo_rejection/utils.py
+-rw-r--r--   0        0        0     4797 2024-05-20 14:59:05.590827 smo_rejection-0.4.3/smo_rejection/xml_export.py
+-rw-r--r--   0        0        0    16485 1970-01-01 00:00:00.000000 smo_rejection-0.4.3/PKG-INFO
```

### Comparing `smo_rejection-0.4.2/README.md` & `smo_rejection-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.2/smo_rejection/exception.py` & `smo_rejection-0.4.3/smo_rejection/exception.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.2/smo_rejection/models.py` & `smo_rejection-0.4.3/smo_rejection/models.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.2/smo_rejection/pdf_export.py` & `smo_rejection-0.4.3/smo_rejection/pdf_export.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.2/smo_rejection/processing.py` & `smo_rejection-0.4.3/smo_rejection/processing.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.2/smo_rejection/simulation.py` & `smo_rejection-0.4.3/smo_rejection/simulation.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.2/smo_rejection/utils.py` & `smo_rejection-0.4.3/smo_rejection/utils.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.2/smo_rejection/xml_export.py` & `smo_rejection-0.4.3/smo_rejection/xml_export.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.2/PKG-INFO` & `smo_rejection-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smo_rejection
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: mbtmrw
 Author-email: keks2324098@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

