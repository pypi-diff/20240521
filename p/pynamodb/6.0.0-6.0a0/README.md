# Comparing `tmp/pynamodb-6.0.0.tar.gz` & `tmp/pynamodb-6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb-6.0.0.tar", last modified: Sun Jan 14 15:41:35 2024, max compression
+gzip compressed data, was "pynamodb-6.0a0.tar", last modified: Sun Jan 14 03:01:44 2024, max compression
```

## Comparing `pynamodb-6.0.0.tar` & `pynamodb-6.0a0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 15:41:35.107903 pynamodb-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-14 15:41:16.000000 pynamodb-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-14 15:41:16.000000 pynamodb-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-01-14 15:41:35.107903 pynamodb-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-01-14 15:41:16.000000 pynamodb-6.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-14 15:41:16.000000 pynamodb-6.0.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 15:41:35.099903 pynamodb-6.0.0/pynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    58584 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 15:41:35.103903 pynamodb-6.0.0/pynamodb/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/connection/_botocore_private.py
--rw-r--r--   0 runner    (1001) docker     (127)    50888 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/connection/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/connection/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 15:41:35.103903 pynamodb-6.0.0/pynamodb/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/expressions/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/expressions/operand.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/expressions/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/expressions/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/expressions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    49590 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-14 15:41:16.000000 pynamodb-6.0.0/pynamodb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 15:41:35.107903 pynamodb-6.0.0/pynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-01-14 15:41:35.000000 pynamodb-6.0.0/pynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-14 15:41:35.000000 pynamodb-6.0.0/pynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 15:41:35.000000 pynamodb-6.0.0/pynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 15:41:34.000000 pynamodb-6.0.0/pynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-14 15:41:35.000000 pynamodb-6.0.0/pynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-14 15:41:35.000000 pynamodb-6.0.0/pynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-14 15:41:16.000000 pynamodb-6.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-14 15:41:35.107903 pynamodb-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-01-14 15:41:16.000000 pynamodb-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 15:41:35.103903 pynamodb-6.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    50686 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    54302 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_binary_legacy_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30876 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)   127499 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    20252 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_table_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-01-14 15:41:16.000000 pynamodb-6.0.0/tests/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.116251 pynamodb-6.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-14 03:01:23.000000 pynamodb-6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-14 03:01:23.000000 pynamodb-6.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-01-14 03:01:44.116251 pynamodb-6.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-01-14 03:01:23.000000 pynamodb-6.0a0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-14 03:01:23.000000 pynamodb-6.0a0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.108251 pynamodb-6.0a0/pynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58584 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.108251 pynamodb-6.0a0/pynamodb/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/connection/_botocore_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50888 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/connection/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/connection/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.108251 pynamodb-6.0a0/pynamodb/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/operand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49590 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.112251 pynamodb-6.0a0/pynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 03:01:43.000000 pynamodb-6.0a0/pynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-14 03:01:23.000000 pynamodb-6.0a0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-14 03:01:44.116251 pynamodb-6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-01-14 03:01:23.000000 pynamodb-6.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.112251 pynamodb-6.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    50686 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54302 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_binary_legacy_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30876 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127499 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20252 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_table_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_transaction.py
```

### Comparing `pynamodb-6.0.0/LICENSE` & `pynamodb-6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/PKG-INFO` & `pynamodb-6.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb
-Version: 6.0.0
+Version: 6.0a0
 Summary: A Pythonic Interface to DynamoDB
 Home-page: http://jlafon.io/pynamodb.html
 Author: Jharrod LaFon
 Author-email: jlafon@eyesopen.com
 License: MIT
 Project-URL: Source, https://github.com/pynamodb/PynamoDB
 Keywords: python dynamodb amazon
```

### Comparing `pynamodb-6.0.0/README.rst` & `pynamodb-6.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/_schema.py` & `pynamodb-6.0a0/pynamodb/_schema.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/_util.py` & `pynamodb-6.0a0/pynamodb/_util.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/attributes.py` & `pynamodb-6.0a0/pynamodb/attributes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/connection/_botocore_private.py` & `pynamodb-6.0a0/pynamodb/connection/_botocore_private.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/connection/base.py` & `pynamodb-6.0a0/pynamodb/connection/base.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/connection/table.py` & `pynamodb-6.0a0/pynamodb/connection/table.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/constants.py` & `pynamodb-6.0a0/pynamodb/constants.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/exceptions.py` & `pynamodb-6.0a0/pynamodb/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/expressions/condition.py` & `pynamodb-6.0a0/pynamodb/expressions/condition.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/expressions/operand.py` & `pynamodb-6.0a0/pynamodb/expressions/operand.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/expressions/projection.py` & `pynamodb-6.0a0/pynamodb/expressions/projection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/expressions/update.py` & `pynamodb-6.0a0/pynamodb/expressions/update.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/expressions/util.py` & `pynamodb-6.0a0/pynamodb/expressions/util.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/indexes.py` & `pynamodb-6.0a0/pynamodb/indexes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/models.py` & `pynamodb-6.0a0/pynamodb/models.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/pagination.py` & `pynamodb-6.0a0/pynamodb/pagination.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/settings.py` & `pynamodb-6.0a0/pynamodb/settings.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/signals.py` & `pynamodb-6.0a0/pynamodb/signals.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb/transactions.py` & `pynamodb-6.0a0/pynamodb/transactions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/pynamodb.egg-info/PKG-INFO` & `pynamodb-6.0a0/pynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb
-Version: 6.0.0
+Version: 6.0a0
 Summary: A Pythonic Interface to DynamoDB
 Home-page: http://jlafon.io/pynamodb.html
 Author: Jharrod LaFon
 Author-email: jlafon@eyesopen.com
 License: MIT
 Project-URL: Source, https://github.com/pynamodb/PynamoDB
 Keywords: python dynamodb amazon
```

### Comparing `pynamodb-6.0.0/pynamodb.egg-info/SOURCES.txt` & `pynamodb-6.0a0/pynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/setup.py` & `pynamodb-6.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_attributes.py` & `pynamodb-6.0a0/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_base_connection.py` & `pynamodb-6.0a0/tests/test_base_connection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_discriminator.py` & `pynamodb-6.0a0/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_exceptions.py` & `pynamodb-6.0a0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_expressions.py` & `pynamodb-6.0a0/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_model.py` & `pynamodb-6.0a0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_pagination.py` & `pynamodb-6.0a0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_settings.py` & `pynamodb-6.0a0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_signals.py` & `pynamodb-6.0a0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_table_connection.py` & `pynamodb-6.0a0/tests/test_table_connection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.0/tests/test_transaction.py` & `pynamodb-6.0a0/tests/test_transaction.py`

 * *Files identical despite different names*

