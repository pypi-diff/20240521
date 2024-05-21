# Comparing `tmp/safeheron_api_sdk_python-1.1.0.tar.gz` & `tmp/safeheron_api_sdk_python-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeheron_api_sdk_python-1.1.0.tar", last modified: Wed May  8 11:31:14 2024, max compression
+gzip compressed data, was "safeheron_api_sdk_python-1.1.1.tar", last modified: Tue May 21 11:52:35 2024, max compression
```

## Comparing `safeheron_api_sdk_python-1.1.0.tar` & `safeheron_api_sdk_python-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:31:14.347461 safeheron_api_sdk_python-1.1.0/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.1.0/LICENSE
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-08 11:31:14.346524 safeheron_api_sdk_python-1.1.0/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/README.md
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/README.rst
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:31:14.329900 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:31:14.340526 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9379 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/account_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2672 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/coin_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3490 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/mpc_sign_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    13785 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/transaction_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11075 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/web3_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:39:36.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/client.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:31:14.341738 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/cosigner/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3078 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/cosigner/co_signer_converter.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/tools.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:31:14.343084 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/webhook/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1851 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/webhook/webhook_converter.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:31:14.344996 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python.egg-info/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-08 11:31:14.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      675 2024-05-08 11:31:14.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 11:31:14.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       36 2024-05-08 11:31:14.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python.egg-info/requires.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-08 11:31:14.000000 safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 11:31:14.347638 safeheron_api_sdk_python-1.1.0/setup.cfg
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      929 2024-05-08 11:30:59.000000 safeheron_api_sdk_python-1.1.0/setup.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 11:52:35.560096 safeheron_api_sdk_python-1.1.1/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.1.1/LICENSE
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-21 11:52:35.559128 safeheron_api_sdk_python-1.1.1/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     5327 2024-05-17 02:38:51.000000 safeheron_api_sdk_python-1.1.1/README.md
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.1/README.rst
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 11:52:35.525067 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 11:52:35.554172 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9934 2024-05-15 11:09:36.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/account_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2676 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/coin_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3484 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/mpc_sign_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    16938 2024-05-21 11:14:31.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/transaction_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11104 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/web3_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1192 2024-05-17 03:08:06.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/client.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 11:52:35.555338 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/cosigner/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3393 2024-05-21 11:48:29.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/cosigner/co_signer_converter.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    10207 2024-05-21 11:50:19.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/tools.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 11:52:35.556606 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/webhook/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2060 2024-05-21 11:47:35.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/webhook/webhook_converter.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 11:52:35.558234 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python.egg-info/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-21 11:52:35.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      675 2024-05-21 11:52:35.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-21 11:52:35.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       36 2024-05-21 11:52:35.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-21 11:52:35.000000 safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-21 11:52:35.560260 safeheron_api_sdk_python-1.1.1/setup.cfg
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      929 2024-05-21 11:45:35.000000 safeheron_api_sdk_python-1.1.1/setup.py
```

### Comparing `safeheron_api_sdk_python-1.1.0/LICENSE` & `safeheron_api_sdk_python-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.0/README.md` & `safeheron_api_sdk_python-1.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,43 @@
 
 # Installation
 
 ```shell
 $ pip install safeheron-api-sdk-python
 ```
 
+# Usage
+```python
+from safeheron_api_sdk_python.api.account_api import *
+```
+
+> Take [`/v1/account/create`](https://docs.safeheron.com/api/index.html) as an example to explain, the complete code can be found in `demo/api_demo` directory
+
+* Construct `config`
+    ```python
+    # You can get `ApiKey` and `SafeheronRsaPublicKey` from Safeheron Web Console: https://www.safeheron.com/console.
+    config={
+            'apiKey': '5921aa306f*******368db9abf', 
+            'privateKeyPemFile': './my_private.pem',
+            'safeheronPublicKey': 'MIICIjANBgkqhkiG9w0***********+zSdC+8eBdZyI7nMdPIj6xOhUCAwEAAQ==',
+            'baseUrl': 'https://api.safeheron.vip',
+            'RequestTimeout': 10000
+  }
+    ```
+* Call `create_account` api with `config`
+    ```python
+    account_api = AccountApi(config)
+    param = CreateAccountRequest()
+    param.accountName = "accountNameTest"
+    res = account_api.create_account(param)
+    # Your code to process response
+    ...
+    ...
+    ```
+
 # Test
 
 ## Test Create Wallet Account
 * Before run the test code, modify `demo/api_demo/account/config.yaml.example` according to the comments
     ```yaml
     # Your api key, you can get it from Safeheron Web Console: https://www.safeheron.com/console.
     apiKey: 080d****e06e60
@@ -23,14 +52,16 @@
     privateKey: MIIJRQIBA*******DtGRBdennqu8g95jcrMxCUhsifVgzP6vUyg==
     # path to your private key file, pem encoded.PrivateKeyPemFile priority is higher than privateKey.
     privateKeyPemFile: './my_private.pem'
     # Safeheron API public key, you can get it from Safeheron Web Console: https://www.safeheron.com/console.
     safeheronPublicKey: MIICI****QuTOTECAwEAAQ==
     # Safeheron API url
     baseUrl: https://api.safeheron.vip
+    # RequestTimeout (Millisecond), Default: 10000
+    requestTimeout: 10000
     ```
 * Copy config to `config.yaml` file.
     ```bash
     $ cd demo/api_demo/account
     $ cp config.yaml.example config.yaml
     ```
 * Pytest
@@ -46,14 +77,16 @@
     privateKey: MIIJRQIBA*******DtGRBdennqu8g95jcrMxCUhsifVgzP6vUyg==
     # path to your private key file, pem encoded.PrivateKeyPemFile priority is higher than privateKey.
     privateKeyPemFile: './my_private.pem'
     # Safeheron API public key, you can get it from Safeheron Web Console: https://www.safeheron.com/console.
     safeheronPublicKey: MIICI****QuTOTECAwEAAQ==
     # Safeheron API url
     baseUrl: https://api.safeheron.vip
+    # RequestTimeout (Millisecond), Default: 10000
+    requestTimeout: 10000
     # Wallet Account key
     accountKey: account****5ecad40
     # To address
     destinationAddress: "0x943****0BF95f5"
     ```
 * Copy config to `config.yaml` file.
     ```bash
@@ -74,14 +107,16 @@
     privateKey: MIIJRQIBA*******DtGRBdennqu8g95jcrMxCUhsifVgzP6vUyg==
     # path to your private key file, pem encoded.PrivateKeyPemFile priority is higher than privateKey.
     privateKeyPemFile: './my_private.pem'
     # Safeheron API public key, you can get it from Safeheron Web Console: https://www.safeheron.com/console.
     safeheronPublicKey: MIICI****QuTOTECAwEAAQ==
     # Safeheron API url
     baseUrl: https://api.safeheron.vip
+    # RequestTimeout (Millisecond), Default: 10000
+    requestTimeout: 10000
     # Wallet Account key
     accountKey: account****5ecad40
     # Goerli testnet token address in wallet account
     accountTokenAddress: "0x970****4ffD59"
     # erc20 token contract address
     erc20ContractAddress: "0x078****Eaa37F"
     # address to receive token
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/account_api.py` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/account_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,21 @@
         self.hiddenOnUI = None
         # Filter the response based on this account name prefix
         self.namePrefix = None
         # Filter the response based on this account name suffix
         self.nameSuffix = None
 
 
+class OneAccountRequest:
+    def __init__(self):
+        # Wallet account key
+        self.accountKey = None
+
+
+
 class CreateAccountRequest:
     def __init__(self):
         # Account name, within 30 characters
         self.accountName = None
         # 	Whether display in Safeheron Console
         # True: not display
         # False: display
@@ -36,14 +43,19 @@
         self.coinKeyList = None
 
 
 class BatchCreateAccountRequest:
     def __init__(self):
         # The prefix of wallet account name, 30 characters max
         self.accountName = None
+        # Display status in Safeheron App
+        # True: not display
+        # False: display
+        # Default: true
+        self.hiddenOnUI = None
         # Number of wallets to be created, greater than 0, less than 100
         self.count = None
         # Account tag
         self.accountTag = None
 
 
 class UpdateAccountShowStateRequest:
@@ -137,83 +149,87 @@
         # The number, max is 100
         self.addressGroupName = None
 
 
 class AccountApi:
 
     def __init__(self, config):
-        global api_client
-        api_client = Client(config)
+        self.api_client = Client(config)
 
     # List Wallet Accounts
     # Filter wallet account lists in team according to different combinations of conditions.
     def list_accounts(self, request: ListAccountRequest):
-        return api_client.send_request(request, '/v1/account/list')
+        return self.api_client.send_request(request, '/v1/account/list')
+
+    # Retrieve a Single Wallet Account
+    # Retrieve a single wallet account in the team by providing accountKey.
+    def one_accounts(self, request: OneAccountRequest):
+        return self.api_client.send_request(request, '/v1/account/one')
 
     # Create a new wallet account.
     def create_account(self, request: CreateAccountRequest):
-        return api_client.send_request(request, '/v1/account/create')
+        return self.api_client.send_request(request, '/v1/account/create')
 
     # Batch Create Wallet Accounts V1
     # Generate a batch of wallet accounts based on a specified quantity. By default, the wallet accounts created in bulk will not be displayed in the Safeheron App. For optimal results, we recommend using the V2 version.
     def batchCreate_accountV1(self, request: BatchCreateAccountRequest):
-        return api_client.send_request(request, '/v1/account/batch/create')
+        return self.api_client.send_request(request, '/v1/account/batch/create')
 
     # Batch Create Wallet Accounts V2
     # Generate a batch of wallet accounts based on a specified quantity. By default, the wallet accounts created in bulk will not be displayed in the Safeheron App.
     def batch_create_accountV2(self, request: BatchCreateAccountRequest):
-        return api_client.send_request(request, '/v2/account/batch/create')
+        return self.api_client.send_request(request, '/v2/account/batch/create')
 
     # Change Display of Wallet Account in App
     # Change wallet account status in Safeheron App.
     def update_account_show_state(self, request: UpdateAccountShowStateRequest):
-        return api_client.send_request(request, '/v1/account/update/show/state')
+        return self.api_client.send_request(request, '/v1/account/update/show/state')
 
     # Batch Label Wallet Accounts
     # Relabel a batch of wallet accounts.
     # Please note that it only supports to label wallets which are created by API. And, the wallets have been used to sweep the target account cannot be relabelled.
     def batch_update_account_tag(self, request: BatchUpdateAccountTagRequest):
-        return api_client.send_request(request, '/v1/account/batch/update/tag')
+        return self.api_client.send_request(request, '/v1/account/batch/update/tag')
 
     # Add Coins to a Wallet Account
     # Add a new coin to your wallet account, while generating the default address group for the added coin. Once successfully completed, it will return the address information of the newly created default address group. In case the added currency already exists within the account, it will promptly return the existing default address group information for that coin.
     # In a wallet account, UTXO-based cryptocurrencies can have multiple address groups, while other types of cryptocurrencies usually have only one. To check whether a particular cryptocurrency supports the addition of multiple address groups, simply check the 'isMultipleAddress' parameter through the Coin List.
     def create_account_coin(self, request: CreateAccountCoinRequest):
-        return api_client.send_request(request, '/v1/account/coin/create')
+        return self.api_client.send_request(request, '/v1/account/coin/create')
 
     # Batch Add Coins to Wallet Accounts
     # Bulk addition of specified coins to designated wallet accounts. And, it creates a default address group for each coin and returns the address information contained within the newly created default address group. If a wallet account already contains the currency being added, the function will return the default address group data for that existing coin.
     #
     def batch_create_account_coin(self, request: BatchCreateAccountCoinRequest):
-        return api_client.send_request(request, '/v1/account/batch/coin/create')
+        return self.api_client.send_request(request, '/v1/account/batch/coin/create')
 
     # List Coins Within a Wallet Account
     # Retrieve a complete list of all coins associated with a wallet account, along with the default address group information for each coin.
     #
     def list_account_coin(self, request: ListAccountCoinRequest):
-        return api_client.send_request(request, '/v1/account/coin/list')
+        return self.api_client.send_request(request, '/v1/account/coin/list')
 
     # List Coin Address Group of a Wallet Account
     # Retrieve all address groups for a coin within the wallet account.
     #
     def list_account_coin_address(self, request: ListAccountCoinAddressRequest):
-        return api_client.send_request(request, '/v1/account/coin/address/list')
+        return self.api_client.send_request(request, '/v1/account/coin/address/list')
 
     # Retrieve The Balance of an Address
     # Retrieve the balance of a specific coin address.
     def info_account_coin_address(self, request: InfoAccountCoinAddressRequest):
-        return api_client.send_request(request, '/v1/account/coin/address/info')
+        return self.api_client.send_request(request, '/v1/account/coin/address/info')
 
     # Rename Coin Address Group of a Wallet Account
     # Rename a coin address group of a wallet account.
     def rename_account_coin_address(self, request: RenameAccountCoinAddressRequest):
-        return api_client.send_request(request, '/v1/account/coin/address/name')
+        return self.api_client.send_request(request, '/v1/account/coin/address/name')
 
     # Add Address Group for UTXO-Based Coin
     # Add a new address group for UTXO-based cryptocurrencies under a wallet account. If the coin does not exist, it will be added first, followed by the new address group. The function will return the details of the added address(es).
     def create_account_coin_address(self, request: CreateAccountCoinAddressRequest):
-        return api_client.send_request(request, '/v1/account/coin/address/create')
+        return self.api_client.send_request(request, '/v1/account/coin/address/create')
 
     # Batch Add Address Groups for UTXO-Based Coin
     # For UTXO-based coins in a wallet account, it is possible to add multiple address groups to the account in bulk by specifying the wallet account and the desired number of address groups. The function will return the details of the added address groups. If the specified coin does not exist in the account, it will be added first, followed by the addition of the corresponding number of address groups.
     def batch_create_account_coin_UTXO(self, request: BatchCreateAccountCoinUTXORequest):
-        return api_client.send_request(request, '/v1/account/coin/utxo/batch/create')
+        return self.api_client.send_request(request, '/v1/account/coin/utxo/batch/create')
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/coin_api.py` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/coin_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,34 +36,33 @@
         # Coin key, multiple coin keys are separated by commas
         self.coinKey = None
 
 
 class CoinApi:
 
     def __init__(self, config):
-        global api_client
-        api_client = Client(config)
+        self.api_client = Client(config)
 
     # Coin List
     # Retrieve the list of coins supported by Safeheron.
     def list_coin(self):
-        return api_client.send_request(None, '/v1/coin/list')
+        return self.api_client.send_request(None, '/v1/coin/list')
 
     # Coin Maintenance List
     # Retrieve the information of coins under maintenance in Safeheron.
     def list_coin_maintain(self):
-        return api_client.send_request(None, '/v1/coin/maintain/list')
+        return self.api_client.send_request(None, '/v1/coin/maintain/list')
 
     # Verify Coin Address
     # Verify the correctness of a cryptocurrency address based on the provided validation attributes.
     def check_coin_address(self, request: CheckCoinAddressRequest):
-        return api_client.send_request(request, '/v1/coin/address/check')
+        return self.api_client.send_request(request, '/v1/coin/address/check')
 
     # Snapshot the Coin Balance
     # Safeheron takes and stores daily snapshots of balances based on the transaction block's creation time in GMT+8. Please note that the snapshot only keeps data within 30 days.
     def coin_balance_snapshot(self, request: CoinBalanceSnapshotRequest):
-        return api_client.send_request(request, '/v1/coin/balance/snapshot')
+        return self.api_client.send_request(request, '/v1/coin/balance/snapshot')
 
     # Retrieve Current Block Height for Currency
     # Retrieve the current block height for a specific cryptocurrency by providing its key.
     def coin_block_height(self, request: CoinBlockHeightRequest):
-        return api_client.send_request(request, '/v1/coin/block/height')
+        return self.api_client.send_request(request, '/v1/coin/block/height')
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/mpc_sign_api.py` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/mpc_sign_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,25 +53,24 @@
         # End time for creating a transaction, UNIX timestamp (ms) (If no value is provided, the default value is the current UTC time)
         self.createTimeMax = None
 
 
 class MPCSignApi:
 
     def __init__(self, config):
-        global api_client
-        api_client = Client(config)
+        self.api_client = Client(config)
 
     # Create an MPC Sign Transaction
     # Merchant can initiate MPC Sign via this interface. The merchant must first serialize the transaction data and generate a hash before using this interface to submit the hash and create a transaction. The resulting signature can be retrieved via the MPC Sign transaction interface or webhook. The merchant can proceed with the necessary follow-up processes to obtain the signature according to their specific needs.
     def create_mpc_sign_transactions(self, request: CreateMPCSignTransactionRequest):
         request.asDict()
-        return api_client.send_request(request, '/v1/transactions/mpcsign/create')
+        return self.api_client.send_request(request, '/v1/transactions/mpcsign/create')
 
     # Retrieve a Single MPC Sign Transaction
     # To query a specific MPC Sign transaction, either customerRefId or txKey must be provided. If both parameters are provided, the query will be based on the txKey parameter.
     def one_mpc_sign_transactions(self, request: OneMPCSignTransactionsRequest):
-        return api_client.send_request(request, '/v1/transactions/mpcsign/one')
+        return self.api_client.send_request(request, '/v1/transactions/mpcsign/one')
 
     # MPC Sign Transaction List
     # Filter MPC Sign transaction history by various conditions.
     def list_mpc_sign_transactions(self, request: ListMPCSignTransactionsRequest):
-        return api_client.send_request(request, '/v1/transactions/mpcsign/list')
+        return self.api_client.send_request(request, '/v1/transactions/mpcsign/list')
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/transaction_api.py` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/transaction_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -132,14 +132,16 @@
         self.destinationTag = None
         # Bitcoin enabled for RBF (Replace-by-fee is a protocol in the Bitcoin mempool that allows for the replacement of an unconfirmed transaction with another one)
         self.isRbf = None
         # The default setting for the parameter is [true]. This parameter determines whether a transaction can be created when the target address is a smart contract. If set to [false], a transaction can still be created for a contract address
         self.failOnContract = None
         # Custom nonce
         self.nonce = None
+        # Customizable sequence number on Aptos, similar to the nonce in the EVM.
+        self.sequenceNumber = None
         # Balance verification, BALANCE_CHECK by default
         self.balanceVerifyType = None
 
     def asDict(self):
         dict = self.__dict__
         dict["feeRateDto"] = dict["feeRateDto"].__dict__
         return dict
@@ -157,14 +159,64 @@
         self.maxFee = None
         # Filecoin gas premium, similar to EIP-1559 max priority fee
         self.gasPremium = None
         # Filecoin gas fee cap, similar to EIP-1559 max fee
         self.gasFeeCap = None
         # SUI gas budget, similar to EIP-1559 max fee
         self.gasBudget = None
+        # The gas price the transaction sender is willing to pay, similar to EVM gasPrice
+        self.gasUnitPrice = None
+        # The maximum number of gas units that the transaction sender is willing to spend to execute the transaction, similar to EVM gasLimit
+        self.maxGasAmount = None
+
+class CreateTransactionsUTXOMultiDestRequest:
+    def __init__(self):
+        # Merchant unique business ID (100 characters max)
+        self.customerRefId = None
+        # Merchant extended field (defined by merchant) shown to merchant (255 characters max)
+        self.customerExt1 = None
+        # Merchant extended field (defined by merchant) shown to merchant (255 characters max)
+        self.customerExt2 = None
+        # Transaction note (180 characters max)
+        self.note = None
+        # Coin key
+        self.coinKey = None
+        # Transaction Fee Rate Grade
+        # Choose between transaction fees. If the transaction fee rate is preset, it will take priority
+        self.txFeeLevel = None
+        # Transaction fee rate, either txFeeLevel or feeRateDto
+        self.feeRateDto = FeeRateDto()
+        # Maximum estimated transaction fee rate for a given transaction
+        self.maxTxFeeRate = None
+        # Source account key
+        self.sourceAccountKey = None
+        # Account type
+        self.sourceAccountType = None
+        # Destination address list
+        self.destinationAddressList = [DestinationAddress]
+        # Destination Tag
+        self.destinationTag = None
+        # Bitcoin enabled for RBF (Replace-by-fee is a protocol in the Bitcoin mempool that allows for the replacement of an unconfirmed transaction with another one)
+        self.isRbf = None
+
+    def asDict(self):
+        dict = self.__dict__
+        dict["feeRateDto"] = dict["feeRateDto"].__dict__
+        destinationAddressList = []
+        for time in dict["destinationAddressList"]:
+            destinationAddressList.append(time.__dict__)
+        dict["destinationAddressList"] = destinationAddressList
+        return dict
+
+class DestinationAddress:
+    def __init__(self):
+        # Destination address
+        self.address = None
+        # Transaction amount
+        self.amount = None
 
 
 class RecreateTransactionRequest:
     def __init__(self):
         # Transaction key
         self.txKey = None
         # Transaction hash
@@ -199,17 +251,27 @@
         self.txHash = None
         # Source account key, required for UTXO-based coins
         self.sourceAccountKey = None
         # Source address are required for TRON when estimating transaction fees. For EVM-based transactions, the source address is required when retrieving the gas limit on the blockchain. Otherwise, a default fixed gas limit value will be returned
         self.sourceAddress = None
         # Destination address is optional for TRON and FIL when estimating transaction fees (although providing it may result in a more accurate fee estimation). For EVM-based transactions, the destination address is required when retrieving the gas limit on the blockchain. Otherwise, a default fixed gas limit value will be returned
         self.destinationAddress = None
+        # Destination address list
+        self.destinationAddressList = [DestinationAddress]
         # Transfer amount is required to calculate gas limit more accurately when using EVM chains. When using UTXO, providing the amount can estimate transaction fees more accurately. If no amount is provided, the calculation is based on the maximum UTXO quantity. When using SUI, providing the amount can estimate gas budget more accurately
         self.value = None
 
+    def asDict(self):
+        dict = self.__dict__
+        destinationAddressList = []
+        for time in dict["destinationAddressList"]:
+            destinationAddressList.append(time.__dict__)
+        dict["destinationAddressList"] = destinationAddressList
+        return dict
+
 
 class CancelTransactionRequest:
     def __init__(self):
         # Transaction key
         self.txKey = None
         # Transaction type, TRANSACTION by default
         self.txType = None
@@ -249,50 +311,54 @@
         # Destination Tag
         self.destinationTag = None
 
 
 class TransactionApi:
 
     def __init__(self, config):
-        global api_client
-        api_client = Client(config)
+        self.api_client = Client(config)
 
     # Transaction List V1
     # Filter transaction history by various conditions. For optimal results, we recommend using the V2 version.
     def list_transactions_v1(self, request: ListTransactionsV1Request):
-        return api_client.send_request(request, '/v1/transactions/list')
+        return self.api_client.send_request(request, '/v1/transactions/list')
 
     # Transaction List V2
     # Filter transaction history by various conditions.
     def list_transactions_v2(self, request: ListTransactionsV2Request):
-        return api_client.send_request(request, '/v2/transactions/list')
+        return self.api_client.send_request(request, '/v2/transactions/list')
 
     # Create a new transaction.
     def create_transactions(self, request: CreateTransactionRequest):
         request.asDict()
-        return api_client.send_request(request, '/v2/transactions/create')
+        return self.api_client.send_request(request, '/v2/transactions/create')
+
+    # For UTXOs that natively support multiple OUTPUTs, this interface allows a single transaction to transfer funds to multiple destination addresses simultaneously.(To use the Co-Signer, please use version 1.5.9 or higher)
+    def create_transactions_UTXO_multiDest(self, request: CreateTransactionsUTXOMultiDestRequest):
+        request.asDict()
+        return self.api_client.send_request(request, '/v1/transactions/utxo/multidest/create')
 
     # Speed up EVM and UTXO-based Transactions
     # Transactions with low transaction fees and those that have been pending for a long time can be sped up. EVM-based and BTC transactions can be sped up through RBF(If 'isRbf' is set to true during transaction creation, the transaction will be accelerated using RBF acceleration. Otherwise, CPFP acceleration will be used.) For other UTXO-based transactions, CPFP will be used.
     def recreate_transactions(self, request: RecreateTransactionRequest):
         request.asDict()
-        return api_client.send_request(request, '/v2/transactions/recreate')
+        return self.api_client.send_request(request, '/v2/transactions/recreate')
 
     # Retrieve a Transaction
     # To query a transaction, either customerRefId or txKey are required. If both values are provided, the retrieval will be based on the txKey.
     def one_transactions(self, request: OneTransactionsRequest):
-        return api_client.send_request(request, '/v1/transactions/one')
+        return self.api_client.send_request(request, '/v1/transactions/one')
 
     # Estimate Transaction Fee
     # This interface provides users with an estimated range of transaction fee rates of a given cryptocurrency when creating or speeding up transactions.
     def transaction_fee_rate(self, request: TransactionsFeeRateRequest):
-        return api_client.send_request(request, '/v2/transactions/getFeeRate')
+        return self.api_client.send_request(request, '/v2/transactions/getFeeRate')
 
     # Cancel Transaction
     # Cancel the authorization-pending transaction and the signing-in-progress transaction.
     def cancel_transactions(self, request: CancelTransactionRequest):
-        return api_client.send_request(request, '/v1/transactions/cancel')
+        return self.api_client.send_request(request, '/v1/transactions/cancel')
 
     # UTXO-Based Coin Sweeping
     # For multi-address UTXO coins under a wallet account, this interface allows users to collect the balances of certain qualifying addresses into a specified destination address.
     def collectionTransactionsUTXO(self, request: CollectionTransactionsUTXORequest):
-        return api_client.send_request(request, '/v1/transactions/utxo/collection')
+        return self.api_client.send_request(request, '/v1/transactions/utxo/collection')
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/api/web3_api.py` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/api/web3_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,62 +196,61 @@
         # End time for creating a transaction, UNIX timestamp (ms) (If no value is provided, the default value is the current UTC time)
         self.createTimeMax = None
 
 
 class Web3Api:
 
     def __init__(self, config):
-        global api_client
-        api_client = Client(config)
+        self.api_client = Client(config)
 
     # Create a Web3 Wallet Account
     def createWeb3Account(self, request: CreateWeb3AccountRequest):
-        return api_client.send_request(request, '/v1/web3/account/create')
+        return self.api_client.send_request(request, '/v1/web3/account/create')
 
     # Batch Create Web3 Wallet Accounts
     # Create a batch of wallet accounts based on specified number. Web3 wallet accounts created in batches are not displayed in the Safeheron App by default.
     def batchCreateWeb3Account(self, request: BatchCreateWeb3AccountRequest):
-        return api_client.send_request(request, '/v1/web3/batch/account/create')
+        return self.api_client.send_request(request, '/v1/web3/batch/account/create')
 
     # List Web3 Wallet Accounts
     # Filter Web3 wallet account lists by various conditions.
     def listWeb3Accounts(self, request: ListWeb3AccountRequest):
-        return api_client.send_request(request, '/v1/web3/account/list')
+        return self.api_client.send_request(request, '/v1/web3/account/list')
 
     # Create ethSign
     # Merchants can initiate an ethSign signature through this interface. The merchant is required to serialize the transaction data, generating a corresponding hash (supporting both 0x and non-0x formatted data). The hash is then submitted through this interface to create a signature, which can be obtained by Retrieve a Single Web3 Signature interface or webhook. From there, merchants can complete the subsequent steps according to their own needs once they have obtained the signature.
     def createWeb3EthSign(self, request: CreateWeb3EthSignRequest):
         request.asDict();
-        return api_client.send_request(request, '/v1/web3/sign/ethSign')
+        return self.api_client.send_request(request, '/v1/web3/sign/ethSign')
 
     # Create personalSign
     # Merchants can initiate a personalSign signature for any text using this interface. The merchant only needs to prepare the data to be signed and submit it through this interface to create the signature. The resulting signature can then be obtained by Retrieve a Single Web3 Signature interface or via webhook. From there, merchants can complete the subsequent steps according to their own needs once they have obtained the signature.
     def createWeb3PersonalSign(self, request: CreateWeb3PersonalSignRequest):
         request.asDict()
-        return api_client.send_request(request, '/v1/web3/sign/personalSign')
+        return self.api_client.send_request(request, '/v1/web3/sign/personalSign')
 
     # Create ethSignTypedData
     # Merchants can initiate an ethSignTypedData signature of specific formatted data (supporting data formats of v1, v3, and v4) through this interface. Merchants will need to format their signature data and submit it through the interface. Once the signature is created, the result can be retrieved via Retrieve a Single Web3 Signature interface or webhook. From there, merchants can complete the subsequent steps according to their own needs once they have obtained the signature.
     def createWeb3EthSignTypedData(self, request: CreateWeb3EthSignTypedDataRequest):
         request.asDict()
-        return api_client.send_request(request, '/v1/web3/sign/ethSignTypedData')
+        return self.api_client.send_request(request, '/v1/web3/sign/ethSignTypedData')
 
     # Create ethSignTransaction
     # Merchants can initiate ethSignTransaction signature transactions through this interface. The merchant must prepare transaction-related data, such as from, to, nonce, gas limit, gas price, value, data, and more. Once this data is submitted, a signature is created and the result can be obtained by Retrieve a Single Web3 Signature interface or webhook. From there, merchants can complete the subsequent steps according to their own needs once they have obtained the signature.
     def createWeb3EthSignTransaction(self, request: CreateWeb3EthSignTransactionRequest):
         request.asDict()
-        return api_client.send_request(request, '/v1/web3/sign/ethSignTransaction')
+        return self.api_client.send_request(request, '/v1/web3/sign/ethSignTransaction')
 
     # Cancel Signature
     # Cancel pending signatures.
     def cancelWeb3Sign(self, request: CancelWeb3SignRequest):
-        return api_client.send_request(request, '/v1/web3/sign/cancel')
+        return self.api_client.send_request(request, '/v1/web3/sign/cancel')
 
     # Retrieve a Single Web3 Signature
     # To query a transaction, either customerRefId or txKey are required. If both values are provided, the retrieval will be based on the txKey.
     def oneWeb3Sign(self, request: OneWeb3SignRequest):
-        return api_client.send_request(request, '/v1/web3/sign/one')
+        return self.api_client.send_request(request, '/v1/web3/sign/one')
 
     # Web3 Sign Transaction List
     # Filter Web3 Sign history by various conditions.
     def listWeb3Sign(self, request: ListWeb3SignRequest):
-        return api_client.send_request(request, '/v1/web3/sign/list')
+        return self.api_client.send_request(request, '/v1/web3/sign/list')
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/cosigner/co_signer_converter.py` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/cosigner/co_signer_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,60 +11,70 @@
         # txKey
         self.txKey = None
 
 
 class CoSignerConverter:
 
     def __init__(self, config):
-        global api_pub_key
-        global biz_privKey
-        api_pub_key = config['apiPubKey']
-        if 'bizPrivKey' in config:
-            biz_privKey = PEM_PRIVATE_HEAD + config['bizPrivKey'] + PEM_PRIVATE_END
-        if 'bizPrivKeyPemFile' in config:
-            private_key_pem_file = config['bizPrivKeyPemFile']
-            if private_key_pem_file is not None and private_key_pem_file != '':
-                biz_privKey = load_rsa_private_key(private_key_pem_file)
+        self.api_pub_key = config['apiPubKey']
+        if config.get('bizPrivKey'):
+            self.biz_privKey = PEM_PRIVATE_HEAD + config['bizPrivKey'] + PEM_PRIVATE_END
+        if config.get('bizPrivKeyPemFile'):
+            self.biz_privKey = load_rsa_private_key(config['bizPrivKeyPemFile'])
+
 
     def request_convert(self, co_signer_call_back):
-        platform_rsa_pk = get_rsa_key(PEM_PUBLIC_HEAD + api_pub_key + PEM_PUBLIC_END)
-        api_user_rsa_sk = get_rsa_key(biz_privKey)
+        platform_rsa_pk = get_rsa_key(PEM_PUBLIC_HEAD + self.api_pub_key + PEM_PUBLIC_END)
+        api_user_rsa_sk = get_rsa_key(self.biz_privKey)
         required_keys = {
             'key',
             'sig',
             'bizContent',
             'timestamp',
         }
 
         missing_keys = required_keys.difference(co_signer_call_back.keys())
         if missing_keys:
             raise Exception(co_signer_call_back)
 
         # 1 rsa verify
+        if "rsaType" in co_signer_call_back:
+            rsaType = co_signer_call_back.pop('rsaType')
+
+
+        if "aesType" in co_signer_call_back:
+            aesType = co_signer_call_back.pop('aesType')
+
         sig = co_signer_call_back.pop('sig')
         need_sign_message = sort_request(co_signer_call_back)
         v = rsa_verify(platform_rsa_pk, need_sign_message, sig)
         if not v:
             raise Exception("rsa verify: false")
 
         # 2 get aes key and iv
         key = co_signer_call_back.pop('key')
-        aes_data = rsa_decrypt(api_user_rsa_sk, key)
+        if ECB_OAEP_TYPE == rsaType:
+            aes_data = rsa_oaep_decrypt(api_user_rsa_sk, key)
+        else:
+            aes_data = rsa_decrypt(api_user_rsa_sk, key)
         aes_key = aes_data[0:32]
         aes_iv = aes_data[32:48]
 
         # 3 aes decrypt data, get response data
-        r = aes_decrypt(aes_key, aes_iv, b64decode(co_signer_call_back['bizContent']))
+        if GCM_TYPE == aesType:
+            r = aes_gcm_decrypt(aes_key, aes_iv, b64decode(co_signer_call_back['bizContent']))
+        else:
+            r = aes_decrypt(aes_key, aes_iv, b64decode(co_signer_call_back['bizContent']))
         # response_dict['bizContent'] = json.loads(r.decode())
 
         return json.loads(r.decode())
 
     def response_converter(self, co_signer_response: CoSignerResponse):
-        platform_rsa_pk = get_rsa_key(PEM_PUBLIC_HEAD + api_pub_key + PEM_PUBLIC_END)
-        api_user_rsa_sk = get_rsa_key(PEM_PRIVATE_HEAD + biz_privKey + PEM_PRIVATE_END)
+        platform_rsa_pk = get_rsa_key(PEM_PUBLIC_HEAD + self.api_pub_key + PEM_PUBLIC_END)
+        api_user_rsa_sk = get_rsa_key(PEM_PRIVATE_HEAD + self.biz_privKey + PEM_PRIVATE_END)
 
         ret = dict()
 
         # prepare aes key and iv
         aes_key = get_random_bytes(32)
         aes_iv = get_random_bytes(16)
         response_data = json.dumps(co_signer_response.__dict__).replace('\'', '\"').replace('\n', '').encode('utf-8')
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/tools.py` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-# Crypto 可直接替换为 Cryptodome
 from Cryptodome.Cipher import AES
 from Cryptodome.Util.Padding import pad, unpad
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Random import get_random_bytes
 from base64 import b64encode, b64decode
 from Cryptodome.Signature import PKCS1_v1_5 as Signature_pkcs1_v1_5
 from Cryptodome.Cipher import PKCS1_v1_5 as Cipher_pkcs1_v1_5
 from Cryptodome.Hash import SHA256, SHA1
 from Cryptodome import Random
+from Crypto.Cipher import PKCS1_OAEP
 import json
 import time
 import requests
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.backends import default_backend
 
 
 PEM_PUBLIC_HEAD = "-----BEGIN PUBLIC KEY-----\n"
 PEM_PUBLIC_END = "\n-----END PUBLIC KEY-----"
 PEM_PRIVATE_HEAD = "-----BEGIN RSA PRIVATE KEY-----\n"
 PEM_PRIVATE_END = "\n-----END RSA PRIVATE KEY-----"
 
+
+GCM_TYPE = "GCM_NOPADDING"
+ECB_OAEP_TYPE = "ECB_OAEP"
+
 def load_rsa_private_key(file_path, password=None):
     try:
         with open(file_path, "rb") as key_file:
             private_key = serialization.load_pem_private_key(
                 key_file.read(),
                 password=password,
                 backend=default_backend()
@@ -51,24 +55,44 @@
         cipher = AES.new(key, AES.MODE_CBC, iv)
         encrypt_text = cipher.encrypt(message)
     except Exception as e:
         raise Exception("aes encrypt error: %s" % e)
     return encrypt_text
 
 
+def aes_gcm_encrypt(key: bytes, iv: bytes, message: bytes):
+    check_key_and_iv(key, iv)
+    try:
+        cipher = AES.new(key, AES.MODE_GCM, iv)
+        cipher_text, tag = cipher.encrypt_and_digest(message)
+    except Exception as e:
+        raise Exception("aes encrypt error: %s" % e)
+    return cipher_text + tag
+
+
 def aes_decrypt(key: bytes, iv: bytes, encrypt_text: bytes):
     check_key_and_iv(key, iv)
     try:
         cipher = AES.new(key, AES.MODE_CBC, iv)
         pad_text = cipher.decrypt(encrypt_text)
     except Exception as e:
         raise Exception("aes decrypt error: %s" % e)
     return unpad(pad_text, AES.block_size)
 
 
+def aes_gcm_decrypt(key: bytes, iv: bytes, encrypt_text: bytes):
+    check_key_and_iv(key, iv)
+    try:
+        cipher = AES.new(key, AES.MODE_GCM, iv)
+        pad_text = cipher.decrypt(encrypt_text)
+    except Exception as e:
+        raise Exception("aes decrypt error: %s" % e)
+    return pad_text[0:len(pad_text)-len(iv)]
+
+
 def get_rsa_key(key_pem, passphrase=None):
     if key_pem == '':
         raise Exception("rsa encrypt error: pubkey can't be none")
     if passphrase is None:
         return RSA.import_key(key_pem)
     else:
         return RSA.import_key(key_pem, passphrase=passphrase)
@@ -80,24 +104,43 @@
         encrypt_text = cipher_rsa.encrypt(message)
     except Exception as e:
         raise Exception("rsa encrypt error: %s" % e)
     encrypt_text_base64 = b64encode(encrypt_text)
     return encrypt_text_base64.decode('utf-8')
 
 
+def rsa_oaep_encrypt(public_key, message: bytes):
+    try:
+        cipher = PKCS1_OAEP.new(public_key, hashAlgo=SHA256)
+        encrypt_text = cipher.encrypt(message)
+    except Exception as e:
+        raise Exception("rsa encrypt error: %s" % e)
+    encrypt_text_base64 = b64encode(encrypt_text)
+    return encrypt_text_base64.decode('utf-8')
+
+
 def rsa_decrypt(private_key, message: str):
     encrypt_text = b64decode(message)
     try:
         cipher_rsa = Cipher_pkcs1_v1_5.new(private_key)
         sentinel = Random.new().read(SHA1.digest_size)
         return cipher_rsa.decrypt(encrypt_text, sentinel)
     except Exception as e:
         raise Exception("rsa decrypt error: %s" % e)
 
 
+def rsa_oaep_decrypt(private_key, message: str):
+    encrypt_text = b64decode(message)
+    try:
+        cipher_rsa = PKCS1_OAEP.new(private_key, hashAlgo=SHA256)
+        return cipher_rsa.decrypt(encrypt_text)
+    except Exception as e:
+        raise Exception("rsa decrypt error: %s" % e)
+
+
 def rsa_sign(private_key, message_hash: bytes):
     try:
         signer = Signature_pkcs1_v1_5.new(private_key)
         digest = SHA256.new()
         digest.update(message_hash)
         signed = signer.sign(digest)
         return b64encode(signed).decode()
@@ -117,15 +160,15 @@
 
 def sort_request(r: dict):
     sortData = json.dumps(r, sort_keys=True).replace(' ', '')
     strArr = []
     data1 = json.loads(sortData)
     for key, value in data1.items():
         # print(value, type(value))
-        if isinstance(value, dict):  # 注意：对于dict类型的数据，一定要保留双引号，但python默认都是单引号
+        if isinstance(value, dict):
             val = json.dumps(value).replace(' ', '')
         else:
             val = value
         strArr.append(key + '=' + str(val))
     return "&".join(strArr).encode('utf-8')
 
 
@@ -140,29 +183,30 @@
     # prepare aes key and iv
     aes_key = get_random_bytes(32)
     aes_iv = get_random_bytes(16)
 
 
     # 1 rsa encrypt aes key + iv
     aes_data = aes_key + aes_iv
-    ret['key'] = rsa_encrypt(platform_rsa_pk, aes_data)
+    ret['key'] = rsa_oaep_encrypt(platform_rsa_pk, aes_data)
 
     # 2 aes encrypt request data
     if request_dict is not None:
         request_data = json.dumps(request_dict.__dict__).replace('\'', '\"').replace('\n', '').encode('utf-8')
-        aes_encrypted_bytes = aes_encrypt(aes_key, aes_iv, request_data)
+        aes_encrypted_bytes = aes_gcm_encrypt(aes_key, aes_iv, request_data)
         ret['bizContent'] = b64encode(aes_encrypted_bytes).decode()
 
     # 3 set timestamp
     ret['timestamp'] = str(int(time.time() * 1000))
 
     # 4 sign request
     need_sign_message = sort_request(ret)
     ret['sig'] = rsa_sign(api_user_rsa_sk, need_sign_message)
-
+    ret['rsaType'] = ECB_OAEP_TYPE
+    ret['aesType'] = GCM_TYPE
     return ret
 
 
 def decrypt_response(response_dict, platform_rsa_pk, api_user_rsa_sk):
     platform_rsa_pk = get_rsa_key(PEM_PUBLIC_HEAD + platform_rsa_pk + PEM_PUBLIC_END)
     api_user_rsa_sk = get_rsa_key(api_user_rsa_sk)
     required_keys = {
@@ -174,28 +218,41 @@
         'message'
     }
     missing_keys = required_keys.difference(response_dict.keys())
     if missing_keys:
         raise Exception(response_dict)
 
     # 1 rsa verify
+    if "rsaType" in response_dict:
+        rsaType = response_dict.pop('rsaType')
+
+
+    if "aesType" in response_dict:
+        aesType = response_dict.pop('aesType')
+
     sig = response_dict.pop('sig')
     need_sign_message = sort_request(response_dict)
     v = rsa_verify(platform_rsa_pk, need_sign_message, sig)
     if not v:
         raise Exception("rsa verify: false")
 
     # 2 get aes key and iv
     key = response_dict.pop('key')
-    aes_data = rsa_decrypt(api_user_rsa_sk, key)
+    if ECB_OAEP_TYPE == rsaType:
+        aes_data = rsa_oaep_decrypt(api_user_rsa_sk, key)
+    else:
+        aes_data = rsa_decrypt(api_user_rsa_sk, key)
     aes_key = aes_data[0:32]
     aes_iv = aes_data[32:48]
 
     # 3 aes decrypt data, get response data
-    r = aes_decrypt(aes_key, aes_iv, b64decode(response_dict['bizContent']))
+    if GCM_TYPE == aesType:
+        r = aes_gcm_decrypt(aes_key, aes_iv, b64decode(response_dict['bizContent']))
+    else:
+        r = aes_decrypt(aes_key, aes_iv, b64decode(response_dict['bizContent']))
     #response_dict['bizContent'] = json.loads(r.decode())
 
     return json.loads(r.decode())
 
 #Used for webhook decryption callback request data
 def decrypt_request(response_dict, verify_rsa_pk, decrypt_rsa_sk):
     verify_rsa_pk = get_rsa_key(PEM_PUBLIC_HEAD + verify_rsa_pk + PEM_PUBLIC_END)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python/webhook/webhook_converter.py` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python/webhook/webhook_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,49 +3,57 @@
 sys.path.pop(0)
 from safeheron_api_sdk_python.tools import *
 
 
 class WebhookConverter:
 
     def __init__(self, config):
-        global safeheron_webHook_rsa_public_key
-        global web_hook_rsa_private_key
-        safeheron_webHook_rsa_public_key = config['safeheronWebHookRsaPublicKey']
-        if 'webHookRsaPrivateKey' in config:
-            web_hook_rsa_private_key = PEM_PRIVATE_HEAD + config['webHookRsaPrivateKey'] + PEM_PRIVATE_END
-        if 'webHookRsaPrivateKeyPemFile' in config:
-            private_key_pem_file = config['webHookRsaPrivateKeyPemFile']
-            if private_key_pem_file is not None and private_key_pem_file != '':
-                web_hook_rsa_private_key = load_rsa_private_key(private_key_pem_file)
+        self.safeheron_webHook_rsa_public_key = config['safeheronWebHookRsaPublicKey']
+        if config.get('webHookRsaPrivateKey'):
+            self.web_hook_rsa_private_key = PEM_PRIVATE_HEAD + config['webHookRsaPrivateKey'] + PEM_PRIVATE_END
+        if config.get('webHookRsaPrivateKeyPemFile'):
+            self.web_hook_rsa_private_key = load_rsa_private_key(config['webHookRsaPrivateKeyPemFile'])
 
     def converter(self, webhook):
-        platform_rsa_pk = get_rsa_key(PEM_PUBLIC_HEAD + safeheron_webHook_rsa_public_key + PEM_PUBLIC_END)
-        api_user_rsa_sk = get_rsa_key(web_hook_rsa_private_key)
+        platform_rsa_pk = get_rsa_key(PEM_PUBLIC_HEAD + self.safeheron_webHook_rsa_public_key + PEM_PUBLIC_END)
+        api_user_rsa_sk = get_rsa_key(self.web_hook_rsa_private_key)
         required_keys = {
             'key',
             'sig',
             'bizContent',
             'timestamp',
         }
 
         missing_keys = required_keys.difference(webhook.keys())
         if missing_keys:
             raise Exception(webhook)
 
         # 1 rsa verify
+        if "rsaType" in webhook:
+            rsaType = webhook.pop('rsaType')
+
+        if "aesType" in webhook:
+            aesType = webhook.pop('aesType')
+
         sig = webhook.pop('sig')
         need_sign_message = sort_request(webhook)
         v = rsa_verify(platform_rsa_pk, need_sign_message, sig)
         if not v:
             raise Exception("rsa verify: false")
 
         # 2 get aes key and iv
         key = webhook.pop('key')
-        aes_data = rsa_decrypt(api_user_rsa_sk, key)
+        if ECB_OAEP_TYPE == rsaType:
+            aes_data = rsa_oaep_decrypt(api_user_rsa_sk, key)
+        else:
+            aes_data = rsa_decrypt(api_user_rsa_sk, key)
         aes_key = aes_data[0:32]
         aes_iv = aes_data[32:48]
 
         # 3 aes decrypt data, get response data
-        r = aes_decrypt(aes_key, aes_iv, b64decode(webhook['bizContent']))
+        if GCM_TYPE == aesType:
+            r = aes_gcm_decrypt(aes_key, aes_iv, b64decode(webhook['bizContent']))
+        else:
+            r = aes_decrypt(aes_key, aes_iv, b64decode(webhook['bizContent']))
         # response_dict['bizContent'] = json.loads(r.decode())
 
         return json.loads(r.decode())
```

### Comparing `safeheron_api_sdk_python-1.1.0/safeheron_api_sdk_python.egg-info/SOURCES.txt` & `safeheron_api_sdk_python-1.1.1/safeheron_api_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.0/setup.py` & `safeheron_api_sdk_python-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r") as f:
     long_description = f.read()
 setup(name='safeheron_api_sdk_python',
-      version='1.1.0',
+      version='1.1.1',
       description='Python for Safeheron API',
       long_description=long_description,
       author='safeheron',
       author_email='support@safeheron.com',
       url='https://github.com/Safeheron/safeheron-api-sdk-python',
       install_requires=[
             'pyCryptodomex',
```

