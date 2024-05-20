# Comparing `tmp/tastytrade-7.3.tar.gz` & `tmp/tastytrade-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-7.3.tar", last modified: Mon May 20 23:13:32 2024, max compression
+gzip compressed data, was "tastytrade-8.0.tar", last modified: Thu Apr 25 23:10:43 2024, max compression
```

## Comparing `tastytrade-7.3.tar` & `tastytrade-8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:13:32.618757 tastytrade-7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 23:13:29.000000 tastytrade-7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-05-20 23:13:32.618757 tastytrade-7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-20 23:13:29.000000 tastytrade-7.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:13:32.618757 tastytrade-7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-20 23:13:29.000000 tastytrade-7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:13:32.614757 tastytrade-7.3/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38231 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:13:32.614757 tastytrade-7.3/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/dxfeed/underlying.py
--rw-r--r--   0 runner    (1001) docker     (127)    35007 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    23983 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-20 23:13:29.000000 tastytrade-7.3/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:13:32.618757 tastytrade-7.3/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-05-20 23:13:32.000000 tastytrade-7.3/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-20 23:13:32.000000 tastytrade-7.3/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:13:32.000000 tastytrade-7.3/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-20 23:13:32.000000 tastytrade-7.3/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 23:13:32.000000 tastytrade-7.3/tastytrade.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:13:32.618757 tastytrade-7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-20 23:13:29.000000 tastytrade-7.3/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-20 23:13:29.000000 tastytrade-7.3/tests/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-20 23:13:29.000000 tastytrade-7.3/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-20 23:13:29.000000 tastytrade-7.3/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-20 23:13:29.000000 tastytrade-7.3/tests/test_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-20 23:13:29.000000 tastytrade-7.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-20 23:13:29.000000 tastytrade-7.3/tests/test_watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:10:43.049715 tastytrade-8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 23:10:40.000000 tastytrade-8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-25 23:10:43.049715 tastytrade-8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-04-25 23:10:40.000000 tastytrade-8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 23:10:43.049715 tastytrade-8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-25 23:10:40.000000 tastytrade-8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:10:43.045715 tastytrade-8.0/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38073 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:10:43.049715 tastytrade-8.0/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/dxfeed/underlying.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34978 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23458 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-25 23:10:40.000000 tastytrade-8.0/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:10:43.049715 tastytrade-8.0/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-25 23:10:43.000000 tastytrade-8.0/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-25 23:10:43.000000 tastytrade-8.0/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 23:10:43.000000 tastytrade-8.0/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-25 23:10:43.000000 tastytrade-8.0/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 23:10:43.000000 tastytrade-8.0/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:10:43.049715 tastytrade-8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-25 23:10:40.000000 tastytrade-8.0/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-25 23:10:40.000000 tastytrade-8.0/tests/test_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 23:10:40.000000 tastytrade-8.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 23:10:40.000000 tastytrade-8.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-25 23:10:40.000000 tastytrade-8.0/tests/test_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-25 23:10:40.000000 tastytrade-8.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-25 23:10:40.000000 tastytrade-8.0/tests/test_watchlists.py
```

### Comparing `tastytrade-7.3/LICENSE` & `tastytrade-8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/PKG-INFO` & `tastytrade-8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 7.3
+Version: 8.0
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests<3
 Requires-Dist: websockets>=11.0.3
 Requires-Dist: pydantic>=2.6.3
 Requires-Dist: pandas_market_calendars>=4.3.3
-Requires-Dist: fake_useragent>=1.5.1
 
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
    :target: https://pypi.org/project/tastytrade
@@ -43,16 +42,16 @@
 ------------------
 
 A session object is required to authenticate your requests to the Tastytrade API.
 You can create a real session using your normal login, or a certification (test) session using your certification login.
 
 .. code-block:: python
 
-   from tastytrade import ProductionSession
-   session = ProductionSession('username', 'password')
+   from tastytrade import Session
+   session = Session('username', 'password')
 
 Using the streamer
 ------------------
 
 The streamer is a websocket connection to dxfeed (the Tastytrade data provider) that allows you to subscribe to real-time data for quotes, greeks, and more.
 
 .. code-block:: python
@@ -63,30 +62,34 @@
    async with DXLinkStreamer(session) as streamer:
        subs_list = ['SPY']  # list of symbols to subscribe to
        await streamer.subscribe(EventType.QUOTE, subs_list)
        # this example fetches quotes once, then exits
        quote = await streamer.get_event(EventType.QUOTE)
        print(quote)
 
->>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
+.. code-block:: bash
+
+   >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Note that this is asynchronous code, so you can't run it as is unless you're using a Jupyter notebook or something similar.
 
 Getting current positions
 -------------------------
 
 .. code-block:: python
    
    from tastytrade import Account
 
    account = Account.get_accounts(session)[0]
    positions = account.get_positions(session)
    print(positions[0])
 
->>> CurrentPosition(account_number='5WX01234', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
+.. code-block:: bash
+
+   >>> CurrentPosition(account_number='5WX01234', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
 
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
@@ -104,15 +107,17 @@
        legs=[leg],  # you can have multiple legs in an order
        price=Decimal('10'),  # limit price, $10/share for a total value of $50
        price_effect=PriceEffect.DEBIT
    )
    response = account.place_order(session, order, dry_run=True)  # a test order
    print(response)
 
->>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
+.. code-block:: bash
+
+   >>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
 
 Options chain/streaming greeks
 ------------------------------
 
 .. code-block:: python
 
    from tastytrade import DXLinkStreamer
@@ -124,15 +129,17 @@
    subs_list = [chain[exp][0].streamer_symbol]
 
    async with DXLinkStreamer(session) as streamer:
        await streamer.subscribe(EventType.GREEKS, subs_list)
        greeks = await streamer.get_event(EventType.GREEKS)
        print(greeks)
 
->>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
+.. code-block:: bash
+
+   >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
 
 For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
         
 Disclaimer
 ----------
 
 This is an unofficial SDK for Tastytrade. There is no implied warranty for any actions and results which arise from using it.
```

### Comparing `tastytrade-7.3/README.rst` & `tastytrade-8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 ------------------
 
 A session object is required to authenticate your requests to the Tastytrade API.
 You can create a real session using your normal login, or a certification (test) session using your certification login.
 
 .. code-block:: python
 
-   from tastytrade import ProductionSession
-   session = ProductionSession('username', 'password')
+   from tastytrade import Session
+   session = Session('username', 'password')
 
 Using the streamer
 ------------------
 
 The streamer is a websocket connection to dxfeed (the Tastytrade data provider) that allows you to subscribe to real-time data for quotes, greeks, and more.
 
 .. code-block:: python
@@ -47,30 +47,34 @@
    async with DXLinkStreamer(session) as streamer:
        subs_list = ['SPY']  # list of symbols to subscribe to
        await streamer.subscribe(EventType.QUOTE, subs_list)
        # this example fetches quotes once, then exits
        quote = await streamer.get_event(EventType.QUOTE)
        print(quote)
 
->>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
+.. code-block:: bash
+
+   >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Note that this is asynchronous code, so you can't run it as is unless you're using a Jupyter notebook or something similar.
 
 Getting current positions
 -------------------------
 
 .. code-block:: python
    
    from tastytrade import Account
 
    account = Account.get_accounts(session)[0]
    positions = account.get_positions(session)
    print(positions[0])
 
->>> CurrentPosition(account_number='5WX01234', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
+.. code-block:: bash
+
+   >>> CurrentPosition(account_number='5WX01234', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
 
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
@@ -88,15 +92,17 @@
        legs=[leg],  # you can have multiple legs in an order
        price=Decimal('10'),  # limit price, $10/share for a total value of $50
        price_effect=PriceEffect.DEBIT
    )
    response = account.place_order(session, order, dry_run=True)  # a test order
    print(response)
 
->>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
+.. code-block:: bash
+
+   >>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
 
 Options chain/streaming greeks
 ------------------------------
 
 .. code-block:: python
 
    from tastytrade import DXLinkStreamer
@@ -108,15 +114,17 @@
    subs_list = [chain[exp][0].streamer_symbol]
 
    async with DXLinkStreamer(session) as streamer:
        await streamer.subscribe(EventType.GREEKS, subs_list)
        greeks = await streamer.get_event(EventType.GREEKS)
        print(greeks)
 
->>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
+.. code-block:: bash
+
+   >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
 
 For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
         
 Disclaimer
 ----------
 
 This is an unofficial SDK for Tastytrade. There is no implied warranty for any actions and results which arise from using it.
```

### Comparing `tastytrade-7.3/setup.py` & `tastytrade-8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 
 f = open('README.rst', 'r')
 LONG_DESCRIPTION = f.read()
 f.close()
 
 setup(
     name='tastytrade',
-    version='7.3',
+    version='8.0',
     description='An unofficial SDK for Tastytrade!',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     author='Graeme Holliday',
     author_email='graeme.holliday@pm.me',
     url='https://github.com/tastyware/tastytrade',
     license='MIT',
     install_requires=[
         'requests<3',
         'websockets>=11.0.3',
         'pydantic>=2.6.3',
-        'pandas_market_calendars>=4.3.3',
-        'fake_useragent>=1.5.1',
+        'pandas_market_calendars>=4.3.3'
     ],
     packages=find_packages(exclude=['ez_setup', 'tests*']),
     include_package_data=True
 )
```

### Comparing `tastytrade-7.3/tastytrade/account.py` & `tastytrade-8.0/tastytrade/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests
 from pydantic import BaseModel
 
 from tastytrade import logger
 from tastytrade.order import (InstrumentType, NewComplexOrder, NewOrder,
                               OrderStatus, PlacedComplexOrder, PlacedOrder,
                               PlacedOrderResponse, PriceEffect)
-from tastytrade.session import ProductionSession, Session
+from tastytrade.session import Session
 from tastytrade.utils import (TastytradeError, TastytradeJsonDataclass,
                               today_in_new_york, validate_response)
 
 
 class EmptyDict(BaseModel):
     class Config:
         extra = 'forbid'
@@ -170,31 +170,31 @@
 class MarginReportEntry(TastytradeJsonDataclass):
     """
     Dataclass containing an individual entry (relating to a specific position)
     as part of the overall margin report.
     """
     description: str
     code: str
-    buying_power: Decimal
-    buying_power_effect: PriceEffect
+    underlying_symbol: str
+    underlying_type: str
     margin_calculation_type: str
     margin_requirement: Decimal
     margin_requirement_effect: PriceEffect
+    maintenance_requirement: Decimal
+    maintenance_requirement_effect: PriceEffect
+    buying_power: Decimal
+    buying_power_effect: PriceEffect
+    groups: List[Dict[str, Any]]
+    price_increase_percent: Decimal
+    price_decrease_percent: Decimal
     expected_price_range_up_percent: Optional[Decimal] = None
     expected_price_range_down_percent: Optional[Decimal] = None
-    groups: Optional[List[Dict[str, Any]]] = None
+    point_of_no_return_percent: Optional[Decimal] = None
     initial_requirement: Optional[Decimal] = None
     initial_requirement_effect: Optional[PriceEffect] = None
-    maintenance_requirement: Optional[Decimal] = None
-    maintenance_requirement_effect: Optional[PriceEffect] = None
-    point_of_no_return_percent: Optional[Decimal] = None
-    price_increase_percent: Optional[Decimal] = None
-    price_decrease_percent: Optional[Decimal] = None
-    underlying_symbol: Optional[str] = None
-    underlying_type: Optional[str] = None
 
 
 class MarginReport(TastytradeJsonDataclass):
     """
     Dataclass containing an overall portfolio margin report.
     """
     account_number: str
@@ -719,15 +719,15 @@
         )
         validate_response(response)
 
         return response.json()['data']
 
     def get_net_liquidating_value_history(
         self,
-        session: ProductionSession,
+        session: Session,
         time_back: Optional[str] = None,
         start_time: Optional[datetime] = None
     ) -> List[NetLiqOhlc]:
         """
         Returns a list of account net liquidating value snapshots over the
         specified time period.
 
@@ -782,15 +782,15 @@
 
         data = response.json()['data']
 
         return PositionLimit(**data)
 
     def get_effective_margin_requirements(
         self,
-        session: ProductionSession,
+        session: Session,
         symbol: str
     ) -> MarginRequirement:
         """
         Get the effective margin requirements for a given symbol.
 
         :param session:
             the session to use for the request, can't be certification
```

### Comparing `tastytrade-7.3/tastytrade/dxfeed/candle.py` & `tastytrade-8.0/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/event.py` & `tastytrade-8.0/tastytrade/dxfeed/event.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/greeks.py` & `tastytrade-8.0/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/profile.py` & `tastytrade-8.0/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/quote.py` & `tastytrade-8.0/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/summary.py` & `tastytrade-8.0/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/theoprice.py` & `tastytrade-8.0/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/timeandsale.py` & `tastytrade-8.0/tastytrade/dxfeed/timeandsale.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/trade.py` & `tastytrade-8.0/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/dxfeed/underlying.py` & `tastytrade-8.0/tastytrade/dxfeed/underlying.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/instruments.py` & `tastytrade-8.0/tastytrade/instruments.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from decimal import Decimal
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 import requests
 
 from tastytrade.order import InstrumentType, TradeableTastytradeJsonDataclass
-from tastytrade.session import ProductionSession, Session
+from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass, validate_response
 
 
 class OptionType(str, Enum):
     """
     This is an :class:`~enum.Enum` that contains the valid types of options
     and their abbreviations in the API.
@@ -1115,15 +1115,15 @@
         else:
             chain[option.expiration_date].append(option)
 
     return chain
 
 
 def get_future_option_chain(
-    session: ProductionSession,
+    session: Session,
     symbol: str
 ) -> Dict[date, List[FutureOption]]:
     """
     Returns a mapping of expiration date to a list of futures options
     objects representing the options chain for the given symbol.
 
     In the case that there are two expiries on the same day (e.g. EW
```

### Comparing `tastytrade-7.3/tastytrade/metrics.py` & `tastytrade-8.0/tastytrade/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import date, datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Optional
 
 import requests
 
-from tastytrade.session import ProductionSession, Session
+from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass, validate_response
 
 
 class DividendInfo(TastytradeJsonDataclass):
     """
     Dataclass representing dividend information for a given symbol.
     """
@@ -104,15 +104,15 @@
     dividend_yield: Optional[Decimal] = None
     listed_market: Optional[str] = None
     lendability: Optional[str] = None
     borrow_rate: Optional[Decimal] = None
 
 
 def get_market_metrics(
-    session: ProductionSession,
+    session: Session,
     symbols: List[str]
 ) -> List[MarketMetricInfo]:
     """
     Retrieves market metrics for the given symbols.
 
     :param session: active user session to use
     :param symbols: list of symbols to retrieve metrics for
@@ -128,15 +128,15 @@
 
     data = response.json()['data']['items']
 
     return [MarketMetricInfo(**entry) for entry in data]
 
 
 def get_dividends(
-    session: ProductionSession,
+    session: Session,
     symbol: str
 ) -> List[DividendInfo]:
     """
     Retrieves dividend information for the given symbol.
 
     :param session: active user session to use
     :param symbol: symbol to retrieve dividend information for
@@ -153,15 +153,15 @@
 
     data = response.json()['data']['items']
 
     return [DividendInfo(**entry) for entry in data]
 
 
 def get_earnings(
-    session: ProductionSession,
+    session: Session,
     symbol: str,
     start_date: date
 ) -> List[EarningsInfo]:
     """
     Retrieves earnings information for the given symbol.
 
     :param session: active user session to use
```

### Comparing `tastytrade-7.3/tastytrade/order.py` & `tastytrade-8.0/tastytrade/order.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/search.py` & `tastytrade-8.0/tastytrade/search.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List
 
 import requests
 
-from tastytrade.session import ProductionSession
+from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass
 
 
 class SymbolData(TastytradeJsonDataclass):
     """
     Dataclass holding search results for an individual item.
     """
     symbol: str
     description: str
 
 
 def symbol_search(
-    session: ProductionSession,
+    session: Session,
     symbol: str
 ) -> List[SymbolData]:  # pragma: no cover
     """
     Performs a symbol search using the Tastytrade API and returns a
     list of symbols that are similar to the given search phrase.
 
     :param session: active user session to use
```

### Comparing `tastytrade-7.3/tastytrade/streamer.py` & `tastytrade-8.0/tastytrade/streamer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import asyncio
 import json
 from asyncio import Lock, Queue
 from collections import defaultdict
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
-from ssl import SSLContext, create_default_context
 from typing import Any, AsyncIterator, Dict, List, Optional, Union
 
 import websockets
-from websockets import WebSocketClientProtocol
 
 from tastytrade import logger
 from tastytrade.account import (Account, AccountBalance, CurrentPosition,
                                 TradingStatus)
 from tastytrade.dxfeed import (Candle, Event, EventType, Greeks, Profile,
                                Quote, Summary, TheoPrice, TimeAndSale, Trade,
                                Underlying)
 from tastytrade.order import (InstrumentType, OrderChain, PlacedOrder,
                               PriceEffect)
-from tastytrade.session import CertificationSession, ProductionSession, Session
+from tastytrade.session import Session
 from tastytrade.utils import TastytradeError, TastytradeJsonDataclass
 from tastytrade.watchlists import Watchlist
 
 CERT_STREAMER_URL = 'wss://streamer.cert.tastyworks.com'
 STREAMER_URL = 'wss://streamer.tastyworks.com'
 
-DXLINK_VERSION = '0.1-js/0.40.4-WB2'
+DXLINK_VERSION = '1.0.0'
 
 
 class QuoteAlert(TastytradeJsonDataclass):
     """
     Dataclass that contains information about a quote alert
     """
     user_external_id: str
@@ -103,20 +101,19 @@
                 print(data)
 
     """
     def __init__(self, session: Session):
         #: The active session used to initiate the streamer or make requests
         self.token: str = session.session_token
         #: The base url for the streamer websocket
-        is_certification = isinstance(session, CertificationSession)
         self.base_url: str = \
-            CERT_STREAMER_URL if is_certification else STREAMER_URL
+            CERT_STREAMER_URL if session.is_test else STREAMER_URL
 
         self._queue: Queue = Queue()
-        self._websocket: Optional[WebSocketClientProtocol] = None
+        self._websocket = None
         self._connect_task = asyncio.create_task(self._connect())
 
     async def __aenter__(self):
         time_out = 100
         while not self._websocket:
             await asyncio.sleep(0.1)
             time_out -= 1
@@ -142,18 +139,18 @@
 
     async def _connect(self) -> None:
         """
         Connect to the websocket server using the URL and authorization
         token provided during initialization.
         """
         headers = {'Authorization': f'Bearer {self.token}'}
-        async with websockets.connect(
+        async with websockets.connect(  # type: ignore
             self.base_url,
             extra_headers=headers
-        ) as websocket:  # type: ignore
+        ) as websocket:
             self._websocket = websocket
             self._heartbeat_task = asyncio.create_task(self._heartbeat())
 
             while True:
                 raw_message = await self._websocket.recv()  # type: ignore
                 logger.debug('raw message: %s', raw_message)
                 await self._queue.put(json.loads(raw_message))
@@ -272,19 +269,15 @@
         async with DXLinkStreamer(session) as streamer:
             subs = ['SPY']  # list of quotes to subscribe to
             await streamer.subscribe(EventType.QUOTE, subs)
             quote = await streamer.get_event(EventType.QUOTE)
             print(quote)
 
     """
-    def __init__(
-        self,
-        session: ProductionSession,
-        ssl_context: SSLContext = create_default_context()
-    ):
+    def __init__(self, session: Session):
         self._counter = 0
         self._lock: Lock = Lock()
         self._queues: Dict[EventType, Queue] = defaultdict(Queue)
         self._channels: Dict[EventType, int] = {
             EventType.CANDLE: 1,
             EventType.GREEKS: 3,
             EventType.PROFILE: 5,
@@ -299,35 +292,30 @@
             defaultdict(lambda: 'CHANNEL_CLOSED')
 
         #: The unique client identifier received from the server
         self._session = session
         self._authenticated = False
         self._wss_url = session.dxlink_url
         self._auth_token = session.streamer_token
-        self._ssl_context = ssl_context
 
         self._connect_task = asyncio.create_task(self._connect())
 
     async def __aenter__(self):
         time_out = 100
         while not self._authenticated:
             await asyncio.sleep(0.1)
             time_out -= 1
             if time_out < 0:
                 raise TastytradeError('Connection timed out')
 
         return self
 
     @classmethod
-    async def create(
-        cls,
-        session: ProductionSession,
-        ssl_context: SSLContext = create_default_context()
-    ) -> 'DXLinkStreamer':
-        self = cls(session, ssl_context=ssl_context)
+    async def create(cls, session: Session) -> 'DXLinkStreamer':
+        self = cls(session)
         return await self.__aenter__()
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.close()
 
     async def close(self):
         """
@@ -337,18 +325,16 @@
         self._heartbeat_task.cancel()
 
     async def _connect(self) -> None:
         """
         Connect to the websocket server using the URL and
         authorization token provided during initialization.
         """
-
-        async with websockets.connect(
-            self._wss_url,
-            ssl=self._ssl_context
+        async with websockets.connect(  # type: ignore
+            self._wss_url
         ) as websocket:
             self._websocket = websocket
             await self._setup_connection()
 
             # main loop
             while True:
                 raw_message = await self._websocket.recv()
@@ -567,17 +553,17 @@
         :param extended_trading_hours: whether to include extended trading
         """
         await self._channel_request(EventType.CANDLE)
         message = {
             'type': 'FEED_SUBSCRIPTION',
             'channel': self._channels[EventType.CANDLE],
             'add': [{
-                f'{ticker}{{={interval}}}'
+                'symbol': f'{ticker}{{={interval},tho=true}}'
                 if extended_trading_hours
-                else 'symbol': f'{ticker}{{={interval},tho=true}}',
+                else f'{ticker}{{={interval}}}',
                 'type': 'Candle',
                 'fromTime': int(start_time.timestamp() * 1000)
             } for ticker in symbols]
         }
         if end_time is not None:
             raise TastytradeError('End time no longer supported')
         await self._websocket.send(json.dumps(message))
@@ -597,17 +583,17 @@
             whether candle to unsubscribe from contains extended trading hours
         """
         await self._channel_request(EventType.CANDLE)
         message = {
             'type': 'FEED_SUBSCRIPTION',
             'channel': self._channels[EventType.CANDLE],
             'remove': [{
-                f'{ticker}{{={interval}}}'
+                'symbol': f'{ticker}{{={interval},tho=true}}'
                 if extended_trading_hours
-                else 'symbol': f'{ticker}{{={interval},tho=true}}',
+                else f'{ticker}{{={interval}}}',
                 'type': 'Candle',
             }]
         }
         await self._websocket.send(json.dumps(message))
 
     async def _map_message(self, message) -> None:
         """
```

### Comparing `tastytrade-7.3/tastytrade/utils.py` & `tastytrade-8.0/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tastytrade/watchlists.py` & `tastytrade-8.0/tastytrade/watchlists.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List, Optional
 
 import requests
 
 from tastytrade.instruments import InstrumentType
-from tastytrade.session import ProductionSession
+from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass, validate_response
 
 
 class Pair(TastytradeJsonDataclass):
     """
     Dataclass that represents a specific pair in a pairs watchlist.
     """
@@ -26,15 +26,15 @@
     name: str
     order_index: int
     pairs_equations: List[Pair]
 
     @classmethod
     def get_pairs_watchlists(
         cls,
-        session: ProductionSession
+        session: Session
     ) -> List['PairsWatchlist']:
         """
         Fetches a list of all Tastytrade public pairs watchlists.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`PairsWatchlist` objects.
@@ -47,15 +47,15 @@
         data = response.json()['data']['items']
 
         return [cls(**entry) for entry in data]
 
     @classmethod
     def get_pairs_watchlist(
         cls,
-        session: ProductionSession,
+        session: Session,
         name: str
     ) -> 'PairsWatchlist':
         """
         Fetches a Tastytrade public pairs watchlist by name.
 
         :param session: the session to use for the request.
         :param name: the name of the pairs watchlist to fetch.
@@ -82,15 +82,15 @@
     watchlist_entries: Optional[List[Dict[str, str]]] = None
     group_name: str = 'default'
     order_index: int = 9999
 
     @classmethod
     def get_public_watchlists(
         cls,
-        session: ProductionSession,
+        session: Session,
         counts_only: bool = False
     ) -> List['Watchlist']:
         """
         Fetches a list of all Tastytrade public watchlists.
 
         :param session: the session to use for the request.
         :param counts_only: whether to only fetch the counts of the watchlists.
@@ -107,15 +107,15 @@
         data = response.json()['data']['items']
 
         return [cls(**entry) for entry in data]
 
     @classmethod
     def get_public_watchlist(
         cls,
-        session: ProductionSession,
+        session: Session,
         name: str
     ) -> 'Watchlist':
         """
         Fetches a Tastytrade public watchlist by name.
 
         :param session: the session to use for the request.
         :param name: the name of the watchlist to fetch.
@@ -131,15 +131,15 @@
         data = response.json()['data']
 
         return cls(**data)
 
     @classmethod
     def get_private_watchlists(
         cls,
-        session: ProductionSession
+        session: Session
     ) -> List['Watchlist']:
         """
         Fetches a the user's private watchlists.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`Watchlist` objects.
@@ -153,15 +153,15 @@
         data = response.json()['data']['items']
 
         return [cls(**entry) for entry in data]
 
     @classmethod
     def get_private_watchlist(
         cls,
-        session: ProductionSession,
+        session: Session,
         name: str
     ) -> 'Watchlist':
         """
         Fetches a user's watchlist by name.
 
         :param session: the session to use for the request.
         :param name: the name of the watchlist to fetch.
@@ -177,43 +177,43 @@
         data = response.json()['data']
 
         return cls(**data)
 
     @classmethod
     def remove_private_watchlist(
         cls,
-        session: ProductionSession,
+        session: Session,
         name: str
     ) -> None:
         """
         Deletes the named private watchlist.
 
         :param session: the session to use for the request.
         :param name: the name of the watchlist to delete.
         """
         response = requests.delete(
             f'{session.base_url}/watchlists/{name}',
             headers=session.headers
         )
         validate_response(response)
 
-    def upload_private_watchlist(self, session: ProductionSession) -> None:
+    def upload_private_watchlist(self, session: Session) -> None:
         """
         Creates a private remote watchlist identical to this local one.
 
         :param session: the session to use for the request.
         """
         response = requests.post(
             f'{session.base_url}/watchlists',
             headers=session.headers,
             json=self.dict(by_alias=True)
         )
         validate_response(response)
 
-    def update_private_watchlist(self, session: ProductionSession) -> None:
+    def update_private_watchlist(self, session: Session) -> None:
         """
         Updates the existing private remote watchlist.
 
         :param session: the session to use for the request.
         """
         response = requests.put(
             f'{session.base_url}/watchlists/{self.name}',
```

### Comparing `tastytrade-7.3/tastytrade.egg-info/PKG-INFO` & `tastytrade-8.0/tastytrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 7.3
+Version: 8.0
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests<3
 Requires-Dist: websockets>=11.0.3
 Requires-Dist: pydantic>=2.6.3
 Requires-Dist: pandas_market_calendars>=4.3.3
-Requires-Dist: fake_useragent>=1.5.1
 
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
    :target: https://pypi.org/project/tastytrade
@@ -43,16 +42,16 @@
 ------------------
 
 A session object is required to authenticate your requests to the Tastytrade API.
 You can create a real session using your normal login, or a certification (test) session using your certification login.
 
 .. code-block:: python
 
-   from tastytrade import ProductionSession
-   session = ProductionSession('username', 'password')
+   from tastytrade import Session
+   session = Session('username', 'password')
 
 Using the streamer
 ------------------
 
 The streamer is a websocket connection to dxfeed (the Tastytrade data provider) that allows you to subscribe to real-time data for quotes, greeks, and more.
 
 .. code-block:: python
@@ -63,30 +62,34 @@
    async with DXLinkStreamer(session) as streamer:
        subs_list = ['SPY']  # list of symbols to subscribe to
        await streamer.subscribe(EventType.QUOTE, subs_list)
        # this example fetches quotes once, then exits
        quote = await streamer.get_event(EventType.QUOTE)
        print(quote)
 
->>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
+.. code-block:: bash
+
+   >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Note that this is asynchronous code, so you can't run it as is unless you're using a Jupyter notebook or something similar.
 
 Getting current positions
 -------------------------
 
 .. code-block:: python
    
    from tastytrade import Account
 
    account = Account.get_accounts(session)[0]
    positions = account.get_positions(session)
    print(positions[0])
 
->>> CurrentPosition(account_number='5WX01234', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
+.. code-block:: bash
+
+   >>> CurrentPosition(account_number='5WX01234', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
 
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
@@ -104,15 +107,17 @@
        legs=[leg],  # you can have multiple legs in an order
        price=Decimal('10'),  # limit price, $10/share for a total value of $50
        price_effect=PriceEffect.DEBIT
    )
    response = account.place_order(session, order, dry_run=True)  # a test order
    print(response)
 
->>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
+.. code-block:: bash
+
+   >>> PlacedOrderResponse(buying_power_effect=BuyingPowerEffect(change_in_margin_requirement=Decimal('125.0'), change_in_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, change_in_buying_power=Decimal('125.004'), change_in_buying_power_effect=<PriceEffect.DEBIT: 'Debit'>, current_buying_power=Decimal('1000.0'), current_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, new_buying_power=Decimal('874.996'), new_buying_power_effect=<PriceEffect.CREDIT: 'Credit'>, isolated_order_margin_requirement=Decimal('125.0'), isolated_order_margin_requirement_effect=<PriceEffect.DEBIT: 'Debit'>, is_spread=False, impact=Decimal('125.004'), effect=<PriceEffect.DEBIT: 'Debit'>), fee_calculation=FeeCalculation(regulatory_fees=Decimal('0.0'), regulatory_fees_effect=<PriceEffect.NONE: 'None'>, clearing_fees=Decimal('0.004'), clearing_fees_effect=<PriceEffect.DEBIT: 'Debit'>, commission=Decimal('0.0'), commission_effect=<PriceEffect.NONE: 'None'>, proprietary_index_option_fees=Decimal('0.0'), proprietary_index_option_fees_effect=<PriceEffect.NONE: 'None'>, total_fees=Decimal('0.004'), total_fees_effect=<PriceEffect.DEBIT: 'Debit'>), order=PlacedOrder(account_number='5WV69754', time_in_force=<OrderTimeInForce.DAY: 'Day'>, order_type=<OrderType.LIMIT: 'Limit'>, size='5', underlying_symbol='USO', underlying_instrument_type=<InstrumentType.EQUITY: 'Equity'>, status=<OrderStatus.RECEIVED: 'Received'>, cancellable=True, editable=True, edited=False, updated_at=datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc), legs=[Leg(instrument_type=<InstrumentType.EQUITY: 'Equity'>, symbol='USO', action=<OrderAction.BUY_TO_OPEN: 'Buy to Open'>, quantity=Decimal('5'), remaining_quantity=Decimal('5'), fills=[])], id=None, price=Decimal('50.0'), price_effect=<PriceEffect.DEBIT: 'Debit'>, gtc_date=None, value=None, value_effect=None, stop_trigger=None, contingent_status=None, confirmation_status=None, cancelled_at=None, cancel_user_id=None, cancel_username=None, replacing_order_id=None, replaces_order_id=None, in_flight_at=None, live_at=None, received_at=None, reject_reason=None, user_id=None, username=None, terminal_at=None, complex_order_id=None, complex_order_tag=None, preflight_id=None, order_rule=None), complex_order=None, warnings=[Message(code='tif_next_valid_sesssion', message='Your order will begin working during next valid session.', preflight_id=None)], errors=None)
 
 Options chain/streaming greeks
 ------------------------------
 
 .. code-block:: python
 
    from tastytrade import DXLinkStreamer
@@ -124,15 +129,17 @@
    subs_list = [chain[exp][0].streamer_symbol]
 
    async with DXLinkStreamer(session) as streamer:
        await streamer.subscribe(EventType.GREEKS, subs_list)
        greeks = await streamer.get_event(EventType.GREEKS)
        print(greeks)
 
->>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
+.. code-block:: bash
+
+   >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
 
 For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
         
 Disclaimer
 ----------
 
 This is an unofficial SDK for Tastytrade. There is no implied warranty for any actions and results which arise from using it.
```

### Comparing `tastytrade-7.3/tastytrade.egg-info/SOURCES.txt` & `tastytrade-8.0/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tests/test_account.py` & `tastytrade-8.0/tests/test_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from decimal import Decimal
 from time import sleep
 
 import pytest
 
-from tastytrade import Account, CertificationSession
+from tastytrade import Account, Session
 from tastytrade.instruments import Equity
 from tastytrade.order import (NewComplexOrder, NewOrder, OrderAction,
-                              OrderStatus, OrderTimeInForce, OrderType,
-                              PriceEffect)
+                              OrderTimeInForce, OrderType, PriceEffect)
 
 
 @pytest.fixture(scope='session')
 def account(session):
     return Account.get_accounts(session)[0]
 
 
 @pytest.fixture(scope='session')
 def cert_session(get_cert_credentials):
     usr, pwd = get_cert_credentials
-    session = CertificationSession(usr, pwd)
+    session = Session(usr, pwd, is_test=True)
     yield session
     session.destroy()
 
 
 @pytest.fixture(scope='session')
 def cert_account(cert_session):
     return Account.get_accounts(cert_session)[1]
@@ -120,22 +119,22 @@
 
 def test_place_oco_order(cert_session, cert_account):
     session = cert_session
     account = cert_account
     # first, buy share of SPY to set up the OCO order
     symbol = Equity.get_equity(session, 'SPY')
     opening = symbol.build_leg(Decimal(1), OrderAction.BUY_TO_OPEN)
-    resp1 = account.place_order(session, NewOrder(
+    _ = account.place_order(session, NewOrder(
         time_in_force=OrderTimeInForce.DAY,
         order_type=OrderType.LIMIT,
         legs=[opening],
         price=Decimal('2.5'),  # should fill immediately for cert account
         price_effect=PriceEffect.DEBIT
     ), dry_run=False)
-    assert resp1.order.status != OrderStatus.REJECTED
+    sleep(3)
 
     closing = symbol.build_leg(Decimal(1), OrderAction.SELL_TO_CLOSE)
     oco = NewComplexOrder(
         orders=[
             NewOrder(
                 time_in_force=OrderTimeInForce.GTC,
                 order_type=OrderType.LIMIT,
```

### Comparing `tastytrade-7.3/tests/test_instruments.py` & `tastytrade-8.0/tests/test_instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tests/test_streamer.py` & `tastytrade-8.0/tests/test_streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tests/test_utils.py` & `tastytrade-8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.3/tests/test_watchlists.py` & `tastytrade-8.0/tests/test_watchlists.py`

 * *Files identical despite different names*

