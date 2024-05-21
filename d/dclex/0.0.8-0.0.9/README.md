# Comparing `tmp/dclex-0.0.8.tar.gz` & `tmp/dclex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dclex-0.0.8.tar", last modified: Mon May 13 14:54:35 2024, max compression
+gzip compressed data, was "dclex-0.0.9.tar", last modified: Mon May 13 16:03:11 2024, max compression
```

## Comparing `dclex-0.0.8.tar` & `dclex-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.533091 dclex-0.0.8/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     8250 2024-01-31 17:39:20.000000 dclex-0.0.8/LICENSE
--rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-13 14:54:35.533091 dclex-0.0.8/PKG-INFO
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      450 2024-04-05 14:00:22.000000 dclex-0.0.8/README.md
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      739 2024-05-13 11:24:27.000000 dclex-0.0.8/pyproject.toml
--rw-rw-r--   0 clouds    (1001) clouds    (1001)       38 2024-05-13 14:54:35.533091 dclex-0.0.8/setup.cfg
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.529091 dclex-0.0.8/src/
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.529091 dclex-0.0.8/src/dclex/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      208 2024-05-09 11:47:56.000000 dclex-0.0.8/src/dclex/__init__.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    12427 2024-05-13 11:23:39.000000 dclex-0.0.8/src/dclex/dclex.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    12993 2024-05-10 16:55:28.000000 dclex-0.0.8/src/dclex/dclex_client.py
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.533091 dclex-0.0.8/src/dclex/resources/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    19297 2024-02-02 17:33:59.000000 dclex-0.0.8/src/dclex/resources/digital_identity_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    15662 2024-02-02 17:33:59.000000 dclex-0.0.8/src/dclex/resources/factory_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6200 2024-02-02 17:33:59.000000 dclex-0.0.8/src/dclex/resources/usdc_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     9883 2024-02-02 17:33:59.000000 dclex-0.0.8/src/dclex/resources/vault_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1188 2024-03-01 16:20:01.000000 dclex-0.0.8/src/dclex/settings.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     2285 2024-03-01 16:30:00.000000 dclex-0.0.8/src/dclex/types.py
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.533091 dclex-0.0.8/src/dclex.egg-info/
--rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/PKG-INFO
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      580 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/SOURCES.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)        1 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/dependency_links.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)       60 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/requires.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)        6 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/top_level.txt
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.533091 dclex-0.0.8/tests/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1167 2024-03-04 19:14:07.000000 dclex-0.0.8/tests/test_account.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6062 2024-03-04 19:14:07.000000 dclex-0.0.8/tests/test_orders.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1534 2024-04-05 13:55:04.000000 dclex-0.0.8/tests/test_stocks.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     7431 2024-05-13 11:23:39.000000 dclex-0.0.8/tests/test_transfers.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 16:03:11.959954 dclex-0.0.9/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     8250 2024-01-31 17:39:20.000000 dclex-0.0.9/LICENSE
+-rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-13 16:03:11.959954 dclex-0.0.9/PKG-INFO
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      450 2024-04-05 14:00:22.000000 dclex-0.0.9/README.md
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      739 2024-05-13 16:01:03.000000 dclex-0.0.9/pyproject.toml
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)       38 2024-05-13 16:03:11.959954 dclex-0.0.9/setup.cfg
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 16:03:11.955954 dclex-0.0.9/src/
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 16:03:11.959954 dclex-0.0.9/src/dclex/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      208 2024-05-09 11:47:56.000000 dclex-0.0.9/src/dclex/__init__.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    12517 2024-05-13 15:31:09.000000 dclex-0.0.9/src/dclex/dclex.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    13211 2024-05-13 15:45:09.000000 dclex-0.0.9/src/dclex/dclex_client.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 16:03:11.959954 dclex-0.0.9/src/dclex/resources/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    19297 2024-02-02 17:33:59.000000 dclex-0.0.9/src/dclex/resources/digital_identity_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    15662 2024-02-02 17:33:59.000000 dclex-0.0.9/src/dclex/resources/factory_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6200 2024-02-02 17:33:59.000000 dclex-0.0.9/src/dclex/resources/usdc_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     9883 2024-02-02 17:33:59.000000 dclex-0.0.9/src/dclex/resources/vault_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1188 2024-05-13 15:57:51.000000 dclex-0.0.9/src/dclex/settings.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     2285 2024-03-01 16:30:00.000000 dclex-0.0.9/src/dclex/types.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 16:03:11.959954 dclex-0.0.9/src/dclex.egg-info/
+-rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-13 16:03:11.000000 dclex-0.0.9/src/dclex.egg-info/PKG-INFO
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      580 2024-05-13 16:03:11.000000 dclex-0.0.9/src/dclex.egg-info/SOURCES.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)        1 2024-05-13 16:03:11.000000 dclex-0.0.9/src/dclex.egg-info/dependency_links.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)       60 2024-05-13 16:03:11.000000 dclex-0.0.9/src/dclex.egg-info/requires.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)        6 2024-05-13 16:03:11.000000 dclex-0.0.9/src/dclex.egg-info/top_level.txt
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 16:03:11.959954 dclex-0.0.9/tests/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1167 2024-03-04 19:14:07.000000 dclex-0.0.9/tests/test_account.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6218 2024-05-13 15:57:36.000000 dclex-0.0.9/tests/test_orders.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1534 2024-04-05 13:55:04.000000 dclex-0.0.9/tests/test_stocks.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     7431 2024-05-13 11:23:39.000000 dclex-0.0.9/tests/test_transfers.py
```

### Comparing `dclex-0.0.8/LICENSE` & `dclex-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/PKG-INFO` & `dclex-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dclex
-Version: 0.0.8
+Version: 0.0.9
 Summary: DCLEX python library
 License: DCLEX API Non-Commercial License
         
         This DCLEX API Non-Commercial License ("License") is an agreement between DCLEX inc. ("DCLEX") and You, and governs Your use of the API Code. By loging to your DCLEX account programmatically , you acknowledge that You consent to be legally bound by this Agreement.
         
         1. Introduction.
         1.1 DCLEX has developed application program interface ("API") code to permit its customers to use their own internal proprietary software tools in managing their accounts with DCLEX. This License is intended only for users who wish to use the API Code by itself as is, or in connection with or for the development of their own internal proprietary tools to manage their own DCLEX accounts. This License is NOT for anybody who is developing software applications that they wish to: (a) sell to third party users for a fee, or (b) give to third party users to generate an indirect financial benefit (e.g., commissions). If You wish to make a software application for the purposes described in the preceding sentence then please us at info@dclex.com.
```

### Comparing `dclex-0.0.8/pyproject.toml` & `dclex-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dclex"
-version = "0.0.8"
+version = "0.0.9"
 description = "DCLEX python library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 classifiers = [
     "Intended Audience :: Financial and Insurance Industry",
     "Programming Language :: Python :: 3.7",
```

### Comparing `dclex-0.0.8/src/dclex/dclex.py` & `dclex-0.0.9/src/dclex/dclex.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,7 +345,10 @@
                 ),
             }
         )
         signed_transaction = self._account.sign_transaction(transaction)
         return self._web3.eth.send_raw_transaction(
             signed_transaction.rawTransaction
         ).hex()
+
+    def is_market_open(self) -> bool:
+        return self._dclex_client.is_market_open()
```

### Comparing `dclex-0.0.8/src/dclex/dclex_client.py` & `dclex-0.0.9/src/dclex/dclex_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     pass
 
 
 class DclexClient:
     def __init__(self) -> None:
         self._token = None
 
-    def get_nonce(self) -> str:
+    @staticmethod
+    def get_nonce() -> str:
         response = requests.get(f"{DCLEX_BASE_URL}/users/nonce/")
         response.raise_for_status()
         return response.json()["nonce"]
 
     def login(self, message: str, signature: str, nonce: str) -> None:
         response = requests.post(
             f"{DCLEX_BASE_URL}/users/verify/",
@@ -311,14 +312,20 @@
                 symbol=price_data["symbol"],
                 last_price=Decimal(price_data["price"]),
                 timestamp=self._parse_timestamp(price_data["timestamp"]),
                 percentage_change=Decimal(price_data["percentageChange"]),
             )
 
     @staticmethod
+    def is_market_open() -> bool:
+        response = requests.get(f"{DCLEX_BASE_URL}/market-status/")
+        response.raise_for_status()
+        return response.json()["isMarketOpen"]
+
+    @staticmethod
     def _parse_timestamp(timestamp: str) -> datetime:
         return datetime.fromisoformat(timestamp).replace(tzinfo=timezone.utc)
 
     def _authorized_post(self, endpoint: str, request_data: dict) -> dict:
         response = requests.post(
             f"{DCLEX_BASE_URL}{endpoint}",
             headers={"Authorization": f"Token {self._token}"},
```

### Comparing `dclex-0.0.8/src/dclex/resources/digital_identity_contract_abi.json` & `dclex-0.0.9/src/dclex/resources/digital_identity_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/src/dclex/resources/factory_contract_abi.json` & `dclex-0.0.9/src/dclex/resources/factory_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/src/dclex/resources/usdc_contract_abi.json` & `dclex-0.0.9/src/dclex/resources/usdc_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/src/dclex/resources/vault_contract_abi.json` & `dclex-0.0.9/src/dclex/resources/vault_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/src/dclex/settings.py` & `dclex-0.0.9/src/dclex/settings.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/src/dclex/types.py` & `dclex-0.0.9/src/dclex/types.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/src/dclex.egg-info/PKG-INFO` & `dclex-0.0.9/src/dclex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dclex
-Version: 0.0.8
+Version: 0.0.9
 Summary: DCLEX python library
 License: DCLEX API Non-Commercial License
         
         This DCLEX API Non-Commercial License ("License") is an agreement between DCLEX inc. ("DCLEX") and You, and governs Your use of the API Code. By loging to your DCLEX account programmatically , you acknowledge that You consent to be legally bound by this Agreement.
         
         1. Introduction.
         1.1 DCLEX has developed application program interface ("API") code to permit its customers to use their own internal proprietary software tools in managing their accounts with DCLEX. This License is intended only for users who wish to use the API Code by itself as is, or in connection with or for the development of their own internal proprietary tools to manage their own DCLEX accounts. This License is NOT for anybody who is developing software applications that they wish to: (a) sell to third party users for a fee, or (b) give to third party users to generate an indirect financial benefit (e.g., commissions). If You wish to make a software application for the purposes described in the preceding sentence then please us at info@dclex.com.
```

### Comparing `dclex-0.0.8/src/dclex.egg-info/SOURCES.txt` & `dclex-0.0.9/src/dclex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/tests/test_account.py` & `dclex-0.0.9/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/tests/test_orders.py` & `dclex-0.0.9/tests/test_orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,7 +179,12 @@
         type="LIMIT",
         symbol="AMZN",
         quantity=2,
         price=Decimal(170),
         status=OrderStatus.CANCELED,
         date_of_cancellation=date.today() + timedelta(days=10),
     )
+
+
+def test_is_market_open_returns_if_market_is_currently_open(dclex, provider_url):
+    result = dclex.is_market_open()
+    assert isinstance(result, bool)
```

### Comparing `dclex-0.0.8/tests/test_stocks.py` & `dclex-0.0.9/tests/test_stocks.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.8/tests/test_transfers.py` & `dclex-0.0.9/tests/test_transfers.py`

 * *Files identical despite different names*

