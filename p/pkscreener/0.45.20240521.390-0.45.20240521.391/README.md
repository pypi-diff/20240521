# Comparing `tmp/pkscreener-0.45.20240521.390.tar.gz` & `tmp/pkscreener-0.45.20240521.391.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240521.390.tar", last modified: Tue May 21 17:40:55 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240521.391.tar", last modified: Tue May 21 18:31:59 2024, max compression
```

## Comparing `pkscreener-0.45.20240521.390.tar` & `pkscreener-0.45.20240521.391.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 17:40:55.964700 pkscreener-0.45.20240521.390/
--rw-rw-rw-   0        0        0     1086 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/LICENSE-Others
--rw-rw-rw-   0        0        0    27920 2024-05-21 17:40:55.964700 pkscreener-0.45.20240521.390/PKG-INFO
--rw-rw-rw-   0        0        0    26981 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 17:40:55.949074 pkscreener-0.45.20240521.390/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 17:40:55.964700 pkscreener-0.45.20240521.390/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5641 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34249 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45624 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8313 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156228 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56423 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    85591 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-21 17:40:48.000000 pkscreener-0.45.20240521.390/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   146404 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1089 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53062 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34370 2024-05-21 17:35:49.000000 pkscreener-0.45.20240521.390/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-21 17:40:55.949074 pkscreener-0.45.20240521.390/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27920 2024-05-21 17:40:55.000000 pkscreener-0.45.20240521.390/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-21 17:40:55.000000 pkscreener-0.45.20240521.390/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 17:40:55.000000 pkscreener-0.45.20240521.390/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-21 17:40:55.000000 pkscreener-0.45.20240521.390/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-21 17:40:55.000000 pkscreener-0.45.20240521.390/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-21 17:40:55.000000 pkscreener-0.45.20240521.390/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-21 17:40:55.964700 pkscreener-0.45.20240521.390/setup.cfg
--rw-rw-rw-   0        0        0     5728 2024-05-21 17:35:50.000000 pkscreener-0.45.20240521.390/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:59.568541 pkscreener-0.45.20240521.391/
+-rw-rw-rw-   0        0        0     1086 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/LICENSE-Others
+-rw-rw-rw-   0        0        0    27920 2024-05-21 18:31:59.568541 pkscreener-0.45.20240521.391/PKG-INFO
+-rw-rw-rw-   0        0        0    26981 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:59.552947 pkscreener-0.45.20240521.391/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:59.568541 pkscreener-0.45.20240521.391/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34249 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45624 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8313 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156228 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56423 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    85654 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-21 18:31:49.000000 pkscreener-0.45.20240521.391/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   147079 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1089 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53062 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34370 2024-05-21 18:26:45.000000 pkscreener-0.45.20240521.391/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:31:59.568541 pkscreener-0.45.20240521.391/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27920 2024-05-21 18:31:59.000000 pkscreener-0.45.20240521.391/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-21 18:31:59.000000 pkscreener-0.45.20240521.391/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 18:31:59.000000 pkscreener-0.45.20240521.391/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-21 18:31:59.000000 pkscreener-0.45.20240521.391/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 18:31:59.000000 pkscreener-0.45.20240521.391/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-21 18:31:59.000000 pkscreener-0.45.20240521.391/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-21 18:31:59.568541 pkscreener-0.45.20240521.391/setup.cfg
+-rw-rw-rw-   0        0        0     5728 2024-05-21 18:26:46.000000 pkscreener-0.45.20240521.391/setup.py
```

### Comparing `pkscreener-0.45.20240521.390/LICENSE` & `pkscreener-0.45.20240521.391/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/LICENSE-Others` & `pkscreener-0.45.20240521.391/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/PKG-INFO` & `pkscreener-0.45.20240521.391/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.390
+Version: 0.45.20240521.391
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.390.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.391.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.390/README.md` & `pkscreener-0.45.20240521.391/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.390/pkscreener/__init__.py` & `pkscreener-0.45.20240521.391/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1007,15 +1007,15 @@
                     + colorText.FAIL
                     + "[+] Market Stock Data is not cached, or forced to redownload .."
                     + colorText.END
                 )
         OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.GREEN
-                + "[+] Downloading cache from server for faster processing, Please Wait.."
+                + f"[+] Downloading {'Intraday' if configManager.isIntradayConfig() else 'Daily'} cache from server for faster processing, Please Wait.."
                 + colorText.END
             )
         cache_url = (
                 "https://raw.githubusercontent.com/pkjmesra/PKScreener/actions-data-download/actions-data-download/"
                 + cache_file  # .split(os.sep)[-1]
             )
         headers = {
```

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/classes/keys.py` & `pkscreener-0.45.20240521.391/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/courbd.ttf` & `pkscreener-0.45.20240521.391/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/globals.py` & `pkscreener-0.45.20240521.391/pkscreener/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -819,17 +819,18 @@
                 updateMenuChoiceHierarchy()
                 if userPassedArgs.pipedmenus is not None:
                     chosenOptions = scannerOption.split("-o ")[1]
                     userPassedArgs.options = chosenOptions.replace("'","")
                     return addOrRunPipedMenus()
                 launcher = sys.argv[0]
                 launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
-                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} {scannerOption}{colorText.END}")
+                scannerOptionQuoted = scannerOption.replace("'",'"')
+                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} {scannerOptionQuoted}{colorText.END}")
                 sleep(2)
-                os.system(f"{launcher} {scannerOption}")
+                os.system(f"{launcher} {scannerOptionQuoted}")
                 OutputControls().printOutput(
                         colorText.GREEN
                         + f"[+] Finished running all piped scanners!"
                         + colorText.END
                     )
                 if defaultAnswer is None:
                     input("Press <Enter> to exit...")
@@ -1085,15 +1086,16 @@
             or insideBarToLookback is None
             or respChartPattern == 0
             or (maLength == 0 and respChartPattern in [1, 2, 3, 6])
         ):
             return None, None
         else:
             selectedChoice["3"] = str(respChartPattern)
-            selectedChoice["4"] = str(maLength)
+            selectedChoice["4"] = str(insideBarToLookback) if (respChartPattern in [1, 2, 3] and (userPassedArgs is not None and userPassedArgs.pipedmenus is not None)) else str(maLength)
+            selectedChoice["5"] = str(maLength) if (respChartPattern in [1, 2, 3] and (userPassedArgs is not None and userPassedArgs.pipedmenus is not None)) else ""
     if executeOption == 8:
         if len(options) >= 5:
             if "".join(str(options[3]).split(".")).isdecimal():
                 minRSI = int(options[3])
             if "".join(str(options[4]).split(".")).isdecimal():
                 maxRSI = int(options[4])
             if str(options[3]).upper() == "D":
@@ -1569,17 +1571,19 @@
             if pinOption in ["1","2"]:
                 if pinOption in ["2"]:
                     monitorOption = "X:0:0"
                     prevOutput_results = ",".join(prevOutput_results)
                     monitorOption = f"{monitorOption}:{prevOutput_results}"
                 launcher = sys.argv[0]
                 launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
-                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with pinned scan option. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -m '{monitorOption}'{colorText.END}")
+                monitorOption = f'"{monitorOption}"'
+                scannerOptionQuoted = monitorOption.replace("'",'"')
+                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with pinned scan option. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -m {scannerOptionQuoted}{colorText.END}")
                 sleep(2)
-                os.system(f"{launcher} -a Y -m '{monitorOption}'")
+                os.system(f"{launcher} -a Y -m {scannerOptionQuoted}")
 
     if userPassedArgs is not None:
         if userPassedArgs.runintradayanalysis:
             analysis_df = screenResults.copy()
             analysis_df.reset_index(inplace=True)
             if 'index' in analysis_df.columns:
                 analysis_df.drop('index', axis=1, inplace=True, errors="ignore")
@@ -1684,30 +1688,32 @@
     
     return summary_df,sorting,sortKeys
 
 def addOrRunPipedMenus():
     global userPassedArgs
     # User must have selected menu "P" earlier
     savedPipes = f"{userPassedArgs.pipedmenus}:>|" if len(userPassedArgs.pipedmenus) > 0 else ""
-    userPassedArgs.pipedmenus = f"{savedPipes}{userPassedArgs.options}"
+    userPassedArgs.pipedmenus = f"{savedPipes}{userPassedArgs.options}:D:D:D:"
     userPassedArgs.pipedmenus = userPassedArgs.pipedmenus.replace("::",":D:")
     userPassedArgs.pipedmenus = f"{userPassedArgs.pipedmenus}{('i '+configManager.duration) if configManager.isIntradayConfig() else ''}"
     updateMenuChoiceHierarchy()
     OutputControls().printOutput(
             colorText.GREEN
             + f"[+] {len(userPassedArgs.pipedmenus.split('|'))} Scanners piped so far: {colorText.END}{colorText.WARN+userPassedArgs.pipedmenus+colorText.END}\n{colorText.GREEN}[+] Do you want to add any more scanners into the pipe?"
             + colorText.END
         )
     shouldAddMoreIntoPipe = input(colorText.FAIL + "[+] Select [Y/N] (Default:N): " + colorText.END) or 'n'
     if shouldAddMoreIntoPipe.lower() != 'y':
         launcher = sys.argv[0]
         launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
-        OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -o '{userPassedArgs.pipedmenus}'{colorText.END}")
+        monitorOption = f'"{userPassedArgs.pipedmenus}"'
+        scannerOptionQuoted = monitorOption.replace("'",'"').replace(":>",":D:D:D:>").replace("::",":")
+        OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -o {scannerOptionQuoted}{colorText.END}")
         sleep(2)
-        os.system(f"{launcher} --systemlaunched -a Y -e -o '{userPassedArgs.pipedmenus}'")
+        os.system(f"{launcher} --systemlaunched -a Y -e -o {scannerOptionQuoted}")
         userPassedArgs.pipedmenus = None
         OutputControls().printOutput(
                 colorText.GREEN
                 + f"[+] Finished running all piped scanners!"
                 + colorText.END
             )
         if defaultAnswer is None:
```

### Comparing `pkscreener-0.45.20240521.390/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240521.391/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240521.391/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240521.391/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240521.391/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.390
+Version: 0.45.20240521.391
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.390.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.391.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.389/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.390/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.390/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240521.391/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.390/setup.py` & `pkscreener-0.45.20240521.391/setup.py`

 * *Files identical despite different names*

