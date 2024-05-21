# Comparing `tmp/pkscreener-0.45.20240519.386.tar.gz` & `tmp/pkscreener-0.45.20240521.387.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240519.386.tar", last modified: Sun May 19 14:04:36 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240521.387.tar", last modified: Tue May 21 08:00:15 2024, max compression
```

## Comparing `pkscreener-0.45.20240519.386.tar` & `pkscreener-0.45.20240521.387.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 14:04:36.471211 pkscreener-0.45.20240519.386/
--rw-rw-rw-   0        0        0     1086 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-19 14:04:36.471211 pkscreener-0.45.20240519.386/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 14:04:36.455587 pkscreener-0.45.20240519.386/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 14:04:36.471211 pkscreener-0.45.20240519.386/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5641 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34249 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45624 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8313 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156140 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56423 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    85480 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-19 14:04:30.000000 pkscreener-0.45.20240519.386/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   145426 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1089 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53044 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34370 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-19 14:04:36.455587 pkscreener-0.45.20240519.386/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-19 14:04:36.000000 pkscreener-0.45.20240519.386/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-19 14:04:36.000000 pkscreener-0.45.20240519.386/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 14:04:36.000000 pkscreener-0.45.20240519.386/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-19 14:04:36.000000 pkscreener-0.45.20240519.386/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-19 14:04:36.000000 pkscreener-0.45.20240519.386/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-19 14:04:36.000000 pkscreener-0.45.20240519.386/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-19 14:04:36.471211 pkscreener-0.45.20240519.386/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-19 14:01:40.000000 pkscreener-0.45.20240519.386/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:00:15.468199 pkscreener-0.45.20240521.387/
+-rw-rw-rw-   0        0        0     1086 2024-05-21 07:56:07.000000 pkscreener-0.45.20240521.387/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-21 07:56:07.000000 pkscreener-0.45.20240521.387/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-21 08:00:15.468199 pkscreener-0.45.20240521.387/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-21 07:56:07.000000 pkscreener-0.45.20240521.387/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 08:00:15.452581 pkscreener-0.45.20240521.387/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:00:15.468199 pkscreener-0.45.20240521.387/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34249 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45624 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8313 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156140 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56423 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    85480 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-21 08:00:06.000000 pkscreener-0.45.20240521.387/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   145457 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1089 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53044 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34370 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:00:15.468199 pkscreener-0.45.20240521.387/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-21 08:00:15.000000 pkscreener-0.45.20240521.387/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-21 08:00:15.000000 pkscreener-0.45.20240521.387/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 08:00:15.000000 pkscreener-0.45.20240521.387/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-21 08:00:15.000000 pkscreener-0.45.20240521.387/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 08:00:15.000000 pkscreener-0.45.20240521.387/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-21 08:00:15.000000 pkscreener-0.45.20240521.387/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-21 08:00:15.468199 pkscreener-0.45.20240521.387/setup.cfg
+-rw-rw-rw-   0        0        0     5728 2024-05-21 07:56:08.000000 pkscreener-0.45.20240521.387/setup.py
```

### Comparing `pkscreener-0.45.20240519.386/LICENSE` & `pkscreener-0.45.20240521.387/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/LICENSE-Others` & `pkscreener-0.45.20240521.387/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/PKG-INFO` & `pkscreener-0.45.20240521.387/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240519.386
+Version: 0.45.20240521.387
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240519.386.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.387.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240519.386/README.md` & `pkscreener-0.45.20240521.387/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240519.386/pkscreener/__init__.py` & `pkscreener-0.45.20240521.387/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/classes/keys.py` & `pkscreener-0.45.20240521.387/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/courbd.ttf` & `pkscreener-0.45.20240521.387/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/globals.py` & `pkscreener-0.45.20240521.387/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1788,15 +1788,15 @@
     return sorting
 
 def resetConfigToDefault():
     global userPassedArgs
     isIntraday = userPassedArgs is not None and userPassedArgs.intraday is not None
     if configManager.isIntradayConfig() or isIntraday:
         configManager.toggleConfig(candleDuration="1d", clearCache=False)
-    if userPassedArgs.monitor is None:
+    if userPassedArgs is not None and userPassedArgs.monitor is None:
         if "PKDevTools_Default_Log_Level" in os.environ.keys():
             if userPassedArgs is None or (userPassedArgs is not None and userPassedArgs.options is not None and "|" not in userPassedArgs.options):
                 del os.environ['PKDevTools_Default_Log_Level']
         configManager.logsEnabled = False
     configManager.setConfig(ConfigManager.parser,default=True,showFileCreatedText=False)
 
 def prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption):
```

### Comparing `pkscreener-0.45.20240519.386/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240521.387/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240521.387/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240521.387/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240519.386/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240521.387/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240519.386
+Version: 0.45.20240521.387
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240519.386.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.387.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.385/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240519.386/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240519.386/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240521.387/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*
