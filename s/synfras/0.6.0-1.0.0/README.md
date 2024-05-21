# Comparing `tmp/synfras-0.6.0.tar.gz` & `tmp/synfras-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synfras-0.6.0.tar", max compression
+gzip compressed data, was "synfras-1.0.0.tar", max compression
```

## Comparing `synfras-0.6.0.tar` & `synfras-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      726 2024-05-12 14:10:19.119812 synfras-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      542 2024-05-07 03:29:24.028213 synfras-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-02-13 06:43:19.642186 synfras-0.6.0/synfras/__init__.py
--rw-r--r--   0        0        0       68 2024-05-07 02:18:48.798900 synfras-0.6.0/synfras/config.py
--rw-r--r--   0        0        0     1513 2024-05-12 14:16:33.438093 synfras-0.6.0/synfras/database.py
--rw-r--r--   0        0        0     1189 2024-05-07 02:18:48.801460 synfras-0.6.0/synfras/parallel.py
--rw-r--r--   0        0        0      816 2024-05-08 08:38:21.923774 synfras-0.6.0/synfras/utils.py
--rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 synfras-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      725 2024-05-21 14:41:51.255974 synfras-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      542 2024-05-07 03:29:24.028213 synfras-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-13 06:43:19.642186 synfras-1.0.0/synfras/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-07 02:18:48.798900 synfras-1.0.0/synfras/config.py
+-rw-r--r--   0        0        0     1513 2024-05-12 14:16:33.438093 synfras-1.0.0/synfras/database.py
+-rw-r--r--   0        0        0     1189 2024-05-07 02:18:48.801460 synfras-1.0.0/synfras/parallel.py
+-rw-r--r--   0        0        0      816 2024-05-08 08:38:21.923774 synfras-1.0.0/synfras/utils.py
+-rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 synfras-1.0.0/PKG-INFO
```

### Comparing `synfras-0.6.0/pyproject.toml` & `synfras-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name        = "synfras"
-version     = "0.6.0"
+version     = "1.0.0"
 description = ""
 authors     = ["Trung Dang <dangtrung96@gmail.com>"]
 readme      = "README.md"
 
 [tool.poetry.dependencies]
 python     = "^3.11"
 dynaconf   = "^3.2.4"
-tqdm       = "^4.66.2"
-sqlalchemy = "^2.0.27"
-psycopg2   = "^2.9.9"
-oracledb   = "^2.0.1"
 pandas     = "^2.2.1"
-pymssql    = "2.2.7"
+sqlalchemy = "^2.0.27"
+tqdm       = "^4.66.2"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.0.0"
-yapf   = "^0.40.2"
+pytest   = "^8.0.0"
+psycopg2 = "^2.9.9"
+pymssql  = "^2.3.0"
+oracledb = "^2.2.0"
+yapf     = "^0.40.2"
 
 [tool.pytest.ini_options]
 addopts = "-vv -s --no-header -q"
 
 [tool.yapf]
 based_on_style                        = "facebook"
 blank_line_before_nested_class_or_def = true
```

### Comparing `synfras-0.6.0/README.md` & `synfras-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `synfras-0.6.0/synfras/database.py` & `synfras-1.0.0/synfras/database.py`

 * *Files identical despite different names*

### Comparing `synfras-0.6.0/synfras/parallel.py` & `synfras-1.0.0/synfras/parallel.py`

 * *Files identical despite different names*

### Comparing `synfras-0.6.0/synfras/utils.py` & `synfras-1.0.0/synfras/utils.py`

 * *Files identical despite different names*

### Comparing `synfras-0.6.0/PKG-INFO` & `synfras-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: synfras
-Version: 0.6.0
+Version: 1.0.0
 Summary: 
 Author: Trung Dang
 Author-email: dangtrung96@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dynaconf (>=3.2.4,<4.0.0)
-Requires-Dist: oracledb (>=2.0.1,<3.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
-Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
-Requires-Dist: pymssql (==2.2.7)
 Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Sample Configs
 
 ## `.env`
```

