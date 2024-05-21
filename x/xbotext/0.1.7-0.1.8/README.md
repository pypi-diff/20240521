# Comparing `tmp/xbotext-0.1.7.tar.gz` & `tmp/xbotext-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbotext-0.1.7.tar", max compression
+gzip compressed data, was "xbotext-0.1.8.tar", max compression
```

## Comparing `xbotext-0.1.7.tar` & `xbotext-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      234 2024-05-08 03:17:22.621333 xbotext-0.1.7/README.md
--rw-r--r--   0        0        0      255 2024-05-08 03:21:32.671245 xbotext-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      100 2024-05-08 01:56:54.282987 xbotext-0.1.7/xbotext/__init__.py
--rw-r--r--   0        0        0     2511 2024-05-08 03:19:58.231279 xbotext-0.1.7/xbotext/app.py
--rw-r--r--   0        0        0     3336 2024-05-07 12:12:34.225851 xbotext-0.1.7/xbotext/cache.py
--rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.7/xbotext/chromium.py
--rw-r--r--   0        0        0        0 2024-05-08 01:56:35.912993 xbotext-0.1.7/xbotext/excel.py
--rw-r--r--   0        0        0      605 2024-05-07 11:55:00.763736 xbotext-0.1.7/xbotext/regedit.py
--rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.7/xbotext/sofaware.py
--rw-r--r--   0        0        0      101 2024-05-07 11:55:00.763736 xbotext-0.1.7/xbotext/system.py
--rw-r--r--   0        0        0      541 2024-05-08 01:44:20.433247 xbotext-0.1.7/xbotext/web.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 xbotext-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      234 2024-05-08 03:17:22.621333 xbotext-0.1.8/README.md
+-rw-r--r--   0        0        0      255 2024-05-21 06:08:22.553882 xbotext-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-05-08 01:56:54.282987 xbotext-0.1.8/xbotext/__init__.py
+-rw-r--r--   0        0        0     3129 2024-05-21 06:07:57.873897 xbotext-0.1.8/xbotext/app.py
+-rw-r--r--   0        0        0     3336 2024-05-07 12:12:34.225851 xbotext-0.1.8/xbotext/cache.py
+-rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.8/xbotext/chromium.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:56:35.912993 xbotext-0.1.8/xbotext/excel.py
+-rw-r--r--   0        0        0     1357 2024-05-08 03:44:53.410766 xbotext-0.1.8/xbotext/os.py
+-rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.8/xbotext/sofaware.py
+-rw-r--r--   0        0        0      541 2024-05-08 01:44:20.433247 xbotext-0.1.8/xbotext/web.py
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 xbotext-0.1.8/PKG-INFO
```

### Comparing `xbotext-0.1.7/xbotext/cache.py` & `xbotext-0.1.8/xbotext/cache.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.7/xbotext/chromium.py` & `xbotext-0.1.8/xbotext/chromium.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.7/xbotext/web.py` & `xbotext-0.1.8/xbotext/web.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.7/PKG-INFO` & `xbotext-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbotext
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: woni
 Author-email: 320753691@qq.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

