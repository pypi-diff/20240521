# Comparing `tmp/bitopro-client-1.0.4.tar.gz` & `tmp/bitopro-client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitopro-client-1.0.4.tar", last modified: Thu Mar 14 13:35:23 2024, max compression
+gzip compressed data, was "bitopro-client-1.0.5.tar", last modified: Tue May 21 15:17:11 2024, max compression
```

## Comparing `bitopro-client-1.0.4.tar` & `bitopro-client-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 13:35:23.926305 bitopro-client-1.0.4/
--rw-rw-rw-   0        0        0     1084 2023-12-17 12:09:19.000000 bitopro-client-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      454 2024-03-14 13:35:23.925319 bitopro-client-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    13274 2023-12-19 07:01:25.000000 bitopro-client-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 13:35:23.913339 bitopro-client-1.0.4/bitoproClient/
--rw-rw-rw-   0        0        0     2316 2023-12-18 13:54:10.000000 bitopro-client-1.0.4/bitoproClient/bitopro_indicator.py
--rw-rw-rw-   0        0        0    20433 2023-12-18 07:01:48.000000 bitopro-client-1.0.4/bitoproClient/bitopro_restful_client.py
--rw-rw-rw-   0        0        0      660 2023-12-17 12:10:21.000000 bitopro-client-1.0.4/bitoproClient/bitopro_util.py
--rw-rw-rw-   0        0        0     4575 2023-12-17 12:13:30.000000 bitopro-client-1.0.4/bitoproClient/bitopro_websocket_client.py
-drwxrwxrwx   0        0        0        0 2024-03-14 13:35:23.923312 bitopro-client-1.0.4/bitopro_client.egg-info/
--rw-rw-rw-   0        0        0      454 2024-03-14 13:35:23.000000 bitopro-client-1.0.4/bitopro_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-03-14 13:35:23.000000 bitopro-client-1.0.4/bitopro_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 13:35:23.000000 bitopro-client-1.0.4/bitopro_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-14 13:35:23.000000 bitopro-client-1.0.4/bitopro_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-14 13:35:23.927302 bitopro-client-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      548 2024-03-14 13:32:58.000000 bitopro-client-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:11.437508 bitopro-client-1.0.5/
+-rw-rw-rw-   0        0        0     1084 2023-12-17 12:09:19.000000 bitopro-client-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      454 2024-05-21 15:17:11.436512 bitopro-client-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13274 2023-12-19 07:01:25.000000 bitopro-client-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:11.425715 bitopro-client-1.0.5/bitoproClient/
+-rw-rw-rw-   0        0        0     2316 2023-12-18 13:54:10.000000 bitopro-client-1.0.5/bitoproClient/bitopro_indicator.py
+-rw-rw-rw-   0        0        0    21319 2024-05-21 14:51:47.000000 bitopro-client-1.0.5/bitoproClient/bitopro_restful_client.py
+-rw-rw-rw-   0        0        0      660 2023-12-17 12:10:21.000000 bitopro-client-1.0.5/bitoproClient/bitopro_util.py
+-rw-rw-rw-   0        0        0     4575 2023-12-17 12:13:30.000000 bitopro-client-1.0.5/bitoproClient/bitopro_websocket_client.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:11.434561 bitopro-client-1.0.5/bitopro_client.egg-info/
+-rw-rw-rw-   0        0        0      454 2024-05-21 15:17:11.000000 bitopro-client-1.0.5/bitopro_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-21 15:17:11.000000 bitopro-client-1.0.5/bitopro_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:17:11.000000 bitopro-client-1.0.5/bitopro_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 15:17:11.000000 bitopro-client-1.0.5/bitopro_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:17:11.437508 bitopro-client-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      548 2024-05-21 15:09:25.000000 bitopro-client-1.0.5/setup.py
```

### Comparing `bitopro-client-1.0.4/LICENSE` & `bitopro-client-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.4/README.md` & `bitopro-client-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.4/bitoproClient/bitopro_indicator.py` & `bitopro-client-1.0.5/bitoproClient/bitopro_indicator.py`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.4/bitoproClient/bitopro_restful_client.py` & `bitopro-client-1.0.5/bitoproClient/bitopro_restful_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 
 class StatusKind(Enum):
     ALL = 0
     OPEN = 1
     DONE = 1
 
 class DepositStatus(Enum):
-    CANCELLED = 0
-    WAIT_PROCESS = 1
+    CANCELLED = 0,
+    WAIT_PROCESS = 1,
+    PROCESSING = 2,
+    COMPLETE = 3,
+    EXPIRED = 4,
+    INVALID = 5,
 
 class WithdrawProtocol(Enum):
     MAIN = 0,
     ERC20 = 1, 
     OMNI = 2, 
     TRX = 3, 
     BSC = 4,
@@ -309,14 +313,31 @@
         :return: an order infomation
         """   
         endpoint = f"/orders/{pair}/{order_id}"
         complete_url = self.baseUrl + endpoint
         header = {"identity": "", "nonce": get_current_timestamp()}
         headers = build_headers(self.__api_key, self.__api_secret, params=header)
         return self.send_request(method="GET", url=complete_url, headers=headers)
+    
+    def get_open_orders(self, pair:str=None):
+        """
+        https://github.com/bitoex/bitopro-offical-api-docs/blob/add_list_open_orders_doc/api/v3/private/get_open_orders_data.md
+        :param pair: the trading pair in format.
+        :param order_id: the id of the order.	
+        :return: all open orders and descending ordered by updated time
+        """   
+        endpoint = f"/orders/open"
+        complete_url = self.baseUrl + endpoint
+        params = {
+            **({"pair": pair} if pair is not None else {}),
+        }
+
+        header = {"identity": "", "nonce": get_current_timestamp()}
+        headers = build_headers(self.__api_key, self.__api_secret, params=header)
+        return self.send_request(method="GET", url=complete_url, headers=headers, data=params)
 
     def get_trades_list(self, pair:str=None, start_timestamp:int=None, end_timestamp:int=None, order_id:str=None, trade_id:str=None, limit:int=100):
         """
         https://github.com/bitoex/bitopro-offical-api-docs/blob/master/api/v3/private/get_trades_data.md
         :param pair: the trading pair in format.
         :param start_timestamp: start time in unix timestamp.
         :param end_timestamp: end time in unix timestamp.
```

### Comparing `bitopro-client-1.0.4/bitoproClient/bitopro_util.py` & `bitopro-client-1.0.5/bitoproClient/bitopro_util.py`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.4/bitoproClient/bitopro_websocket_client.py` & `bitopro-client-1.0.5/bitoproClient/bitopro_websocket_client.py`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.4/setup.py` & `bitopro-client-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import pathlib
 from setuptools import setup, find_packages
  
 HERE = pathlib.Path(__file__).parent.resolve()
 
 setup(name='bitopro-client',
-    version='1.0.4',
+    version='1.0.5',
     description='For BitoPro crypto currency exchange written in Python',
     url='https://github.com/bitoex/bitopro-api-python.git',
     author='Bitoex',
     author_email='support@bitopro.com',
     license='MIT',
     packages=['bitoproClient'],
     python_requires = ">=3.9",
```

