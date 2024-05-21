# Comparing `tmp/fennel_invest_api-1.0.4.tar.gz` & `tmp/fennel_invest_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fennel_invest_api-1.0.4.tar", last modified: Tue Apr 23 15:54:53 2024, max compression
+gzip compressed data, was "fennel_invest_api-1.0.5.tar", last modified: Tue May 21 13:56:53 2024, max compression
```

## Comparing `fennel_invest_api-1.0.4.tar` & `fennel_invest_api-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:54:53.472663 fennel_invest_api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-23 15:54:53.468663 fennel_invest_api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-23 15:54:49.000000 fennel_invest_api-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:54:53.468663 fennel_invest_api-1.0.4/fennel_invest_api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 15:54:49.000000 fennel_invest_api-1.0.4/fennel_invest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-23 15:54:49.000000 fennel_invest_api-1.0.4/fennel_invest_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-23 15:54:49.000000 fennel_invest_api-1.0.4/fennel_invest_api/fennel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:54:53.468663 fennel_invest_api-1.0.4/fennel_invest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-23 15:54:53.000000 fennel_invest_api-1.0.4/fennel_invest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 15:54:53.000000 fennel_invest_api-1.0.4/fennel_invest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:54:53.000000 fennel_invest_api-1.0.4/fennel_invest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 15:54:53.000000 fennel_invest_api-1.0.4/fennel_invest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 15:54:53.000000 fennel_invest_api-1.0.4/fennel_invest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:54:53.472663 fennel_invest_api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-23 15:54:49.000000 fennel_invest_api-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:56:53.218773 fennel_invest_api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-21 13:56:53.218773 fennel_invest_api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:56:53.214773 fennel_invest_api-1.0.5/fennel_invest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/fennel_invest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/fennel_invest_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/fennel_invest_api/fennel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:56:53.218773 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:56:53.218773 fennel_invest_api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/setup.py
```

### Comparing `fennel_invest_api-1.0.4/PKG-INFO` & `fennel_invest_api-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-dotenv
 
 # Unofficial Fennel Invest API
 
 This is an unofficial API for Fennel.com. It is a simple Python wrapper around the Fennel.com GraphQL API. It is not affiliated with Fennel.com in any way.
 
@@ -42,28 +43,36 @@
     wait_for_2fa=False
     code="123456" # Should be six-digit integer from email
 )
 ```
 
 ## Usage: Get Stock Holdings
 ```python
-positions = fennel.get_stock_holdings()
-for position in positions:
-    print(position)
+account_ids = fennel.get_account_ids()
+for account_id in account_ids:
+    print(account_id)
+    positions = fennel.get_stock_holdings(account_id)
+    for position in positions:
+        print(position)
 ```
 
 ## Usage: Get Portfolio
 ```python
-portfolio = fennel.get_portfolio_summary()
+# For all accounts
+full_portfolio = fennel.get_full_accounts()
+print(full_portfolio)
+# For a single account ID
+portfolio = fennel.get_portfolio_summary(account_id)
 print(portfolio)
 ```
 
 ## Usage: Placing Orders
 ```python
 order = fennel.place_order(
+    account_id=account_id,
     symbol="AAPL",
     quantity=1,
     side="buy", # Must be "buy" or "sell"
     price="market" # Only market orders are supported for now
 )
 print(order)
 ```
```

### Comparing `fennel_invest_api-1.0.4/README.md` & `fennel_invest_api-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -32,28 +32,36 @@
     wait_for_2fa=False
     code="123456" # Should be six-digit integer from email
 )
 ```
 
 ## Usage: Get Stock Holdings
 ```python
-positions = fennel.get_stock_holdings()
-for position in positions:
-    print(position)
+account_ids = fennel.get_account_ids()
+for account_id in account_ids:
+    print(account_id)
+    positions = fennel.get_stock_holdings(account_id)
+    for position in positions:
+        print(position)
 ```
 
 ## Usage: Get Portfolio
 ```python
-portfolio = fennel.get_portfolio_summary()
+# For all accounts
+full_portfolio = fennel.get_full_accounts()
+print(full_portfolio)
+# For a single account ID
+portfolio = fennel.get_portfolio_summary(account_id)
 print(portfolio)
 ```
 
 ## Usage: Placing Orders
 ```python
 order = fennel.place_order(
+    account_id=account_id,
     symbol="AAPL",
     quantity=1,
     side="buy", # Must be "buy" or "sell"
     price="market" # Only market orders are supported for now
 )
 print(order)
 ```
```

### Comparing `fennel_invest_api-1.0.4/fennel_invest_api/fennel.py` & `fennel_invest_api-1.0.5/fennel_invest_api/fennel.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     def __init__(self, filename="fennel_credentials.pkl", path=None) -> None:
         self.session = requests.Session()
         self.endpoints = Endpoints()
         self.Bearer = None
         self.Refresh = None
         self.ID_Token = None
         self.timeout = 10
-        self.account_number = (
-            "00000000"  # Fennel only has 1 account which they don't share
-        )
+        self.account_ids = []  # For multiple accounts
         self.client_id = "FXGlhcVdamwozAFp8BZ2MWl6coPl6agX"
         self.filename = filename
         self.path = None
         if path is not None:
             self.path = path
         self._load_credentials()
 
@@ -112,14 +110,15 @@
             raise Exception(f"Failed to login: {response.text}")
         response = response.json()
         self.Bearer = response["access_token"]
         self.Refresh = response["refresh_token"]
         self.ID_Token = response["id_token"]
         self.refresh_token()
         self._save_credentials()
+        self.get_account_ids()
         return True
 
     def refresh_token(self):
         url = self.endpoints.oauth_url()
         headers = self.endpoints.build_headers(accounts_host=True)
         payload = {
             "grant_type": "refresh_token",
@@ -133,52 +132,91 @@
         response = response.json()
         self.Bearer = f"{response['access_token']}"
         self.Refresh = response["refresh_token"]
         self.ID_Token = response["id_token"]
         return response
 
     def _verify_login(self):
-        # Test login by getting portfolio summary
+        # Test login by getting Account IDs
         try:
-            self.get_portfolio_summary()
+            self.get_account_ids()
             return True
         except Exception:
             try:
                 self.refresh_token()
-                self.get_portfolio_summary()
+                self.get_account_ids()
                 return True
             except Exception:
                 return False
 
     @check_login
-    def get_portfolio_summary(self):
-        query = self.endpoints.portfolio_query()
+    def get_account_ids(self):
+        query = self.endpoints.account_ids_query()
+        headers = self.endpoints.build_headers(self.Bearer)
+        response = self.session.post(
+            self.endpoints.graphql, headers=headers, data=query
+        )
+        if response.status_code != 200:
+            raise Exception(
+                f"Account ID Check failed with status code {response.status_code}: {response.text}"
+            )
+        response = response.json()["data"]["user"]["accounts"]
+        response_list = sorted(response, key=lambda x: x["created"])
+        account_ids = []
+        for account in response_list:
+            if account["status"] == "APPROVED":
+                account_ids.append(account["id"])
+        self.account_ids = account_ids
+        return account_ids
+
+    @check_login
+    def get_full_accounts(self):
+        query = self.endpoints.list_full_accounts_query()
+        headers = self.endpoints.build_headers(self.Bearer)
+        response = self.session.post(
+            self.endpoints.graphql, headers=headers, data=query
+        )
+        if response.status_code != 200:
+            raise Exception(
+                f"Full Account Request failed with status code {response.status_code}: {response.text}"
+            )
+        response = response.json()["data"]["user"]["accounts"]
+        response_list = sorted(response, key=lambda x: x["created"])
+        approved_accounts = []
+        for account in response_list:
+            if account["status"] == "APPROVED":
+                approved_accounts.append(account)
+        return approved_accounts
+
+    @check_login
+    def get_portfolio_summary(self, account_id):
+        query = self.endpoints.portfolio_query(account_id)
         headers = self.endpoints.build_headers(self.Bearer)
         response = self.session.post(
             self.endpoints.graphql, headers=headers, data=query
         )
         if response.status_code != 200:
             raise Exception(
                 f"Portfolio Request failed with status code {response.status_code}: {response.text}"
             )
-        return response.json()["data"]["portfolio"]
+        return response.json()["data"]["account"]["portfolio"]
 
     @check_login
-    def get_stock_holdings(self):
-        query = self.endpoints.stock_holdings_query()
+    def get_stock_holdings(self, account_id):
+        query = self.endpoints.stock_holdings_query(account_id)
         headers = self.endpoints.build_headers(self.Bearer)
         response = self.session.post(
             self.endpoints.graphql, headers=headers, data=query
         )
         if response.status_code != 200:
             raise Exception(
                 f"Stock Holdings Request failed with status code {response.status_code}: {response.text}"
             )
         response = response.json()
-        return response["data"]["portfolio"]["bulbs"]
+        return response["data"]["account"]["portfolio"]["bulbs"]
 
     @check_login
     def is_market_open(self):
         query = self.endpoints.is_market_open_query()
         headers = self.endpoints.build_headers(self.Bearer)
         response = self.session.post(
             self.endpoints.graphql, headers=headers, data=query
@@ -187,15 +225,15 @@
             raise Exception(
                 f"Market Open Request failed with status code {response.status_code}: {response.text}"
             )
         response = response.json()
         return response["data"]["securityMarketInfo"]["isOpen"]
 
     @check_login
-    def place_order(self, ticker, quantity, side, price="market", dry_run=False):
+    def place_order(self, account_id, ticker, quantity, side, price="market", dry_run=False):
         if side.lower() not in ["buy", "sell"]:
             raise Exception("Side must be either 'buy' or 'sell'")
         # Check if market is open
         if not self.is_market_open():
             raise Exception("Market is closed. Cannot place order.")
         # Search for stock "isin"
         query = self.endpoints.stock_search_query(ticker)
@@ -207,18 +245,20 @@
             raise Exception(
                 f"Stock Search Request failed with status code {search_response.status_code}: {search_response.text}"
             )
         search_response = search_response.json()
         if dry_run:
             return search_response
         if len(search_response["data"]["searchSearch"]["searchSecurities"]) == 0:
-            raise Exception(f"No stock found with ticker {ticker}. Please check the app to see if it is valid.")
+            raise Exception(
+                f"No stock found with ticker {ticker}. Please check the app to see if it is valid."
+            )
         isin = search_response["data"]["searchSearch"]["searchSecurities"][0]["isin"]
         # Place order
-        query = self.endpoints.stock_order_query(ticker, quantity, isin, side, price)
+        query = self.endpoints.stock_order_query(account_id, ticker, quantity, isin, side, price)
         order_response = self.session.post(
             self.endpoints.graphql, headers=headers, data=query
         )
         if order_response.status_code != 200:
             raise Exception(
                 f"Order Request failed with status code {order_response.status_code}: {order_response.text}"
             )
```

### Comparing `fennel_invest_api-1.0.4/fennel_invest_api.egg-info/PKG-INFO` & `fennel_invest_api-1.0.5/fennel_invest_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-dotenv
 
 # Unofficial Fennel Invest API
 
 This is an unofficial API for Fennel.com. It is a simple Python wrapper around the Fennel.com GraphQL API. It is not affiliated with Fennel.com in any way.
 
@@ -42,28 +43,36 @@
     wait_for_2fa=False
     code="123456" # Should be six-digit integer from email
 )
 ```
 
 ## Usage: Get Stock Holdings
 ```python
-positions = fennel.get_stock_holdings()
-for position in positions:
-    print(position)
+account_ids = fennel.get_account_ids()
+for account_id in account_ids:
+    print(account_id)
+    positions = fennel.get_stock_holdings(account_id)
+    for position in positions:
+        print(position)
 ```
 
 ## Usage: Get Portfolio
 ```python
-portfolio = fennel.get_portfolio_summary()
+# For all accounts
+full_portfolio = fennel.get_full_accounts()
+print(full_portfolio)
+# For a single account ID
+portfolio = fennel.get_portfolio_summary(account_id)
 print(portfolio)
 ```
 
 ## Usage: Placing Orders
 ```python
 order = fennel.place_order(
+    account_id=account_id,
     symbol="AAPL",
     quantity=1,
     side="buy", # Must be "buy" or "sell"
     price="market" # Only market orders are supported for now
 )
 print(order)
 ```
```

