# Comparing `tmp/camalis-0.0.2.tar.gz` & `tmp/camalis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camalis-0.0.2.tar", max compression
+gzip compressed data, was "camalis-0.0.3.tar", max compression
```

## Comparing `camalis-0.0.2.tar` & `camalis-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      113 2024-05-09 14:48:58.269856 camalis-0.0.2/camalis/__init__.py
--rw-r--r--   0        0        0     1335 2024-05-09 19:47:55.427179 camalis-0.0.2/camalis/core.py
--rw-r--r--   0        0        0      188 2024-04-24 11:51:17.662890 camalis-0.0.2/camalis/event.py
--rw-r--r--   0        0        0      167 2024-04-23 16:23:39.038037 camalis-0.0.2/camalis/exceptions.py
--rw-r--r--   0        0        0     1881 2024-05-09 19:47:55.433250 camalis-0.0.2/camalis/main.py
--rw-r--r--   0        0        0      810 2024-04-25 14:33:17.981011 camalis-0.0.2/camalis/state.py
--rw-r--r--   0        0        0      795 2024-05-09 12:44:56.932449 camalis-0.0.2/camalis/utils.py
--rw-r--r--   0        0        0     2491 2024-05-09 13:11:52.072437 camalis-0.0.2/camalis/variable.py
--rw-r--r--   0        0        0      527 2024-05-13 13:20:18.561245 camalis-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      141 2024-04-22 14:15:12.162481 camalis-0.0.2/README.md
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 camalis-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-09 14:48:58.269856 camalis-0.0.3/camalis/__init__.py
+-rw-r--r--   0        0        0     1335 2024-05-09 19:47:55.427179 camalis-0.0.3/camalis/core.py
+-rw-r--r--   0        0        0      188 2024-04-24 11:51:17.662890 camalis-0.0.3/camalis/event.py
+-rw-r--r--   0        0        0      167 2024-04-23 16:23:39.038037 camalis-0.0.3/camalis/exceptions.py
+-rw-r--r--   0        0        0     1881 2024-05-09 19:47:55.433250 camalis-0.0.3/camalis/main.py
+-rw-r--r--   0        0        0      810 2024-04-25 14:33:17.981011 camalis-0.0.3/camalis/state.py
+-rw-r--r--   0        0        0      795 2024-05-09 12:44:56.932449 camalis-0.0.3/camalis/utils.py
+-rw-r--r--   0        0        0     2491 2024-05-09 13:11:52.072437 camalis-0.0.3/camalis/variable.py
+-rw-r--r--   0        0        0      526 2024-05-21 15:26:22.911611 camalis-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      141 2024-04-22 14:15:12.162481 camalis-0.0.3/README.md
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 camalis-0.0.3/PKG-INFO
```

### Comparing `camalis-0.0.2/camalis/core.py` & `camalis-0.0.3/camalis/core.py`

 * *Files identical despite different names*

### Comparing `camalis-0.0.2/camalis/main.py` & `camalis-0.0.3/camalis/main.py`

 * *Files identical despite different names*

### Comparing `camalis-0.0.2/camalis/state.py` & `camalis-0.0.3/camalis/state.py`

 * *Files identical despite different names*

### Comparing `camalis-0.0.2/camalis/utils.py` & `camalis-0.0.3/camalis/utils.py`

 * *Files identical despite different names*

### Comparing `camalis-0.0.2/camalis/variable.py` & `camalis-0.0.3/camalis/variable.py`

 * *Files identical despite different names*

### Comparing `camalis-0.0.2/pyproject.toml` & `camalis-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "camalis"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["RN Tecnologia <contato@rntecnologia.com.br>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.12"
-requests = "^2.31.0"
+python = "^3.9"
+requests = "^2.32.1"
 python-dotenv = "^1.0.1"
 pytest-mock = "^3.14.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 isort = "^5.13.2"
```

### Comparing `camalis-0.0.2/PKG-INFO` & `camalis-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: camalis
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: RN Tecnologia
 Author-email: contato@rntecnologia.com.br
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest-mock (>=3.14.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 #
 [ ] Authenticate with camalis api
 [ ] Get historic by variable id
 [ ] Write specialist variable value
 [ ] Get snapshot by variable id
```

