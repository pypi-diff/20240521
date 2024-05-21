# Comparing `tmp/pkscreener-0.45.20240521.393.tar.gz` & `tmp/pkscreener-0.45.20240521.394.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240521.393.tar", last modified: Tue May 21 19:29:43 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240521.394.tar", last modified: Tue May 21 20:39:23 2024, max compression
```

## Comparing `pkscreener-0.45.20240521.393.tar` & `pkscreener-0.45.20240521.394.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 19:29:43.339882 pkscreener-0.45.20240521.393/
--rw-rw-rw-   0        0        0     1086 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/LICENSE-Others
--rw-rw-rw-   0        0        0    27920 2024-05-21 19:29:43.339882 pkscreener-0.45.20240521.393/PKG-INFO
--rw-rw-rw-   0        0        0    26981 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 19:29:43.324264 pkscreener-0.45.20240521.393/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:29:43.339882 pkscreener-0.45.20240521.393/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5641 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34249 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45624 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8313 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156748 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56423 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    85654 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-21 19:29:31.000000 pkscreener-0.45.20240521.393/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   147079 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1089 2024-05-21 19:24:04.000000 pkscreener-0.45.20240521.393/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53062 2024-05-21 19:24:04.000000 pkscreener-0.45.20240521.393/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34370 2024-05-21 19:24:04.000000 pkscreener-0.45.20240521.393/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:29:43.324264 pkscreener-0.45.20240521.393/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27920 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-21 19:29:43.339882 pkscreener-0.45.20240521.393/setup.cfg
--rw-rw-rw-   0        0        0     5728 2024-05-21 19:24:04.000000 pkscreener-0.45.20240521.393/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:39:23.287707 pkscreener-0.45.20240521.394/
+-rw-rw-rw-   0        0        0     1086 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/LICENSE-Others
+-rw-rw-rw-   0        0        0    27920 2024-05-21 20:39:23.287707 pkscreener-0.45.20240521.394/PKG-INFO
+-rw-rw-rw-   0        0        0    26981 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 20:39:23.272086 pkscreener-0.45.20240521.394/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:39:23.287707 pkscreener-0.45.20240521.394/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34249 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45624 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8313 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156748 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56423 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    85688 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-21 20:39:13.000000 pkscreener-0.45.20240521.394/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   147508 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1089 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53062 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34370 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:39:23.272086 pkscreener-0.45.20240521.394/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27920 2024-05-21 20:39:23.000000 pkscreener-0.45.20240521.394/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-21 20:39:23.000000 pkscreener-0.45.20240521.394/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 20:39:23.000000 pkscreener-0.45.20240521.394/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-21 20:39:23.000000 pkscreener-0.45.20240521.394/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 20:39:23.000000 pkscreener-0.45.20240521.394/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-21 20:39:23.000000 pkscreener-0.45.20240521.394/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-21 20:39:23.287707 pkscreener-0.45.20240521.394/setup.cfg
+-rw-rw-rw-   0        0        0     5728 2024-05-21 20:33:20.000000 pkscreener-0.45.20240521.394/setup.py
```

### Comparing `pkscreener-0.45.20240521.393/LICENSE` & `pkscreener-0.45.20240521.394/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/LICENSE-Others` & `pkscreener-0.45.20240521.394/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/PKG-INFO` & `pkscreener-0.45.20240521.394/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.393
+Version: 0.45.20240521.394
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.393.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.394.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.393/README.md` & `pkscreener-0.45.20240521.394/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.393/pkscreener/__init__.py` & `pkscreener-0.45.20240521.394/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,15 @@
         stdFont_oneLinelabel_width, stdFont_oneLinelabel_height = stdfont.getsize_multiline(label)
         stdFont_scanResulttext_width, stdFont_scanResulttext_height = stdfont.getsize_multiline(table) if len(table) > 0 else (0,0)
         unstyled_backtestsummary = tools.removeAllColorStyles(backtestSummary)
         unstyled_backtestDetail = tools.removeAllColorStyles(backtestDetail)
         stdFont_backtestSummary_text_width,stdFont_backtestSummary_text_height= stdfont.getsize_multiline(unstyled_backtestsummary) if len(unstyled_backtestsummary) > 0 else (0,0)
         stdFont_backtestDetail_text_width, stdFont_backtestDetail_text_height = stdfont.getsize_multiline(unstyled_backtestDetail) if len(unstyled_backtestDetail) > 0 else (0,0)
         artfont_scanResultText_width, _ = artfont.getsize_multiline(table) if len(table) > 0 else (0,0)
-        artfont_backtestSummary_text_width, _ = artfont.getsize_multiline(backtestSummary) if len(backtestSummary) > 0 else (0,0)
+        artfont_backtestSummary_text_width, _ = artfont.getsize_multiline(backtestSummary) if (backtestSummary is not None and len(backtestSummary)) > 0 else (0,0)
         stdfont_addendumtext_height = 0
         stdfont_addendumtext_width = 0
         if addendum is not None and len(addendum) > 0:
             unstyled_addendum = tools.removeAllColorStyles(addendum)
             stdfont_addendumtext_width , stdfont_addendumtext_height = stdfont.getsize_multiline(unstyled_addendum)
             titleLabels.append(addendumLabel)
             dfs_to_print.append(addendum)
```

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/classes/keys.py` & `pkscreener-0.45.20240521.394/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/courbd.ttf` & `pkscreener-0.45.20240521.394/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/globals.py` & `pkscreener-0.45.20240521.394/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1497,22 +1497,29 @@
                             addendumLabel="NSE Stocks giving bonus:",
                             backtestSummary=shareable_strings[2],
                             backtestDetail="",
                             summaryLabel = "NSE Stocks with corporate action type stock split:",
                             detailLabel = None,
                             )
                 elif "|" not in userPassedArgs.options:
-                    printNotifySaveScreenedResults(
-                        screenResults,
-                        saveResults,
-                        selectedChoice,
-                        menuChoiceHierarchy,
-                        testing,
-                        user=user,
-                    )
+                    try:
+                        printNotifySaveScreenedResults(
+                            screenResults,
+                            saveResults,
+                            selectedChoice,
+                            menuChoiceHierarchy,
+                            testing,
+                            user=user,
+                        )
+                    except Exception as e:
+                        default_logger().debug(e, exc_info=True)
+                        if userPassedArgs.log:
+                            import traceback
+                            traceback.print_exc()
+                        pass
         if menuOption in ["X","C"] and userPassedArgs.monitor is None:
             finishScreening(
                 downloadOnly,
                 testing,
                 stockDictPrimary,
                 configManager,
                 loadCount,
@@ -2028,15 +2035,15 @@
         if "Stock" in saveResults.columns:
             saveResults.drop_duplicates(keep="first", inplace=True)
     
     reportTitle = f"{userPassedArgs.pipedtitle}|" if userPassedArgs is not None and userPassedArgs.pipedtitle is not None else ""
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
-        + f"[+] You chose: {reportTitle}{menuChoiceHierarchy}"
+        + f"[+] You chose: {reportTitle}{menuChoiceHierarchy}[{len(screenResults) if screenResults is not None and not screenResults.empty else 0}]"
         + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
         + colorText.END
         , enableMultipleLineOutput=True
     )
     pngName = f'PKS_{PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)}_{PKDateUtilities.currentDateTime().strftime("%d-%m-%y_%H.%M.%S")}'
     pngExtension = ".png"
     eligible = is_token_telegram_configured()
```

### Comparing `pkscreener-0.45.20240521.393/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240521.394/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240521.394/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240521.394/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240521.394/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.393
+Version: 0.45.20240521.394
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.393.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.394.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.393/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.393/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240521.394/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.393/setup.py` & `pkscreener-0.45.20240521.394/setup.py`

 * *Files identical despite different names*

