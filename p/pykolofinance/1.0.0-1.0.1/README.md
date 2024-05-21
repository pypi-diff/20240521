# Comparing `tmp/pykolofinance-1.0.0.tar.gz` & `tmp/pykolofinance-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykolofinance-1.0.0.tar", max compression
+gzip compressed data, was "pykolofinance-1.0.1.tar", max compression
```

## Comparing `pykolofinance-1.0.0.tar` & `pykolofinance-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      158 2024-05-20 12:10:03.148960 pykolofinance-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-20 12:06:37.293451 pykolofinance-1.0.0/pykolofinance/__init__.py
--rw-r--r--   0        0        0     2227 2024-05-20 12:10:26.798650 pykolofinance-1.0.0/pykolofinance/audtilog/readme.md
--rw-r--r--   0        0        0     1697 2024-05-20 13:28:34.664562 pykolofinance-1.0.0/pykolofinance/authentication.py
--rw-r--r--   0        0        0      198 2024-05-20 12:10:16.569830 pykolofinance-1.0.0/pykolofinance/enums.py
--rw-r--r--   0        0        0      805 2024-05-20 12:10:16.572615 pykolofinance-1.0.0/pykolofinance/filters.py
--rw-r--r--   0        0        0     1562 2024-05-20 12:10:16.575441 pykolofinance-1.0.0/pykolofinance/middlewares.py
--rw-r--r--   0        0        0        0 2024-05-20 12:10:26.803433 pykolofinance-1.0.0/pykolofinance/permissions/__init__.py
--rw-r--r--   0        0        0     1132 2024-05-20 12:10:26.804139 pykolofinance-1.0.0/pykolofinance/permissions/checker.py
--rw-r--r--   0        0        0    18896 2024-05-20 12:10:26.805492 pykolofinance-1.0.0/pykolofinance/permissions/perm_list.py
--rw-r--r--   0        0        0        0 2024-05-20 12:10:26.809249 pykolofinance-1.0.0/pykolofinance/services/__init__.py
--rw-r--r--   0        0        0      887 2024-05-20 12:10:26.809868 pykolofinance-1.0.0/pykolofinance/services/auth.py
--rw-r--r--   0        0        0     1036 2024-05-20 12:10:26.810363 pykolofinance-1.0.0/pykolofinance/services/base.py
--rw-r--r--   0        0        0      580 2024-05-20 13:32:44.300607 pykolofinance-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 pykolofinance-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      690 2024-05-21 08:58:57.837212 pykolofinance-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 12:06:37.293451 pykolofinance-1.0.1/pykolofinance/__init__.py
+-rw-r--r--   0        0        0     2227 2024-05-20 12:10:26.798650 pykolofinance-1.0.1/pykolofinance/audtilog/readme.md
+-rw-r--r--   0        0        0     1697 2024-05-20 13:28:34.664562 pykolofinance-1.0.1/pykolofinance/authentication.py
+-rw-r--r--   0        0        0      198 2024-05-20 12:10:16.569830 pykolofinance-1.0.1/pykolofinance/enums.py
+-rw-r--r--   0        0        0      805 2024-05-20 12:10:16.572615 pykolofinance-1.0.1/pykolofinance/filters.py
+-rw-r--r--   0        0        0     1562 2024-05-20 12:10:16.575441 pykolofinance-1.0.1/pykolofinance/middlewares.py
+-rw-r--r--   0        0        0        0 2024-05-20 12:10:26.803433 pykolofinance-1.0.1/pykolofinance/permissions/__init__.py
+-rw-r--r--   0        0        0     1132 2024-05-20 12:10:26.804139 pykolofinance-1.0.1/pykolofinance/permissions/checker.py
+-rw-r--r--   0        0        0    18896 2024-05-20 12:10:26.805492 pykolofinance-1.0.1/pykolofinance/permissions/perm_list.py
+-rw-r--r--   0        0        0        0 2024-05-20 12:10:26.809249 pykolofinance-1.0.1/pykolofinance/services/__init__.py
+-rw-r--r--   0        0        0      887 2024-05-20 12:10:26.809868 pykolofinance-1.0.1/pykolofinance/services/auth.py
+-rw-r--r--   0        0        0     1036 2024-05-20 12:10:26.810363 pykolofinance-1.0.1/pykolofinance/services/base.py
+-rw-r--r--   0        0        0      580 2024-05-21 08:59:26.543570 pykolofinance-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 pykolofinance-1.0.1/PKG-INFO
```

### Comparing `pykolofinance-1.0.0/pykolofinance/audtilog/readme.md` & `pykolofinance-1.0.1/pykolofinance/audtilog/readme.md`

 * *Files identical despite different names*

### Comparing `pykolofinance-1.0.0/pykolofinance/authentication.py` & `pykolofinance-1.0.1/pykolofinance/authentication.py`

 * *Files identical despite different names*

### Comparing `pykolofinance-1.0.0/pykolofinance/filters.py` & `pykolofinance-1.0.1/pykolofinance/filters.py`

 * *Files identical despite different names*

### Comparing `pykolofinance-1.0.0/pykolofinance/middlewares.py` & `pykolofinance-1.0.1/pykolofinance/middlewares.py`

 * *Files identical despite different names*

### Comparing `pykolofinance-1.0.0/pykolofinance/permissions/checker.py` & `pykolofinance-1.0.1/pykolofinance/permissions/checker.py`

 * *Files identical despite different names*

### Comparing `pykolofinance-1.0.0/pykolofinance/permissions/perm_list.py` & `pykolofinance-1.0.1/pykolofinance/permissions/perm_list.py`

 * *Files identical despite different names*

### Comparing `pykolofinance-1.0.0/pykolofinance/services/auth.py` & `pykolofinance-1.0.1/pykolofinance/services/auth.py`

 * *Files identical despite different names*

### Comparing `pykolofinance-1.0.0/pykolofinance/services/base.py` & `pykolofinance-1.0.1/pykolofinance/services/base.py`

 * *Files identical despite different names*

### Comparing `pykolofinance-1.0.0/pyproject.toml` & `pykolofinance-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykolofinance"
-version = "1.0.0"
+version = "1.0.1"
 description = "A utility package for kolomoni agency banking microservices"
 authors = ["Daniel Ale <danielale9291@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pykolofinance"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

