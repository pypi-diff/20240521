# Comparing `tmp/backtrader_bybit-2.0.8.tar.gz` & `tmp/backtrader_bybit-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtrader_bybit-2.0.8.tar", last modified: Sat Apr  6 04:52:18 2024, max compression
+gzip compressed data, was "backtrader_bybit-2.0.9.tar", last modified: Tue May 21 04:28:32 2024, max compression
```

## Comparing `backtrader_bybit-2.0.8.tar` & `backtrader_bybit-2.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 04:52:18.536586 backtrader_bybit-2.0.8/
--rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_bybit-2.0.8/LICENSE
--rw-rw-rw-   0        0        0    31184 2024-04-06 04:52:18.536586 backtrader_bybit-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    29811 2024-03-18 06:34:30.000000 backtrader_bybit-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 04:52:18.531586 backtrader_bybit-2.0.8/backtrader_bybit/
--rw-rw-rw-   0        0        0       36 2024-02-03 14:15:41.000000 backtrader_bybit-2.0.8/backtrader_bybit/__init__.py
--rw-rw-rw-   0        0        0     9171 2024-02-05 17:46:55.000000 backtrader_bybit-2.0.8/backtrader_bybit/bybit_broker.py
--rw-rw-rw-   0        0        0    13887 2024-04-06 04:39:55.000000 backtrader_bybit-2.0.8/backtrader_bybit/bybit_feed.py
--rw-rw-rw-   0        0        0     6277 2024-03-06 06:57:44.000000 backtrader_bybit-2.0.8/backtrader_bybit/bybit_store.py
--rw-rw-rw-   0        0        0      828 2024-02-04 18:39:19.000000 backtrader_bybit-2.0.8/backtrader_bybit/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-06 04:52:18.535589 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/
--rw-rw-rw-   0        0        0    31184 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 04:52:18.537585 backtrader_bybit-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2174 2024-04-06 04:51:48.000000 backtrader_bybit-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:28:32.624994 backtrader_bybit-2.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_bybit-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0    31225 2024-05-21 04:28:32.624994 backtrader_bybit-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    29856 2024-05-21 04:26:00.000000 backtrader_bybit-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:28:32.619994 backtrader_bybit-2.0.9/backtrader_bybit/
+-rw-rw-rw-   0        0        0       36 2024-02-03 14:15:41.000000 backtrader_bybit-2.0.9/backtrader_bybit/__init__.py
+-rw-rw-rw-   0        0        0     9171 2024-02-05 17:46:55.000000 backtrader_bybit-2.0.9/backtrader_bybit/bybit_broker.py
+-rw-rw-rw-   0        0        0    13887 2024-04-06 04:39:55.000000 backtrader_bybit-2.0.9/backtrader_bybit/bybit_feed.py
+-rw-rw-rw-   0        0        0     6277 2024-03-06 06:57:44.000000 backtrader_bybit-2.0.9/backtrader_bybit/bybit_store.py
+-rw-rw-rw-   0        0        0      828 2024-02-04 18:39:19.000000 backtrader_bybit-2.0.9/backtrader_bybit/enums.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:28:32.623994 backtrader_bybit-2.0.9/backtrader_bybit.egg-info/
+-rw-rw-rw-   0        0        0    31225 2024-05-21 04:28:32.000000 backtrader_bybit-2.0.9/backtrader_bybit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-05-21 04:28:32.000000 backtrader_bybit-2.0.9/backtrader_bybit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:28:32.000000 backtrader_bybit-2.0.9/backtrader_bybit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-21 04:28:32.000000 backtrader_bybit-2.0.9/backtrader_bybit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-21 04:28:32.000000 backtrader_bybit-2.0.9/backtrader_bybit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:28:32.625994 backtrader_bybit-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2174 2024-05-21 04:27:41.000000 backtrader_bybit-2.0.9/setup.py
```

### Comparing `backtrader_bybit-2.0.8/LICENSE` & `backtrader_bybit-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.8/PKG-INFO` & `backtrader_bybit-2.0.9/backtrader_bybit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: backtrader_bybit
-Version: 2.0.8
+Name: backtrader-bybit
+Version: 2.0.9
 Summary: Bybit API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_bybit
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_bybit/blob/master/README.md
 Keywords: trading,development
@@ -37,19 +37,17 @@
 ✅ Online Example for [LIVE Trading Strategy for Ethereum on Bybit](https://www.kaggle.com/code/olegshpagin/live-trading-strategy-for-ethereum-on-bybit)
 
 
 **You can say Thanks:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
+or by [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** through the exchange (no commission)
 
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
-
-or by [Bybit](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** (no commission) **112927970** through the exchange
+or by [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** through the exchange (no commission)
 
 ## Installation
 1) The simplest way:
 ```shell
 pip install backtrader_bybit
 ```
 or
@@ -242,19 +240,17 @@
 ✅ Online Пример для [LIVE Trading Strategy for Ethereum on Bybit](https://www.kaggle.com/code/olegshpagin/live-trading-strategy-for-ethereum-on-bybit)
 
 
 **Можно сказать Спасибо:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
-
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
+или по [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** через биржу (без комиссии)
 
-или по [Bybit](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** (без комиссии) **112927970** через биржу 
+или по [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** через биржу (без комиссии) 
 
 
 ## Установка
 1) Самый простой способ:
 ```shell
 pip install backtrader_bybit
 ```
```

### Comparing `backtrader_bybit-2.0.8/README.md` & `backtrader_bybit-2.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,17 @@
 ✅ Online Example for [LIVE Trading Strategy for Ethereum on Bybit](https://www.kaggle.com/code/olegshpagin/live-trading-strategy-for-ethereum-on-bybit)
 
 
 **You can say Thanks:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
+or by [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** through the exchange (no commission)
 
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
-
-or by [Bybit](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** (no commission) **112927970** through the exchange
+or by [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** through the exchange (no commission)
 
 ## Installation
 1) The simplest way:
 ```shell
 pip install backtrader_bybit
 ```
 or
@@ -218,19 +216,17 @@
 ✅ Online Пример для [LIVE Trading Strategy for Ethereum on Bybit](https://www.kaggle.com/code/olegshpagin/live-trading-strategy-for-ethereum-on-bybit)
 
 
 **Можно сказать Спасибо:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
-
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
+или по [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** через биржу (без комиссии)
 
-или по [Bybit](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** (без комиссии) **112927970** через биржу 
+или по [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** через биржу (без комиссии) 
 
 
 ## Установка
 1) Самый простой способ:
 ```shell
 pip install backtrader_bybit
 ```
```

### Comparing `backtrader_bybit-2.0.8/backtrader_bybit/bybit_broker.py` & `backtrader_bybit-2.0.9/backtrader_bybit/bybit_broker.py`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.8/backtrader_bybit/bybit_feed.py` & `backtrader_bybit-2.0.9/backtrader_bybit/bybit_feed.py`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.8/backtrader_bybit/bybit_store.py` & `backtrader_bybit-2.0.9/backtrader_bybit/bybit_store.py`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.8/backtrader_bybit/enums.py` & `backtrader_bybit-2.0.9/backtrader_bybit/enums.py`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.8/backtrader_bybit.egg-info/PKG-INFO` & `backtrader_bybit-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: backtrader-bybit
-Version: 2.0.8
+Name: backtrader_bybit
+Version: 2.0.9
 Summary: Bybit API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_bybit
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_bybit/blob/master/README.md
 Keywords: trading,development
@@ -37,19 +37,17 @@
 ✅ Online Example for [LIVE Trading Strategy for Ethereum on Bybit](https://www.kaggle.com/code/olegshpagin/live-trading-strategy-for-ethereum-on-bybit)
 
 
 **You can say Thanks:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
+or by [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** through the exchange (no commission)
 
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
-
-or by [Bybit](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** (no commission) **112927970** through the exchange
+or by [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** through the exchange (no commission)
 
 ## Installation
 1) The simplest way:
 ```shell
 pip install backtrader_bybit
 ```
 or
@@ -242,19 +240,17 @@
 ✅ Online Пример для [LIVE Trading Strategy for Ethereum on Bybit](https://www.kaggle.com/code/olegshpagin/live-trading-strategy-for-ethereum-on-bybit)
 
 
 **Можно сказать Спасибо:**
 
 USDT (Tron TRC20): TEHaXZX7KLjAm4eLWdf4VKfsqRUQpv8fTT
 
-BTC (Bitcoin BTC): 1ENhx1HUMJZjGAfYaT1vfsqwKHgVkqwX1D
-
-ETH (Ethereum ERC20): 0xfd546640c911ba90d1409a4fbbb4322ae73e7814
+или по [**Binance**](https://accounts.binance.com/register?ref=200640624 ) **ID** **200640624** через биржу (без комиссии)
 
-или по [Bybit](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** (без комиссии) **112927970** через биржу 
+или по [**Bybit**](https://www.bybit.com/invite?ref=KXLXXE%230 ) **UID** **112927970** через биржу (без комиссии) 
 
 
 ## Установка
 1) Самый простой способ:
 ```shell
 pip install backtrader_bybit
 ```
```

### Comparing `backtrader_bybit-2.0.8/setup.py` & `backtrader_bybit-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the relevant file
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='backtrader_bybit',
-      version='2.0.8',
+      version='2.0.9',
       author='wiseplat',
       author_email='oshpagin@gmail.com',
       license='MIT License',
       description='Bybit API integration with Backtrader',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/WISEPLAT/backtrader_bybit',
```

