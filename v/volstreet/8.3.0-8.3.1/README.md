# Comparing `tmp/volstreet-8.3.0.tar.gz` & `tmp/volstreet-8.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-8.3.0.tar", last modified: Mon May 20 19:06:57 2024, max compression
+gzip compressed data, was "volstreet-8.3.1.tar", last modified: Mon May 20 19:54:27 2024, max compression
```

## Comparing `volstreet-8.3.0.tar` & `volstreet-8.3.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.154393 volstreet-8.3.0/
--rw-rw-rw-   0        0        0     1293 2024-05-20 19:06:57.154393 volstreet-8.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.3.0/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.3.0/pyproject.toml
--rw-rw-rw-   0        0        0     1155 2024-05-20 19:06:57.154393 volstreet-8.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.060218 volstreet-8.3.0/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.3.0/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.075845 volstreet-8.3.0/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.3.0/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.3.0/volstreet/angel_interface/access_rate_handler.py
--rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.3.0/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     3315 2024-05-06 03:22:49.000000 volstreet-8.3.0/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.3.0/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.3.0/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30773 2024-04-29 09:17:58.000000 volstreet-8.3.0/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.3.0/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.107093 volstreet-8.3.0/volstreet/backtests/
--rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.3.0/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.3.0/volstreet/backtests/analysis.py
--rw-rw-rw-   0        0        0     4181 2024-05-04 08:33:34.000000 volstreet-8.3.0/volstreet/backtests/data_updation.py
--rw-rw-rw-   0        0        0    11651 2024-05-15 10:48:46.000000 volstreet-8.3.0/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.3.0/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    48672 2024-05-02 12:46:20.000000 volstreet-8.3.0/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.3.0/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     7375 2024-05-13 11:20:24.000000 volstreet-8.3.0/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.3.0/volstreet/backtests/result_processing.py
--rw-rw-rw-   0        0        0     6184 2024-05-09 04:00:00.000000 volstreet-8.3.0/volstreet/backtests/runner.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.3.0/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.3.0/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1924 2024-05-13 10:36:16.000000 volstreet-8.3.0/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20882 2024-05-02 08:25:42.000000 volstreet-8.3.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     4712 2024-05-14 04:17:21.000000 volstreet-8.3.0/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.107093 volstreet-8.3.0/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.3.0/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     9819 2024-05-15 11:12:17.000000 volstreet-8.3.0/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.3.0/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    25622 2024-05-06 02:53:39.000000 volstreet-8.3.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.3.0/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.122717 volstreet-8.3.0/volstreet/historical_info/
--rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.3.0/volstreet/historical_info/__init__.py
--rw-rw-rw-   0        0        0    21283 2024-05-17 00:34:51.000000 volstreet-8.3.0/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0    17040 2024-05-17 18:08:08.000000 volstreet-8.3.0/volstreet/historical_info/market_days.pkl
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.122717 volstreet-8.3.0/volstreet/models/
--rw-rw-rw-   0        0        0      568 2024-04-29 10:45:14.000000 volstreet-8.3.0/volstreet/models/__init__.py
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.3.0/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.122717 volstreet-8.3.0/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.3.0/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.3.0/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.3.0/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.138758 volstreet-8.3.0/volstreet/strategies/
--rw-rw-rw-   0        0        0      183 2024-05-03 07:00:07.000000 volstreet-8.3.0/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    32518 2024-05-18 19:36:37.000000 volstreet-8.3.0/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     1925 2024-05-03 06:56:48.000000 volstreet-8.3.0/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    57535 2024-05-20 17:19:10.000000 volstreet-8.3.0/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     6352 2024-05-03 06:56:48.000000 volstreet-8.3.0/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    18537 2024-05-20 15:51:56.000000 volstreet-8.3.0/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0   103760 2024-05-20 19:03:37.000000 volstreet-8.3.0/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0     1251 2024-05-13 11:12:56.000000 volstreet-8.3.0/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.138758 volstreet-8.3.0/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.3.0/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.3.0/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    19390 2024-05-18 19:41:11.000000 volstreet-8.3.0/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    20161 2024-05-20 15:51:56.000000 volstreet-8.3.0/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.154393 volstreet-8.3.0/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.3.0/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    14493 2024-05-14 04:28:00.000000 volstreet-8.3.0/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.3.0/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.3.0/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.3.0/volstreet/vectorized_blackscholes.py
--rw-rw-rw-   0        0        0       16 2024-05-20 19:00:58.000000 volstreet-8.3.0/volstreet/volstreet_mode.json
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.154393 volstreet-8.3.0/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.3.0/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.3.0/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.3.0/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.3.0/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.3.0/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:06:57.154393 volstreet-8.3.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-05-20 19:06:56.000000 volstreet-8.3.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2833 2024-05-20 19:06:57.000000 volstreet-8.3.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 19:06:57.000000 volstreet-8.3.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-05-20 19:06:57.000000 volstreet-8.3.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-20 19:06:57.000000 volstreet-8.3.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.282871 volstreet-8.3.1/
+-rw-rw-rw-   0        0        0     1293 2024-05-20 19:54:27.282871 volstreet-8.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.3.1/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1155 2024-05-20 19:54:27.283880 volstreet-8.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.184116 volstreet-8.3.1/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.3.1/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.204418 volstreet-8.3.1/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.3.1/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.3.1/volstreet/angel_interface/access_rate_handler.py
+-rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.3.1/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     3315 2024-05-06 03:22:49.000000 volstreet-8.3.1/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.3.1/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.3.1/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30773 2024-04-29 09:17:58.000000 volstreet-8.3.1/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.3.1/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.225684 volstreet-8.3.1/volstreet/backtests/
+-rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.3.1/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.3.1/volstreet/backtests/analysis.py
+-rw-rw-rw-   0        0        0     4181 2024-05-04 08:33:34.000000 volstreet-8.3.1/volstreet/backtests/data_updation.py
+-rw-rw-rw-   0        0        0    11651 2024-05-15 10:48:46.000000 volstreet-8.3.1/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.3.1/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    48672 2024-05-02 12:46:20.000000 volstreet-8.3.1/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.3.1/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     7375 2024-05-13 11:20:24.000000 volstreet-8.3.1/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.3.1/volstreet/backtests/result_processing.py
+-rw-rw-rw-   0        0        0     6184 2024-05-09 04:00:00.000000 volstreet-8.3.1/volstreet/backtests/runner.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.3.1/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.3.1/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1924 2024-05-13 10:36:16.000000 volstreet-8.3.1/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20882 2024-05-02 08:25:42.000000 volstreet-8.3.1/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     4712 2024-05-14 04:17:21.000000 volstreet-8.3.1/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.238806 volstreet-8.3.1/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.3.1/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     9819 2024-05-15 11:12:17.000000 volstreet-8.3.1/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.3.1/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    25622 2024-05-06 02:53:39.000000 volstreet-8.3.1/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.3.1/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.242936 volstreet-8.3.1/volstreet/historical_info/
+-rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.3.1/volstreet/historical_info/__init__.py
+-rw-rw-rw-   0        0        0    21283 2024-05-17 00:34:51.000000 volstreet-8.3.1/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0    17053 2024-05-20 19:24:40.000000 volstreet-8.3.1/volstreet/historical_info/market_days.pkl
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.243937 volstreet-8.3.1/volstreet/models/
+-rw-rw-rw-   0        0        0      568 2024-04-29 10:45:14.000000 volstreet-8.3.1/volstreet/models/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.3.1/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.248936 volstreet-8.3.1/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.3.1/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.3.1/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.3.1/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.260069 volstreet-8.3.1/volstreet/strategies/
+-rw-rw-rw-   0        0        0      183 2024-05-03 07:00:07.000000 volstreet-8.3.1/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    32518 2024-05-18 19:36:37.000000 volstreet-8.3.1/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     1925 2024-05-03 06:56:48.000000 volstreet-8.3.1/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    57535 2024-05-20 17:19:10.000000 volstreet-8.3.1/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     6352 2024-05-03 06:56:48.000000 volstreet-8.3.1/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    18537 2024-05-20 15:51:56.000000 volstreet-8.3.1/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0   103760 2024-05-20 19:42:30.000000 volstreet-8.3.1/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0     1251 2024-05-13 11:12:56.000000 volstreet-8.3.1/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.265483 volstreet-8.3.1/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.3.1/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.3.1/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19390 2024-05-18 19:41:11.000000 volstreet-8.3.1/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    20161 2024-05-20 15:51:56.000000 volstreet-8.3.1/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.273236 volstreet-8.3.1/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.3.1/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    14493 2024-05-14 04:28:00.000000 volstreet-8.3.1/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.3.1/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.3.1/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.3.1/volstreet/vectorized_blackscholes.py
+-rw-rw-rw-   0        0        0       16 2024-05-20 19:48:35.000000 volstreet-8.3.1/volstreet/volstreet_mode.json
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.280763 volstreet-8.3.1/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.3.1/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.3.1/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.3.1/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.3.1/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.3.1/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:27.281763 volstreet-8.3.1/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-05-20 19:54:27.000000 volstreet-8.3.1/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2024-05-20 19:54:27.000000 volstreet-8.3.1/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 19:54:27.000000 volstreet-8.3.1/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-05-20 19:54:27.000000 volstreet-8.3.1/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-20 19:54:27.000000 volstreet-8.3.1/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-8.3.0/PKG-INFO` & `volstreet-8.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.3.0
+Version: 8.3.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.3.0/setup.cfg` & `volstreet-8.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 382e 332e 300d 0a61  rsion = 8.3.0..a
+00000020: 7273 696f 6e20 3d20 382e 332e 310d 0a61  rsion = 8.3.1..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-8.3.0/volstreet/angel_interface/access_rate_handler.py` & `volstreet-8.3.1/volstreet/angel_interface/access_rate_handler.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/angel_interface/async_interface.py` & `volstreet-8.3.1/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/angel_interface/base_websocket.py` & `volstreet-8.3.1/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/angel_interface/interface.py` & `volstreet-8.3.1/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/angel_interface/login.py` & `volstreet-8.3.1/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/angel_interface/order_websocket.py` & `volstreet-8.3.1/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/angel_interface/price_websocket.py` & `volstreet-8.3.1/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/angel_interface/smart_connect.py` & `volstreet-8.3.1/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/analysis.py` & `volstreet-8.3.1/volstreet/backtests/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/data_updation.py` & `volstreet-8.3.1/volstreet/backtests/data_updation.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/database.py` & `volstreet-8.3.1/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/delta_hedging.py` & `volstreet-8.3.1/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/delta_optimizer.py` & `volstreet-8.3.1/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/framework.py` & `volstreet-8.3.1/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-8.3.1/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/proxy_functions.py` & `volstreet-8.3.1/volstreet/backtests/proxy_functions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/result_processing.py` & `volstreet-8.3.1/volstreet/backtests/result_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/runner.py` & `volstreet-8.3.1/volstreet/backtests/runner.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/tools.py` & `volstreet-8.3.1/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/trend.py` & `volstreet-8.3.1/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/backtests/underlying_info.py` & `volstreet-8.3.1/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/blackscholes.py` & `volstreet-8.3.1/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/config.py` & `volstreet-8.3.1/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/database_connection.py` & `volstreet-8.3.1/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/datamodule/analysis.py` & `volstreet-8.3.1/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/datamodule/archive.py` & `volstreet-8.3.1/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/datamodule/data_handling.py` & `volstreet-8.3.1/volstreet/datamodule/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/datamodule/eod_client.py` & `volstreet-8.3.1/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/datamodule/gambling.py` & `volstreet-8.3.1/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/datamodule/intraday_data.py` & `volstreet-8.3.1/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/datamodule/stockmock.py` & `volstreet-8.3.1/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/datamodule/trading_assistance.py` & `volstreet-8.3.1/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/dealingroom.py` & `volstreet-8.3.1/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/decorators.py` & `volstreet-8.3.1/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/discord_bot.py` & `volstreet-8.3.1/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/exceptions.py` & `volstreet-8.3.1/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/historical_info/__init__.py` & `volstreet-8.3.1/volstreet/historical_info/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/historical_info/index_expiries.pkl` & `volstreet-8.3.1/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/historical_info/market_days.pkl` & `volstreet-8.3.1/volstreet/historical_info/market_days.pkl`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9585 4200 0000 0000 005d 9428 8c08  ....B......].(..
+00000000: 8004 9592 4200 0000 0000 005d 9428 8c08  ....B......].(..
 00000010: 6461 7465 7469 6d65 948c 0464 6174 6594  datetime...date.
 00000020: 9394 4304 07e3 0201 9485 9452 9468 0343  ..C........R.h.C
 00000030: 0407 e302 0494 8594 5294 6803 4304 07e3  ........R.h.C...
 00000040: 0205 9485 9452 9468 0343 0407 e302 0694  .....R.h.C......
 00000050: 8594 5294 6803 4304 07e3 0207 9485 9452  ..R.h.C........R
 00000060: 9468 0343 0407 e302 0894 8594 5294 6803  .h.C........R.h.
 00000070: 4304 07e3 020b 9485 9452 9468 0343 0407  C........R.h.C..
@@ -1058,8 +1058,9 @@
 00004210: 07e8 0506 9485 9452 9468 0343 0407 e805  .......R.h.C....
 00004220: 0794 8594 5294 6803 4304 07e8 0508 9485  ....R.h.C.......
 00004230: 9452 9468 0343 0407 e805 0994 8594 5294  .R.h.C........R.
 00004240: 6803 4304 07e8 050a 9485 9452 9468 0343  h.C........R.h.C
 00004250: 0407 e805 0d94 8594 5294 6803 4304 07e8  ........R.h.C...
 00004260: 050e 9485 9452 9468 0343 0407 e805 0f94  .....R.h.C......
 00004270: 8594 5294 6803 4304 07e8 0510 9485 9452  ..R.h.C........R
-00004280: 9468 0343 0407 e805 1194 8594 5294 652e  .h.C........R.e.
+00004280: 9468 0343 0407 e805 1194 8594 5294 6803  .h.C........R.h.
+00004290: 4304 07e8 0512 9485 9452 9465 2e         C........R.e.
```

### Comparing `volstreet-8.3.0/volstreet/models/__init__.py` & `volstreet-8.3.1/volstreet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/parallelization.py` & `volstreet-8.3.1/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/performance_tracking.py` & `volstreet-8.3.1/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/position_dashboard/app.py` & `volstreet-8.3.1/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/position_dashboard/formatting.py` & `volstreet-8.3.1/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/strategies/deployment.py` & `volstreet-8.3.1/volstreet/strategies/deployment.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/strategies/error_handling.py` & `volstreet-8.3.1/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/strategies/helpers.py` & `volstreet-8.3.1/volstreet/strategies/helpers.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/strategies/monitoring.py` & `volstreet-8.3.1/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/strategies/optimization.py` & `volstreet-8.3.1/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/strategies/strats.py` & `volstreet-8.3.1/volstreet/strategies/strats.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2470,15 +2470,14 @@
         f"Lower limit: {price_boundaries[1]:0.2f}.",
         notification_url,
         "INFO",
     )
     entries = 0
     movement = 0
     while entries < max_entries and current_time().time() < exit_time_object:
-        trend_position.update_all_options(True)
 
         # Scan for entry condition
         notifier(
             f"{underlying.name} trender {entries+1} scanning for entry condition.",
             notification_url,
             "INFO",
         )
@@ -2508,14 +2507,15 @@
             f"{underlying.name} at {price}. "
             f"Stop loss at {stop_loss_price}.",
             notification_url,
             "INFO",
         )
 
         # Set quantities and enter the position
+        trend_position.update_all_options(True)
         trend_position.set_recommended_qty(
             optimized=optimized,
             target_delta=target_delta,
             trend_direction=action,
             hedge_offset=hedge_offset,
         )
         trend_position.enter_positions(at_market=at_market)
```

### Comparing `volstreet-8.3.0/volstreet/strategies/tools.py` & `volstreet-8.3.1/volstreet/strategies/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/trade_interface/instruments.py` & `volstreet-8.3.1/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/trade_interface/order_execution.py` & `volstreet-8.3.1/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/trade_interface/underlyings.py` & `volstreet-8.3.1/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/utils/change_config.py` & `volstreet-8.3.1/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/utils/communication.py` & `volstreet-8.3.1/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/utils/core.py` & `volstreet-8.3.1/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/utils/data_io.py` & `volstreet-8.3.1/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/utils/scrip_processing.py` & `volstreet-8.3.1/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/vectorized_blackscholes.py` & `volstreet-8.3.1/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/vslogging/formatters.py` & `volstreet-8.3.1/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/vslogging/logging_config.json` & `volstreet-8.3.1/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/vslogging/logging_setup.py` & `volstreet-8.3.1/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet/vslogging/parsing.py` & `volstreet-8.3.1/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.0/volstreet.egg-info/PKG-INFO` & `volstreet-8.3.1/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.3.0
+Version: 8.3.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.3.0/volstreet.egg-info/SOURCES.txt` & `volstreet-8.3.1/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

