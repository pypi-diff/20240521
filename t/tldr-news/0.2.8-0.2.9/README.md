# Comparing `tmp/tldr_news-0.2.8.tar.gz` & `tmp/tldr_news-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldr_news-0.2.8.tar", max compression
+gzip compressed data, was "tldr_news-0.2.9.tar", max compression
```

## Comparing `tldr_news-0.2.8.tar` & `tldr_news-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1046 2024-01-23 03:03:28.336153 tldr_news-0.2.8/README.md
--rw-r--r--   0        0        0     1195 2024-01-23 03:03:52.764260 tldr_news-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       22 2024-01-23 03:03:52.764260 tldr_news-0.2.8/tldr_news/__init__.py
--rw-r--r--   0        0        0     1081 2024-01-23 03:03:28.340153 tldr_news-0.2.8/tldr_news/cli.py
--rw-r--r--   0        0        0      204 2024-01-23 03:03:28.340153 tldr_news-0.2.8/tldr_news/main.css
--rw-r--r--   0        0        0      698 2024-01-23 03:03:28.340153 tldr_news-0.2.8/tldr_news/ui.py
--rw-r--r--   0        0        0     1810 2024-01-23 03:03:28.340153 tldr_news-0.2.8/tldr_news/utils.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 tldr_news-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1046 2024-02-22 01:08:26.570061 tldr_news-0.2.9/README.md
+-rw-r--r--   0        0        0     1195 2024-02-22 01:08:51.890046 tldr_news-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-02-22 01:08:51.890046 tldr_news-0.2.9/tldr_news/__init__.py
+-rw-r--r--   0        0        0     1081 2024-02-22 01:08:26.574061 tldr_news-0.2.9/tldr_news/cli.py
+-rw-r--r--   0        0        0      204 2024-02-22 01:08:26.574061 tldr_news-0.2.9/tldr_news/main.css
+-rw-r--r--   0        0        0      698 2024-02-22 01:08:26.574061 tldr_news-0.2.9/tldr_news/ui.py
+-rw-r--r--   0        0        0     1810 2024-02-22 01:08:26.574061 tldr_news-0.2.9/tldr_news/utils.py
+-rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 tldr_news-0.2.9/PKG-INFO
```

### Comparing `tldr_news-0.2.8/README.md` & `tldr_news-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.8/pyproject.toml` & `tldr_news-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tldr-news"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["Harry Tran <huytran.quang080199@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tldr_news"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tldr_news-0.2.8/tldr_news/cli.py` & `tldr_news-0.2.9/tldr_news/cli.py`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.8/tldr_news/ui.py` & `tldr_news-0.2.9/tldr_news/ui.py`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.8/tldr_news/utils.py` & `tldr_news-0.2.9/tldr_news/utils.py`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.8/PKG-INFO` & `tldr_news-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldr-news
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Harry Tran
 Author-email: huytran.quang080199@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

