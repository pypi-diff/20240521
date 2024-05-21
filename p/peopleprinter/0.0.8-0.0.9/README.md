# Comparing `tmp/peopleprinter-0.0.8.tar.gz` & `tmp/peopleprinter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopleprinter-0.0.8.tar", last modified: Sun May 12 16:31:02 2024, max compression
+gzip compressed data, was "peopleprinter-0.0.9.tar", last modified: Tue May 21 16:45:56 2024, max compression
```

## Comparing `peopleprinter-0.0.8.tar` & `peopleprinter-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.999618 peopleprinter-0.0.8/
--rw-rw-rw-   0        0        0      498 2024-05-12 16:31:01.999618 peopleprinter-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.953761 peopleprinter-0.0.8/peopleprinter/
--rw-rw-rw-   0        0        0       86 2024-05-12 16:29:31.000000 peopleprinter-0.0.8/peopleprinter/__init__.py
--rw-rw-rw-   0        0        0     1806 2024-05-12 16:20:11.000000 peopleprinter-0.0.8/peopleprinter/main.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.972690 peopleprinter-0.0.8/peopleprinter/manufacturers/
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.985663 peopleprinter-0.0.8/peopleprinter/manufacturers/HP/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/HP/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/HP/major_hp.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.991661 peopleprinter-0.0.8/peopleprinter/manufacturers/KYOCERA/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/KYOCERA/__init__.py
--rw-rw-rw-   0        0        0     3736 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py
--rw-rw-rw-   0        0        0     2413 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/KYOCERA/major_kyocera.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.993633 peopleprinter-0.0.8/peopleprinter/manufacturers/PANTUM/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/PANTUM/__init__.py
--rw-rw-rw-   0        0        0     1018 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/PANTUM/major_pantum.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.995633 peopleprinter-0.0.8/peopleprinter/manufacturers/Xerox/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/Xerox/__init__.py
--rw-rw-rw-   0        0        0     3050 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/Xerox/major_xerox.py
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/manufacturers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.996625 peopleprinter-0.0.8/peopleprinter/src/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.8/peopleprinter/src/__init__.py
--rw-rw-rw-   0        0        0     2334 2024-05-12 16:24:07.000000 peopleprinter-0.0.8/peopleprinter/sub_main.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:01.997623 peopleprinter-0.0.8/peopleprinter.egg-info/
--rw-rw-rw-   0        0        0      498 2024-05-12 16:31:01.000000 peopleprinter-0.0.8/peopleprinter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2024-05-12 16:31:01.000000 peopleprinter-0.0.8/peopleprinter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:31:01.000000 peopleprinter-0.0.8/peopleprinter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 16:31:01.000000 peopleprinter-0.0.8/peopleprinter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      575 2024-05-12 16:30:55.000000 peopleprinter-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 16:31:02.000622 peopleprinter-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.982993 peopleprinter-0.0.9/
+-rw-rw-rw-   0        0        0      498 2024-05-21 16:45:56.978989 peopleprinter-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-05-21 15:46:06.000000 peopleprinter-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.927986 peopleprinter-0.0.9/peopleprinter/
+-rw-rw-rw-   0        0        0       67 2024-05-21 08:51:57.000000 peopleprinter-0.0.9/peopleprinter/__init__.py
+-rw-rw-rw-   0        0        0     3825 2024-05-21 15:49:09.000000 peopleprinter-0.0.9/peopleprinter/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.948986 peopleprinter-0.0.9/peopleprinter/manufacturers/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.951987 peopleprinter-0.0.9/peopleprinter/manufacturers/HP/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/HP/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/HP/major_hp.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.959988 peopleprinter-0.0.9/peopleprinter/manufacturers/KYOCERA/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/KYOCERA/__init__.py
+-rw-rw-rw-   0        0        0     3736 2024-05-21 15:46:06.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py
+-rw-rw-rw-   0        0        0     2413 2024-05-21 15:46:06.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/KYOCERA/major_kyocera.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.962987 peopleprinter-0.0.9/peopleprinter/manufacturers/PANTUM/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/PANTUM/__init__.py
+-rw-rw-rw-   0        0        0     1018 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/PANTUM/major_pantum.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.966985 peopleprinter-0.0.9/peopleprinter/manufacturers/Xerox/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/Xerox/__init__.py
+-rw-rw-rw-   0        0        0     3050 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/Xerox/major_xerox.py
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/manufacturers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.971989 peopleprinter-0.0.9/peopleprinter/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:57:41.000000 peopleprinter-0.0.9/peopleprinter/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:45:56.975989 peopleprinter-0.0.9/peopleprinter.egg-info/
+-rw-rw-rw-   0        0        0      498 2024-05-21 16:45:56.000000 peopleprinter-0.0.9/peopleprinter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2024-05-21 16:45:56.000000 peopleprinter-0.0.9/peopleprinter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:45:56.000000 peopleprinter-0.0.9/peopleprinter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 16:45:56.000000 peopleprinter-0.0.9/peopleprinter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      569 2024-05-21 16:44:28.000000 peopleprinter-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:45:56.982993 peopleprinter-0.0.9/setup.cfg
```

### Comparing `peopleprinter-0.0.8/peopleprinter/manufacturers/HP/major_hp.py` & `peopleprinter-0.0.9/peopleprinter/manufacturers/HP/major_hp.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.8/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py` & `peopleprinter-0.0.9/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.8/peopleprinter/manufacturers/KYOCERA/major_kyocera.py` & `peopleprinter-0.0.9/peopleprinter/manufacturers/KYOCERA/major_kyocera.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.8/peopleprinter/manufacturers/PANTUM/major_pantum.py` & `peopleprinter-0.0.9/peopleprinter/manufacturers/PANTUM/major_pantum.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.8/peopleprinter/manufacturers/Xerox/major_xerox.py` & `peopleprinter-0.0.9/peopleprinter/manufacturers/Xerox/major_xerox.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.8/peopleprinter.egg-info/SOURCES.txt` & `peopleprinter-0.0.9/peopleprinter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 README.md
 pyproject.toml
 peopleprinter/__init__.py
 peopleprinter/main.py
-peopleprinter/sub_main.py
 peopleprinter.egg-info/PKG-INFO
 peopleprinter.egg-info/SOURCES.txt
 peopleprinter.egg-info/dependency_links.txt
 peopleprinter.egg-info/top_level.txt
 peopleprinter/manufacturers/__init__.py
 peopleprinter/manufacturers/HP/__init__.py
 peopleprinter/manufacturers/HP/major_hp.py
```

### Comparing `peopleprinter-0.0.8/pyproject.toml` & `peopleprinter-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-requires = ["bs4", "requests", "re"]
+requires = ["bs4", "requests"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peopleprinter"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Guazah", email="guazah@gmail.com" },
 ]
 description = "Parsing printers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

