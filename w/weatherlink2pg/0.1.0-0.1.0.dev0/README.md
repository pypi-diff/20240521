# Comparing `tmp/weatherlink2pg-0.1.0.tar.gz` & `tmp/weatherlink2pg-0.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherlink2pg-0.1.0.tar", max compression
+gzip compressed data, was "weatherlink2pg-0.1.0.dev0.tar", max compression
```

## Comparing `weatherlink2pg-0.1.0.tar` & `weatherlink2pg-0.1.0.dev0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      223 2024-05-21 14:00:18.884858 weatherlink2pg-0.1.0/README.md
--rw-r--r--   0        0        0     1943 2024-05-21 14:15:28.736946 weatherlink2pg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-21 14:00:18.888858 weatherlink2pg-0.1.0/src/weatherlink2pg/__init__.py
--rw-r--r--   0        0        0     6183 2024-05-21 14:00:18.888858 weatherlink2pg-0.1.0/src/weatherlink2pg/helpers.py
--rw-r--r--   0        0        0     2161 2024-05-21 14:00:18.888858 weatherlink2pg-0.1.0/src/weatherlink2pg/main.py
--rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 weatherlink2pg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      223 2024-05-21 13:49:30.981855 weatherlink2pg-0.1.0.dev0/README.md
+-rw-r--r--   0        0        0     1949 2024-05-21 13:55:14.297099 weatherlink2pg-0.1.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-21 09:47:48.530699 weatherlink2pg-0.1.0.dev0/src/weatherlink2pg/__init__.py
+-rw-r--r--   0        0        0     6183 2024-05-21 12:52:04.703529 weatherlink2pg-0.1.0.dev0/src/weatherlink2pg/helpers.py
+-rw-r--r--   0        0        0     2161 2024-05-21 13:49:42.913828 weatherlink2pg-0.1.0.dev0/src/weatherlink2pg/main.py
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 weatherlink2pg-0.1.0.dev0/PKG-INFO
```

### Comparing `weatherlink2pg-0.1.0/pyproject.toml` & `weatherlink2pg-0.1.0.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weatherlink2pg"
-version = "0.1.0"
+version = "0.1.0-dev0"
 description = "Simple python app to store weatherlink data into PostgreSQL through API"
 authors = [
     "Johan Rocheteau <johan.rocheteau@hotmail.fr>",
     "Frédéric CLOITRE <no-reply@lpo.fr>",
 ]
 readme = "README.md"
 maintainers = [
@@ -31,15 +31,15 @@
 packages = [{include = "weatherlink2pg", from = "src"}]
 
 
 [tool.poetry.scripts]
 weatherlink2pg = "weatherlink2pg.main:cli"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11"
 pandas = "^2.2.2"
 requests = "^2.31.0"
 tqdm = "^4.66.2"
 python-dotenv = "^1.0.1"
 sqlalchemy = "^2.0.29"
 psycopg2 = "^2.9.9"
```

### Comparing `weatherlink2pg-0.1.0/src/weatherlink2pg/helpers.py` & `weatherlink2pg-0.1.0.dev0/src/weatherlink2pg/helpers.py`

 * *Files identical despite different names*

### Comparing `weatherlink2pg-0.1.0/src/weatherlink2pg/main.py` & `weatherlink2pg-0.1.0.dev0/src/weatherlink2pg/main.py`

 * *Files identical despite different names*

### Comparing `weatherlink2pg-0.1.0/PKG-INFO` & `weatherlink2pg-0.1.0.dev0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: weatherlink2pg
-Version: 0.1.0
+Version: 0.1.0.dev0
 Summary: Simple python app to store weatherlink data into PostgreSQL through API
 Home-page: https://github.com/lpoaura/weatherlink2pg/
 License: AGPL-3.0-or-later
 Keywords: WeatherLink
 Author: Johan Rocheteau
 Author-email: johan.rocheteau@hotmail.fr
 Maintainer: Johan Rocheteau
 Maintainer-email: johan.rocheteau@hotmail.fr
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: French
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Installation/Setup
```

