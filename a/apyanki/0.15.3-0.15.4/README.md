# Comparing `tmp/apyanki-0.15.3.tar.gz` & `tmp/apyanki-0.15.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apyanki-0.15.3.tar", max compression
+gzip compressed data, was "apyanki-0.15.4.tar", max compression
```

## Comparing `apyanki-0.15.3.tar` & `apyanki-0.15.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.3/LICENSE.md
--rw-r--r--   0        0        0    11250 2024-04-19 20:43:04.288990 apyanki-0.15.3/README.md
--rw-r--r--   0        0        0     1561 2024-04-24 20:54:26.964655 apyanki-0.15.3/pyproject.toml
--rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.3/src/apyanki/__init__.py
--rw-r--r--   0        0        0    16917 2024-04-19 20:21:19.756773 apyanki-0.15.3/src/apyanki/anki.py
--rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.3/src/apyanki/cards.py
--rw-r--r--   0        0        0    14640 2024-04-11 17:03:04.491873 apyanki-0.15.3/src/apyanki/cli.py
--rw-r--r--   0        0        0     2064 2024-04-19 20:39:20.334116 apyanki-0.15.3/src/apyanki/config.py
--rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.3/src/apyanki/console.py
--rw-r--r--   0        0        0     9169 2024-04-19 20:40:01.254397 apyanki-0.15.3/src/apyanki/fields.py
--rw-r--r--   0        0        0    23307 2024-04-11 17:08:37.727403 apyanki-0.15.3/src/apyanki/note.py
--rw-r--r--   0        0        0     2987 2024-04-11 17:11:39.668604 apyanki-0.15.3/src/apyanki/utilities.py
--rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.4/LICENSE.md
+-rw-r--r--   0        0        0    11250 2024-04-19 20:43:04.288990 apyanki-0.15.4/README.md
+-rw-r--r--   0        0        0     1561 2024-05-21 20:23:03.331872 apyanki-0.15.4/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.4/src/apyanki/__init__.py
+-rw-r--r--   0        0        0    16917 2024-04-19 20:21:19.756773 apyanki-0.15.4/src/apyanki/anki.py
+-rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.4/src/apyanki/cards.py
+-rw-r--r--   0        0        0    14640 2024-04-11 17:03:04.491873 apyanki-0.15.4/src/apyanki/cli.py
+-rw-r--r--   0        0        0     2064 2024-04-19 20:39:20.334116 apyanki-0.15.4/src/apyanki/config.py
+-rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.4/src/apyanki/console.py
+-rw-r--r--   0        0        0     9169 2024-04-19 20:40:01.254397 apyanki-0.15.4/src/apyanki/fields.py
+-rw-r--r--   0        0        0    23307 2024-04-11 17:08:37.727403 apyanki-0.15.4/src/apyanki/note.py
+-rw-r--r--   0        0        0     2987 2024-04-11 17:11:39.668604 apyanki-0.15.4/src/apyanki/utilities.py
+-rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.4/PKG-INFO
```

### Comparing `apyanki-0.15.3/LICENSE.md` & `apyanki-0.15.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/README.md` & `apyanki-0.15.4/README.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/pyproject.toml` & `apyanki-0.15.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apyanki"
-version = "0.15.3"
+version = "0.15.4"
 description = "CLI script for interacting with local Anki collection"
 authors = ["Karl Yngve Lervåg <karl.yngve@lervag.net>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `apyanki-0.15.3/src/apyanki/anki.py` & `apyanki-0.15.4/src/apyanki/anki.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/src/apyanki/cards.py` & `apyanki-0.15.4/src/apyanki/cards.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/src/apyanki/cli.py` & `apyanki-0.15.4/src/apyanki/cli.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/src/apyanki/config.py` & `apyanki-0.15.4/src/apyanki/config.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/src/apyanki/console.py` & `apyanki-0.15.4/src/apyanki/console.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/src/apyanki/fields.py` & `apyanki-0.15.4/src/apyanki/fields.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/src/apyanki/note.py` & `apyanki-0.15.4/src/apyanki/note.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/src/apyanki/utilities.py` & `apyanki-0.15.4/src/apyanki/utilities.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.3/PKG-INFO` & `apyanki-0.15.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apyanki
-Version: 0.15.3
+Version: 0.15.4
 Summary: CLI script for interacting with local Anki collection
 Home-page: https://github.com/lervag/apy
 Author: Karl Yngve Lervåg
 Author-email: karl.yngve@lervag.net
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

