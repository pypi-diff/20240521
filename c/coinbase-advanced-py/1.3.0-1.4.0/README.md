# Comparing `tmp/coinbase-advanced-py-1.3.0.tar.gz` & `tmp/coinbase-advanced-py-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinbase-advanced-py-1.3.0.tar", last modified: Mon May  6 20:13:54 2024, max compression
+gzip compressed data, was "coinbase-advanced-py-1.4.0.tar", last modified: Tue May 21 15:25:00 2024, max compression
```

## Comparing `coinbase-advanced-py-1.3.0.tar` & `coinbase-advanced-py-1.4.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.203229 coinbase-advanced-py-1.3.0/
--rw-r--r--   0 urischwartz   (501) staff       (20)    11343 2023-12-07 15:44:33.000000 coinbase-advanced-py-1.3.0/LICENSE.md
--rw-r--r--   0 urischwartz   (501) staff       (20)    17508 2024-05-06 20:13:54.202543 coinbase-advanced-py-1.3.0/PKG-INFO
--rw-r--r--   0 urischwartz   (501) staff       (20)    16394 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/README.md
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.188504 coinbase-advanced-py-1.3.0/coinbase/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-11-21 15:58:27.000000 coinbase-advanced-py-1.3.0/coinbase/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)       22 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/__version__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2169 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/api_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      773 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/constants.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2350 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.3.0/coinbase/jwt_generator.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.192585 coinbase-advanced-py-1.3.0/coinbase/rest/
--rwxr-xr-x   0 urischwartz   (501) staff       (20)     3379 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1466 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/accounts.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2974 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/convert.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      927 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/fees.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4806 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.3.0/coinbase/rest/futures.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1684 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/market_data.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    85326 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/orders.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1280 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.3.0/coinbase/rest/payments.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2866 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/perpetuals.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4125 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/portfolios.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     3223 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/products.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     5457 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/public.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     7258 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/rest_base.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.193395 coinbase-advanced-py-1.3.0/coinbase/websocket/
--rw-r--r--   0 urischwartz   (501) staff       (20)     1013 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/coinbase/websocket/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    15436 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/websocket/channels.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    20143 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/websocket/websocket_base.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.195039 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/
--rw-r--r--   0 urischwartz   (501) staff       (20)    17508 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/PKG-INFO
--rw-r--r--   0 urischwartz   (501) staff       (20)     1339 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/SOURCES.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)        1 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/dependency_links.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)      167 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/requires.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)       15 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/top_level.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)       38 2024-05-06 20:13:54.203355 coinbase-advanced-py-1.3.0/setup.cfg
--rw-r--r--   0 urischwartz   (501) staff       (20)     1642 2024-02-12 19:40:21.000000 coinbase-advanced-py-1.3.0/setup.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.195575 coinbase-advanced-py-1.3.0/tests/
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.199953 coinbase-advanced-py-1.3.0/tests/rest/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-12-18 21:35:16.000000 coinbase-advanced-py-1.3.0/tests/rest/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1531 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/rest/test_accounts.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2924 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/rest/test_convert.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      968 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/rest/test_fees.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     5011 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.3.0/tests/rest/test_futures.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1711 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/rest/test_market_data.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    77962 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/rest/test_orders.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1392 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.3.0/tests/rest/test_payments.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     3268 2024-02-01 19:31:57.000000 coinbase-advanced-py-1.3.0/tests/rest/test_perpetuals.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4429 2024-01-29 17:15:12.000000 coinbase-advanced-py-1.3.0/tests/rest/test_portfolios.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2701 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/rest/test_products.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     5600 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/rest/test_public.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     7860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/rest/test_rest_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/test_api_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1749 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.3.0/tests/test_jwt_generator.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.201259 coinbase-advanced-py-1.3.0/tests/websocket/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/websocket/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2217 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/websocket/mock_ws_server.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     6651 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/websocket/test_channels.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    20856 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/websocket/test_websocket_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.580436 coinbase-advanced-py-1.4.0/
+-rw-r--r--   0 urischwartz   (501) staff       (20)    11343 2023-12-07 15:44:33.000000 coinbase-advanced-py-1.4.0/LICENSE.md
+-rw-r--r--   0 urischwartz   (501) staff       (20)    17519 2024-05-21 15:25:00.580057 coinbase-advanced-py-1.4.0/PKG-INFO
+-rw-r--r--   0 urischwartz   (501) staff       (20)    16405 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/README.md
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.565272 coinbase-advanced-py-1.4.0/coinbase/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-11-21 15:58:27.000000 coinbase-advanced-py-1.4.0/coinbase/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)       22 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/__version__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2169 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/coinbase/api_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      773 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/coinbase/constants.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2350 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.4.0/coinbase/jwt_generator.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.569720 coinbase-advanced-py-1.4.0/coinbase/rest/
+-rwxr-xr-x   0 urischwartz   (501) staff       (20)     3572 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1454 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/accounts.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2956 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/convert.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      921 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/fees.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7002 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/futures.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1672 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/market_data.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    85103 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/orders.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1268 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/payments.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4364 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/perpetuals.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4089 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/portfolios.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     3199 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/products.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     5421 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/public.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7258 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/coinbase/rest/rest_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.570735 coinbase-advanced-py-1.4.0/coinbase/websocket/
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1013 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/coinbase/websocket/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    15244 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/websocket/channels.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    20143 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/coinbase/websocket/websocket_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.572008 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/
+-rw-r--r--   0 urischwartz   (501) staff       (20)    17519 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/PKG-INFO
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1339 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/SOURCES.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)        1 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/dependency_links.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)      167 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/requires.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)       15 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/top_level.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)       38 2024-05-21 15:25:00.580513 coinbase-advanced-py-1.4.0/setup.cfg
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1642 2024-02-12 19:40:21.000000 coinbase-advanced-py-1.4.0/setup.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.572448 coinbase-advanced-py-1.4.0/tests/
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.577388 coinbase-advanced-py-1.4.0/tests/rest/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-12-18 21:35:16.000000 coinbase-advanced-py-1.4.0/tests/rest/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1531 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/rest/test_accounts.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2924 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/rest/test_convert.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      968 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/rest/test_fees.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7243 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/tests/rest/test_futures.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1711 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/rest/test_market_data.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    77962 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/rest/test_orders.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1392 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.4.0/tests/rest/test_payments.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4950 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/tests/rest/test_perpetuals.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4429 2024-01-29 17:15:12.000000 coinbase-advanced-py-1.4.0/tests/rest/test_portfolios.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2701 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/rest/test_products.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     5600 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/rest/test_public.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/rest/test_rest_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/test_api_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1749 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.4.0/tests/test_jwt_generator.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.578821 coinbase-advanced-py-1.4.0/tests/websocket/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/websocket/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2217 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/websocket/mock_ws_server.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     6651 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/websocket/test_channels.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    20856 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/websocket/test_websocket_base.py
```

### Comparing `coinbase-advanced-py-1.3.0/LICENSE.md` & `coinbase-advanced-py-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/PKG-INFO` & `coinbase-advanced-py-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-advanced-py
-Version: 1.3.0
+Version: 1.4.0
 Summary: Coinbase Advanced API Python SDK
 Home-page: https://github.com/coinbase/coinbase-advanced-py
 Author: Coinbase
 License: Apache 2.0
 Keywords: Coinbase,Advanced Trade,API,Advanced API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -29,30 +29,30 @@
 Requires-Dist: isort==5.12.0; extra == "lint"
 
 # Coinbase Advanced API Python SDK
 [![PyPI version](https://badge.fury.io/py/coinbase-advanced-py.svg)](https://badge.fury.io/py/coinbase-advanced-py)
 [![License](https://img.shields.io/badge/License-Apache%202.0-green.svg)](https://opensource.org/license/apache-2-0/)
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 
-Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/welcome).
-This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
+Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cdp.coinbase.com/advanced-trade/docs/welcome).
+This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview).
 
 For thorough documentation of all available functions, refer to the following link: https://coinbase.github.io/coinbase-advanced-py
 
 ___
 ## Installation
 
 ```bash
 pip3 install coinbase-advanced-py
 ```
 
 ___
 ## Coinbase Developer Platform (CDP) API Keys
 
-This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
+This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cdp.coinbase.com/advanced-trade/docs/auth).
 Make sure to save your API key and secret in a safe place. You will not be able to retrieve your secret again.
 
 WARNING: We do not recommend that you save your API secrets directly in your code outside of testing purposes. Best practice is to use a secrets manager and access your secrets that way. You should be careful about exposing your secrets publicly if posting code that leverages this library.
 
 Optional: Set your API key and secret in your environment (make sure to put these in quotation marks). For example:
 ```bash
 export COINBASE_API_KEY="organizations/{org_id}/apiKeys/{key_id}"
@@ -100,15 +100,15 @@
 print(dumps(accounts, indent=2))
 
 order = client.market_order_buy(client_order_id="clientOrderId", product_id="BTC-USD", quote_size="1")
 print(dumps(order, indent=2))
 ```
 This code calls the `get_accounts` and `market_order_buy` endpoints.
 
-Refer to the [Advanced API Reference](https://docs.cloud.coinbase.com/advanced-trade-api/reference) for detailed information on each exposed endpoint.
+Refer to the [Advanced API Reference](https://docs.cdp.coinbase.com/advanced-trade/reference) for detailed information on each exposed endpoint.
 Look in the `coinbase.rest` module to see the API hooks that are exposed.
 
 ### Passing in additional parameters
 Use `kwargs` to pass in any additional parameters. For example:
 ```python
 kwargs = {
     "param1": 10,
@@ -120,26 +120,26 @@
 ### Generic REST Calls
 You can make generic REST calls using the `get`, `post`, `put`, and `delete` methods. For example:
 ```python
 market_trades = client.get("/api/v3/brokerage/products/BTC-USD/ticker", params={"limit": 5})
 
 portfolio = client.post("/api/v3/brokerage/portfolios", data={"name": "TestPortfolio"})
 ```
-Here we are calling the [GetMarketTrades](https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getmarkettrades) and [CreatePortfolio](https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_createportfolio) endpoints through the generic REST functions.
+Here we are calling the [GetMarketTrades](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getmarkettrades) and [CreatePortfolio](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_createportfolio) endpoints through the generic REST functions.
 Once again, the built-in way to query these through the SDK would be:
 ```python
 market_trades = client.get_market_trades(product_id="BTC-USD", limit=5)
 
 portfolio = client.create_portfolio(name="TestPortfolio")
 ```
 
 ___
 ## WebSocket API Client
-We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
-Refer to the [Advanced Trade WebSocket Channels](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels) page for detailed information on each offered channel.
+We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview).
+Refer to the [Advanced Trade WebSocket Channels](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels) page for detailed information on each offered channel.
 
 In your code, import the WSClient class and instantiate it. The WSClient requires an API key and secret to be passed in as arguments. You can also use a key file or environment variables as described in the RESTClient instructions above.
 
 You must specify an `on_message` function that will be called when a message is received from the WebSocket API. This function must take in a single argument, which will be the raw message received from the WebSocket API. For example:
 ```python
 from coinbase.websocket import WSClient
 
@@ -267,15 +267,15 @@
 ws_client = WSClient(api_key=api_key, api_secret=api_secret, on_message=on_message, verbose=True)
 ```
 
 ___
 ## Authentication
 Authentication of CDP API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
 
-However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
+However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
 ```python
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 uri = "/api/v3/brokerage/orders"
@@ -293,15 +293,15 @@
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 jwt = jwt_generator.build_ws_jwt(api_key, api_secret)
 ```
-Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview#sending-messages-using-cloud-api-keys) for more details.
+Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview#sending-messages-with-cdp-keys) for more details.
 
 ___
 ## Accessing public endpoints without authentication
 
 Both clients contain public endpoints which can be accessed without authentication. 
 
 To do so, simply initialize the clients without providing any API keys as arguments. 
@@ -309,36 +309,36 @@
 **_Notes:_**
 
 - Making calls to private endpoints or channels while unauthenticated will return an error
 - Unauthenticated requests are rate-limited more aggressively. Because of this we recommend that you authenticate your requests
 
 ### REST Client
 
-In the REST client, here is an example calling [Get Public Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
+In the REST client, here is an example calling [Get Public Products](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
 It does _not_ require authentication and is the public counterpart to 
-[Get Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
+[Get Products](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
 
 Both endpoints return the same data.
 
 
 ```
 from coinbase.rest import RESTClient
 
 client = RESTClient()
 
 public_products = client.get_public_products()
 print(public_products)
 ```
-_Full list of all public REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
+_Full list of all public REST endpoints [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
 
-_Rate limit details for REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
+_Rate limit details for REST endpoints [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
 
 ### Websocket Client
 
-In the Websocket client, here is an example subscribing to the [ticker](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
+In the Websocket client, here is an example subscribing to the [ticker](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
 Unlike the REST client, Websocket channels handle both authenticated and unauthenticated requests. 
 At the moment, most channels in the Websocket client are public and can be used without keys.
 
 ```
 import time
 from coinbase.websocket import WSClient
 
@@ -352,22 +352,22 @@
 
 time.sleep(10)
 
 client.ticker_unsubscribe(product_ids=["BTC-USD"])
 client.close()
 ```
 
-_Full list of all public Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels)_
+_Full list of all public Websocket channels [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels)_
 
-_Rate limit details for Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-rate-limits)_
+_Rate limit details for Websocket channels [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-rate-limits)_
 
 
 ___
 ## Changelog
 For a detailed list of changes, see the [Changelog](https://github.com/coinbase/coinbase-advanced-py/blob/master/CHANGELOG.md).
 
 ___
 ## Contributing
 
 If you've found a bug within this project, open an issue on this repo and add the "bug" label to it.
 If you would like to request a new feature, open an issue on this repo and add the "enhancement" label to it.
-Direct concerns or questions on the API to the [Advanced API Developer Forum](https://forums.coinbasecloud.dev/c/advanced-trade-api/20).
+Direct concerns or questions on the API to the [Advanced API Discord](https://discord.com/channels/1220414409550336183/1220464268743278613) (use this [invite link](https://discord.com/invite/cdp) if it's your first time accessing the Discord).
```

### Comparing `coinbase-advanced-py-1.3.0/README.md` & `coinbase-advanced-py-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Coinbase Advanced API Python SDK
 [![PyPI version](https://badge.fury.io/py/coinbase-advanced-py.svg)](https://badge.fury.io/py/coinbase-advanced-py)
 [![License](https://img.shields.io/badge/License-Apache%202.0-green.svg)](https://opensource.org/license/apache-2-0/)
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 
-Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/welcome).
-This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
+Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cdp.coinbase.com/advanced-trade/docs/welcome).
+This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview).
 
 For thorough documentation of all available functions, refer to the following link: https://coinbase.github.io/coinbase-advanced-py
 
 ___
 ## Installation
 
 ```bash
 pip3 install coinbase-advanced-py
 ```
 
 ___
 ## Coinbase Developer Platform (CDP) API Keys
 
-This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
+This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cdp.coinbase.com/advanced-trade/docs/auth).
 Make sure to save your API key and secret in a safe place. You will not be able to retrieve your secret again.
 
 WARNING: We do not recommend that you save your API secrets directly in your code outside of testing purposes. Best practice is to use a secrets manager and access your secrets that way. You should be careful about exposing your secrets publicly if posting code that leverages this library.
 
 Optional: Set your API key and secret in your environment (make sure to put these in quotation marks). For example:
 ```bash
 export COINBASE_API_KEY="organizations/{org_id}/apiKeys/{key_id}"
@@ -70,15 +70,15 @@
 print(dumps(accounts, indent=2))
 
 order = client.market_order_buy(client_order_id="clientOrderId", product_id="BTC-USD", quote_size="1")
 print(dumps(order, indent=2))
 ```
 This code calls the `get_accounts` and `market_order_buy` endpoints.
 
-Refer to the [Advanced API Reference](https://docs.cloud.coinbase.com/advanced-trade-api/reference) for detailed information on each exposed endpoint.
+Refer to the [Advanced API Reference](https://docs.cdp.coinbase.com/advanced-trade/reference) for detailed information on each exposed endpoint.
 Look in the `coinbase.rest` module to see the API hooks that are exposed.
 
 ### Passing in additional parameters
 Use `kwargs` to pass in any additional parameters. For example:
 ```python
 kwargs = {
     "param1": 10,
@@ -90,26 +90,26 @@
 ### Generic REST Calls
 You can make generic REST calls using the `get`, `post`, `put`, and `delete` methods. For example:
 ```python
 market_trades = client.get("/api/v3/brokerage/products/BTC-USD/ticker", params={"limit": 5})
 
 portfolio = client.post("/api/v3/brokerage/portfolios", data={"name": "TestPortfolio"})
 ```
-Here we are calling the [GetMarketTrades](https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getmarkettrades) and [CreatePortfolio](https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_createportfolio) endpoints through the generic REST functions.
+Here we are calling the [GetMarketTrades](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getmarkettrades) and [CreatePortfolio](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_createportfolio) endpoints through the generic REST functions.
 Once again, the built-in way to query these through the SDK would be:
 ```python
 market_trades = client.get_market_trades(product_id="BTC-USD", limit=5)
 
 portfolio = client.create_portfolio(name="TestPortfolio")
 ```
 
 ___
 ## WebSocket API Client
-We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
-Refer to the [Advanced Trade WebSocket Channels](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels) page for detailed information on each offered channel.
+We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview).
+Refer to the [Advanced Trade WebSocket Channels](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels) page for detailed information on each offered channel.
 
 In your code, import the WSClient class and instantiate it. The WSClient requires an API key and secret to be passed in as arguments. You can also use a key file or environment variables as described in the RESTClient instructions above.
 
 You must specify an `on_message` function that will be called when a message is received from the WebSocket API. This function must take in a single argument, which will be the raw message received from the WebSocket API. For example:
 ```python
 from coinbase.websocket import WSClient
 
@@ -237,15 +237,15 @@
 ws_client = WSClient(api_key=api_key, api_secret=api_secret, on_message=on_message, verbose=True)
 ```
 
 ___
 ## Authentication
 Authentication of CDP API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
 
-However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
+However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
 ```python
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 uri = "/api/v3/brokerage/orders"
@@ -263,15 +263,15 @@
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 jwt = jwt_generator.build_ws_jwt(api_key, api_secret)
 ```
-Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview#sending-messages-using-cloud-api-keys) for more details.
+Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview#sending-messages-with-cdp-keys) for more details.
 
 ___
 ## Accessing public endpoints without authentication
 
 Both clients contain public endpoints which can be accessed without authentication. 
 
 To do so, simply initialize the clients without providing any API keys as arguments. 
@@ -279,36 +279,36 @@
 **_Notes:_**
 
 - Making calls to private endpoints or channels while unauthenticated will return an error
 - Unauthenticated requests are rate-limited more aggressively. Because of this we recommend that you authenticate your requests
 
 ### REST Client
 
-In the REST client, here is an example calling [Get Public Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
+In the REST client, here is an example calling [Get Public Products](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
 It does _not_ require authentication and is the public counterpart to 
-[Get Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
+[Get Products](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
 
 Both endpoints return the same data.
 
 
 ```
 from coinbase.rest import RESTClient
 
 client = RESTClient()
 
 public_products = client.get_public_products()
 print(public_products)
 ```
-_Full list of all public REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
+_Full list of all public REST endpoints [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
 
-_Rate limit details for REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
+_Rate limit details for REST endpoints [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
 
 ### Websocket Client
 
-In the Websocket client, here is an example subscribing to the [ticker](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
+In the Websocket client, here is an example subscribing to the [ticker](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
 Unlike the REST client, Websocket channels handle both authenticated and unauthenticated requests. 
 At the moment, most channels in the Websocket client are public and can be used without keys.
 
 ```
 import time
 from coinbase.websocket import WSClient
 
@@ -322,22 +322,22 @@
 
 time.sleep(10)
 
 client.ticker_unsubscribe(product_ids=["BTC-USD"])
 client.close()
 ```
 
-_Full list of all public Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels)_
+_Full list of all public Websocket channels [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels)_
 
-_Rate limit details for Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-rate-limits)_
+_Rate limit details for Websocket channels [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-rate-limits)_
 
 
 ___
 ## Changelog
 For a detailed list of changes, see the [Changelog](https://github.com/coinbase/coinbase-advanced-py/blob/master/CHANGELOG.md).
 
 ___
 ## Contributing
 
 If you've found a bug within this project, open an issue on this repo and add the "bug" label to it.
 If you would like to request a new feature, open an issue on this repo and add the "enhancement" label to it.
-Direct concerns or questions on the API to the [Advanced API Developer Forum](https://forums.coinbasecloud.dev/c/advanced-trade-api/20).
+Direct concerns or questions on the API to the [Advanced API Discord](https://discord.com/channels/1220414409550336183/1220464268743278613) (use this [invite link](https://discord.com/invite/cdp) if it's your first time accessing the Discord).
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/api_base.py` & `coinbase-advanced-py-1.4.0/coinbase/api_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/coinbase/constants.py` & `coinbase-advanced-py-1.4.0/coinbase/constants.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/coinbase/jwt_generator.py` & `coinbase-advanced-py-1.4.0/coinbase/jwt_generator.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/__init__.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 class RESTClient(RESTBase):
     from .accounts import get_account, get_accounts
     from .convert import commit_convert_trade, create_convert_quote, get_convert_trade
     from .fees import get_transaction_summary
     from .futures import (
         cancel_pending_futures_sweep,
         close_position,
+        get_current_margin_window,
         get_futures_balance_summary,
         get_futures_position,
+        get_intraday_margin_setting,
         list_futures_positions,
         list_futures_sweeps,
         schedule_futures_sweep,
+        set_intraday_margin_setting,
     )
     from .market_data import get_candles, get_market_trades
     from .orders import (
         cancel_orders,
         create_order,
         edit_order,
         get_fills,
@@ -78,17 +81,19 @@
         trigger_bracket_order_gtd,
         trigger_bracket_order_gtd_buy,
         trigger_bracket_order_gtd_sell,
     )
     from .payments import get_payment_method, list_payment_methods
     from .perpetuals import (
         allocate_portfolio,
+        get_perps_portfolio_balances,
         get_perps_portfolio_summary,
         get_perps_position,
         list_perps_positions,
+        opt_in_or_out_multi_asset_collateral,
     )
     from .portfolios import (
         create_portfolio,
         delete_portfolio,
         edit_portfolio,
         get_portfolio_breakdown,
         get_portfolios,
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/accounts.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     **Description:**
 
     Get a list of authenticated accounts for the current user.
 
     __________
 
-    **Read more on the official documentation:** `List Accounts <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getaccounts>`_
+    **Read more on the official documentation:** `List Accounts <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getaccounts>`_
 
     """
     endpoint = f"{API_PREFIX}/accounts"
     params = {
         "limit": limit,
         "cursor": cursor,
         "retail_portfolio_id": retail_portfolio_id,
@@ -47,12 +47,12 @@
 
     **Description:**
 
     Get a list of information about an account, given an account UUID.
 
     __________
 
-    **Read more on the official documentation:** `Get Account <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getaccount>`_
+    **Read more on the official documentation:** `Get Account <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getaccount>`_
     """
     endpoint = f"{API_PREFIX}/accounts/{account_uuid}"
 
     return self.get(endpoint, **kwargs)
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/convert.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/convert.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     **Description:**
 
     Create a convert quote with a specified source currency, target currency, and amount.
 
     __________
 
-    **Read more on the official documentation:** `Create Convert Quote <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_createconvertquote>`_
+    **Read more on the official documentation:** `Create Convert Quote <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_createconvertquote>`_
     """
     endpoint = f"{API_PREFIX}/convert/quote"
 
     data = {
         "from_account": from_account,
         "to_account": to_account,
         "amount": amount,
@@ -65,15 +65,15 @@
 
     **Description:**
 
     Gets a list of information about a convert trade with a specified trade ID, source currency, and target currency.
 
     __________
 
-    **Read more on the official documentation:** `Get Convert Trade <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getconverttrade>`_
+    **Read more on the official documentation:** `Get Convert Trade <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getconverttrade>`_
     """
     endpoint = f"{API_PREFIX}/convert/trade/{trade_id}"
 
     params = {
         "from_account": from_account,
         "to_account": to_account,
     }
@@ -94,15 +94,15 @@
 
     **Description:**
 
     Commits a convert trade with a specified trade ID, source currency, and target currency.
 
     __________
 
-    **Read more on the official documentation:** `Commit Convert Trade <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_commitconverttrade>`_
+    **Read more on the official documentation:** `Commit Convert Trade <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_commitconverttrade>`_
     """
     endpoint = f"{API_PREFIX}/convert/trade/{trade_id}"
 
     data = {
         "from_account": from_account,
         "to_account": to_account,
     }
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/fees.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/fees.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     **Description:**
 
     Get a summary of transactions with fee tiers, total volume, and fees.
 
     __________
 
-    **Read more on the official documentation:** `Create Convert Quote <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_createconvertquote>`_
+    **Read more on the official documentation:** `Create Convert Quote <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_createconvertquote>`_
     """
     endpoint = f"{API_PREFIX}/transaction_summary"
 
     params = {
         "product_type": product_type,
         "contract_expiry_type": contract_expiry_type,
     }
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/futures.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/futures.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     **Description:**
 
     Places an order to close any open positions for a specified ``product_id``.
 
     __________
 
     **Read more on the official documentation:** `Close Position
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_closeposition>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_closeposition>`_
     """
     endpoint = f"{API_PREFIX}/orders/close_position"
     data = {"client_order_id": client_order_id, "product_id": product_id, "size": size}
 
     return self.post(endpoint, data=data, **kwargs)
 
 
@@ -41,15 +41,15 @@
     **Description:**
 
     Get information on your balances related to `Coinbase Financial Markets <https://www.coinbase.com/fcm>`_ (CFM) futures trading.
 
     __________
 
     **Read more on the official documentation:** `Get Futures Balance Summary
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getfcmbalancesummary>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getfcmbalancesummary>`_
     """
     endpoint = f"{API_PREFIX}/cfm/balance_summary"
 
     return self.get(endpoint, **kwargs)
 
 
 def list_futures_positions(self, **kwargs) -> Dict[str, Any]:
@@ -64,15 +64,15 @@
     **Description:**
 
     Get a list of all open positions in CFM futures products.
 
     __________
 
     **Read more on the official documentation:** `List Futures Positions
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getfcmpositions>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getfcmpositions>`_
     """
     endpoint = f"{API_PREFIX}/cfm/positions"
 
     return self.get(endpoint, **kwargs)
 
 
 def get_futures_position(self, product_id: str, **kwargs) -> Dict[str, Any]:
@@ -87,15 +87,15 @@
     **Description:**
 
     Get the position of a specific CFM futures product.
 
     __________
 
     **Read more on the official documentation:** `Get Futures Position
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getfcmposition>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getfcmposition>`_
     """
     endpoint = f"{API_PREFIX}/cfm/positions/{product_id}"
 
     return self.get(endpoint, **kwargs)
 
 
 def schedule_futures_sweep(self, usd_amount: str, **kwargs) -> Dict[str, Any]:
@@ -110,15 +110,15 @@
     **Description:**
 
     Schedule a sweep of funds from your CFTC-regulated futures account to your Coinbase Inc. USD Spot wallet.
 
     __________
 
     **Read more on the official documentation:** `Schedule Futures Sweep
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_schedulefcmsweep>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_schedulefcmsweep>`_
     """
     endpoint = f"{API_PREFIX}/cfm/sweeps/schedule"
 
     data = {"usd_amount": usd_amount}
 
     return self.post(endpoint, data=data, **kwargs)
 
@@ -135,15 +135,15 @@
     **Description:**
 
     Get information on your pending and/or processing requests to sweep funds from your CFTC-regulated futures account to your Coinbase Inc. USD Spot wallet.
 
     __________
 
     **Read more on the official documentation:** `List Futures Sweeps
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getfcmsweeps>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getfcmsweeps>`_
     """
     endpoint = f"{API_PREFIX}/cfm/sweeps"
 
     return self.get(endpoint, **kwargs)
 
 
 def cancel_pending_futures_sweep(self, **kwargs) -> Dict[str, Any]:
@@ -158,12 +158,89 @@
     **Description:**
 
     Cancel your pending sweep of funds from your CFTC-regulated futures account to your Coinbase Inc. USD Spot wallet.
 
     __________
 
     **Read more on the official documentation:** `Cancel Pending Futures Sweep
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_cancelfcmsweep>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_cancelfcmsweep>`_
     """
     endpoint = f"{API_PREFIX}/cfm/sweeps"
 
     return self.delete(endpoint, **kwargs)
+
+
+def get_intraday_margin_setting(self, **kwargs) -> Dict[str, Any]:
+    """
+    **Get Intraday Margin Setting**
+    _______________________________
+
+    [GET] https://api.coinbase.com/api/v3/brokerage/cfm/intraday/margin_setting
+
+    __________
+
+    **Description:**
+
+    Get the status of whether your account is opted in to receive increased leverage on futures trades on weekdays from 8am-4pm ET.
+
+    __________
+
+    **Read more on the official documentation:** `Get Intraday Margin Setting
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getintradaymarginsetting>`_
+    """
+    endpoint = f"{API_PREFIX}/cfm/intraday/margin_setting"
+
+    return self.get(endpoint, **kwargs)
+
+
+def get_current_margin_window(
+    self, margin_profile_type: str, **kwargs
+) -> Dict[str, Any]:
+    """
+    **Get Current Margin Window**
+    ________________________________
+
+    [GET] https://api.coinbase.com/api/v3/brokerage/cfm/intraday/current_margin_window
+
+    __________
+
+    **Description:**
+
+    Get the current margin window to determine whether intraday or overnight margin rates are in effect.
+
+    __________
+
+    **Read more on the official documentation:** `Get Current Margin Window
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getcurrentmarginwindow>`_
+    """
+
+    endpoint = f"{API_PREFIX}/cfm/intraday/current_margin_window"
+
+    params = {"margin_profile_type": margin_profile_type}
+
+    return self.get(endpoint, params=params, **kwargs)
+
+
+def set_intraday_margin_setting(self, setting: str, **kwargs) -> Dict[str, Any]:
+    """
+    **Set Intraday Margin Setting**
+    ________________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/cfm/intraday/margin_setting
+
+    __________
+
+    **Description:**
+
+    Opt in to receive increased leverage on futures trades on weekdays from 8am-4pm ET.
+
+    __________
+
+    **Read more on the official documentation:** `Set Intraday Margin Setting
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_setintradaymarginsetting>`_
+    """
+
+    endpoint = f"{API_PREFIX}/cfm/intraday/margin_setting"
+
+    data = {"setting": setting}
+
+    return self.post(endpoint, data=data, **kwargs)
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/market_data.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/market_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     **Description:**
 
     Get rates for a single product by product ID, grouped in buckets.
 
     __________
 
     **Read more on the official documentation:** `Get Product Candles
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getcandles>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getcandles>`_
     """
     endpoint = f"{API_PREFIX}/products/{product_id}/candles"
 
     params = {
         "start": start,
         "end": end,
         "granularity": granularity,
@@ -53,14 +53,14 @@
     **Description:**
 
     Get snapshot information, by product ID, about the last trades (ticks), best bid/ask, and 24h volume.
 
     __________
 
     **Read more on the official documentation:** `Get Market Trades
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getmarkettrades>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getmarkettrades>`_
     """
     endpoint = f"{API_PREFIX}/products/{product_id}/ticker"
 
     params = {"limit": limit, "start": start, "end": end}
 
     return self.get(endpoint, params=params, **kwargs)
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/orders.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/orders.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     **Description:**
 
     Create an order with a specified ``product_id`` (asset-pair), ``side`` (buy/sell), etc.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     endpoint = f"{API_PREFIX}/orders"
 
     data = {
         "client_order_id": client_order_id,
         "product_id": product_id,
         "side": side,
@@ -74,15 +74,15 @@
 
     Place a market order to BUY or SELL the desired product at the given market price. If you wish to purchase the
     product, provide a quote_size and if you wish to sell the product, provide a base_size.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
 
     market_market_ioc = {"quote_size": quote_size, "base_size": base_size}
     filtered_market_market_ioc = {
         key: value for key, value in market_market_ioc.items() if value is not None
     }
 
@@ -102,15 +102,16 @@
     )
 
 
 def market_order_buy(
     self,
     client_order_id: str,
     product_id: str,
-    quote_size: str,
+    quote_size: Optional[str] = None,
+    base_size: Optional[str] = None,
     self_trade_prevention_id: Optional[str] = None,
     leverage: Optional[str] = None,
     margin_type: Optional[str] = None,
     retail_portfolio_id: Optional[str] = None,
     **kwargs,
 ) -> Dict[str, Any]:
     """
@@ -124,22 +125,23 @@
     **Description:**
 
     Place a market order to BUY the desired product at the given market price.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return market_order(
         self,
         client_order_id,
         product_id,
         "BUY",
         quote_size=quote_size,
+        base_size=base_size,
         self_trade_prevention_id=self_trade_prevention_id,
         leverage=leverage,
         margin_type=margin_type,
         retail_portfolio_id=retail_portfolio_id,
         **kwargs,
     )
 
@@ -166,15 +168,15 @@
     **Description:**
 
     Place a market order to SELL the desired product at the given market price.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return market_order(
         self,
         client_order_id,
         product_id,
         "SELL",
         base_size=base_size,
@@ -212,15 +214,15 @@
 
     Place a Limit Order with a IOC time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
 
     sor_limit_ioc = {"base_size": base_size, "limit_price": limit_price}
 
     order_configuration = {"sor_limit_ioc": sor_limit_ioc}
 
     return create_order(
@@ -261,15 +263,15 @@
 
     Place a Buy Limit Order with a IOC time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
 
     return limit_order_ioc(
         self,
         client_order_id,
         product_id,
         "BUY",
@@ -307,15 +309,15 @@
 
     Place a Sell Limit Order with a IOC time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
 
     return limit_order_ioc(
         self,
         client_order_id,
         product_id,
         "SELL",
@@ -356,15 +358,15 @@
 
     Place a Limit Order with a GTC time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     order_configuration = {
         "limit_limit_gtc": {
             "base_size": base_size,
             "limit_price": limit_price,
             "post_only": post_only,
         }
@@ -409,15 +411,15 @@
 
     Place a BUY Limit Order with a GTC time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return limit_order_gtc(
         self,
         client_order_id,
         product_id,
         "BUY",
         base_size=base_size,
@@ -456,15 +458,15 @@
 
     Place a SELL Limit Order with a GTC time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return limit_order_gtc(
         self,
         client_order_id,
         product_id,
         "SELL",
         base_size=base_size,
@@ -506,15 +508,15 @@
 
     Place a Limit Order with a GTD time-in-force policy. Unlike a Limit Order with a GTC time-in-force policy,
     this order type requires an end-time that indicates when this order should expire.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     order_configuration = {
         "limit_limit_gtd": {
             "base_size": base_size,
             "limit_price": limit_price,
             "end_time": end_time,
             "post_only": post_only,
@@ -561,15 +563,15 @@
 
     Place a BUY Limit Order with a GTD time-in-force policy. Unlike a Limit Order with a GTC time-in-force policy,
     this order type requires an end-time that indicates when this order should expire.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return limit_order_gtd(
         self,
         client_order_id,
         product_id,
         "BUY",
         base_size=base_size,
@@ -610,15 +612,15 @@
 
     Place a SELL Limit Order with a GTD time-in-force policy. Unlike a Limit Order with a GTC time-in-force policy,
     this order type requires an end-time that indicates when this order should expire.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return limit_order_gtd(
         self,
         client_order_id,
         product_id,
         "SELL",
         base_size=base_size,
@@ -659,15 +661,15 @@
 
     Place a Limit Order with a FOK time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
 
     limit_limit_fok = {"base_size": base_size, "limit_price": limit_price}
 
     order_configuration = {"limit_limit_fok": limit_limit_fok}
 
     return create_order(
@@ -708,15 +710,15 @@
 
     Place a Buy Limit Order with a FOK time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
 
     return limit_order_fok(
         self,
         client_order_id,
         product_id,
         "BUY",
@@ -754,15 +756,15 @@
 
     Place a Sell Limit Order with a FOK time-in-force policy. Provide the base_size (quantity of your base currency to
     spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
 
     return limit_order_fok(
         self,
         client_order_id,
         product_id,
         "SELL",
@@ -804,15 +806,15 @@
 
     Place a Stop Limit order with a GTC time-in-force policy. Stop orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     order_configuration = {
         "stop_limit_stop_limit_gtc": {
             "base_size": base_size,
             "limit_price": limit_price,
             "stop_price": stop_price,
             "stop_direction": stop_direction,
@@ -859,15 +861,15 @@
 
     Place a BUY Stop Limit order with a GTC time-in-force policy. Stop orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return stop_limit_order_gtc(
         self,
         client_order_id,
         product_id,
         "BUY",
         base_size=base_size,
@@ -908,15 +910,15 @@
 
     Place a SELL Stop Limit order with a GTC time-in-force policy. Stop orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return stop_limit_order_gtc(
         self,
         client_order_id,
         product_id,
         "SELL",
         base_size=base_size,
@@ -960,15 +962,15 @@
 
     Place a Stop Limit order with a GTD time-in-force policy. Stop orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     order_configuration = {
         "stop_limit_stop_limit_gtd": {
             "base_size": base_size,
             "limit_price": limit_price,
             "stop_price": stop_price,
             "end_time": end_time,
@@ -1017,15 +1019,15 @@
 
     Place a BUY Stop Limit order with a GTD time-in-force policy. Stop orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return stop_limit_order_gtd(
         self,
         client_order_id,
         product_id,
         "BUY",
         base_size=base_size,
@@ -1068,15 +1070,15 @@
 
     Place a SELL Stop Limit order with a GTD time-in-force policy. Stop orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return stop_limit_order_gtd(
         self,
         client_order_id,
         product_id,
         "SELL",
         base_size=base_size,
@@ -1119,15 +1121,15 @@
 
     Place a Trigger Bracket order with a GTC time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     order_configuration = {
         "trigger_bracket_gtc": {
             "base_size": base_size,
             "limit_price": limit_price,
             "stop_trigger_price": stop_trigger_price,
         }
@@ -1172,15 +1174,15 @@
 
     Place a BUY Trigger Bracket order with a GTC time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return trigger_bracket_order_gtc(
         self,
         client_order_id,
         product_id,
         "BUY",
         base_size=base_size,
@@ -1219,15 +1221,15 @@
 
     Place a SELL Trigger Bracket order with a GTC time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return trigger_bracket_order_gtc(
         self,
         client_order_id,
         product_id,
         "SELL",
         base_size=base_size,
@@ -1269,15 +1271,15 @@
 
     Place a Trigger Bracket order with a GTD time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     order_configuration = {
         "trigger_bracket_gtd": {
             "base_size": base_size,
             "limit_price": limit_price,
             "stop_trigger_price": stop_trigger_price,
             "end_time": end_time,
@@ -1324,15 +1326,15 @@
 
     Place a BUY Trigger Bracket order with a GTD time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return trigger_bracket_order_gtd(
         self,
         client_order_id,
         product_id,
         "BUY",
         base_size=base_size,
@@ -1373,15 +1375,15 @@
 
     Place a SELL Trigger Bracket order with a GTD time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
     the movement of the last trade price. The last trade price is the last price at which an order was filled.
 
     __________
 
     **Read more on the official documentation:** `Create Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_postorder>`_
     """
     return trigger_bracket_order_gtd(
         self,
         client_order_id,
         product_id,
         "SELL",
         base_size=base_size,
@@ -1408,15 +1410,15 @@
     **Description:**
 
     Get a single order by order ID.
 
     __________
 
     **Read more on the official documentation:** `Get Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_gethistoricalorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_gethistoricalorder>`_
     """
     endpoint = f"{API_PREFIX}/orders/historical/{order_id}"
 
     return self.get(endpoint, **kwargs)
 
 
 def list_orders(
@@ -1447,15 +1449,15 @@
     **Description:**
 
     Get a list of orders filtered by optional query parameters (``product_id``, ``order_status``, etc).
 
     __________
 
     **Read more on the official documentation:** `List Orders
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_gethistoricalorders>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_gethistoricalorders>`_
     """
     endpoint = f"{API_PREFIX}/orders/historical/batch"
     params = {
         "product_id": product_id,
         "order_status": order_status,
         "limit": limit,
         "start_date": start_date,
@@ -1494,15 +1496,15 @@
     **Description:**
 
     Get a list of fills filtered by optional query parameters (``product_id``, ``order_id``, etc).
 
     __________
 
     **Read more on the official documentation:** `List Fills
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getfills>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getfills>`_
     """
     endpoint = f"{API_PREFIX}/orders/historical/fills"
     params = {
         "order_id": order_id,
         "product_id": product_id,
         "start_sequence_timestamp": start_sequence_timestamp,
         "end_sequence_timestamp": end_sequence_timestamp,
@@ -1531,15 +1533,15 @@
     **Description:**
 
     Edit an order with a specified new ``size``, or new ``price``. Only limit order types, with time in force type of good-till-cancelled can be edited.
 
     __________
 
     **Read more on the official documentation:** `Edit Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_editorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_editorder>`_
     """
     endpoint = f"{API_PREFIX}/orders/edit"
     data = {
         "order_id": order_id,
         "size": size,
         "price": price,
     }
@@ -1565,15 +1567,15 @@
     **Description:**
 
     Simulate an edit order request with a specified new ``size``, or new ``price``, to preview the result of an edit. Only limit order types, with time in force type of good-till-cancelled can be edited.
 
     __________
 
     **Read more on the official documentation:** `Edit Order Preview
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeweditorder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeweditorder>`_
     """
     endpoint = f"{API_PREFIX}/orders/edit_preview"
     data = {
         "order_id": order_id,
         "size": size,
         "price": price,
     }
@@ -1593,15 +1595,15 @@
     **Description:**
 
     Initiate cancel requests for one or more orders.
 
     __________
 
     **Read more on the official documentation:** `Cancel Orders
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_cancelorders>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_cancelorders>`_
     """
     endpoint = f"{API_PREFIX}/orders/batch_cancel"
     data = {
         "order_ids": order_ids,
     }
 
     return self.post(endpoint, data=data, **kwargs)
@@ -1632,15 +1634,15 @@
     **Description:**
 
     Preview the results of an order request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     endpoint = f"{API_PREFIX}/orders/preview"
 
     if commission_rate:
         commission_rate = {"value": commission_rate}
 
     data = {
@@ -1686,15 +1688,15 @@
     **Description:**
 
     Preview the results of a market order request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
 
     market_market_ioc = {"quote_size": quote_size, "base_size": base_size}
     filtered_market_market_ioc = {
         key: value for key, value in market_market_ioc.items() if value is not None
     }
 
@@ -1716,14 +1718,15 @@
     )
 
 
 def preview_market_order_buy(
     self,
     product_id: str,
     quote_size: Optional[str] = None,
+    base_size: Optional[str] = None,
     commission_rate: Optional[str] = None,
     is_max: Optional[bool] = False,
     tradable_balance: Optional[str] = None,
     skip_fcm_risk_check: Optional[bool] = False,
     leverage: Optional[str] = None,
     margin_type: Optional[str] = None,
     retail_portfolio_id: Optional[str] = None,
@@ -1740,21 +1743,22 @@
     **Description:**
 
     Preview the results of a market order buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_market_order(
         self,
         product_id,
         "BUY",
         quote_size=quote_size,
+        base_size=base_size,
         commission_rate=commission_rate,
         is_max=is_max,
         tradable_balance=tradable_balance,
         skip_fcm_risk_check=skip_fcm_risk_check,
         leverage=leverage,
         margin_type=margin_type,
         retail_portfolio_id=retail_portfolio_id,
@@ -1786,15 +1790,15 @@
     **Description:**
 
     Preview the results of a market order sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_market_order(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         commission_rate=commission_rate,
@@ -1835,15 +1839,15 @@
     **Description:**
 
     Preview the results of a limit order IOC request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     order_configuration = {
         "sor_limit_ioc": {"base_size": base_size, "limit_price": limit_price}
     }
 
     return preview_order(
         self,
@@ -1886,15 +1890,15 @@
     **Description:**
 
     Preview the results of a limit order IOC buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_limit_order_ioc(
         self,
         product_id,
         "BUY",
         base_size=base_size,
         limit_price=limit_price,
@@ -1934,15 +1938,15 @@
     **Description:**
 
     Preview the results of a limit order IOC sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_limit_order_ioc(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         limit_price=limit_price,
@@ -1985,15 +1989,15 @@
     **Description:**
 
     Preview the results of a limit order GTC request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     order_configuration = {
         "limit_limit_gtc": {
             "base_size": base_size,
             "limit_price": limit_price,
             "post_only": post_only,
         }
@@ -2041,15 +2045,15 @@
     **Description:**
 
     Preview the results of a limit order GTC buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_limit_order_gtc(
         self,
         product_id,
         "BUY",
         base_size=base_size,
         limit_price=limit_price,
@@ -2091,15 +2095,15 @@
     **Description:**
 
     Preview the results of a limit order GTC sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_limit_order_gtc(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         limit_price=limit_price,
@@ -2144,15 +2148,15 @@
     **Description:**
 
     Preview the results of a limit order GTD request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     order_configuration = {
         "limit_limit_gtd": {
             "base_size": base_size,
             "limit_price": limit_price,
             "end_time": end_time,
             "post_only": post_only,
@@ -2202,15 +2206,15 @@
     **Description:**
 
     Preview the results of a limit order GTD buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_limit_order_gtd(
         self,
         product_id,
         "BUY",
         base_size=base_size,
         limit_price=limit_price,
@@ -2254,15 +2258,15 @@
     **Description:**
 
     Preview the results of a limit order GTD sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_limit_order_gtd(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         limit_price=limit_price,
@@ -2305,15 +2309,15 @@
     **Description:**
 
     Preview the results of a limit order FOK request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     order_configuration = {
         "limit_limit_fok": {"base_size": base_size, "limit_price": limit_price}
     }
 
     return preview_order(
         self,
@@ -2356,15 +2360,15 @@
     **Description:**
 
     Preview the results of a limit order FOK buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_limit_order_fok(
         self,
         product_id,
         "BUY",
         base_size=base_size,
         limit_price=limit_price,
@@ -2404,15 +2408,15 @@
     **Description:**
 
     Preview the results of a limit order FOK sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_limit_order_fok(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         limit_price=limit_price,
@@ -2456,15 +2460,15 @@
     **Description:**
 
     Preview the results of a stop limit GTC order request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     order_configuration = {
         "stop_limit_stop_limit_gtc": {
             "base_size": base_size,
             "limit_price": limit_price,
             "stop_price": stop_price,
             "stop_direction": stop_direction,
@@ -2514,15 +2518,15 @@
     **Description:**
 
     Preview the results of a stop limit GTC order buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_stop_limit_order_gtc(
         self,
         product_id,
         "BUY",
         base_size=base_size,
         limit_price=limit_price,
@@ -2566,15 +2570,15 @@
     **Description:**
 
     Preview the results of a stop limit GTC order sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_stop_limit_order_gtc(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         limit_price=limit_price,
@@ -2621,15 +2625,15 @@
     **Description:**
 
     Preview the results of a stop limit GTD order request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     order_configuration = {
         "stop_limit_stop_limit_gtd": {
             "base_size": base_size,
             "limit_price": limit_price,
             "stop_price": stop_price,
             "end_time": end_time,
@@ -2681,15 +2685,15 @@
     **Description:**
 
     Preview the results of a stop limit GTD order buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_stop_limit_order_gtd(
         self,
         product_id,
         "BUY",
         base_size=base_size,
         limit_price=limit_price,
@@ -2735,15 +2739,15 @@
     **Description:**
 
     Preview the results of a stop limit GTD order sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_stop_limit_order_gtd(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         limit_price=limit_price,
@@ -2789,15 +2793,15 @@
     **Description:**
 
     Preview the results of a trigger bracket GTC order request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     order_configuration = {
         "trigger_bracket_gtc": {
             "base_size": base_size,
             "limit_price": limit_price,
             "stop_trigger_price": stop_trigger_price,
         }
@@ -2845,15 +2849,15 @@
     **Description:**
 
     Preview the results of a trigger bracket GTC order buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_trigger_bracket_order_gtc(
         self,
         product_id,
         "BUY",
         base_size=base_size,
         limit_price=limit_price,
@@ -2895,15 +2899,15 @@
     **Description:**
 
     Preview the results of a trigger bracket GTC order sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_trigger_bracket_order_gtc(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         limit_price=limit_price,
@@ -2948,15 +2952,15 @@
     **Description:**
 
     Preview the results of a trigger bracket GTD order request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     order_configuration = {
         "trigger_bracket_gtd": {
             "base_size": base_size,
             "limit_price": limit_price,
             "stop_trigger_price": stop_trigger_price,
             "end_time": end_time,
@@ -3006,15 +3010,15 @@
     **Description:**
 
     Preview the results of a trigger bracket GTD order buy request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_trigger_bracket_order_gtd(
         self,
         product_id,
         "BUY",
         base_size=base_size,
         limit_price=limit_price,
@@ -3058,15 +3062,15 @@
     **Description:**
 
     Preview the results of a trigger bracket GTD order sell request before sending.
 
     __________
 
     **Read more on the official documentation:** `Preview Order
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_previeworder>`_
     """
     return preview_trigger_bracket_order_gtd(
         self,
         product_id,
         "SELL",
         base_size=base_size,
         limit_price=limit_price,
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/payments.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/payments.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     **Description:**
 
     Get a list of payment methods for the current user.
 
     __________
 
-    **Read more on the official documentation:** `List Payment Methods <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getpaymentmethods>`_
+    **Read more on the official documentation:** `List Payment Methods <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpaymentmethods>`_
     """
 
     endpoint = f"{API_PREFIX}/payment_methods"
 
     return self.get(endpoint, **kwargs)
 
 
@@ -35,13 +35,13 @@
 
     **Description:**
 
     Get information about a payment method for the current user.
 
     __________
 
-    **Read more on the official documentation:** `Get Payment Method <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getpaymentmethod>`_
+    **Read more on the official documentation:** `Get Payment Method <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpaymentmethod>`_
     """
 
     endpoint = f"{API_PREFIX}/payment_methods/{payment_method_id}"
 
     return self.get(endpoint, **kwargs)
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/portfolios.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/portfolios.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     **Description:**
 
     Get a list of all portfolios of a user.
 
     __________
 
     **Read more on the official documentation:** `List Portfolios
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getportfolios>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getportfolios>`_
     """
     endpoint = f"{API_PREFIX}/portfolios"
 
     params = {"portfolio_type": portfolio_type}
 
     return self.get(endpoint, params=params, **kwargs)
 
@@ -42,15 +42,15 @@
     **Description:**
 
     Create a portfolio.
 
     __________
 
     **Read more on the official documentation:** `Create Portfolio
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_createportfolio>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_createportfolio>`_
     """
     endpoint = f"{API_PREFIX}/portfolios"
 
     data = {
         "name": name,
     }
 
@@ -69,15 +69,15 @@
     **Description:**
 
     Get the breakdown of a portfolio by portfolio ID.
 
     __________
 
     **Read more on the official documentation:** `Get Portfolio Breakdown
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getportfoliobreakdown>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getportfoliobreakdown>`_
     """
     endpoint = f"{API_PREFIX}/portfolios/{portfolio_uuid}"
 
     return self.get(endpoint, **kwargs)
 
 
 def move_portfolio_funds(
@@ -99,15 +99,15 @@
     **Description:**
 
     Transfer funds between portfolios.
 
     __________
 
     **Read more on the official documentation:** `Move Portfolio Funds
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_moveportfoliofunds>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_moveportfoliofunds>`_
     """
     endpoint = f"{API_PREFIX}/portfolios/move_funds"
 
     data = {
         "funds": {
             "value": value,
             "currency": currency,
@@ -131,15 +131,15 @@
     **Description:**
 
     Modify a portfolio by portfolio ID.
 
     __________
 
     **Read more on the official documentation:** `Edit Portfolio
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_editportfolio>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_editportfolio>`_
     """
     endpoint = f"{API_PREFIX}/portfolios/{portfolio_uuid}"
 
     data = {
         "name": name,
     }
 
@@ -158,12 +158,12 @@
     **Description:**
 
     Delete a portfolio by portfolio ID.
 
     __________
 
     **Read more on the official documentation:** `Delete Portfolio
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_deleteportfolio>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_deleteportfolio>`_
     """
     endpoint = f"{API_PREFIX}/portfolios/{portfolio_uuid}"
 
     return self.delete(endpoint, **kwargs)
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/products.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/products.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     **Description:**
 
     Get a list of the available currency pairs for trading.
 
     __________
 
     **Read more on the official documentation:** `List Products
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getproducts>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts>`_
     """
     endpoint = f"{API_PREFIX}/products"
 
     params = {
         "limit": limit,
         "offset": offset,
         "product_type": product_type,
@@ -56,15 +56,15 @@
     **Description:**
 
     Get information on a single product by product ID.
 
     __________
 
     **Read more on the official documentation:** `Get Product
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getproduct>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproduct>`_
     """
     endpoint = f"{API_PREFIX}/products/{product_id}"
 
     return self.get(endpoint, **kwargs)
 
 
 def get_product_book(
@@ -81,15 +81,15 @@
     **Description:**
 
     Get a list of bids/asks for a single product. The amount of detail shown can be customized with the limit parameter.
 
     __________
 
     **Read more on the official documentation:** `Get Product Book
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getproductbook>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproductbook>`_
     """
     endpoint = f"{API_PREFIX}/product_book"
 
     params = {"product_id": product_id, "limit": limit}
 
     return self.get(endpoint, params=params, **kwargs)
 
@@ -108,15 +108,15 @@
     **Description:**
 
     Get the best bid/ask for all products. A subset of all products can be returned instead by using the product_ids input.
 
     __________
 
     **Read more on the official documentation:** `Get Best Bid/Ask
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getproductbook>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproductbook>`_
     """
     endpoint = f"{API_PREFIX}/best_bid_ask"
 
     params = {
         "product_ids": product_ids,
     }
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/public.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/public.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     **Description:**
 
     Get the current time from the Coinbase Advanced API. This is a public endpoint.
 
     __________
 
-    **Read more on the official documentation:** `Get Server Time <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getservertime>`_
+    **Read more on the official documentation:** `Get Server Time <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getservertime>`_
     """
 
     endpoint = f"{API_PREFIX}/time"
 
     return self.get(endpoint, public=True, **kwargs)
 
 
@@ -43,15 +43,15 @@
 
     **API Key Permissions:**
 
     This endpoint is public and does not need authentication.
 
     __________
 
-    **Read more on the official documentation:** `Get Public Product Book <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getpublicproductbook>`_
+    **Read more on the official documentation:** `Get Public Product Book <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproductbook>`_
     """
 
     endpoint = f"{API_PREFIX}/market/product_book"
 
     params = {"product_id": product_id, "limit": limit}
 
     return self.get(endpoint, params=params, public=True, **kwargs)
@@ -84,15 +84,15 @@
     **API Key Permissions:**
 
     This endpoint is public and does not need authentication.
 
     __________
 
     **Read more on the official documentation:** `List Public Products
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getpublicproducts>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts>`_
     """
     endpoint = f"{API_PREFIX}/market/products"
 
     params = {
         "limit": limit,
         "offset": offset,
         "product_type": product_type,
@@ -122,15 +122,15 @@
     **API Key Permissions:**
 
     This endpoint is public and does not need authentication.
 
     __________
 
     **Read more on the official documentation:** `Get Public Product
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getpublicproduct>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproduct>`_
     """
     endpoint = f"{API_PREFIX}/market/products/{product_id}"
 
     return self.get(endpoint, public=True, **kwargs)
 
 
 def get_public_candles(
@@ -153,15 +153,15 @@
     **API Key Permissions:**
 
     This endpoint is public and does not need authentication.
 
     __________
 
     **Read more on the official documentation:** `Get Public Product Candles
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getpubliccandles>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpubliccandles>`_
     """
     endpoint = f"{API_PREFIX}/market/products/{product_id}/candles"
 
     params = {
         "start": start,
         "end": end,
         "granularity": granularity,
@@ -195,14 +195,14 @@
     **API Key Permissions:**
 
     This endpoint is public and does not need authentication.
 
     __________
 
     **Read more on the official documentation:** `Get Public Market Trades
-    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getpublicmarkettrades>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicmarkettrades>`_
     """
     endpoint = f"{API_PREFIX}/market/products/{product_id}/ticker"
 
     params = {"limit": limit, "start": start, "end": end}
 
     return self.get(endpoint, params=params, public=True, **kwargs)
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/rest/rest_base.py` & `coinbase-advanced-py-1.4.0/coinbase/rest/rest_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/coinbase/websocket/__init__.py` & `coinbase-advanced-py-1.4.0/coinbase/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/coinbase/websocket/channels.py` & `coinbase-advanced-py-1.4.0/coinbase/websocket/channels.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     **Description:**
 
     Subscribe to heartbeats channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Heartbeats Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#heartbeats-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#heartbeats-channel>`_
     """
     self.subscribe(product_ids, [HEARTBEATS])
 
 
 async def heartbeats_async(self, product_ids: List[str]) -> None:
     """
     **Heartbeats Subscribe Async**
@@ -41,15 +41,15 @@
     **Description:**
 
     Async subscribe to heartbeats channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Heartbeats Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#heartbeats-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#heartbeats-channel>`_
     """
     await self.subscribe_async(product_ids, [HEARTBEATS])
 
 
 def heartbeats_unsubscribe(self, product_ids: List[str]) -> None:
     """
     **Heartbeats Unsubscribe**
@@ -60,15 +60,15 @@
     **Description:**
 
     Unsubscribe to heartbeats channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Heartbeats Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#heartbeats-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#heartbeats-channel>`_
     """
     self.unsubscribe(product_ids, [HEARTBEATS])
 
 
 async def heartbeats_unsubscribe_async(self, product_ids: List[str]) -> None:
     """
     **Heartbeats Unsubscribe Async**
@@ -79,15 +79,15 @@
     **Description:**
 
     Async unsubscribe to heartbeats channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Heartbeats Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#heartbeats-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#heartbeats-channel>`_
     """
     await self.unsubscribe_async(product_ids, [HEARTBEATS])
 
 
 def candles(self, product_ids: List[str]) -> None:
     """
     **Candles Subscribe**
@@ -98,15 +98,15 @@
     **Description:**
 
     Subscribe to candles channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Candles Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#candles-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#candles-channel>`_
     """
     self.subscribe(product_ids, [CANDLES])
 
 
 async def candles_async(self, product_ids: List[str]) -> None:
     """
     **Candles Subscribe Async**
@@ -117,15 +117,15 @@
     **Description:**
 
     Async subscribe to candles channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Candles Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#candles-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#candles-channel>`_
     """
     await self.subscribe_async(product_ids, [CANDLES])
 
 
 def candles_unsubscribe(self, product_ids: List[str]) -> None:
     """
     **Candles Unsubscribe**
@@ -136,15 +136,15 @@
     **Description:**
 
     Unsubscribe to candles channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Candles Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#candles-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#candles-channel>`_
     """
     self.unsubscribe(product_ids, [CANDLES])
 
 
 async def candles_unsubscribe_async(self, product_ids: List[str]) -> None:
     """
     **Candles Unsubscribe Async**
@@ -155,15 +155,15 @@
     **Description:**
 
     Async unsubscribe to candles channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Candles Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#candles-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#candles-channel>`_
     """
     await self.unsubscribe_async(product_ids, [CANDLES])
 
 
 def market_trades(self, product_ids: List[str]) -> None:
     """
     **Market Trades Subscribe**
@@ -174,15 +174,15 @@
     **Description:**
 
     Subscribe to market_trades channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Market Trades Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#market-trades-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#market-trades-channel>`_
     """
     self.subscribe(product_ids, [MARKET_TRADES])
 
 
 async def market_trades_async(self, product_ids: List[str]) -> None:
     """
     **Market Trades Subscribe Async**
@@ -193,15 +193,15 @@
     **Description:**
 
     Async subscribe to market_trades channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Market Trades Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#market-trades-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#market-trades-channel>`_
     """
     await self.subscribe_async(product_ids, [MARKET_TRADES])
 
 
 def market_trades_unsubscribe(self, product_ids: List[str]) -> None:
     """
     **Market Trades Unsubscribe**
@@ -212,15 +212,15 @@
     **Description:**
 
     Unsubscribe to market_trades channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Market Trades Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#market-trades-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#market-trades-channel>`_
     """
     self.unsubscribe(product_ids, [MARKET_TRADES])
 
 
 async def market_trades_unsubscribe_async(self, product_ids: List[str]) -> None:
     """
     **Market Trades Unsubscribe Async**
@@ -231,15 +231,15 @@
     **Description:**
 
     Async unsubscribe to market_trades channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Market Trades Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#market-trades-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#market-trades-channel>`_
     """
     await self.unsubscribe_async(product_ids, [MARKET_TRADES])
 
 
 def status(self, product_ids: List[str]) -> None:
     """
     **Status Subscribe**
@@ -250,15 +250,15 @@
     **Description:**
 
     Subscribe to status channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Status Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#status-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#status-channel>`_
     """
     self.subscribe(product_ids, [STATUS])
 
 
 async def status_async(self, product_ids: List[str]) -> None:
     """
     **Status Subscribe Async**
@@ -269,15 +269,15 @@
     **Description:**
 
     Async subscribe to status channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Status Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#status-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#status-channel>`_
     """
     await self.subscribe_async(product_ids, [STATUS])
 
 
 def status_unsubscribe(self, product_ids: List[str]) -> None:
     """
     **Status Unsubscribe**
@@ -288,15 +288,15 @@
     **Description:**
 
     Unsubscribe to status channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Status Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#status-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#status-channel>`_
     """
     self.unsubscribe(product_ids, [STATUS])
 
 
 async def status_unsubscribe_async(self, product_ids: List[str]) -> None:
     """
     **Status Unsubscribe Async**
@@ -307,15 +307,15 @@
     **Description:**
 
     Async unsubscribe to status channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Status Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#status-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#status-channel>`_
     """
     await self.unsubscribe_async(product_ids, [STATUS])
 
 
 def ticker(self, product_ids: List[str]) -> None:
     """
     **Ticker Subscribe**
@@ -326,15 +326,15 @@
     **Description:**
 
     Subscribe to ticker channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Ticker Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#ticker-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel>`_
     """
     self.subscribe(product_ids, [TICKER])
 
 
 async def ticker_async(self, product_ids: List[str]) -> None:
     """
     **Ticker Subscribe Async**
@@ -345,15 +345,15 @@
     **Description:**
 
     Async subscribe to ticker channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Ticker Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#ticker-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel>`_
     """
     await self.subscribe_async(product_ids, [TICKER])
 
 
 def ticker_unsubscribe(self, product_ids: List[str]) -> None:
     """
     **Ticker Unsubscribe**
@@ -364,15 +364,15 @@
     **Description:**
 
     Unsubscribe to ticker channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Ticker Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#ticker-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel>`_
     """
     self.unsubscribe(product_ids, [TICKER])
 
 
 async def ticker_unsubscribe_async(self, product_ids: List[str]) -> None:
     """
     **Ticker Unsubscribe Async**
@@ -383,15 +383,15 @@
     **Description:**
 
     Async unsubscribe to ticker channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Ticker Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#ticker-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel>`_
     """
     await self.unsubscribe_async(product_ids, [TICKER])
 
 
 def ticker_batch(self, product_ids: List[str]) -> None:
     """
     **Ticker Batch Subscribe**
@@ -402,15 +402,15 @@
     **Description:**
 
     Subscribe to ticker_batch channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Ticker Batch Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#ticker-batch-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-batch-channel>`_
     """
     self.subscribe(product_ids, [TICKER_BATCH])
 
 
 async def ticker_batch_async(self, product_ids: List[str]) -> None:
     """
     **Ticker Batch Subscribe Async**
@@ -421,15 +421,15 @@
     **Description:**
 
     Async subscribe to ticker_batch channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Ticker Batch Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#ticker-batch-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-batch-channel>`_
     """
     await self.subscribe_async(product_ids, [TICKER_BATCH])
 
 
 def ticker_batch_unsubscribe(self, product_ids: List[str]) -> None:
     """
     **Ticker Batch Unsubscribe**
@@ -440,15 +440,15 @@
     **Description:**
 
     Unsubscribe to ticker_batch channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Ticker Batch Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#ticker-batch-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-batch-channel>`_
     """
     self.unsubscribe(product_ids, [TICKER_BATCH])
 
 
 async def ticker_batch_unsubscribe_async(self, product_ids: List[str]) -> None:
     """
     **Ticker Batch Unsubscribe Async**
@@ -459,15 +459,15 @@
     **Description:**
 
     Async unsubscribe to ticker_batch channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Ticker Batch Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#ticker-batch-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-batch-channel>`_
     """
     await self.unsubscribe_async(product_ids, [TICKER_BATCH])
 
 
 def level2(self, product_ids: List[str]) -> None:
     """
     **Level2 Subscribe**
@@ -478,15 +478,15 @@
     **Description:**
 
     Subscribe to level2 channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Level2 Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#level2-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#level2-channel>`_
     """
     self.subscribe(product_ids, [LEVEL2])
 
 
 async def level2_async(self, product_ids: List[str]) -> None:
     """
     **Level2 Subscribe Async**
@@ -497,15 +497,15 @@
     **Description:**
 
     Async subscribe to level2 channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Level2 Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#level2-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#level2-channel>`_
     """
     await self.subscribe_async(product_ids, [LEVEL2])
 
 
 def level2_unsubscribe(self, product_ids: List[str]) -> None:
     """
     **Level2 Unsubscribe**
@@ -516,15 +516,15 @@
     **Description:**
 
     Unsubscribe to level2 channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Level2 Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#level2-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#level2-channel>`_
     """
     self.unsubscribe(product_ids, [LEVEL2])
 
 
 async def level2_unsubscribe_async(self, product_ids: List[str]) -> None:
     """
     **Level2 Unsubscribe Async**
@@ -535,15 +535,15 @@
     **Description:**
 
     Async unsubscribe to level2 channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `Level2 Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#level2-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#level2-channel>`_
     """
     await self.unsubscribe_async(product_ids, [LEVEL2])
 
 
 def user(self, product_ids: List[str]) -> None:
     """
     **User Subscribe**
@@ -554,15 +554,15 @@
     **Description:**
 
     Subscribe to user channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `User Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#user-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#user-channel>`_
     """
     self.subscribe(product_ids, [USER])
 
 
 async def user_async(self, product_ids: List[str]) -> None:
     """
     **User Subscribe Async**
@@ -573,15 +573,15 @@
     **Description:**
 
     Async subscribe to user channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `User Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#user-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#user-channel>`_
     """
     await self.subscribe_async(product_ids, [USER])
 
 
 def user_unsubscribe(self, product_ids: List[str]) -> None:
     """
     **User Unsubscribe**
@@ -592,15 +592,15 @@
     **Description:**
 
     Unsubscribe to user channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `User Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#user-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#user-channel>`_
     """
     self.unsubscribe(product_ids, [USER])
 
 
 async def user_unsubscribe_async(self, product_ids: List[str]) -> None:
     """
     **User Unsubscribe Async**
@@ -611,10 +611,10 @@
     **Description:**
 
     Async unsubscribe to user channel for a list of products_ids.
 
     __________
 
     **Read more on the official documentation:** `User Channel
-    <https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels#user-channel>`_
+    <https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#user-channel>`_
     """
     await self.unsubscribe_async(product_ids, [USER])
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase/websocket/websocket_base.py` & `coinbase-advanced-py-1.4.0/coinbase/websocket/websocket_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/PKG-INFO` & `coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-advanced-py
-Version: 1.3.0
+Version: 1.4.0
 Summary: Coinbase Advanced API Python SDK
 Home-page: https://github.com/coinbase/coinbase-advanced-py
 Author: Coinbase
 License: Apache 2.0
 Keywords: Coinbase,Advanced Trade,API,Advanced API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -29,30 +29,30 @@
 Requires-Dist: isort==5.12.0; extra == "lint"
 
 # Coinbase Advanced API Python SDK
 [![PyPI version](https://badge.fury.io/py/coinbase-advanced-py.svg)](https://badge.fury.io/py/coinbase-advanced-py)
 [![License](https://img.shields.io/badge/License-Apache%202.0-green.svg)](https://opensource.org/license/apache-2-0/)
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 
-Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/welcome).
-This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
+Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cdp.coinbase.com/advanced-trade/docs/welcome).
+This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview).
 
 For thorough documentation of all available functions, refer to the following link: https://coinbase.github.io/coinbase-advanced-py
 
 ___
 ## Installation
 
 ```bash
 pip3 install coinbase-advanced-py
 ```
 
 ___
 ## Coinbase Developer Platform (CDP) API Keys
 
-This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
+This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cdp.coinbase.com/advanced-trade/docs/auth).
 Make sure to save your API key and secret in a safe place. You will not be able to retrieve your secret again.
 
 WARNING: We do not recommend that you save your API secrets directly in your code outside of testing purposes. Best practice is to use a secrets manager and access your secrets that way. You should be careful about exposing your secrets publicly if posting code that leverages this library.
 
 Optional: Set your API key and secret in your environment (make sure to put these in quotation marks). For example:
 ```bash
 export COINBASE_API_KEY="organizations/{org_id}/apiKeys/{key_id}"
@@ -100,15 +100,15 @@
 print(dumps(accounts, indent=2))
 
 order = client.market_order_buy(client_order_id="clientOrderId", product_id="BTC-USD", quote_size="1")
 print(dumps(order, indent=2))
 ```
 This code calls the `get_accounts` and `market_order_buy` endpoints.
 
-Refer to the [Advanced API Reference](https://docs.cloud.coinbase.com/advanced-trade-api/reference) for detailed information on each exposed endpoint.
+Refer to the [Advanced API Reference](https://docs.cdp.coinbase.com/advanced-trade/reference) for detailed information on each exposed endpoint.
 Look in the `coinbase.rest` module to see the API hooks that are exposed.
 
 ### Passing in additional parameters
 Use `kwargs` to pass in any additional parameters. For example:
 ```python
 kwargs = {
     "param1": 10,
@@ -120,26 +120,26 @@
 ### Generic REST Calls
 You can make generic REST calls using the `get`, `post`, `put`, and `delete` methods. For example:
 ```python
 market_trades = client.get("/api/v3/brokerage/products/BTC-USD/ticker", params={"limit": 5})
 
 portfolio = client.post("/api/v3/brokerage/portfolios", data={"name": "TestPortfolio"})
 ```
-Here we are calling the [GetMarketTrades](https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getmarkettrades) and [CreatePortfolio](https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_createportfolio) endpoints through the generic REST functions.
+Here we are calling the [GetMarketTrades](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getmarkettrades) and [CreatePortfolio](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_createportfolio) endpoints through the generic REST functions.
 Once again, the built-in way to query these through the SDK would be:
 ```python
 market_trades = client.get_market_trades(product_id="BTC-USD", limit=5)
 
 portfolio = client.create_portfolio(name="TestPortfolio")
 ```
 
 ___
 ## WebSocket API Client
-We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
-Refer to the [Advanced Trade WebSocket Channels](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels) page for detailed information on each offered channel.
+We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview).
+Refer to the [Advanced Trade WebSocket Channels](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels) page for detailed information on each offered channel.
 
 In your code, import the WSClient class and instantiate it. The WSClient requires an API key and secret to be passed in as arguments. You can also use a key file or environment variables as described in the RESTClient instructions above.
 
 You must specify an `on_message` function that will be called when a message is received from the WebSocket API. This function must take in a single argument, which will be the raw message received from the WebSocket API. For example:
 ```python
 from coinbase.websocket import WSClient
 
@@ -267,15 +267,15 @@
 ws_client = WSClient(api_key=api_key, api_secret=api_secret, on_message=on_message, verbose=True)
 ```
 
 ___
 ## Authentication
 Authentication of CDP API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
 
-However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
+However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
 ```python
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 uri = "/api/v3/brokerage/orders"
@@ -293,15 +293,15 @@
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 jwt = jwt_generator.build_ws_jwt(api_key, api_secret)
 ```
-Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview#sending-messages-using-cloud-api-keys) for more details.
+Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-overview#sending-messages-with-cdp-keys) for more details.
 
 ___
 ## Accessing public endpoints without authentication
 
 Both clients contain public endpoints which can be accessed without authentication. 
 
 To do so, simply initialize the clients without providing any API keys as arguments. 
@@ -309,36 +309,36 @@
 **_Notes:_**
 
 - Making calls to private endpoints or channels while unauthenticated will return an error
 - Unauthenticated requests are rate-limited more aggressively. Because of this we recommend that you authenticate your requests
 
 ### REST Client
 
-In the REST client, here is an example calling [Get Public Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
+In the REST client, here is an example calling [Get Public Products](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
 It does _not_ require authentication and is the public counterpart to 
-[Get Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
+[Get Products](https://docs.cdp.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
 
 Both endpoints return the same data.
 
 
 ```
 from coinbase.rest import RESTClient
 
 client = RESTClient()
 
 public_products = client.get_public_products()
 print(public_products)
 ```
-_Full list of all public REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
+_Full list of all public REST endpoints [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
 
-_Rate limit details for REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
+_Rate limit details for REST endpoints [here](https://docs.cdp.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
 
 ### Websocket Client
 
-In the Websocket client, here is an example subscribing to the [ticker](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
+In the Websocket client, here is an example subscribing to the [ticker](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
 Unlike the REST client, Websocket channels handle both authenticated and unauthenticated requests. 
 At the moment, most channels in the Websocket client are public and can be used without keys.
 
 ```
 import time
 from coinbase.websocket import WSClient
 
@@ -352,22 +352,22 @@
 
 time.sleep(10)
 
 client.ticker_unsubscribe(product_ids=["BTC-USD"])
 client.close()
 ```
 
-_Full list of all public Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels)_
+_Full list of all public Websocket channels [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-channels)_
 
-_Rate limit details for Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-rate-limits)_
+_Rate limit details for Websocket channels [here](https://docs.cdp.coinbase.com/advanced-trade/docs/ws-rate-limits)_
 
 
 ___
 ## Changelog
 For a detailed list of changes, see the [Changelog](https://github.com/coinbase/coinbase-advanced-py/blob/master/CHANGELOG.md).
 
 ___
 ## Contributing
 
 If you've found a bug within this project, open an issue on this repo and add the "bug" label to it.
 If you would like to request a new feature, open an issue on this repo and add the "enhancement" label to it.
-Direct concerns or questions on the API to the [Advanced API Developer Forum](https://forums.coinbasecloud.dev/c/advanced-trade-api/20).
+Direct concerns or questions on the API to the [Advanced API Discord](https://discord.com/channels/1220414409550336183/1220464268743278613) (use this [invite link](https://discord.com/invite/cdp) if it's your first time accessing the Discord).
```

### Comparing `coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/SOURCES.txt` & `coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/setup.py` & `coinbase-advanced-py-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_accounts.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_accounts.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_convert.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_convert.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_fees.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_fees.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_futures.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_portfolios.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,149 +3,128 @@
 from requests_mock import Mocker
 
 from coinbase.rest import RESTClient
 
 from ..constants import TEST_API_KEY, TEST_API_SECRET
 
 
-class FuturesTest(unittest.TestCase):
-    def test_close_position(self):
-        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
-
-        expected_response = {
-            "client_order_id": "client_order_id_1",
-            "product_id": "product_id_1",
-        }
-
-        with Mocker() as m:
-            m.request(
-                "POST",
-                "https://api.coinbase.com/api/v3/brokerage/orders/close_position",
-                json=expected_response,
-            )
-            closedOrder = client.close_position(
-                "client_order_id_1", "product_id_1", "100"
-            )
-
-            captured_request = m.request_history[0]
-            captured_json = captured_request.json()
-
-            self.assertEqual(captured_request.query, "")
-            self.assertEqual(
-                captured_json,
-                {
-                    "client_order_id": "client_order_id_1",
-                    "product_id": "product_id_1",
-                    "size": "100",
-                },
-            )
-            self.assertEqual(closedOrder, expected_response)
-
-    def test_get_futures_balance_summary(self):
+class PortfoliosTest(unittest.TestCase):
+    def test_get_portfolios(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
                 "GET",
-                "https://api.coinbase.com/api/v3/brokerage/cfm/balance_summary",
+                "https://api.coinbase.com/api/v3/brokerage/portfolios",
                 json=expected_response,
             )
-            balance_summary = client.get_futures_balance_summary()
+            portfolios = client.get_portfolios("DEFAULT")
 
             captured_request = m.request_history[0]
 
-            self.assertEqual(captured_request.query, "")
-            self.assertEqual(balance_summary, expected_response)
+            self.assertEqual(captured_request.query, "portfolio_type=default")
+            self.assertEqual(portfolios, expected_response)
 
-    def test_list_futures_positions(self):
+    def test_create_portfolio(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
-                "GET",
-                "https://api.coinbase.com/api/v3/brokerage/cfm/positions",
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/portfolios",
                 json=expected_response,
             )
-            positions = client.list_futures_positions()
+            portfolio = client.create_portfolio("Test Portfolio")
 
             captured_request = m.request_history[0]
+            captured_json = captured_request.json()
 
             self.assertEqual(captured_request.query, "")
-            self.assertEqual(positions, expected_response)
+            self.assertEqual(captured_json, {"name": "Test Portfolio"})
+            self.assertEqual(portfolio, expected_response)
 
-    def test_get_futures_position(self):
+    def test_get_portfolio_breakdown(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
                 "GET",
-                "https://api.coinbase.com/api/v3/brokerage/cfm/positions/PRODUCT_ID_1",
+                "https://api.coinbase.com/api/v3/brokerage/portfolios/1234",
                 json=expected_response,
             )
-            position = client.get_futures_position("PRODUCT_ID_1")
+            breakdown = client.get_portfolio_breakdown("1234")
 
             captured_request = m.request_history[0]
 
             self.assertEqual(captured_request.query, "")
-            self.assertEqual(position, expected_response)
+            self.assertEqual(breakdown, expected_response)
 
-    def test_schedule_futures_sweep(self):
+    def test_move_portfolio_funds(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
                 "POST",
-                "https://api.coinbase.com/api/v3/brokerage/cfm/sweeps/schedule",
+                "https://api.coinbase.com/api/v3/brokerage/portfolios/move_funds",
                 json=expected_response,
             )
-            response = client.schedule_futures_sweep("5")
+            move = client.move_portfolio_funds("100", "USD", "1234", "5678")
 
             captured_request = m.request_history[0]
             captured_json = captured_request.json()
 
             self.assertEqual(captured_request.query, "")
-            self.assertEqual(captured_json, {"usd_amount": "5"})
-            self.assertEqual(response, expected_response)
+            self.assertEqual(
+                captured_json,
+                {
+                    "funds": {"value": "100", "currency": "USD"},
+                    "source_portfolio_uuid": "1234",
+                    "target_portfolio_uuid": "5678",
+                },
+            )
+            self.assertEqual(move, expected_response)
 
-    def test_list_futures_sweeps(self):
+    def test_edit_portfolio(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
-                "GET",
-                "https://api.coinbase.com/api/v3/brokerage/cfm/sweeps",
+                "PUT",
+                "https://api.coinbase.com/api/v3/brokerage/portfolios/1234",
                 json=expected_response,
             )
-            sweeps = client.list_futures_sweeps()
+            edit = client.edit_portfolio("1234", "Test Portfolio")
 
             captured_request = m.request_history[0]
+            captured_json = captured_request.json()
 
             self.assertEqual(captured_request.query, "")
-            self.assertEqual(sweeps, expected_response)
+            self.assertEqual(captured_json, {"name": "Test Portfolio"})
+            self.assertEqual(edit, expected_response)
 
-    def test_cancel_pending_futures_sweep(self):
+    def test_delete_portfolio(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
                 "DELETE",
-                "https://api.coinbase.com/api/v3/brokerage/cfm/sweeps",
+                "https://api.coinbase.com/api/v3/brokerage/portfolios/1234",
                 json=expected_response,
             )
-            delete = client.cancel_pending_futures_sweep()
+            delete = client.delete_portfolio("1234")
 
             captured_request = m.request_history[0]
 
             self.assertEqual(captured_request.query, "")
             self.assertEqual(delete, expected_response)
```

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_market_data.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_market_data.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_orders.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_orders.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_payments.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_payments.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_perpetuals.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_perpetuals.py`

 * *Files 22% similar despite different names*

```diff
@@ -92,7 +92,54 @@
                 portfolio_uuid="test_uuid", symbol="BTC-PERP-INTX"
             )
 
             captured_request = m.request_history[0]
 
             self.assertEqual(captured_request.query, "")
             self.assertEqual(portfolios, expected_response)
+
+    def test_get_perps_portfolio_balances(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"key_1": "value_1", "key_2": "value_2"}
+
+        with Mocker() as m:
+            m.request(
+                "GET",
+                "https://api.coinbase.com/api/v3/brokerage/intx/balances/test_uuid",
+                json=expected_response,
+            )
+            portfolios = client.get_perps_portfolio_balances(portfolio_uuid="test_uuid")
+
+            captured_request = m.request_history[0]
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(portfolios, expected_response)
+
+    def test_opt_in_or_out_multi_asset_collateral(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"key_1": "value_1", "key_2": "value_2"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/intx/multi_asset_collateral",
+                json=expected_response,
+            )
+            response = client.opt_in_or_out_multi_asset_collateral(
+                portfolio_uuid="test_uuid",
+                multi_asset_collateral_enabled=True,
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "portfolio_uuid": "test_uuid",
+                    "multi_asset_collateral_enabled": True,
+                },
+            )
+            self.assertEqual(response, expected_response)
```

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_products.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_products.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_public.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_public.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/rest/test_rest_base.py` & `coinbase-advanced-py-1.4.0/tests/rest/test_rest_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/test_api_base.py` & `coinbase-advanced-py-1.4.0/tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/test_jwt_generator.py` & `coinbase-advanced-py-1.4.0/tests/test_jwt_generator.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/websocket/mock_ws_server.py` & `coinbase-advanced-py-1.4.0/tests/websocket/mock_ws_server.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/websocket/test_channels.py` & `coinbase-advanced-py-1.4.0/tests/websocket/test_channels.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.3.0/tests/websocket/test_websocket_base.py` & `coinbase-advanced-py-1.4.0/tests/websocket/test_websocket_base.py`

 * *Files identical despite different names*

