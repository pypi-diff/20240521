# Comparing `tmp/ferfereh-1.120.1.tar.gz` & `tmp/ferfereh-1.123.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferfereh-1.120.1.tar", last modified: Mon May 20 05:11:38 2024, max compression
+gzip compressed data, was "ferfereh-1.123.1.tar", last modified: Tue May 21 05:59:27 2024, max compression
```

## Comparing `ferfereh-1.120.1.tar` & `ferfereh-1.123.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 05:11:38.862838 ferfereh-1.120.1/
--rw-r--r--   0 kamangir   (502) staff       (20)      105 2024-05-20 05:11:38.862344 ferfereh-1.120.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4080 2024-02-26 00:07:14.000000 ferfereh-1.120.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 05:11:38.860026 ferfereh-1.120.1/ferfereh/
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-20 05:11:30.000000 ferfereh-1.120.1/ferfereh/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      959 2024-02-25 23:42:23.000000 ferfereh-1.120.1/ferfereh/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2768 2024-02-25 23:44:02.000000 ferfereh-1.120.1/ferfereh/coords.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:12.000000 ferfereh-1.120.1/ferfereh/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-02-27 00:15:30.000000 ferfereh-1.120.1/ferfereh/urls.py
--rw-r--r--   0 kamangir   (502) staff       (20)      642 2024-03-04 07:37:30.000000 ferfereh-1.120.1/ferfereh/utils.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 05:11:38.861848 ferfereh-1.120.1/ferfereh.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      105 2024-05-20 05:11:38.000000 ferfereh-1.120.1/ferfereh.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      261 2024-05-20 05:11:38.000000 ferfereh-1.120.1/ferfereh.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-20 05:11:38.000000 ferfereh-1.120.1/ferfereh.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-20 05:11:38.000000 ferfereh-1.120.1/ferfereh.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-20 05:11:38.862955 ferfereh-1.120.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      197 2024-02-25 23:46:49.000000 ferfereh-1.120.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 05:59:27.388739 ferfereh-1.123.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 05:59:00.000000 ferfereh-1.123.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4901 2024-05-21 05:59:27.388169 ferfereh-1.123.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4080 2024-02-26 00:07:14.000000 ferfereh-1.123.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 05:59:27.384581 ferfereh-1.123.1/ferfereh/
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-21 05:59:17.000000 ferfereh-1.123.1/ferfereh/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      959 2024-02-25 23:42:23.000000 ferfereh-1.123.1/ferfereh/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2768 2024-02-25 23:44:02.000000 ferfereh-1.123.1/ferfereh/coords.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:12.000000 ferfereh-1.123.1/ferfereh/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-02-27 00:15:30.000000 ferfereh-1.123.1/ferfereh/urls.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      642 2024-03-04 07:37:30.000000 ferfereh-1.123.1/ferfereh/utils.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 05:59:27.387265 ferfereh-1.123.1/ferfereh.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4901 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      336 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 05:52:18.000000 ferfereh-1.123.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:56:20.000000 ferfereh-1.123.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 05:59:27.388839 ferfereh-1.123.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-21 05:56:26.000000 ferfereh-1.123.1/setup.py
```

### Comparing `ferfereh-1.120.1/README.md` & `ferfereh-1.123.1/README.md`

 * *Files identical despite different names*

### Comparing `ferfereh-1.120.1/ferfereh/__main__.py` & `ferfereh-1.123.1/ferfereh/__main__.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.120.1/ferfereh/coords.py` & `ferfereh-1.123.1/ferfereh/coords.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.120.1/ferfereh/utils.py` & `ferfereh-1.123.1/ferfereh/utils.py`

 * *Files identical despite different names*

