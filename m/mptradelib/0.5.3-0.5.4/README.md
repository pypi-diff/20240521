# Comparing `tmp/mptradelib-0.5.3.tar.gz` & `tmp/mptradelib-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.5.3.tar", max compression
+gzip compressed data, was "mptradelib-0.5.4.tar", max compression
```

## Comparing `mptradelib-0.5.3.tar` & `mptradelib-0.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.3/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.3/mptradelib/__init__.py
--rw-r--r--   0        0        0     4562 2024-05-19 20:11:23.024752 mptradelib-0.5.3/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.3/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.3/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.3/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.3/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.3/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.3/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.3/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.3/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.3/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.3/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.3/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.3/mptradelib/livetrade.py
--rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.3/mptradelib/optimizers/__init__.py
--rw-r--r--   0        0        0     5533 2024-05-19 20:11:15.319126 mptradelib-0.5.3/mptradelib/optimizers/walkforward.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.3/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.3/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.3/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.5.3/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.3/mptradelib/utils/utils.py
--rw-r--r--   0        0        0      822 2024-05-19 20:15:14.649317 mptradelib-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.4/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4562 2024-05-19 20:11:23.024752 mptradelib-0.5.4/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.4/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.4/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.4/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.4/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.4/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.4/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.4/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.4/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.4/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.4/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.4/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.4/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.4/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     8133 2024-05-21 12:30:56.533060 mptradelib-0.5.4/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.4/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.4/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.4/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.5.4/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.4/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0      822 2024-05-21 12:31:03.905881 mptradelib-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.4/PKG-INFO
```

### Comparing `mptradelib-0.5.3/README.md` & `mptradelib-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/backtest.py` & `mptradelib-0.5.4/mptradelib/backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/broker/broker.py` & `mptradelib-0.5.4/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/broker/session.py` & `mptradelib-0.5.4/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/broker/shoonya.py` & `mptradelib-0.5.4/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/broker/ticker.py` & `mptradelib-0.5.4/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/cli/new.py` & `mptradelib-0.5.4/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.5.4/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.5.4/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.5.4/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/feed.py` & `mptradelib-0.5.4/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/livetrade.py` & `mptradelib-0.5.4/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/test_renko.py` & `mptradelib-0.5.4/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/utils/simulated_trades.py` & `mptradelib-0.5.4/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/utils/tearsheet.py` & `mptradelib-0.5.4/mptradelib/utils/tearsheet.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/mptradelib/utils/utils.py` & `mptradelib-0.5.4/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.3/pyproject.toml` & `mptradelib-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.5.3"
+version = "0.5.4"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.5.3/PKG-INFO` & `mptradelib-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.5.3
+Version: 0.5.4
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

