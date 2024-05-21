# Comparing `tmp/italia-0.2.0.tar.gz` & `tmp/italia-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "italia-0.2.0.tar", last modified: Mon May 20 18:37:47 2024, max compression
+gzip compressed data, was "italia-0.2.1.tar", last modified: Tue May 21 12:05:08 2024, max compression
```

## Comparing `italia-0.2.0.tar` & `italia-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-20 18:37:33.568165 italia-0.2.0/LICENCE
--rw-r--r--   0        0        0     2663 2024-05-20 18:37:33.568165 italia-0.2.0/README.md
--rw-r--r--   0        0        0       56 2024-05-20 18:37:33.568165 italia-0.2.0/italia/__init__.py
--rw-r--r--   0        0        0     1883 2024-05-20 18:37:33.568165 italia-0.2.0/italia/story.py
--rw-r--r--   0        0        0      607 2024-05-20 18:37:33.568165 italia-0.2.0/italia/team.py
--rw-r--r--   0        0        0      532 2024-05-20 18:37:47.936270 italia-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 18:37:33.568165 italia-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      203 2024-05-20 18:37:33.568165 italia-0.2.0/tests/test_italia.py
--rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 italia-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-21 12:04:50.326476 italia-0.2.1/LICENCE
+-rw-r--r--   0        0        0     2663 2024-05-21 12:04:50.326476 italia-0.2.1/README.md
+-rw-r--r--   0        0        0       56 2024-05-21 12:04:50.326476 italia-0.2.1/italia/__init__.py
+-rw-r--r--   0        0        0     1883 2024-05-21 12:04:50.326476 italia-0.2.1/italia/story.py
+-rw-r--r--   0        0        0      608 2024-05-21 12:04:50.326476 italia-0.2.1/italia/team.py
+-rw-r--r--   0        0        0      532 2024-05-21 12:05:08.126413 italia-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-21 12:04:50.326476 italia-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-21 12:04:50.326476 italia-0.2.1/tests/test_italia.py
+-rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 italia-0.2.1/PKG-INFO
```

### Comparing `italia-0.2.0/LICENCE` & `italia-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `italia-0.2.0/README.md` & `italia-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `italia-0.2.0/italia/story.py` & `italia-0.2.1/italia/story.py`

 * *Files identical despite different names*

### Comparing `italia-0.2.0/italia/team.py` & `italia-0.2.1/italia/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Ambra Tonon
 Carlo Miron
 Edo Abati
 Ernesto Arbitrio
 Ester Beltrami
 Fiorella De Luca
 Gionathan Desogus
-Juna Salvati
-Lerio Campanile
+Juna Salviati
+Lelio Campanile
 Marco Acierno
 Marco Beri
 Matteo Benci
 Orlando Testa
 Paolo Melchiorre
 Patrick Arminio
 Pietro Peterlongo
```

### Comparing `italia-0.2.0/pyproject.toml` & `italia-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "italia"
-version = "0.2.0"
+version = "0.2.1"
 description = "A fun package celebrating the Python Italia association and PyCon Italia"
 authors = [
     { name = "Python Italia", email = "help@pycon.it" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
```

### Comparing `italia-0.2.0/PKG-INFO` & `italia-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italia
-Version: 0.2.0
+Version: 0.2.1
 Summary: A fun package celebrating the Python Italia association and PyCon Italia
 Author-Email: Python Italia <help@pycon.it>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Italia: A Celebration of Python Italia 🇮🇹
```

