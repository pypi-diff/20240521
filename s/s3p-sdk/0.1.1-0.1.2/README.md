# Comparing `tmp/s3p_sdk-0.1.1.tar.gz` & `tmp/s3p_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3p_sdk-0.1.1.tar", max compression
+gzip compressed data, was "s3p_sdk-0.1.2.tar", max compression
```

## Comparing `s3p_sdk-0.1.1.tar` & `s3p_sdk-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/LICENSE
--rw-r--r--   0        0        0        9 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/README.md
--rw-r--r--   0        0        0      815 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       59 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/src/s3p_sdk/__init__.py
--rw-r--r--   0        0        0       29 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/src/s3p_sdk/plugin/__init__.py
--rw-r--r--   0        0        0      166 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/__init__.py
--rw-r--r--   0        0        0      185 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/abc_payload_base.py
--rw-r--r--   0        0        0      150 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/parsers/__init__.py
--rw-r--r--   0        0        0      776 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/parsers/abc_parser_base.py
--rw-r--r--   0        0        0     1573 2024-03-21 10:12:41.640005 s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/parsers/parser_base.py
--rw-r--r--   0        0        0      544 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/payload_base.py
--rw-r--r--   0        0        0       25 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/repository/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/repository/db/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/repository/db/document.py
--rw-r--r--   0        0        0      514 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/repository/db/main.py
--rw-r--r--   0        0        0     2029 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/repository/db/user.py
--rw-r--r--   0        0        0      418 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/__init__.py
--rw-r--r--   0        0        0      219 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/digest.py
--rw-r--r--   0        0        0     1130 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/document.py
--rw-r--r--   0        0        0      234 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/export.py
--rw-r--r--   0        0        0      223 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/node.py
--rw-r--r--   0        0        0      395 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/plugin.py
--rw-r--r--   0        0        0      645 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/refer.py
--rw-r--r--   0        0        0      309 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/role.py
--rw-r--r--   0        0        0      412 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/score.py
--rw-r--r--   0        0        0      350 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/task.py
--rw-r--r--   0        0        0      345 2024-03-21 10:12:41.644005 s3p_sdk-0.1.1/src/s3p_sdk/types/user.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 s3p_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-21 10:35:12.715768 s3p_sdk-0.1.2/LICENSE
+-rw-r--r--   0        0        0        9 2024-05-21 10:35:12.715768 s3p_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0      822 2024-05-21 10:35:12.715768 s3p_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/plugin/__init__.py
+-rw-r--r--   0        0        0      166 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/abc_payload_base.py
+-rw-r--r--   0        0        0      150 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/parsers/__init__.py
+-rw-r--r--   0        0        0      776 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/parsers/abc_parser_base.py
+-rw-r--r--   0        0        0     1573 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/parsers/parser_base.py
+-rw-r--r--   0        0        0      544 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/payload_base.py
+-rw-r--r--   0        0        0       25 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/repository/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/repository/db/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/repository/db/document.py
+-rw-r--r--   0        0        0      514 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/repository/db/main.py
+-rw-r--r--   0        0        0     2029 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/repository/db/user.py
+-rw-r--r--   0        0        0      462 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/__init__.py
+-rw-r--r--   0        0        0      219 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/digest.py
+-rw-r--r--   0        0        0     1130 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/document.py
+-rw-r--r--   0        0        0      234 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/export.py
+-rw-r--r--   0        0        0      223 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/node.py
+-rw-r--r--   0        0        0      395 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/plugin.py
+-rw-r--r--   0        0        0      645 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/refer.py
+-rw-r--r--   0        0        0      309 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/role.py
+-rw-r--r--   0        0        0      412 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/score.py
+-rw-r--r--   0        0        0      350 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/task.py
+-rw-r--r--   0        0        0      345 2024-05-21 10:35:12.719768 s3p_sdk-0.1.2/src/s3p_sdk/types/user.py
+-rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 s3p_sdk-0.1.2/PKG-INFO
```

### Comparing `s3p_sdk-0.1.1/LICENSE` & `s3p_sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s3p_sdk-0.1.1/pyproject.toml` & `s3p_sdk-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "s3p-sdk"
-version = "0.1.1"
+version = "0.1.2"
 description = "A small SDK for simple creating a microservises or plugins for the S3 Platform"
 authors = [
     "Roman Lupashko <romal5754@gmail.com>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/CuberHuber/S3P-SDK"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-psycopg2 = "2.9.9"
+psycopg2-binary = "2.9.9"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "*"
 tox = "4.14.1"
```

### Comparing `s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/parsers/abc_parser_base.py` & `s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/parsers/abc_parser_base.py`

 * *Files identical despite different names*

### Comparing `s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/parsers/parser_base.py` & `s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `s3p_sdk-0.1.1/src/s3p_sdk/plugin/payloads/payload_base.py` & `s3p_sdk-0.1.2/src/s3p_sdk/plugin/payloads/payload_base.py`

 * *Files identical despite different names*

### Comparing `s3p_sdk-0.1.1/src/s3p_sdk/repository/db/main.py` & `s3p_sdk-0.1.2/src/s3p_sdk/repository/db/main.py`

 * *Files identical despite different names*

### Comparing `s3p_sdk-0.1.1/src/s3p_sdk/repository/db/user.py` & `s3p_sdk-0.1.2/src/s3p_sdk/repository/db/user.py`

 * *Files identical despite different names*

### Comparing `s3p_sdk-0.1.1/src/s3p_sdk/types/document.py` & `s3p_sdk-0.1.2/src/s3p_sdk/types/document.py`

 * *Files identical despite different names*

### Comparing `s3p_sdk-0.1.1/src/s3p_sdk/types/refer.py` & `s3p_sdk-0.1.2/src/s3p_sdk/types/refer.py`

 * *Files identical despite different names*

### Comparing `s3p_sdk-0.1.1/PKG-INFO` & `s3p_sdk-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: s3p-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small SDK for simple creating a microservises or plugins for the S3 Platform
 Home-page: https://github.com/CuberHuber/S3P-SDK
 License: GPL-3.0-or-later
 Author: Roman Lupashko
 Author-email: romal5754@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: psycopg2 (==2.9.9)
+Requires-Dist: psycopg2-binary (==2.9.9)
 Project-URL: Repository, https://github.com/CuberHuber/S3P-SDK
 Description-Content-Type: text/markdown
 
 # S3P-SDK
```

