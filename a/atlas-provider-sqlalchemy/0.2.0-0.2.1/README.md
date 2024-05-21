# Comparing `tmp/atlas_provider_sqlalchemy-0.2.0.tar.gz` & `tmp/atlas_provider_sqlalchemy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas_provider_sqlalchemy-0.2.0.tar", max compression
+gzip compressed data, was "atlas_provider_sqlalchemy-0.2.1.tar", max compression
```

## Comparing `atlas_provider_sqlalchemy-0.2.0.tar` & `atlas_provider_sqlalchemy-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-15 06:53:16.155091 atlas_provider_sqlalchemy-0.2.0/LICENSE
--rw-r--r--   0        0        0     3960 2024-05-15 06:53:16.155091 atlas_provider_sqlalchemy-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-15 06:53:16.155091 atlas_provider_sqlalchemy-0.2.0/atlas_provider_sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2937 2024-05-15 06:53:16.155091 atlas_provider_sqlalchemy-0.2.0/atlas_provider_sqlalchemy/ddl.py
--rw-r--r--   0        0        0     1255 2024-05-15 06:53:16.159091 atlas_provider_sqlalchemy-0.2.0/atlas_provider_sqlalchemy/main.py
--rw-r--r--   0        0        0      723 2024-05-15 06:53:24.427144 atlas_provider_sqlalchemy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 atlas_provider_sqlalchemy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-21 08:16:10.699121 atlas_provider_sqlalchemy-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3960 2024-05-21 08:16:10.699121 atlas_provider_sqlalchemy-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 08:16:10.699121 atlas_provider_sqlalchemy-0.2.1/atlas_provider_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2937 2024-05-21 08:16:10.703122 atlas_provider_sqlalchemy-0.2.1/atlas_provider_sqlalchemy/ddl.py
+-rw-r--r--   0        0        0     1255 2024-05-21 08:16:10.703122 atlas_provider_sqlalchemy-0.2.1/atlas_provider_sqlalchemy/main.py
+-rw-r--r--   0        0        0      723 2024-05-21 08:16:19.711150 atlas_provider_sqlalchemy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 atlas_provider_sqlalchemy-0.2.1/PKG-INFO
```

### Comparing `atlas_provider_sqlalchemy-0.2.0/LICENSE` & `atlas_provider_sqlalchemy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atlas_provider_sqlalchemy-0.2.0/README.md` & `atlas_provider_sqlalchemy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `atlas_provider_sqlalchemy-0.2.0/atlas_provider_sqlalchemy/ddl.py` & `atlas_provider_sqlalchemy-0.2.1/atlas_provider_sqlalchemy/ddl.py`

 * *Files identical despite different names*

### Comparing `atlas_provider_sqlalchemy-0.2.0/atlas_provider_sqlalchemy/main.py` & `atlas_provider_sqlalchemy-0.2.1/atlas_provider_sqlalchemy/main.py`

 * *Files identical despite different names*

### Comparing `atlas_provider_sqlalchemy-0.2.0/PKG-INFO` & `atlas_provider_sqlalchemy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-provider-sqlalchemy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Load sqlalchemy models into an Atlas project.
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

