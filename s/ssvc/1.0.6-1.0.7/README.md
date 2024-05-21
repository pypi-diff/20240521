# Comparing `tmp/ssvc-1.0.6.tar.gz` & `tmp/ssvc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssvc-1.0.6.tar", max compression
+gzip compressed data, was "ssvc-1.0.7.tar", max compression
```

## Comparing `ssvc-1.0.6.tar` & `ssvc-1.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2024-03-25 11:16:25.817155 ssvc-1.0.6/LICENSE
--rw-r--r--   0        0        0     1949 2024-04-18 11:26:03.741779 ssvc-1.0.6/PYPI.md
--rw-r--r--   0        0        0      640 2024-05-07 12:24:55.356005 ssvc-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6463 2024-04-18 11:26:03.748446 ssvc-1.0.6/src/ssvc/__init__.py
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 ssvc-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-25 11:16:25.817155 ssvc-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1949 2024-04-18 11:26:03.741779 ssvc-1.0.7/PYPI.md
+-rw-r--r--   0        0        0      640 2024-05-21 11:41:57.123951 ssvc-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6463 2024-04-18 11:26:03.748446 ssvc-1.0.7/src/ssvc/__init__.py
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 ssvc-1.0.7/PKG-INFO
```

### Comparing `ssvc-1.0.6/LICENSE` & `ssvc-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.6/PYPI.md` & `ssvc-1.0.7/PYPI.md`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.6/pyproject.toml` & `ssvc-1.0.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "ssvc"
-version = "1.0.6"
+version = "1.0.7"
 description = "A Python implementation of the Stakeholder-Specific Vulnerability Categorization framework."
 authors = ["Christopher Langton <chris@langton.cloud>"]
 readme = "PYPI.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.dev-dependencies]
 setuptools = "^69.5.1"
-uv = "^0.1.39"
+uv = "^0.1.44"
 isort = "^5.13.2"
-pytest = "^8.1.1"
+pytest = "^8.2.1"
 pytest-cov = "^5.0.0"
 coverage-badge = "^1.1.1"
 ruff = "^0.4.3"
-poetry = "^1.8.2"
+poetry = "^1.8.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Repository" = "https://github.com/chrisdlangton/python-ssvc.git"
```

### Comparing `ssvc-1.0.6/src/ssvc/__init__.py` & `ssvc-1.0.7/src/ssvc/__init__.py`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.6/PKG-INFO` & `ssvc-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssvc
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python implementation of the Stakeholder-Specific Vulnerability Categorization framework.
 Author: Christopher Langton
 Author-email: chris@langton.cloud
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

