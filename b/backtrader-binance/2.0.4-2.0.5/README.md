# Comparing `tmp/backtrader_binance-2.0.4.tar.gz` & `tmp/backtrader_binance-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtrader_binance-2.0.4.tar", last modified: Mon Mar 18 06:57:17 2024, max compression
+gzip compressed data, was "backtrader_binance-2.0.5.tar", last modified: Tue May 21 04:29:28 2024, max compression
```

## Comparing `backtrader_binance-2.0.4.tar` & `backtrader_binance-2.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 06:57:17.809908 backtrader_binance-2.0.4/
--rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_binance-2.0.4/LICENSE
--rw-rw-rw-   0        0        0    31815 2024-03-18 06:57:17.809908 backtrader_binance-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    30434 2024-03-18 06:56:59.000000 backtrader_binance-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 06:57:17.803912 backtrader_binance-2.0.4/backtrader_binance/
--rw-rw-rw-   0        0        0       40 2021-06-25 01:58:20.000000 backtrader_binance-2.0.4/backtrader_binance/__init__.py
--rw-rw-rw-   0        0        0     8834 2024-02-05 09:57:13.000000 backtrader_binance-2.0.4/backtrader_binance/binance_broker.py
--rw-rw-rw-   0        0        0     5048 2023-04-05 03:54:03.000000 backtrader_binance-2.0.4/backtrader_binance/binance_feed.py
--rw-rw-rw-   0        0        0     6825 2024-02-05 08:15:28.000000 backtrader_binance-2.0.4/backtrader_binance/binance_store.py
-drwxrwxrwx   0        0        0        0 2024-03-18 06:57:17.808909 backtrader_binance-2.0.4/backtrader_binance.egg-info/
--rw-rw-rw-   0        0        0    31815 2024-03-18 06:57:17.000000 backtrader_binance-2.0.4/backtrader_binance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2024-03-18 06:57:17.000000 backtrader_binance-2.0.4/backtrader_binance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 06:57:17.000000 backtrader_binance-2.0.4/backtrader_binance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-18 06:57:17.000000 backtrader_binance-2.0.4/backtrader_binance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-03-18 06:57:17.000000 backtrader_binance-2.0.4/backtrader_binance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 06:57:17.810910 backtrader_binance-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2177 2024-03-18 06:56:59.000000 backtrader_binance-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:29:28.872952 backtrader_binance-2.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_binance-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0    31838 2024-05-21 04:29:28.872952 backtrader_binance-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    30461 2024-05-21 04:26:23.000000 backtrader_binance-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:29:28.867952 backtrader_binance-2.0.5/backtrader_binance/
+-rw-rw-rw-   0        0        0       40 2021-06-25 01:58:20.000000 backtrader_binance-2.0.5/backtrader_binance/__init__.py
+-rw-rw-rw-   0        0        0     8834 2024-02-05 09:57:13.000000 backtrader_binance-2.0.5/backtrader_binance/binance_broker.py
+-rw-rw-rw-   0        0        0     5048 2023-04-05 03:54:03.000000 backtrader_binance-2.0.5/backtrader_binance/binance_feed.py
+-rw-rw-rw-   0        0        0     6825 2024-02-05 08:15:28.000000 backtrader_binance-2.0.5/backtrader_binance/binance_store.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:29:28.871952 backtrader_binance-2.0.5/backtrader_binance.egg-info/
+-rw-rw-rw-   0        0        0    31838 2024-05-21 04:29:28.000000 backtrader_binance-2.0.5/backtrader_binance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2024-05-21 04:29:28.000000 backtrader_binance-2.0.5/backtrader_binance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:29:28.000000 backtrader_binance-2.0.5/backtrader_binance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-21 04:29:28.000000 backtrader_binance-2.0.5/backtrader_binance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-21 04:29:28.000000 backtrader_binance-2.0.5/backtrader_binance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:29:28.873952 backtrader_binance-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2177 2024-05-21 04:27:12.000000 backtrader_binance-2.0.5/setup.py
```

### Comparing `backtrader_binance-2.0.4/LICENSE` & `backtrader_binance-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `backtrader_binance-2.0.4/PKG-INFO` & `backtrader_binance-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtrader_binance
-Version: 2.0.4
+Version: 2.0.5
 Summary: Binance API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_binance
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
 Keywords: trading,development
@@ -32,19 +32,17 @@
 
 For API connection we are using library [python-binance](https://github.com/sammchardy/python-binance).
 
 **You can say Thanks:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
+or by [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** through the exchange (no commission)
 
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
-
-or by [Binance](https://accounts.binance.com/register?ref=200640624 ) **ID** (no commission) **200640624** through the exchange
+or by [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** through the exchange (no commission)
 
 ## Installation
 1) The simplest way:
 ```shell
 pip install backtrader_binance
 ```
 or
@@ -237,19 +235,17 @@
 
 Для подключения к API мы используем библиотеку [python-binance](https://github.com/sammchardy/python-binance ).
 
 **Можно сказать Спасибо:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
-
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
+или по [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** через биржу (без комиссии)
 
-или по [Binance](https://accounts.binance.com/register?ref=200640624 ) **ID** (без комиссии) **200640624** через биржу
+или по [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** через биржу (без комиссии)
 
 ## Установка
 1) Самый простой способ:
 ```shell
 pip install backtrader_binance
 ```
 или
```

### Comparing `backtrader_binance-2.0.4/README.md` & `backtrader_binance-2.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 
 For API connection we are using library [python-binance](https://github.com/sammchardy/python-binance).
 
 **You can say Thanks:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
+or by [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** through the exchange (no commission)
 
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
-
-or by [Binance](https://accounts.binance.com/register?ref=200640624 ) **ID** (no commission) **200640624** through the exchange
+or by [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** through the exchange (no commission)
 
 ## Installation
 1) The simplest way:
 ```shell
 pip install backtrader_binance
 ```
 or
@@ -213,19 +211,17 @@
 
 Для подключения к API мы используем библиотеку [python-binance](https://github.com/sammchardy/python-binance ).
 
 **Можно сказать Спасибо:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
-
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
+или по [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** через биржу (без комиссии)
 
-или по [Binance](https://accounts.binance.com/register?ref=200640624 ) **ID** (без комиссии) **200640624** через биржу
+или по [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** через биржу (без комиссии)
 
 ## Установка
 1) Самый простой способ:
 ```shell
 pip install backtrader_binance
 ```
 или
```

### Comparing `backtrader_binance-2.0.4/backtrader_binance/binance_broker.py` & `backtrader_binance-2.0.5/backtrader_binance/binance_broker.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-2.0.4/backtrader_binance/binance_feed.py` & `backtrader_binance-2.0.5/backtrader_binance/binance_feed.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-2.0.4/backtrader_binance/binance_store.py` & `backtrader_binance-2.0.5/backtrader_binance/binance_store.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-2.0.4/backtrader_binance.egg-info/PKG-INFO` & `backtrader_binance-2.0.5/backtrader_binance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtrader-binance
-Version: 2.0.4
+Version: 2.0.5
 Summary: Binance API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_binance
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
 Keywords: trading,development
@@ -32,19 +32,17 @@
 
 For API connection we are using library [python-binance](https://github.com/sammchardy/python-binance).
 
 **You can say Thanks:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
+or by [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** through the exchange (no commission)
 
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
-
-or by [Binance](https://accounts.binance.com/register?ref=200640624 ) **ID** (no commission) **200640624** through the exchange
+or by [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** through the exchange (no commission)
 
 ## Installation
 1) The simplest way:
 ```shell
 pip install backtrader_binance
 ```
 or
@@ -237,19 +235,17 @@
 
 Для подключения к API мы используем библиотеку [python-binance](https://github.com/sammchardy/python-binance ).
 
 **Можно сказать Спасибо:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
-
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
+или по [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** через биржу (без комиссии)
 
-или по [Binance](https://accounts.binance.com/register?ref=200640624 ) **ID** (без комиссии) **200640624** через биржу
+или по [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** через биржу (без комиссии)
 
 ## Установка
 1) Самый простой способ:
 ```shell
 pip install backtrader_binance
 ```
 или
```

### Comparing `backtrader_binance-2.0.4/setup.py` & `backtrader_binance-2.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the relevant file
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='backtrader_binance',
-      version='2.0.4',
+      version='2.0.5',
       author='wiseplat',
       author_email='oshpagin@gmail.com',
       license='MIT License',
       description='Binance API integration with Backtrader',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/WISEPLAT/backtrader_binance',
```

