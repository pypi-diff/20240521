# Comparing `tmp/py_alpaca_api-0.5.1.tar.gz` & `tmp/py_alpaca_api-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.5.1.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.5.3.tar", max compression
```

## Comparing `py_alpaca_api-0.5.1.tar` & `py_alpaca_api-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.1/LICENSE
--rw-r--r--   0        0        0    16791 2024-05-19 11:02:34.884010 py_alpaca_api-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.1/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2513 2024-05-19 04:10:18.598262 py_alpaca_api-0.5.1/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.1/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     6009 2024-05-19 04:10:18.608262 py_alpaca_api-0.5.1/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     3750 2024-05-19 04:10:18.608262 py_alpaca_api-0.5.1/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    21161 2024-05-19 04:10:18.608262 py_alpaca_api-0.5.1/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     7736 2024-05-19 02:32:34.142337 py_alpaca_api-0.5.1/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2102 2024-05-19 02:32:34.112337 py_alpaca_api-0.5.1/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    23670 2024-05-19 14:46:57.123704 py_alpaca_api-0.5.1/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0    14954 2024-05-19 02:32:34.172337 py_alpaca_api-0.5.1/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     7359 2024-05-19 12:31:17.233892 py_alpaca_api-0.5.1/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    21392 2024-05-19 17:56:10.781026 py_alpaca_api-0.5.1/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1324 2024-05-19 17:57:01.701018 py_alpaca_api-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.3/LICENSE
+-rw-r--r--   0        0        0    16791 2024-05-19 11:02:34.884010 py_alpaca_api-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.3/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2490 2024-05-19 20:03:29.845131 py_alpaca_api-0.5.3/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.3/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     4672 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.3/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     3789 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.3/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    20726 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.3/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7775 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.3/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2141 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.3/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    13186 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.3/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0    14989 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.3/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     7002 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.3/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    14951 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.3/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1344 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.3/PKG-INFO
```

### Comparing `py_alpaca_api-0.5.1/LICENSE` & `py_alpaca_api-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.1/README.md` & `py_alpaca_api-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.1/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.5.3/py_alpaca_api/alpaca.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
         ValueError:
             ValueError if API Secret is not provided
 
         Example:
         --------
         >>> PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-        PyAlpacaApi()
         """  # noqa
 
         # Check if API Key and Secret are provided
         if not api_key:
             raise ValueError("API Key is required")
         if not api_secret:
             raise ValueError("API Secret is required")
```

### Comparing `py_alpaca_api-0.5.1/py_alpaca_api/src/account.py` & `py_alpaca_api-0.5.3/py_alpaca_api/src/account.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,44 @@
 import json
+from typing import Dict
 
 import pandas as pd
 import requests
 
 from .data_classes import AccountClass, account_class_from_dict
 
 
 class Account:
-    def __init__(self, trade_url: str, headers: object) -> None:
-        """Initialize Account class
-
-        Parameters:
-        ___________
-        trade_url: str
-                Alpaca Trade API URL required
-
-        headers: object
-                API request headers required
-
-        Raises:
-        _______
-        ValueError: If trade URL is not provided
-
-        ValueError: If headers are not provided
-        """  # noqa
-
+    def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
+        """
+        Args:
+            trade_url: The URL for the trade.
+            headers: The headers for the trade request.
+        """
         self.trade_url = trade_url
         self.headers = headers
 
     ########################################################
     # \\\\\\\\\\\\\  Get Account Information ///////////////#
     ########################################################
     def get(self) -> AccountClass:
-        """Get account information from Alpaca API
+        """
+        This method `get` is used to retrieve account information from the Alpaca API.
 
         Returns:
-        ________
-        AccountClass: Account information as an AccountClass object
+            AccountClass: An object representing the account information.
 
         Raises:
-        _______
-        Exception: If the response is not successful
-
-        Example:
-        ________
-        >>> from py_alpaca_api import PyAlpacaApi
-            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-            account = api.account.get()
-            print(account)
+            Exception: If the request to the Alpaca API fails.
 
-        AccountClass(
-            account_blocked=False,
-            account_number="PA2ZVZ6QYJ6U",
-            buying_power=100000,
-            cash=100000,
-            created_at="2021-07-08T18:18:08.182Z",
-            currency="USD",
-            daytrade_count=0,
-            daytrading_buying_power=100000,
-            equity=100000,
-            id="f3b5d9e2-0e4e-4f0f-8d3f-0f0e7b7e4e6e",
-            initial_margin=0,
-            last_equity=100000,
-            last_maintenance_margin=0,
-            long_market_value=0,
-            maintenance_margin=0,
-            multiplier=4,
-            pattern_day_trader=False,
-            portfolio_value=100000,
-            regt_buying_power=200000,
-            short_market_value=0,
-            shorting_enabled=True,
-            sma=0,
-            status="ACTIVE",
-            trade_suspended_by_user=False,
-            trading_blocked=False,
-            transfers_blocked=False,
-            updated_at="2021-07-08T18:18:08.182Z",
-            withdrawable_amount=100000
-        )
-        """  # noqa
+        Example Usage:
+            >>> account = account.get()
+            >>> print(account)
 
+        """
         # Alpaca API URL for account information
         url = f"{self.trade_url}/account"
         # Get request to Alpaca API for account information
         response = requests.get(url, headers=self.headers)
         # Check if response is successful
         if response.status_code == 200:
             # Convert JSON response to dictionary
@@ -121,15 +75,15 @@
 
         Raises:
         _______
         Exception: If the response is not successful
 
         Example:
         ________
-        >>> from py_alpaca_api import PyAlpacaApi
+        >>> from py_alpaca_api.alpaca import PyAlpacaApi
             api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
             portfolio_history = api.account.portfolio_history()
             print(portfolio_history)
 
         timestamp    equity  profit_loss  profit_loss_pct  base_value
         0 2021-07-08  100000.0          0.0              0.0    100000.0
         1 2021-07-09  100000.0          0.0              0.0    100000.0
```

### Comparing `py_alpaca_api-0.5.1/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.5.3/py_alpaca_api/src/asset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
+from typing import Dict
 
 import pandas as pd
 import requests
 
 from .data_classes import AssetClass, asset_class_from_dict
 
 
 class Asset:
-    def __init__(self, trade_url: str, headers: object) -> None:
+    def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
         """Initialize Asset class
 
         Parameters:
         ___________
         trade_url: str
                 Alpaca Trade API URL required
 
@@ -79,15 +80,15 @@
 
         Raises:
         _______
         ValueError: If the response is not successful
 
         Example:
         ________
-        >>> from py_alpaca_api import PyAlpacaApi
+        >>> from py_alpaca_api.alpaca import PyAlpacaApi
             api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
             asset = api.asset.get(symbol="AAPL")
             print(asset)
 
         AssetClass(
             asset_id="375f6b6e-3b5f-4b2b-8f6b-2e6b2a6b2e6b",
             class="us_equity",
```

### Comparing `py_alpaca_api-0.5.1/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.5.3/py_alpaca_api/src/data_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -372,46 +372,41 @@
     )
 
 
 ############################################
 # Data Class Position Conversion Functions
 ############################################
 def position_class_from_dict(data_dict: dict) -> PositionClass:
-    """Converts a dictionary to a PositionClass object.
+    """Converts a dictionary to a PositionClass object."""
 
-    Parameters:
-    -----------
-    data_dict: dict
-        A dictionary containing the position data.
-
-    Returns:
-    --------
-    PositionClass
-        A PositionClass object.
-    """  # noqa
+    def get_string_value(data_d: dict, key: str) -> str:
+        return str(data_d.get(key, ""))
+
+    def get_float_value(data_d: dict, key: str) -> float:
+        return float(data_d.get(key, 0.0))
 
     return PositionClass(
-        asset_id=str(data_dict["asset_id"] if data_dict["asset_id"] else ""),
-        symbol=str(data_dict["symbol"] if data_dict["symbol"] else ""),
-        exchange=str(data_dict["exchange"] if data_dict["exchange"] else ""),
-        asset_class=str(data_dict["asset_class"] if data_dict["asset_class"] else ""),
-        avg_entry_price=float(data_dict["avg_entry_price"] if data_dict["avg_entry_price"] else 0),
-        qty=float(data_dict["qty"] if data_dict["qty"] else 0),
-        qty_available=float(data_dict["qty_available"] if data_dict["qty_available"] else 0),
-        side=str(data_dict["side"] if data_dict["side"] else ""),
-        market_value=float(data_dict["market_value"] if data_dict["market_value"] else 0),
-        cost_basis=float(data_dict["cost_basis"] if data_dict["cost_basis"] else 0),
-        profit_dol=float(data_dict["profit_dol"] if data_dict["profit_dol"] else 0),
-        profit_pct=float(data_dict["profit_pct"] if data_dict["profit_pct"] else 0),
-        intraday_profit_dol=float(data_dict["intraday_profit_dol"] if data_dict["intraday_profit_dol"] else 0),
-        intraday_profit_pct=float(data_dict["intraday_profit_pct"] if data_dict["intraday_profit_pct"] else 0),
-        portfolio_pct=float(data_dict["portfolio_pct"] if data_dict["portfolio_pct"] else 0),
-        current_price=float(data_dict["current_price"] if data_dict["current_price"] else 0),
-        lastday_price=float(data_dict["lastday_price"] if data_dict["lastday_price"] else 0),
-        change_today=float(data_dict["change_today"] if data_dict["change_today"] else 0),
+        asset_id=get_string_value(data_dict, "asset_id"),
+        symbol=get_string_value(data_dict, "symbol"),
+        exchange=get_string_value(data_dict, "exchange"),
+        asset_class=get_string_value(data_dict, "asset_class"),
+        avg_entry_price=get_float_value(data_dict, "avg_entry_price"),
+        qty=get_float_value(data_dict, "qty"),
+        qty_available=get_float_value(data_dict, "qty_available"),
+        side=get_string_value(data_dict, "side"),
+        market_value=get_float_value(data_dict, "market_value"),
+        cost_basis=get_float_value(data_dict, "cost_basis"),
+        profit_dol=get_float_value(data_dict, "profit_dol"),
+        profit_pct=get_float_value(data_dict, "profit_pct"),
+        intraday_profit_dol=get_float_value(data_dict, "intraday_profit_dol"),
+        intraday_profit_pct=get_float_value(data_dict, "intraday_profit_pct"),
+        portfolio_pct=get_float_value(data_dict, "portfolio_pct"),
+        current_price=get_float_value(data_dict, "current_price"),
+        lastday_price=get_float_value(data_dict, "lastday_price"),
+        change_today=get_float_value(data_dict, "change_today"),
         asset_marginable=bool(data_dict["asset_marginable"]),
     )
 
 
 ############################################
 # Data Class Account Conversion Functions
 ############################################
```

### Comparing `py_alpaca_api-0.5.1/py_alpaca_api/src/history.py` & `py_alpaca_api-0.5.3/py_alpaca_api/src/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
+from typing import Dict
 
 import pandas as pd
 import requests
 
 from .asset import Asset
 
 
 class History:
-    def __init__(self, data_url: str, headers: object, asset: Asset) -> None:
+    def __init__(self, data_url: str, headers: Dict[str, str], asset: Asset) -> None:
         """Initialize History class
 
         Parameters:
         ___________
         data_url: str
                 Alpaca Data API URL required
 
@@ -96,15 +97,15 @@
 
         ValueError: If no data is available
 
         ValueError: If invalid timeframe is provided
 
         Example:
         ________
-        >>> from py_alpaca_api import PyAlpacaApi
+        >>> from py_alpaca_api.alpaca import PyAlpacaApi
             api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
             stock_data = api.history.get_stock_data(symbol="AAPL", start="2021-01-01", end="2021-12-31", timeframe="1d")
             print(stock_data)
 
         symbol       date    open    high     low   close    volume  trade_count     vwap
         AAPL    2021-01-04  133.52  133.61  126.76  129.41  143301887      1009115  130.914
         AAPL    2021-01-05  128.89  131.74  128.43  131.01   97664898       678471  130.573
```

### Comparing `py_alpaca_api-0.5.1/py_alpaca_api/src/market.py` & `py_alpaca_api-0.5.3/py_alpaca_api/src/market.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
+from typing import Dict
 
 import requests
 
 from .data_classes import ClockClass, clock_class_from_dict
 
 
 class Market:
-    def __init__(self, trade_url: str, headers: object) -> None:
+    def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
         """Initialize Market class
 
         Parameters:
         ___________
         trade_url: str
                 Alpaca Trade API URL required
 
@@ -39,15 +40,15 @@
 
         Raises:
         _______
         Exception: If the response is not successful
 
         Example:
         ________
-        >>> from py_alpaca_api import PyAlpacaApi
+        >>> from py_alpaca_api.alpaca import PyAlpacaApi
             api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
             clock = api.market.clock()
             print(clock)
 
         ClockClass(
             market_time="2021-07-08T18:18:08.182Z",
             is_open=True,
```

### Comparing `py_alpaca_api-0.5.1/py_alpaca_api/src/position.py` & `py_alpaca_api-0.5.3/py_alpaca_api/src/position.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests
 
 from .account import Account
 from .data_classes import PositionClass, position_class_from_dict
 
 
 class Position:
-    def __init__(self, trade_url: str, headers: object, account: Account) -> None:
+    def __init__(self, trade_url: str, headers: dict[str, str], account: Account) -> None:
         """Initialize Position class
 
         Parameters:
         ___________
         trade_url: str
                 Alpaca Trade API URL required
 
@@ -25,15 +25,14 @@
         Raises:
         _______
         ValueError: If trade URL is not provided
 
         ValueError: If headers are not provided
 
         ValueError: If account is not provided
-
         """  # noqa
 
         self.trade_url = trade_url
         self.headers = headers
         self.account = account
 
     ########################################################
@@ -51,15 +50,15 @@
 
         Raises:
         -------
         Exception: If failed to get positions information
 
         Example:
         --------
-        >>> from py_alpaca_api import PyAlpacaApi
+        >>> from py_alpaca_api.alpaca import PyAlpacaApi
             api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
             positions = api.position.get_all()
             print(positions)
 
         asset_id symbol exchange asset_class  avg_entry_price  qty  qty_available  side  market_value  cost_basis  profit_dol  profit_pct  \
         0           Cash  Cash         Cash          0.0000  0.0            0.0  Cash       10000.0         0.0         0.0      0.000
         1  ASSET_ID   AAPL   NASDAQ   us_equity        100.0000  10.0           10.0  long       1000.0      1000.0         0.0      0.000
@@ -181,15 +180,15 @@
 
         ValueError:     ValueError if both symbol and symbol_dict are provided
 
         Exception:      Exception if failed to get position information
 
         Example:
         --------
-        >>> from py_alpaca_api import PyAlpacaApi
+        >>> from py_alpaca_api.alpaca import PyAlpacaApi
             api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
             position = api.position.get(symbol="AAPL")
             print(position)
 
         PositionClass(
             asset_id="375f6b6e-3b5f-4b2b-8f6b-2e6b2a6b2e6b",
             symbol="AAPL",
@@ -273,15 +272,15 @@
 
         Raises:
         -------
         Exception:      Exception if failed to close positions
 
         Example:
         --------
-        >>> from py_alpaca_api import PyAlpacaApi
+        >>> from py_alpaca_api.alpaca import PyAlpacaApi
             api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
             message = api.position.close_all()
             print(message)
 
         '1 positions have been closed'
         """  # noqa
 
@@ -333,15 +332,15 @@
 
         ValueError:     ValueError if symbol or asset_id is not provided
 
         Exception:      Exception if failed to close position
 
         Example:
         --------
-        >>> from py_alpaca_api import PyAlpacaApi
+        >>> from py_alpaca_api.alpaca import PyAlpacaApi
             api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
             message = api.position.close(symbol_or_id="AAPL", qty=10)
             print(message)
 
         'Position AAPL has been closed'
         """  # noqa
```

### Comparing `py_alpaca_api-0.5.1/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.5.3/py_alpaca_api/src/screener.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
+from typing import Dict
 
 import pandas as pd
 import pendulum
 import requests
 
 from .asset import Asset
 
 # This keeps the date in sync with the market
 # If it's a weekend, it will return the previous Friday
 # If it's a weekday, it will return the previous day, other than Monday
 # If it's Monday, it will return the previous Friday
 today = pendulum.now(tz="America/New_York")
 yesterday = today.subtract(days=1).strftime("%Y-%m-%d")
-if today.day_of_week == (pendulum.SUNDAY or pendulum.MONDAY):
+if today.day_of_week == pendulum.SUNDAY or today.day_of_week == pendulum.MONDAY:
     yesterday = today.previous(pendulum.FRIDAY).strftime("%Y-%m-%d")
-######################################################################
 
 
 class Screener:
-    def __init__(self, data_url: str, headers: object, asset: Asset) -> None:
+    def __init__(self, data_url: str, headers: Dict[str, str], asset: Asset) -> None:
         """Initialize Screener class3
 
         Parameters:
         ___________
         data_url: str
                 Alpaca Data API URL required
 
@@ -153,15 +153,15 @@
         Returns:
         _______
         pd.DataFrame: Percentage changes for the previous day
 
         Raises:
         _______
         ValueError: If failed to get top gainers
-        """  # noqa
+        """
         url = f"{self.data_url}/stocks/bars"
 
         params = {
             "symbols": ",".join(self.asset.get_all()["symbol"].tolist()),
             "limit": 10000,
             "timeframe": timeframe,
             "start": start,
@@ -190,24 +190,17 @@
                         pd.DataFrame.from_dict(res["bars"], orient="index"),
                     ]
                 )
                 page_token = res["next_page_token"]
 
             bars_df.reset_index()
 
-            gainer_df = pd.DataFrame()
+            all_bars_df = pd.DataFrame()
 
             for bar in bars_df.iterrows():
-                # bar[0] is symbol
-                # bar[1][1] is current bar
-                # bar[1][0] is previous bar
-                # bar[1][1]["c"] is current close
-                # bar[1][0]["c"] is previous close
-                # ((current close - previous close) / previous close) * 100
-                # print(bar[1][0])
                 try:
                     change = round(
                         ((bar[1][0]["c"] - bar[1][0]["o"]) / bar[1][0]["o"]) * 100,
                         2,
                     )
 
                     symbol = bar[0]
@@ -215,15 +208,15 @@
                     sym_data = {
                         "symbol": symbol,
                         "change": change,
                         "price": bar[1][0]["c"],
                         "volume": bar[1][0]["v"],
                         "trades": bar[1][0]["n"],
                     }
-                    gainer_df = pd.concat([gainer_df, pd.DataFrame([sym_data])])
+                    all_bars_df = pd.concat([all_bars_df, pd.DataFrame([sym_data])])
 
                 except Exception:
                     pass
-            gainer_df.reset_index(drop=True, inplace=True)
-            return gainer_df
+            all_bars_df.reset_index(drop=True, inplace=True)
+            return all_bars_df
         else:
-            raise ValueError(f"Failed to get top gainers. Response: {response.text}")
+            raise ValueError(f"Failed to get assets. Response: {response.text}")
```

### Comparing `py_alpaca_api-0.5.1/pyproject.toml` & `py_alpaca_api-0.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.5.1"
+version = "0.5.3"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
@@ -24,14 +24,15 @@
 black = "^24.4.2"
 isort = "^5.13.2"
 pre-commit = "^3.7.1"
 ipykernel = "^6.29.4"
 pytest-mock = "^3.14.0"
 pytest-mock-server = "^0.3.0"
 python-dotenv = "^1.0.1"
+coverage = "^7.5.1"
 
 
 [tool.poetry.group.test.dependencies]
 flake8 = "^7.0.0"
 
 
 [tool.poetry.group.doc.dependencies]
```

### Comparing `py_alpaca_api-0.5.1/PKG-INFO` & `py_alpaca_api-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.5.1
+Version: 0.5.3
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

