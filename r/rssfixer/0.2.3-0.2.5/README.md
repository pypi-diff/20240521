# Comparing `tmp/rssfixer-0.2.3.tar.gz` & `tmp/rssfixer-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.2.3.tar", max compression
+gzip compressed data, was "rssfixer-0.2.5.tar", max compression
```

## Comparing `rssfixer-0.2.3.tar` & `rssfixer-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1059 2023-05-02 04:17:59.003602 rssfixer-0.2.3/LICENSE
--rw-r--r--   0        0        0    11524 2023-08-15 04:02:10.511819 rssfixer-0.2.3/README.md
--rw-r--r--   0        0        0     2851 2023-10-03 08:28:59.327805 rssfixer-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       98 2023-05-02 04:17:59.006244 rssfixer-0.2.3/src/rssfixer/__init__.py
--rw-r--r--   0        0        0    15117 2023-08-15 04:02:10.514499 rssfixer-0.2.3/src/rssfixer/rss.py
--rw-r--r--   0        0        0    12174 1970-01-01 00:00:00.000000 rssfixer-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-02 04:17:59.003602 rssfixer-0.2.5/LICENSE
+-rw-r--r--   0        0        0    11524 2023-08-15 04:02:10.511819 rssfixer-0.2.5/README.md
+-rw-r--r--   0        0        0     2851 2024-05-21 09:56:45.733444 rssfixer-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-05-02 04:17:59.006244 rssfixer-0.2.5/src/rssfixer/__init__.py
+-rw-r--r--   0        0        0    15117 2023-08-15 04:02:10.514499 rssfixer-0.2.5/src/rssfixer/rss.py
+-rw-r--r--   0        0        0    12225 1970-01-01 00:00:00.000000 rssfixer-0.2.5/PKG-INFO
```

### Comparing `rssfixer-0.2.3/LICENSE` & `rssfixer-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.2.3/README.md` & `rssfixer-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rssfixer-0.2.3/pyproject.toml` & `rssfixer-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -71,25 +71,25 @@
 line-length = 120
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 [tool.poetry]
 name = "rssfixer"
-version = "0.2.3"
+version = "0.2.5"
 description = "Generate RSS for blogs without a feed."
 authors = ["Peter Reuterås <peter@reuteras.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-beautifulsoup4 = "4.12.2"
+beautifulsoup4 = "4.12.3"
 feedgen = "0.9.0"
-requests = "2.31.0"
+requests = "2.32.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 bandit = "*"
 build = "*"
```

### Comparing `rssfixer-0.2.3/src/rssfixer/rss.py` & `rssfixer-0.2.5/src/rssfixer/rss.py`

 * *Files identical despite different names*

### Comparing `rssfixer-0.2.3/PKG-INFO` & `rssfixer-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.2.3
+Version: 0.2.5
 Summary: Generate RSS for blogs without a feed.
 License: MIT
 Author: Peter Reuterås
 Author-email: peter@reuteras.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (==4.12.2)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: beautifulsoup4 (==4.12.3)
 Requires-Dist: feedgen (==0.9.0)
-Requires-Dist: requests (==2.31.0)
+Requires-Dist: requests (==2.32.1)
 Description-Content-Type: text/markdown
 
 # rssfixer
 
 <!-- CODE:BASH:START -->
 <!-- echo '[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)' -->
 <!-- echo '![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)' -->
```

