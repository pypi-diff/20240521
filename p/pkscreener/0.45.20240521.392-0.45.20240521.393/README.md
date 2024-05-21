# Comparing `tmp/pkscreener-0.45.20240521.392.tar.gz` & `tmp/pkscreener-0.45.20240521.393.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240521.392.tar", last modified: Tue May 21 19:06:38 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240521.393.tar", last modified: Tue May 21 19:29:43 2024, max compression
```

## Comparing `pkscreener-0.45.20240521.392.tar` & `pkscreener-0.45.20240521.393.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 19:06:38.261229 pkscreener-0.45.20240521.392/
--rw-rw-rw-   0        0        0     1086 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/LICENSE-Others
--rw-rw-rw-   0        0        0    27920 2024-05-21 19:06:38.261229 pkscreener-0.45.20240521.392/PKG-INFO
--rw-rw-rw-   0        0        0    26981 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 19:06:38.244912 pkscreener-0.45.20240521.392/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:06:38.261229 pkscreener-0.45.20240521.392/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5641 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34249 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45624 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8313 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156228 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56423 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    85654 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-21 19:06:28.000000 pkscreener-0.45.20240521.392/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   147079 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1089 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53062 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34370 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:06:38.244912 pkscreener-0.45.20240521.392/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27920 2024-05-21 19:06:38.000000 pkscreener-0.45.20240521.392/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-21 19:06:38.000000 pkscreener-0.45.20240521.392/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 19:06:38.000000 pkscreener-0.45.20240521.392/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-21 19:06:38.000000 pkscreener-0.45.20240521.392/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-21 19:06:38.000000 pkscreener-0.45.20240521.392/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-21 19:06:38.000000 pkscreener-0.45.20240521.392/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-21 19:06:38.261229 pkscreener-0.45.20240521.392/setup.cfg
--rw-rw-rw-   0        0        0     5728 2024-05-21 19:00:53.000000 pkscreener-0.45.20240521.392/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:29:43.339882 pkscreener-0.45.20240521.393/
+-rw-rw-rw-   0        0        0     1086 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/LICENSE-Others
+-rw-rw-rw-   0        0        0    27920 2024-05-21 19:29:43.339882 pkscreener-0.45.20240521.393/PKG-INFO
+-rw-rw-rw-   0        0        0    26981 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 19:29:43.324264 pkscreener-0.45.20240521.393/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:29:43.339882 pkscreener-0.45.20240521.393/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34249 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45624 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8313 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156748 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56423 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    85654 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-21 19:29:31.000000 pkscreener-0.45.20240521.393/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   147079 2024-05-21 19:24:03.000000 pkscreener-0.45.20240521.393/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1089 2024-05-21 19:24:04.000000 pkscreener-0.45.20240521.393/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53062 2024-05-21 19:24:04.000000 pkscreener-0.45.20240521.393/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34370 2024-05-21 19:24:04.000000 pkscreener-0.45.20240521.393/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:29:43.324264 pkscreener-0.45.20240521.393/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27920 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-21 19:29:43.000000 pkscreener-0.45.20240521.393/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-21 19:29:43.339882 pkscreener-0.45.20240521.393/setup.cfg
+-rw-rw-rw-   0        0        0     5728 2024-05-21 19:24:04.000000 pkscreener-0.45.20240521.393/setup.py
```

### Comparing `pkscreener-0.45.20240521.392/LICENSE` & `pkscreener-0.45.20240521.393/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/LICENSE-Others` & `pkscreener-0.45.20240521.393/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/PKG-INFO` & `pkscreener-0.45.20240521.393/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.392
+Version: 0.45.20240521.393
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.392.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.393.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.392/README.md` & `pkscreener-0.45.20240521.393/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.392/pkscreener/__init__.py` & `pkscreener-0.45.20240521.393/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/ScreeningStatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -5634,4132 +5634,4164 @@
 00016010: 2020 2020 2020 2020 2320 5765 2064 6964          # We did
 00016020: 206e 6f74 2066 696e 6420 7468 6520 7374   not find the st
 00016030: 6f63 6b3f 2049 7427 7320 6f6b 6179 2e20  ock? It's okay. 
 00016040: 4d6f 7665 206f 6e20 746f 2074 6865 206e  Move on to the n
 00016050: 6578 7420 6f6e 652e 0d0a 2020 2020 2020  ext one...      
 00016060: 2020 2020 2020 2020 2020 2020 2020 7061                pa
 00016070: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
-00016080: 2020 2020 6966 2073 6563 7572 6974 7920      if security 
-00016090: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160b0: 2020 7769 7468 2053 7570 7072 6573 734f    with SuppressO
-000160c0: 7574 7075 7428 7375 7070 7265 7373 5f73  utput(suppress_s
-000160d0: 7464 6572 723d 5472 7565 2c20 7375 7070  tderr=True, supp
-000160e0: 7265 7373 5f73 7464 6f75 743d 5472 7565  ress_stdout=True
-000160f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00016100: 2020 2020 2020 2020 2020 2020 6676 203d              fv =
-00016110: 2073 6563 7572 6974 792e 6661 6972 5661   security.fairVa
-00016120: 6c75 6528 290d 0a20 2020 2020 2020 2020  lue()..         
-00016130: 2020 2020 2020 2020 2020 2069 6620 6676             if fv
-00016140: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016160: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016180: 2020 2020 2020 2020 2066 7652 6573 706f           fvRespo
-00016190: 6e73 6556 616c 7565 203d 2066 765b 226c  nseValue = fv["l
-000161a0: 6174 6573 7446 6169 7256 616c 7565 225d  atestFairValue"]
-000161b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000161c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000161d0: 2066 7652 6573 706f 6e73 6556 616c 7565   fvResponseValue
-000161e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-000161f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016200: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00016210: 6169 7256 616c 7565 203d 2066 6c6f 6174  airValue = float
-00016220: 2866 7652 6573 706f 6e73 6556 616c 7565  (fvResponseValue
-00016230: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00016240: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00016250: 743a 2023 2070 7261 676d 613a 206e 6f20  t: # pragma: no 
-00016260: 636f 7665 720d 0a20 2020 2020 2020 2020  cover..         
+00016080: 2020 2020 6578 6365 7074 2028 5469 6d65      except (Time
+00016090: 6f75 7445 7272 6f72 2c20 436f 6e6e 6563  outError, Connec
+000160a0: 7469 6f6e 4572 726f 7229 2061 7320 653a  tionError) as e:
+000160b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000160c0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+000160d0: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+000160e0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+000160f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00016100: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
+00016110: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00016120: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00016130: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
+00016140: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00016150: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00016160: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+00016170: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+00016180: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00016190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161a0: 6966 2073 6563 7572 6974 7920 6973 206e  if security is n
+000161b0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000161c0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+000161d0: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
+000161e0: 7428 7375 7070 7265 7373 5f73 7464 6572  t(suppress_stder
+000161f0: 723d 5472 7565 2c20 7375 7070 7265 7373  r=True, suppress
+00016200: 5f73 7464 6f75 743d 5472 7565 293a 0d0a  _stdout=True):..
+00016210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016220: 2020 2020 2020 2020 6676 203d 2073 6563          fv = sec
+00016230: 7572 6974 792e 6661 6972 5661 6c75 6528  urity.fairValue(
+00016240: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00016250: 2020 2020 2020 2069 6620 6676 2069 7320         if fv is 
+00016260: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
 00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016280: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+00016280: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
 00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162a0: 2020 2020 2023 2073 656c 662e 6465 6661       # self.defa
-000162b0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
-000162c0: 2866 227b 657d 5c6e 5265 7370 6f6e 7365  (f"{e}\nResponse
-000162d0: 3a66 763a 5c6e 7b66 767d 222c 2065 7863  :fv:\n{fv}", exc
-000162e0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
-000162f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016300: 2066 6169 7256 616c 7565 203d 2072 6f75   fairValue = rou
-00016310: 6e64 2866 6c6f 6174 2866 6169 7256 616c  nd(float(fairVal
-00016320: 7565 292c 3129 0d0a 2020 2020 2020 2020  ue),1)..        
-00016330: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00016340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016350: 2020 2020 2020 2020 2020 686f 7374 4461            hostDa
-00016360: 7461 2e6c 6f63 5b68 6f73 7444 6174 612e  ta.loc[hostData.
-00016370: 696e 6465 785b 2d31 5d2c 2246 6169 7256  index[-1],"FairV
-00016380: 616c 7565 225d 203d 2066 6169 7256 616c  alue"] = fairVal
-00016390: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-000163a0: 2020 2020 2020 2020 6578 6365 7074 2028          except (
-000163b0: 4b65 7945 7272 6f72 2c49 6e64 6578 4572  KeyError,IndexEr
-000163c0: 726f 7229 3a0d 0a20 2020 2020 2020 2020  ror):..         
-000163d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000163e0: 6173 730d 0a20 2020 2020 2020 2072 6574  ass..        ret
-000163f0: 7572 6e20 6661 6972 5661 6c75 650d 0a0d  urn fairValue...
-00016400: 0a20 2020 2064 6566 2067 6574 4d75 7475  .    def getMutu
-00016410: 616c 4675 6e64 5374 6174 7573 2873 656c  alFundStatus(sel
-00016420: 662c 2073 746f 636b 2c6f 6e6c 794d 463d  f, stock,onlyMF=
-00016430: 4661 6c73 652c 2068 6f73 7444 6174 613d  False, hostData=
-00016440: 4e6f 6e65 2c20 666f 7263 653d 4661 6c73  None, force=Fals
-00016450: 652c 6578 6368 616e 6765 4e61 6d65 3d22  e,exchangeName="
-00016460: 494e 4449 4122 293a 0d0a 2020 2020 2020  INDIA"):..      
-00016470: 2020 6966 2068 6f73 7444 6174 6120 6973    if hostData is
-00016480: 204e 6f6e 6520 6f72 206c 656e 2868 6f73   None or len(hos
-00016490: 7444 6174 6129 203c 2031 3a0d 0a20 2020  tData) < 1:..   
-000164a0: 2020 2020 2020 2020 2068 6f73 7444 6174           hostDat
-000164b0: 6120 3d20 7064 2e44 6174 6146 7261 6d65  a = pd.DataFrame
-000164c0: 2829 0d0a 2020 2020 2020 2020 0d0a 2020  ()..        ..  
-000164d0: 2020 2020 2020 6e65 7443 6861 6e67 654d        netChangeM
-000164e0: 4620 3d20 300d 0a20 2020 2020 2020 206e  F = 0..        n
-000164f0: 6574 4368 616e 6765 496e 7374 203d 2030  etChangeInst = 0
-00016500: 0d0a 2020 2020 2020 2020 6c61 7465 7374  ..        latest
-00016510: 5f6d 6664 6174 6520 3d20 4e6f 6e65 0d0a  _mfdate = None..
-00016520: 2020 2020 2020 2020 6c61 7465 7374 5f69          latest_i
-00016530: 6e73 7464 6174 6520 3d20 4e6f 6e65 0d0a  nstdate = None..
-00016540: 2020 2020 2020 2020 6e65 6564 7346 7265          needsFre
-00016550: 7368 5570 6461 7465 203d 2054 7275 650d  shUpdate = True.
-00016560: 0a20 2020 2020 2020 206c 6173 7444 6179  .        lastDay
-00016570: 4c61 7374 4d6f 6e74 6820 3d20 504b 4461  LastMonth = PKDa
-00016580: 7465 5574 696c 6974 6965 732e 6c61 7374  teUtilities.last
-00016590: 5f64 6179 5f6f 665f 7072 6576 696f 7573  _day_of_previous
-000165a0: 5f6d 6f6e 7468 2850 4b44 6174 6555 7469  _month(PKDateUti
-000165b0: 6c69 7469 6573 2e63 7572 7265 6e74 4461  lities.currentDa
-000165c0: 7465 5469 6d65 2829 290d 0a20 2020 2020  teTime())..     
-000165d0: 2020 2069 6620 686f 7374 4461 7461 2069     if hostData i
-000165e0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
-000165f0: 656e 2868 6f73 7444 6174 6129 203e 2030  en(hostData) > 0
-00016600: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00016610: 6620 224d 4622 2069 6e20 686f 7374 4461  f "MF" in hostDa
-00016620: 7461 2e63 6f6c 756d 6e73 206f 7220 2246  ta.columns or "F
-00016630: 4949 2220 696e 2068 6f73 7444 6174 612e  II" in hostData.
-00016640: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
-00016650: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
-00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016670: 2020 2020 6e65 7443 6861 6e67 654d 4620      netChangeMF 
-00016680: 3d20 686f 7374 4461 7461 2e6c 6f63 5b68  = hostData.loc[h
-00016690: 6f73 7444 6174 612e 696e 6465 785b 2d31  ostData.index[-1
-000166a0: 5d2c 224d 4622 5d0d 0a20 2020 2020 2020  ],"MF"]..       
-000166b0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-000166c0: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
-000166d0: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
-000166e0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-000166f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016700: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00016710: 2020 2020 2020 2020 2020 2020 6e65 7443              netC
-00016720: 6861 6e67 6549 6e73 7420 3d20 686f 7374  hangeInst = host
-00016730: 4461 7461 2e6c 6f63 5b68 6f73 7444 6174  Data.loc[hostDat
-00016740: 612e 696e 6465 785b 2d31 5d2c 2246 4949  a.index[-1],"FII
-00016750: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00016760: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
-00016770: 7272 6f72 2c49 6e64 6578 4572 726f 7229  rror,IndexError)
-00016780: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016790: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
-000167a0: 2020 2020 2020 2020 2020 2020 2074 7279               try
-000167b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000167c0: 2020 2020 2020 206c 6174 6573 745f 6d66         latest_mf
-000167d0: 6461 7465 203d 2068 6f73 7444 6174 612e  date = hostData.
-000167e0: 6c6f 635b 686f 7374 4461 7461 2e69 6e64  loc[hostData.ind
-000167f0: 6578 5b2d 315d 2c22 4d46 5f44 6174 6522  ex[-1],"MF_Date"
-00016800: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016810: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00016820: 616e 6365 286c 6174 6573 745f 6d66 6461  ance(latest_mfda
-00016830: 7465 2c20 666c 6f61 7429 3a0d 0a20 2020  te, float):..   
-00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016850: 2020 2020 206c 6174 6573 745f 6d66 6461       latest_mfda
-00016860: 7465 203d 2064 6174 6574 696d 652e 6461  te = datetime.da
-00016870: 7465 7469 6d65 2e66 726f 6d74 696d 6573  tetime.fromtimes
-00016880: 7461 6d70 286c 6174 6573 745f 6d66 6461  tamp(latest_mfda
-00016890: 7465 292e 7374 7266 7469 6d65 2827 2559  te).strftime('%Y
-000168a0: 2d25 6d2d 2564 2729 0d0a 2020 2020 2020  -%m-%d')..      
-000168b0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-000168c0: 2028 4b65 7945 7272 6f72 2c49 6e64 6578   (KeyError,Index
-000168d0: 4572 726f 7229 3a0d 0a20 2020 2020 2020  Error):..       
-000168e0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-000168f0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00016900: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00016910: 2020 2020 2020 2020 2020 2020 206c 6174               lat
-00016920: 6573 745f 696e 7374 6461 7465 203d 2068  est_instdate = h
-00016930: 6f73 7444 6174 612e 6c6f 635b 686f 7374  ostData.loc[host
-00016940: 4461 7461 2e69 6e64 6578 5b2d 315d 2c22  Data.index[-1],"
-00016950: 4649 495f 4461 7465 225d 0d0a 2020 2020  FII_Date"]..    
+000162a0: 2020 2020 2066 7652 6573 706f 6e73 6556       fvResponseV
+000162b0: 616c 7565 203d 2066 765b 226c 6174 6573  alue = fv["lates
+000162c0: 7446 6169 7256 616c 7565 225d 0d0a 2020  tFairValue"]..  
+000162d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162e0: 2020 2020 2020 2020 2020 6966 2066 7652            if fvR
+000162f0: 6573 706f 6e73 6556 616c 7565 2069 7320  esponseValue is 
+00016300: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00016310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016320: 2020 2020 2020 2020 2020 2066 6169 7256             fairV
+00016330: 616c 7565 203d 2066 6c6f 6174 2866 7652  alue = float(fvR
+00016340: 6573 706f 6e73 6556 616c 7565 290d 0a20  esponseValue).. 
+00016350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016360: 2020 2020 2020 2065 7863 6570 743a 2023         except: #
+00016370: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+00016380: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+00016390: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000163a0: 6173 730d 0a20 2020 2020 2020 2020 2020  ass..           
+000163b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163c0: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
+000163d0: 6c6f 6767 6572 2e64 6562 7567 2866 227b  logger.debug(f"{
+000163e0: 657d 5c6e 5265 7370 6f6e 7365 3a66 763a  e}\nResponse:fv:
+000163f0: 5c6e 7b66 767d 222c 2065 7863 5f69 6e66  \n{fv}", exc_inf
+00016400: 6f3d 5472 7565 290d 0a20 2020 2020 2020  o=True)..       
+00016410: 2020 2020 2020 2020 2020 2020 2066 6169               fai
+00016420: 7256 616c 7565 203d 2072 6f75 6e64 2866  rValue = round(f
+00016430: 6c6f 6174 2866 6169 7256 616c 7565 292c  loat(fairValue),
+00016440: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+00016450: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00016460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016470: 2020 2020 2020 686f 7374 4461 7461 2e6c        hostData.l
+00016480: 6f63 5b68 6f73 7444 6174 612e 696e 6465  oc[hostData.inde
+00016490: 785b 2d31 5d2c 2246 6169 7256 616c 7565  x[-1],"FairValue
+000164a0: 225d 203d 2066 6169 7256 616c 7565 0d0a  "] = fairValue..
+000164b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000164c0: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
+000164d0: 7272 6f72 2c49 6e64 6578 4572 726f 7229  rror,IndexError)
+000164e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000164f0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+00016500: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00016510: 6661 6972 5661 6c75 650d 0a0d 0a20 2020  fairValue....   
+00016520: 2064 6566 2067 6574 4d75 7475 616c 4675   def getMutualFu
+00016530: 6e64 5374 6174 7573 2873 656c 662c 2073  ndStatus(self, s
+00016540: 746f 636b 2c6f 6e6c 794d 463d 4661 6c73  tock,onlyMF=Fals
+00016550: 652c 2068 6f73 7444 6174 613d 4e6f 6e65  e, hostData=None
+00016560: 2c20 666f 7263 653d 4661 6c73 652c 6578  , force=False,ex
+00016570: 6368 616e 6765 4e61 6d65 3d22 494e 4449  changeName="INDI
+00016580: 4122 293a 0d0a 2020 2020 2020 2020 6966  A"):..        if
+00016590: 2068 6f73 7444 6174 6120 6973 204e 6f6e   hostData is Non
+000165a0: 6520 6f72 206c 656e 2868 6f73 7444 6174  e or len(hostDat
+000165b0: 6129 203c 2031 3a0d 0a20 2020 2020 2020  a) < 1:..       
+000165c0: 2020 2020 2068 6f73 7444 6174 6120 3d20       hostData = 
+000165d0: 7064 2e44 6174 6146 7261 6d65 2829 0d0a  pd.DataFrame()..
+000165e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000165f0: 2020 6e65 7443 6861 6e67 654d 4620 3d20    netChangeMF = 
+00016600: 300d 0a20 2020 2020 2020 206e 6574 4368  0..        netCh
+00016610: 616e 6765 496e 7374 203d 2030 0d0a 2020  angeInst = 0..  
+00016620: 2020 2020 2020 6c61 7465 7374 5f6d 6664        latest_mfd
+00016630: 6174 6520 3d20 4e6f 6e65 0d0a 2020 2020  ate = None..    
+00016640: 2020 2020 6c61 7465 7374 5f69 6e73 7464      latest_instd
+00016650: 6174 6520 3d20 4e6f 6e65 0d0a 2020 2020  ate = None..    
+00016660: 2020 2020 6e65 6564 7346 7265 7368 5570      needsFreshUp
+00016670: 6461 7465 203d 2054 7275 650d 0a20 2020  date = True..   
+00016680: 2020 2020 206c 6173 7444 6179 4c61 7374       lastDayLast
+00016690: 4d6f 6e74 6820 3d20 504b 4461 7465 5574  Month = PKDateUt
+000166a0: 696c 6974 6965 732e 6c61 7374 5f64 6179  ilities.last_day
+000166b0: 5f6f 665f 7072 6576 696f 7573 5f6d 6f6e  _of_previous_mon
+000166c0: 7468 2850 4b44 6174 6555 7469 6c69 7469  th(PKDateUtiliti
+000166d0: 6573 2e63 7572 7265 6e74 4461 7465 5469  es.currentDateTi
+000166e0: 6d65 2829 290d 0a20 2020 2020 2020 2069  me())..        i
+000166f0: 6620 686f 7374 4461 7461 2069 7320 6e6f  f hostData is no
+00016700: 7420 4e6f 6e65 2061 6e64 206c 656e 2868  t None and len(h
+00016710: 6f73 7444 6174 6129 203e 2030 3a0d 0a20  ostData) > 0:.. 
+00016720: 2020 2020 2020 2020 2020 2069 6620 224d             if "M
+00016730: 4622 2069 6e20 686f 7374 4461 7461 2e63  F" in hostData.c
+00016740: 6f6c 756d 6e73 206f 7220 2246 4949 2220  olumns or "FII" 
+00016750: 696e 2068 6f73 7444 6174 612e 636f 6c75  in hostData.colu
+00016760: 6d6e 733a 0d0a 2020 2020 2020 2020 2020  mns:..          
+00016770: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00016780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016790: 6e65 7443 6861 6e67 654d 4620 3d20 686f  netChangeMF = ho
+000167a0: 7374 4461 7461 2e6c 6f63 5b68 6f73 7444  stData.loc[hostD
+000167b0: 6174 612e 696e 6465 785b 2d31 5d2c 224d  ata.index[-1],"M
+000167c0: 4622 5d0d 0a20 2020 2020 2020 2020 2020  F"]..           
+000167d0: 2020 2020 2065 7863 6570 7420 284b 6579       except (Key
+000167e0: 4572 726f 722c 496e 6465 7845 7272 6f72  Error,IndexError
+000167f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016800: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+00016810: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00016820: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00016830: 2020 2020 2020 2020 6e65 7443 6861 6e67          netChang
+00016840: 6549 6e73 7420 3d20 686f 7374 4461 7461  eInst = hostData
+00016850: 2e6c 6f63 5b68 6f73 7444 6174 612e 696e  .loc[hostData.in
+00016860: 6465 785b 2d31 5d2c 2246 4949 225d 0d0a  dex[-1],"FII"]..
+00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016880: 6578 6365 7074 2028 4b65 7945 7272 6f72  except (KeyError
+00016890: 2c49 6e64 6578 4572 726f 7229 3a0d 0a20  ,IndexError):.. 
+000168a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168b0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+000168c0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168e0: 2020 206c 6174 6573 745f 6d66 6461 7465     latest_mfdate
+000168f0: 203d 2068 6f73 7444 6174 612e 6c6f 635b   = hostData.loc[
+00016900: 686f 7374 4461 7461 2e69 6e64 6578 5b2d  hostData.index[-
+00016910: 315d 2c22 4d46 5f44 6174 6522 5d0d 0a20  1],"MF_Date"].. 
+00016920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016930: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00016940: 286c 6174 6573 745f 6d66 6461 7465 2c20  (latest_mfdate, 
+00016950: 666c 6f61 7429 3a0d 0a20 2020 2020 2020  float):..       
 00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016970: 6966 2069 7369 6e73 7461 6e63 6528 6c61  if isinstance(la
-00016980: 7465 7374 5f69 6e73 7464 6174 652c 2066  test_instdate, f
-00016990: 6c6f 6174 293a 0d0a 2020 2020 2020 2020  loat):..        
-000169a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169b0: 6c61 7465 7374 5f69 6e73 7464 6174 6520  latest_instdate 
-000169c0: 3d20 6461 7465 7469 6d65 2e64 6174 6574  = datetime.datet
-000169d0: 696d 652e 6672 6f6d 7469 6d65 7374 616d  ime.fromtimestam
-000169e0: 7028 6c61 7465 7374 5f69 6e73 7464 6174  p(latest_instdat
-000169f0: 6529 2e73 7472 6674 696d 6528 2725 592d  e).strftime('%Y-
-00016a00: 256d 2d25 6427 290d 0a20 2020 2020 2020  %m-%d')..       
-00016a10: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00016a20: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
-00016a30: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
-00016a40: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00016a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016a60: 2020 6966 206c 6174 6573 745f 6d66 6461    if latest_mfda
-00016a70: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  te is not None:.
-00016a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016a90: 2020 2020 2073 6176 6564 5f6d 6664 6174       saved_mfdat
-00016aa0: 6520 3d20 504b 4461 7465 5574 696c 6974  e = PKDateUtilit
-00016ab0: 6965 732e 6461 7465 4672 6f6d 596d 6453  ies.dateFromYmdS
-00016ac0: 7472 696e 6728 6c61 7465 7374 5f6d 6664  tring(latest_mfd
-00016ad0: 6174 652e 7370 6c69 7428 2254 2229 5b30  ate.split("T")[0
-00016ae0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00016af0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00016b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016b10: 6176 6564 5f6d 6664 6174 6520 3d20 6c61  aved_mfdate = la
-00016b20: 7374 4461 794c 6173 744d 6f6e 7468 202d  stDayLastMonth -
-00016b30: 2064 6174 6574 696d 652e 7469 6d65 6465   datetime.timede
-00016b40: 6c74 6128 3129 0d0a 2020 2020 2020 2020  lta(1)..        
-00016b50: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
-00016b60: 745f 696e 7374 6461 7465 2069 7320 6e6f  t_instdate is no
-00016b70: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00016b80: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00016b90: 6564 5f69 6e73 7464 6174 6520 3d20 504b  ed_instdate = PK
-00016ba0: 4461 7465 5574 696c 6974 6965 732e 6461  DateUtilities.da
-00016bb0: 7465 4672 6f6d 596d 6453 7472 696e 6728  teFromYmdString(
-00016bc0: 6c61 7465 7374 5f69 6e73 7464 6174 652e  latest_instdate.
-00016bd0: 7370 6c69 7428 2254 2229 5b30 5d29 0d0a  split("T")[0])..
-00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bf0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00016c00: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00016c10: 5f69 6e73 7464 6174 6520 3d20 6c61 7374  _instdate = last
-00016c20: 4461 794c 6173 744d 6f6e 7468 202d 2064  DayLastMonth - d
-00016c30: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
-00016c40: 6128 3129 0d0a 2020 2020 2020 2020 2020  a(1)..          
-00016c50: 2020 2020 2020 746f 6461 7920 3d20 504b        today = PK
-00016c60: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
-00016c70: 7272 656e 7444 6174 6554 696d 6528 290d  rrentDateTime().
-00016c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016c90: 206e 6565 6473 4672 6573 6855 7064 6174   needsFreshUpdat
-00016ca0: 6520 3d20 2873 6176 6564 5f6d 6664 6174  e = (saved_mfdat
-00016cb0: 652e 6461 7465 2829 203c 206c 6173 7444  e.date() < lastD
-00016cc0: 6179 4c61 7374 4d6f 6e74 682e 6461 7465  ayLastMonth.date
-00016cd0: 2829 2920 616e 6420 2873 6176 6564 5f69  ()) and (saved_i
-00016ce0: 6e73 7464 6174 652e 6461 7465 2829 203c  nstdate.date() <
-00016cf0: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
-00016d00: 682e 6461 7465 2829 290d 0a20 2020 2020  h.date())..     
-00016d10: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00016d20: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00016d30: 6564 7346 7265 7368 5570 6461 7465 203d  edsFreshUpdate =
-00016d40: 2054 7275 650d 0a0d 0a20 2020 2020 2020   True....       
-00016d50: 2069 6620 6e65 6564 7346 7265 7368 5570   if needsFreshUp
-00016d60: 6461 7465 2061 6e64 2066 6f72 6365 3a0d  date and force:.
-00016d70: 0a20 2020 2020 2020 2020 2020 206e 6574  .            net
-00016d80: 4368 616e 6765 4d46 2c20 6e65 7443 6861  ChangeMF, netCha
-00016d90: 6e67 6549 6e73 742c 206c 6174 6573 745f  ngeInst, latest_
-00016da0: 6d66 6461 7465 2c20 6c61 7465 7374 5f69  mfdate, latest_i
-00016db0: 6e73 7464 6174 6520 3d20 7365 6c66 2e67  nstdate = self.g
-00016dc0: 6574 4672 6573 684d 4649 5374 6174 7573  etFreshMFIStatus
-00016dd0: 2873 746f 636b 2c65 7863 6861 6e67 654e  (stock,exchangeN
-00016de0: 616d 653d 6578 6368 616e 6765 4e61 6d65  ame=exchangeName
-00016df0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00016e00: 6620 6e65 7443 6861 6e67 654d 4620 6973  f netChangeMF is
-00016e10: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00016e20: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00016e30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016e40: 2020 2020 2020 686f 7374 4461 7461 2e6c        hostData.l
-00016e50: 6f63 5b68 6f73 7444 6174 612e 696e 6465  oc[hostData.inde
-00016e60: 785b 2d31 5d2c 224d 4622 5d20 3d20 6e65  x[-1],"MF"] = ne
-00016e70: 7443 6861 6e67 654d 460d 0a20 2020 2020  tChangeMF..     
-00016e80: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00016e90: 7420 284b 6579 4572 726f 722c 496e 6465  t (KeyError,Inde
-00016ea0: 7845 7272 6f72 293a 0d0a 2020 2020 2020  xError):..      
-00016eb0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00016ec0: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
-00016ed0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00016ee0: 2020 2020 2020 206e 6574 4368 616e 6765         netChange
-00016ef0: 4d46 203d 2030 0d0a 2020 2020 2020 2020  MF = 0..        
-00016f00: 2020 2020 6966 206c 6174 6573 745f 6d66      if latest_mf
-00016f10: 6461 7465 2069 7320 6e6f 7420 4e6f 6e65  date is not None
-00016f20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016f30: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00016f40: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
-00016f50: 7444 6174 612e 6c6f 635b 686f 7374 4461  tData.loc[hostDa
-00016f60: 7461 2e69 6e64 6578 5b2d 315d 2c22 4d46  ta.index[-1],"MF
-00016f70: 5f44 6174 6522 5d20 3d20 6c61 7465 7374  _Date"] = latest
-00016f80: 5f6d 6664 6174 650d 0a20 2020 2020 2020  _mfdate..       
-00016f90: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00016fa0: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
-00016fb0: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
-00016fc0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00016fd0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00016fe0: 206e 6574 4368 616e 6765 496e 7374 2069   netChangeInst i
-00016ff0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00017000: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00017010: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00017020: 2020 2020 2020 2068 6f73 7444 6174 612e         hostData.
-00017030: 6c6f 635b 686f 7374 4461 7461 2e69 6e64  loc[hostData.ind
-00017040: 6578 5b2d 315d 2c22 4649 4922 5d20 3d20  ex[-1],"FII"] = 
-00017050: 6e65 7443 6861 6e67 6549 6e73 740d 0a20  netChangeInst.. 
-00017060: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00017070: 7863 6570 7420 284b 6579 4572 726f 722c  xcept (KeyError,
-00017080: 496e 6465 7845 7272 6f72 293a 0d0a 2020  IndexError):..  
-00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170a0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-000170b0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000170c0: 2020 2020 2020 2020 2020 206e 6574 4368             netCh
-000170d0: 616e 6765 496e 7374 203d 2030 0d0a 2020  angeInst = 0..  
-000170e0: 2020 2020 2020 2020 2020 6966 206c 6174            if lat
-000170f0: 6573 745f 696e 7374 6461 7465 2069 7320  est_instdate is 
-00017100: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00017110: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00017120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017130: 2020 2020 2068 6f73 7444 6174 612e 6c6f       hostData.lo
-00017140: 635b 686f 7374 4461 7461 2e69 6e64 6578  c[hostData.index
-00017150: 5b2d 315d 2c22 4649 495f 4461 7465 225d  [-1],"FII_Date"]
-00017160: 203d 206c 6174 6573 745f 696e 7374 6461   = latest_instda
-00017170: 7465 0d0a 2020 2020 2020 2020 2020 2020  te..            
-00017180: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
-00017190: 7272 6f72 2c49 6e64 6578 4572 726f 7229  rror,IndexError)
-000171a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000171b0: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
-000171c0: 2020 2020 206c 6173 7444 6179 4c61 7374       lastDayLast
-000171d0: 4d6f 6e74 6820 3d20 6c61 7374 4461 794c  Month = lastDayL
-000171e0: 6173 744d 6f6e 7468 2e73 7472 6674 696d  astMonth.strftim
-000171f0: 6528 2225 592d 256d 2d25 6454 3030 3a30  e("%Y-%m-%dT00:0
-00017200: 303a 3030 2e30 3030 2229 0d0a 2020 2020  0:00.000")..    
-00017210: 2020 2020 6966 206f 6e6c 794d 463a 0d0a      if onlyMF:..
-00017220: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00017230: 726e 206e 6574 4368 616e 6765 4d46 0d0a  rn netChangeMF..
-00017240: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
-00017250: 745f 696e 7374 6461 7465 203d 3d20 6c61  t_instdate == la
-00017260: 7465 7374 5f6d 6664 6174 653a 0d0a 2020  test_mfdate:..  
-00017270: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017280: 2028 6e65 7443 6861 6e67 654d 4620 2b20   (netChangeMF + 
-00017290: 6e65 7443 6861 6e67 6549 6e73 7429 0d0a  netChangeInst)..
-000172a0: 2020 2020 2020 2020 656c 6966 206c 6174          elif lat
-000172b0: 6573 745f 6d66 6461 7465 203d 3d20 6c61  est_mfdate == la
-000172c0: 7374 4461 794c 6173 744d 6f6e 7468 3a0d  stDayLastMonth:.
-000172d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000172e0: 7572 6e20 6e65 7443 6861 6e67 654d 460d  urn netChangeMF.
-000172f0: 0a20 2020 2020 2020 2065 6c69 6620 6c61  .        elif la
-00017300: 7465 7374 5f69 6e73 7464 6174 6520 3d3d  test_instdate ==
-00017310: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
-00017320: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-00017330: 7265 7475 726e 206e 6574 4368 616e 6765  return netChange
-00017340: 496e 7374 0d0a 2020 2020 2020 2020 656c  Inst..        el
-00017350: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00017360: 2023 2066 696e 6420 7468 6520 6c61 7465   # find the late
-00017370: 7374 2064 6174 650d 0a20 2020 2020 2020  st date..       
-00017380: 2020 2020 2069 6620 6c61 7465 7374 5f6d       if latest_m
-00017390: 6664 6174 6520 6973 206e 6f74 204e 6f6e  fdate is not Non
-000173a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000173b0: 2020 2020 6c61 7465 7374 5f6d 6664 6174      latest_mfdat
-000173c0: 6520 3d20 504b 4461 7465 5574 696c 6974  e = PKDateUtilit
-000173d0: 6965 732e 6461 7465 4672 6f6d 596d 6453  ies.dateFromYmdS
-000173e0: 7472 696e 6728 6c61 7465 7374 5f6d 6664  tring(latest_mfd
-000173f0: 6174 652e 7370 6c69 7428 2254 2229 5b30  ate.split("T")[0
-00017400: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017410: 6966 206c 6174 6573 745f 696e 7374 6461  if latest_instda
-00017420: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  te is not None:.
-00017430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017440: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
-00017450: 203d 2050 4b44 6174 6555 7469 6c69 7469   = PKDateUtiliti
-00017460: 6573 2e64 6174 6546 726f 6d59 6d64 5374  es.dateFromYmdSt
-00017470: 7269 6e67 286c 6174 6573 745f 696e 7374  ring(latest_inst
-00017480: 6461 7465 2e73 706c 6974 2822 5422 295b  date.split("T")[
-00017490: 305d 290d 0a20 2020 2020 2020 2020 2020  0])..           
-000174a0: 2072 6574 7572 6e20 6e65 7443 6861 6e67   return netChang
-000174b0: 654d 4620 6966 2028 286c 6174 6573 745f  eMF if ((latest_
-000174c0: 6d66 6461 7465 2069 7320 6e6f 7420 4e6f  mfdate is not No
-000174d0: 6e65 2920 616e 6420 6c61 7465 7374 5f6d  ne) and latest_m
-000174e0: 6664 6174 6520 3e20 286c 6174 6573 745f  fdate > (latest_
-000174f0: 696e 7374 6461 7465 2069 6620 6c61 7465  instdate if late
-00017500: 7374 5f69 6e73 7464 6174 6520 6973 206e  st_instdate is n
-00017510: 6f74 204e 6f6e 6520 656c 7365 2028 6c61  ot None else (la
-00017520: 7465 7374 5f6d 6664 6174 6520 2d20 6461  test_mfdate - da
-00017530: 7465 7469 6d65 2e74 696d 6564 656c 7461  tetime.timedelta
-00017540: 2831 2929 2929 2065 6c73 6520 6e65 7443  (1)))) else netC
-00017550: 6861 6e67 6549 6e73 740d 0a0d 0a20 2020  hangeInst....   
-00017560: 2064 6566 2067 6574 4672 6573 684d 4649   def getFreshMFI
-00017570: 5374 6174 7573 2873 656c 662c 2073 746f  Status(self, sto
-00017580: 636b 2c65 7863 6861 6e67 654e 616d 653d  ck,exchangeName=
-00017590: 2249 4e44 4941 2229 3a0d 0a20 2020 2020  "INDIA"):..     
-000175a0: 2020 2063 6861 6e67 6553 7461 7475 7344     changeStatusD
-000175b0: 6174 614d 4620 3d20 4e6f 6e65 0d0a 2020  ataMF = None..  
-000175c0: 2020 2020 2020 6368 616e 6765 5374 6174        changeStat
-000175d0: 7573 4461 7461 496e 7374 203d 204e 6f6e  usDataInst = Non
-000175e0: 650d 0a20 2020 2020 2020 206e 6574 4368  e..        netCh
-000175f0: 616e 6765 4d46 203d 2030 0d0a 2020 2020  angeMF = 0..    
-00017600: 2020 2020 6e65 7443 6861 6e67 6549 6e73      netChangeIns
-00017610: 7420 3d20 300d 0a20 2020 2020 2020 206c  t = 0..        l
-00017620: 6174 6573 745f 6d66 6461 7465 203d 204e  atest_mfdate = N
-00017630: 6f6e 650d 0a20 2020 2020 2020 206c 6174  one..        lat
-00017640: 6573 745f 696e 7374 6461 7465 203d 204e  est_instdate = N
-00017650: 6f6e 650d 0a20 2020 2020 2020 2073 6563  one..        sec
-00017660: 7572 6974 7920 3d20 4e6f 6e65 0d0a 2020  urity = None..  
-00017670: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00017680: 2020 2020 2020 2020 7769 7468 2053 7570          with Sup
-00017690: 7072 6573 734f 7574 7075 7428 7375 7070  pressOutput(supp
-000176a0: 7265 7373 5f73 7464 6572 723d 5472 7565  ress_stderr=True
-000176b0: 2c20 7375 7070 7265 7373 5f73 7464 6f75  , suppress_stdou
-000176c0: 743d 5472 7565 293a 0d0a 2020 2020 2020  t=True):..      
-000176d0: 2020 2020 2020 2020 2020 7365 6375 7269            securi
-000176e0: 7479 203d 2053 746f 636b 2873 746f 636b  ty = Stock(stock
-000176f0: 2c65 7863 6861 6e67 653d 6578 6368 616e  ,exchange=exchan
-00017700: 6765 4e61 6d65 290d 0a20 2020 2020 2020  geName)..       
-00017710: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00017720: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00017730: 2023 2057 6520 6469 6420 6e6f 7420 6669   # We did not fi
-00017740: 6e64 2074 6865 2073 746f 636b 3f20 4974  nd the stock? It
-00017750: 2773 206f 6b61 792e 204d 6f76 6520 6f6e  's okay. Move on
-00017760: 2074 6f20 7468 6520 6e65 7874 206f 6e65   to the next one
-00017770: 2e0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
-00017780: 6173 730d 0a20 2020 2020 2020 2069 6620  ass..        if 
-00017790: 7365 6375 7269 7479 2069 7320 6e6f 7420  security is not 
-000177a0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-000177b0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-000177c0: 2020 2020 2020 2020 2077 6974 6820 5375           with Su
-000177d0: 7070 7265 7373 4f75 7470 7574 2873 7570  ppressOutput(sup
-000177e0: 7072 6573 735f 7374 6465 7272 3d54 7275  press_stderr=Tru
-000177f0: 652c 2073 7570 7072 6573 735f 7374 646f  e, suppress_stdo
-00017800: 7574 3d54 7275 6529 3a0d 0a20 2020 2020  ut=True):..     
-00017810: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00017820: 6861 6e67 6553 7461 7475 7352 6f77 734d  hangeStatusRowsM
-00017830: 4620 3d20 7365 6375 7269 7479 2e6d 7574  F = security.mut
-00017840: 7561 6c46 756e 644f 776e 6572 7368 6970  ualFundOwnership
-00017850: 2874 6f70 3d35 290d 0a20 2020 2020 2020  (top=5)..       
-00017860: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00017870: 6e67 6553 7461 7475 7352 6f77 7349 6e73  ngeStatusRowsIns
-00017880: 7420 3d20 7365 6375 7269 7479 2e69 6e73  t = security.ins
-00017890: 7469 7475 7469 6f6e 4f77 6e65 7273 6869  titutionOwnershi
-000178a0: 7028 746f 703d 3529 0d0a 2020 2020 2020  p(top=5)..      
-000178b0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-000178c0: 616e 6765 5374 6174 7573 4461 7461 4d46  angeStatusDataMF
-000178d0: 203d 2073 6563 7572 6974 792e 6d75 7475   = security.mutu
-000178e0: 616c 4675 6e64 4649 4943 6861 6e67 6544  alFundFIIChangeD
-000178f0: 6174 6128 6368 616e 6765 5374 6174 7573  ata(changeStatus
-00017900: 526f 7773 4d46 290d 0a20 2020 2020 2020  RowsMF)..       
-00017910: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00017920: 6e67 6553 7461 7475 7344 6174 6149 6e73  ngeStatusDataIns
-00017930: 7420 3d20 7365 6375 7269 7479 2e6d 7574  t = security.mut
-00017940: 7561 6c46 756e 6446 4949 4368 616e 6765  ualFundFIIChange
-00017950: 4461 7461 2863 6861 6e67 6553 7461 7475  Data(changeStatu
-00017960: 7352 6f77 7349 6e73 7429 0d0a 2020 2020  sRowsInst)..    
-00017970: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00017980: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
-00017990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179a0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-000179b0: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
-000179c0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
-000179d0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-000179e0: 7970 6545 7272 6f72 206f 7220 436f 6e6e  ypeError or Conn
-000179f0: 6563 7469 6f6e 4572 726f 7220 6265 6361  ectionError beca
-00017a00: 7573 6520 7765 2063 6f75 6c64 206e 6f74  use we could not
-00017a10: 2066 696e 6420 7468 6520 7374 6f63 6b20   find the stock 
-00017a20: 6f72 204d 4649 2064 6174 6120 6973 6e27  or MFI data isn'
-00017a30: 7420 6176 6169 6c61 626c 653f 0d0a 2020  t available?..  
-00017a40: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00017a50: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
-00017a60: 6c61 7374 4461 794c 6173 744d 6f6e 7468  lastDayLastMonth
-00017a70: 203d 2050 4b44 6174 6555 7469 6c69 7469   = PKDateUtiliti
-00017a80: 6573 2e6c 6173 745f 6461 795f 6f66 5f70  es.last_day_of_p
-00017a90: 7265 7669 6f75 735f 6d6f 6e74 6828 504b  revious_month(PK
-00017aa0: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
-00017ab0: 7272 656e 7444 6174 6554 696d 6528 2929  rrentDateTime())
-00017ac0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-00017ad0: 7374 4461 794c 6173 744d 6f6e 7468 203d  stDayLastMonth =
-00017ae0: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
-00017af0: 682e 7374 7266 7469 6d65 2822 2559 2d25  h.strftime("%Y-%
-00017b00: 6d2d 2564 5430 303a 3030 3a30 302e 3030  m-%dT00:00:00.00
-00017b10: 3022 290d 0a20 2020 2020 2020 2020 2020  0")..           
-00017b20: 2069 6620 6368 616e 6765 5374 6174 7573   if changeStatus
-00017b30: 4461 7461 4d46 2069 7320 6e6f 7420 4e6f  DataMF is not No
-00017b40: 6e65 2061 6e64 206c 656e 2863 6861 6e67  ne and len(chang
-00017b50: 6553 7461 7475 7344 6174 614d 4629 203e  eStatusDataMF) >
-00017b60: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00017b70: 2020 2020 2064 665f 6772 6f75 7065 644d       df_groupedM
-00017b80: 4620 3d20 6368 616e 6765 5374 6174 7573  F = changeStatus
-00017b90: 4461 7461 4d46 2e67 726f 7570 6279 2822  DataMF.groupby("
-00017ba0: 6461 7465 222c 2073 6f72 743d 4661 6c73  date", sort=Fals
-00017bb0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00017bc0: 2020 2020 666f 7220 6d66 6461 7465 2c20      for mfdate, 
-00017bd0: 6466 5f67 726f 7570 4d46 2069 6e20 6466  df_groupMF in df
-00017be0: 5f67 726f 7570 6564 4d46 3a0d 0a20 2020  _groupedMF:..   
-00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c00: 206e 6574 4368 616e 6765 4d46 203d 2064   netChangeMF = d
-00017c10: 665f 6772 6f75 704d 465b 2263 6861 6e67  f_groupMF["chang
-00017c20: 6541 6d6f 756e 7422 5d2e 7375 6d28 290d  eAmount"].sum().
-00017c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c40: 2020 2020 206c 6174 6573 745f 6d66 6461       latest_mfda
-00017c50: 7465 203d 206d 6664 6174 650d 0a20 2020  te = mfdate..   
-00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c70: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
-00017c80: 2020 2020 6966 2063 6861 6e67 6553 7461      if changeSta
-00017c90: 7475 7344 6174 6149 6e73 7420 6973 206e  tusDataInst is n
-00017ca0: 6f74 204e 6f6e 6520 616e 6420 6c65 6e28  ot None and len(
-00017cb0: 6368 616e 6765 5374 6174 7573 4461 7461  changeStatusData
-00017cc0: 496e 7374 2920 3e20 303a 0d0a 2020 2020  Inst) > 0:..    
-00017cd0: 2020 2020 2020 2020 2020 2020 6466 5f67              df_g
-00017ce0: 726f 7570 6564 496e 7374 203d 2063 6861  roupedInst = cha
-00017cf0: 6e67 6553 7461 7475 7344 6174 6149 6e73  ngeStatusDataIns
-00017d00: 742e 6772 6f75 7062 7928 2264 6174 6522  t.groupby("date"
-00017d10: 2c20 736f 7274 3d46 616c 7365 290d 0a20  , sort=False).. 
-00017d20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00017d30: 6f72 2069 6e73 7464 6174 652c 2064 665f  or instdate, df_
-00017d40: 6772 6f75 7049 6e73 7420 696e 2064 665f  groupInst in df_
-00017d50: 6772 6f75 7065 6449 6e73 743a 0d0a 2020  groupedInst:..  
-00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 2020 6966 2028 6c61 7465 7374 5f6d 6664    if (latest_mfd
-00017d80: 6174 6520 6973 206e 6f74 204e 6f6e 6520  ate is not None 
-00017d90: 616e 6420 6c61 7465 7374 5f6d 6664 6174  and latest_mfdat
-00017da0: 6520 3d3d 2069 6e73 7464 6174 6529 206f  e == instdate) o
-00017db0: 7220 286c 6174 6573 745f 6d66 6461 7465  r (latest_mfdate
-00017dc0: 2069 7320 4e6f 6e65 2920 6f72 2028 696e   is None) or (in
-00017dd0: 7374 6461 7465 203d 3d20 6c61 7374 4461  stdate == lastDa
-00017de0: 794c 6173 744d 6f6e 7468 293a 0d0a 2020  yLastMonth):..  
-00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e00: 2020 2020 2020 6e65 7443 6861 6e67 6549        netChangeI
-00017e10: 6e73 7420 3d20 6466 5f67 726f 7570 496e  nst = df_groupIn
-00017e20: 7374 5b22 6368 616e 6765 416d 6f75 6e74  st["changeAmount
-00017e30: 225d 2e73 756d 2829 0d0a 2020 2020 2020  "].sum()..      
-00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e50: 2020 6c61 7465 7374 5f69 6e73 7464 6174    latest_instdat
-00017e60: 6520 3d20 696e 7374 6461 7465 0d0a 2020  e = instdate..  
-00017e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e80: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-00017e90: 2072 6574 7572 6e20 6e65 7443 6861 6e67   return netChang
-00017ea0: 654d 462c 6e65 7443 6861 6e67 6549 6e73  eMF,netChangeIns
-00017eb0: 742c 6c61 7465 7374 5f6d 6664 6174 652c  t,latest_mfdate,
-00017ec0: 6c61 7465 7374 5f69 6e73 7464 6174 650d  latest_instdate.
-00017ed0: 0a0d 0a0d 0a20 2020 2064 6566 2067 6574  .....    def get
-00017ee0: 4e69 6674 7950 7265 6469 6374 696f 6e28  NiftyPrediction(
-00017ef0: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
-00017f00: 2020 2020 696d 706f 7274 2077 6172 6e69      import warni
-00017f10: 6e67 730d 0a0d 0a20 2020 2020 2020 2077  ngs....        w
-00017f20: 6172 6e69 6e67 732e 6669 6c74 6572 7761  arnings.filterwa
-00017f30: 726e 696e 6773 2822 6967 6e6f 7265 2229  rnings("ignore")
-00017f40: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-00017f50: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
-00017f60: 2020 2020 6d6f 6465 6c2c 2070 6b6c 203d      model, pkl =
-00017f70: 2055 7469 6c69 7479 2e74 6f6f 6c73 2e67   Utility.tools.g
-00017f80: 6574 4e69 6674 794d 6f64 656c 2829 0d0a  etNiftyModel()..
-00017f90: 2020 2020 2020 2020 6966 206d 6f64 656c          if model
-00017fa0: 2069 7320 4e6f 6e65 206f 7220 706b 6c20   is None or pkl 
-00017fb0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00017fc0: 2020 2020 2020 7265 7475 726e 2030 2c20        return 0, 
-00017fd0: 2255 6e6b 6e6f 776e 222c 2022 556e 6b6e  "Unknown", "Unkn
-00017fe0: 6f77 6e22 0d0a 2020 2020 2020 2020 7769  own"..        wi
-00017ff0: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
-00018000: 7428 7375 7070 7265 7373 5f73 7464 6572  t(suppress_stder
-00018010: 723d 5472 7565 2c20 7375 7070 7265 7373  r=True, suppress
-00018020: 5f73 7464 6f75 743d 5472 7565 293a 0d0a  _stdout=True):..
-00018030: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00018040: 203d 2064 6174 615b 706b 6c5b 2263 6f6c   = data[pkl["col
-00018050: 756d 6e73 225d 5d0d 0a20 2020 2020 2020  umns"]]..       
-00018060: 2020 2020 2023 2323 2076 3220 5072 6570       ### v2 Prep
-00018070: 726f 6365 7373 696e 670d 0a20 2020 2020  rocessing..     
-00018080: 2020 2020 2020 2064 6174 615b 2248 6967         data["Hig
-00018090: 6822 5d20 3d20 6461 7461 5b22 4869 6768  h"] = data["High
-000180a0: 225d 2e70 6374 5f63 6861 6e67 6528 2920  "].pct_change() 
-000180b0: 2a20 3130 300d 0a20 2020 2020 2020 2020  * 100..         
-000180c0: 2020 2064 6174 615b 224c 6f77 225d 203d     data["Low"] =
-000180d0: 2064 6174 615b 224c 6f77 225d 2e70 6374   data["Low"].pct
-000180e0: 5f63 6861 6e67 6528 2920 2a20 3130 300d  _change() * 100.
-000180f0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00018100: 615b 224f 7065 6e22 5d20 3d20 6461 7461  a["Open"] = data
-00018110: 5b22 4f70 656e 225d 2e70 6374 5f63 6861  ["Open"].pct_cha
-00018120: 6e67 6528 2920 2a20 3130 300d 0a20 2020  nge() * 100..   
-00018130: 2020 2020 2020 2020 2064 6174 615b 2243           data["C
-00018140: 6c6f 7365 225d 203d 2064 6174 615b 2243  lose"] = data["C
-00018150: 6c6f 7365 225d 2e70 6374 5f63 6861 6e67  lose"].pct_chang
-00018160: 6528 2920 2a20 3130 300d 0a20 2020 2020  e() * 100..     
-00018170: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00018180: 7461 2e69 6c6f 635b 2d31 5d0d 0a20 2020  ta.iloc[-1]..   
-00018190: 2020 2020 2020 2020 2023 2323 0d0a 2020           ###..  
-000181a0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-000181b0: 2070 6b6c 5b22 7363 616c 6572 225d 2e74   pkl["scaler"].t
-000181c0: 7261 6e73 666f 726d 285b 6461 7461 5d29  ransform([data])
-000181d0: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-000181e0: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
-000181f0: 7428 7375 7070 7265 7373 5f73 7464 6f75  t(suppress_stdou
-00018200: 743d 5472 7565 2c20 7375 7070 7265 7373  t=True, suppress
-00018210: 5f73 7464 6572 723d 5472 7565 293a 0d0a  _stderr=True):..
-00018220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018230: 7072 6564 203d 206d 6f64 656c 2e70 7265  pred = model.pre
-00018240: 6469 6374 2864 6174 6129 5b30 5d0d 0a20  dict(data)[0].. 
-00018250: 2020 2020 2020 2069 6620 7072 6564 203e         if pred >
-00018260: 2030 2e35 3a0d 0a20 2020 2020 2020 2020   0.5:..         
-00018270: 2020 206f 7574 5465 7874 203d 2022 4245     outText = "BE
-00018280: 4152 4953 4822 0d0a 2020 2020 2020 2020  ARISH"..        
-00018290: 2020 2020 6f75 7420 3d20 280d 0a20 2020      out = (..   
-000182a0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-000182b0: 6f72 5465 7874 2e42 4f4c 440d 0a20 2020  orText.BOLD..   
-000182c0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-000182d0: 6f6c 6f72 5465 7874 2e46 4149 4c0d 0a20  olorText.FAIL.. 
-000182e0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-000182f0: 206f 7574 5465 7874 0d0a 2020 2020 2020   outText..      
-00018300: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-00018310: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-00018320: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00018330: 6f72 5465 7874 2e42 4f4c 440d 0a20 2020  orText.BOLD..   
-00018340: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00018350: 2020 2020 2020 2020 7375 6720 3d20 2248          sug = "H
-00018360: 6f6c 6420 796f 7572 2053 686f 7274 2070  old your Short p
-00018370: 6f73 6974 696f 6e21 220d 0a20 2020 2020  osition!"..     
-00018380: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00018390: 2020 2020 2020 6f75 7454 6578 7420 3d20        outText = 
-000183a0: 2242 554c 4c49 5348 220d 0a20 2020 2020  "BULLISH"..     
-000183b0: 2020 2020 2020 206f 7574 203d 2028 0d0a         out = (..
-000183c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183d0: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
-000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183f0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-00018400: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
-00018410: 2020 202b 206f 7574 5465 7874 0d0a 2020     + outText..  
-00018420: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00018430: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-00018440: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00018450: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
-00018460: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00018470: 2020 2020 2020 2020 2020 2020 7375 6720              sug 
-00018480: 3d20 2253 7461 7920 4275 6c6c 6973 6821  = "Stay Bullish!
-00018490: 220d 0a20 2020 2020 2020 2069 6620 504b  "..        if PK
-000184a0: 4461 7465 5574 696c 6974 6965 732e 6973  DateUtilities.is
-000184b0: 436c 6f73 696e 6748 6f75 7228 293a 0d0a  ClosingHour():..
-000184c0: 2020 2020 2020 2020 2020 2020 4f75 7470              Outp
-000184d0: 7574 436f 6e74 726f 6c73 2829 2e70 7269  utControls().pri
-000184e0: 6e74 4f75 7470 7574 280d 0a20 2020 2020  ntOutput(..     
-000184f0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00018500: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
-00018510: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00018520: 6f72 5465 7874 2e57 4152 4e0d 0a20 2020  orText.WARN..   
-00018530: 2020 2020 2020 2020 2020 2020 202b 2022               + "
-00018540: 4e6f 7465 3a20 5468 6520 4149 2070 7265  Note: The AI pre
-00018550: 6469 6374 696f 6e20 7368 6f75 6c64 2062  diction should b
-00018560: 6520 6578 6563 7574 6564 2041 6674 6572  e executed After
-00018570: 2033 2050 4d20 6f72 204e 6561 7220 746f   3 PM or Near to
-00018580: 2043 6c6f 7369 6e67 2074 696d 6520 6173   Closing time as
-00018590: 2074 6865 2050 7265 6469 6374 696f 6e20   the Prediction 
-000185a0: 4163 6375 7261 6379 2069 7320 6261 7365  Accuracy is base
-000185b0: 6420 6f6e 2074 6865 2043 6c6f 7369 6e67  d on the Closing
-000185c0: 2070 7269 6365 2122 0d0a 2020 2020 2020   price!"..      
-000185d0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-000185e0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-000185f0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00018600: 2020 7072 6564 6963 7469 6f6e 5465 7874    predictionText
-00018610: 203d 2022 4d61 726b 6574 206d 6179 204f   = "Market may O
-00018620: 7065 6e20 7b7d 206e 6578 7420 6461 7921  pen {} next day!
-00018630: 207b 7d22 2e66 6f72 6d61 7428 6f75 742c   {}".format(out,
-00018640: 2073 7567 290d 0a20 2020 2020 2020 2073   sug)..        s
-00018650: 7472 656e 6774 6854 6578 7420 3d20 2250  trengthText = "P
-00018660: 726f 6261 6269 6c69 7479 2f53 7472 656e  robability/Stren
-00018670: 6774 6820 6f66 2050 7265 6469 6374 696f  gth of Predictio
-00018680: 6e20 3d20 7b7d 2522 2e66 6f72 6d61 7428  n = {}%".format(
-00018690: 0d0a 2020 2020 2020 2020 2020 2020 5574  ..            Ut
-000186a0: 696c 6974 792e 746f 6f6c 732e 6765 7453  ility.tools.getS
-000186b0: 6967 6d6f 6964 436f 6e66 6964 656e 6365  igmoidConfidence
-000186c0: 2870 7265 645b 305d 290d 0a20 2020 2020  (pred[0])..     
-000186d0: 2020 2029 0d0a 2020 2020 2020 2020 4f75     )..        Ou
-000186e0: 7470 7574 436f 6e74 726f 6c73 2829 2e70  tputControls().p
-000186f0: 7269 6e74 4f75 7470 7574 280d 0a20 2020  rintOutput(..   
-00018700: 2020 2020 2020 2020 2063 6f6c 6f72 5465           colorTe
-00018710: 7874 2e42 4f4c 440d 0a20 2020 2020 2020  xt.BOLD..       
-00018720: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-00018730: 2e42 4c55 450d 0a20 2020 2020 2020 2020  .BLUE..         
-00018740: 2020 202b 2022 5c6e 220d 0a20 2020 2020     + "\n"..     
-00018750: 2020 2020 2020 202b 2022 5b2b 5d20 4e69         + "[+] Ni
-00018760: 6674 7920 4149 2050 7265 6469 6374 696f  fty AI Predictio
-00018770: 6e20 2d3e 2022 0d0a 2020 2020 2020 2020  n -> "..        
-00018780: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-00018790: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-000187a0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-000187b0: 440d 0a20 2020 2020 2020 2020 2020 202b  D..            +
-000187c0: 2070 7265 6469 6374 696f 6e54 6578 740d   predictionText.
-000187d0: 0a20 2020 2020 2020 2020 2020 202b 2063  .            + c
-000187e0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-000187f0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00018800: 204f 7574 7075 7443 6f6e 7472 6f6c 7328   OutputControls(
-00018810: 292e 7072 696e 744f 7574 7075 7428 0d0a  ).printOutput(..
-00018820: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00018830: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
-00018840: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00018850: 6578 742e 424c 5545 0d0a 2020 2020 2020  ext.BLUE..      
-00018860: 2020 2020 2020 2b20 225c 6e22 0d0a 2020        + "\n"..  
-00018870: 2020 2020 2020 2020 2020 2b20 225b 2b5d            + "[+]
-00018880: 204e 6966 7479 2041 4920 5072 6564 6963   Nifty AI Predic
-00018890: 7469 6f6e 202d 3e20 220d 0a20 2020 2020  tion -> "..     
-000188a0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-000188b0: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
-000188c0: 2020 2020 2b20 7374 7265 6e67 7468 5465      + strengthTe
-000188d0: 7874 0d0a 2020 2020 2020 2020 290d 0a0d  xt..        )...
-000188e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000188f0: 7072 6564 2c20 7072 6564 6963 7469 6f6e  pred, prediction
-00018900: 5465 7874 2e72 6570 6c61 6365 286f 7574  Text.replace(out
-00018910: 2c20 6f75 7454 6578 7429 2c20 7374 7265  , outText), stre
-00018920: 6e67 7468 5465 7874 0d0a 0d0a 2020 2020  ngthText....    
-00018930: 6465 6620 6d6f 6e69 746f 7246 6976 6545  def monitorFiveE
-00018940: 6d61 2873 656c 662c 2066 6574 6368 6572  ma(self, fetcher
-00018950: 2c20 7265 7375 6c74 5f64 662c 206c 6173  , result_df, las
-00018960: 745f 7369 676e 616c 2c20 7269 736b 5f72  t_signal, risk_r
-00018970: 6577 6172 643d 3329 3a0d 0a20 2020 2020  eward=3):..     
-00018980: 2020 2063 6f6c 5f6e 616d 6573 203d 205b     col_names = [
-00018990: 2248 6967 6822 2c20 224c 6f77 222c 2022  "High", "Low", "
-000189a0: 436c 6f73 6522 2c20 2235 454d 4122 5d0d  Close", "5EMA"].
-000189b0: 0a20 2020 2020 2020 2064 6174 615f 6c69  .        data_li
-000189c0: 7374 203d 205b 226e 6966 7479 5f62 7579  st = ["nifty_buy
-000189d0: 222c 2022 6261 6e6b 6e69 6674 795f 6275  ", "banknifty_bu
-000189e0: 7922 2c20 226e 6966 7479 5f73 656c 6c22  y", "nifty_sell"
-000189f0: 2c20 2262 616e 6b6e 6966 7479 5f73 656c  , "banknifty_sel
-00018a00: 6c22 5d0d 0a0d 0a20 2020 2020 2020 2064  l"]....        d
-00018a10: 6174 615f 7475 706c 6520 3d20 6665 7463  ata_tuple = fetc
-00018a20: 6865 722e 6665 7463 6846 6976 6545 6d61  her.fetchFiveEma
-00018a30: 4461 7461 2829 0d0a 2020 2020 2020 2020  Data()..        
-00018a40: 666f 7220 636e 7420 696e 2072 616e 6765  for cnt in range
-00018a50: 286c 656e 2864 6174 615f 7475 706c 6529  (len(data_tuple)
-00018a60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00018a70: 6420 3d20 6461 7461 5f74 7570 6c65 5b63  d = data_tuple[c
-00018a80: 6e74 5d0d 0a20 2020 2020 2020 2020 2020  nt]..           
-00018a90: 2064 5b22 3545 4d41 225d 203d 2070 6b74   d["5EMA"] = pkt
-00018aa0: 616c 6962 2e45 4d41 2864 5b22 436c 6f73  alib.EMA(d["Clos
-00018ab0: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-00018ac0: 3529 0d0a 2020 2020 2020 2020 2020 2020  5)..            
-00018ad0: 6420 3d20 645b 636f 6c5f 6e61 6d65 735d  d = d[col_names]
-00018ae0: 0d0a 2020 2020 2020 2020 2020 2020 6420  ..            d 
-00018af0: 3d20 642e 6472 6f70 6e61 2829 2e72 6f75  = d.dropna().rou
-00018b00: 6e64 2832 290d 0a0d 0a20 2020 2020 2020  nd(2)....       
-00018b10: 2020 2020 2077 6974 6820 5375 7070 7265       with Suppre
-00018b20: 7373 4f75 7470 7574 2873 7570 7072 6573  ssOutput(suppres
-00018b30: 735f 7374 6465 7272 3d54 7275 652c 2073  s_stderr=True, s
-00018b40: 7570 7072 6573 735f 7374 646f 7574 3d54  uppress_stdout=T
-00018b50: 7275 6529 3a0d 0a20 2020 2020 2020 2020  rue):..         
-00018b60: 2020 2020 2020 2069 6620 2273 656c 6c22         if "sell"
-00018b70: 2069 6e20 6461 7461 5f6c 6973 745b 636e   in data_list[cn
-00018b80: 745d 3a0d 0a20 2020 2020 2020 2020 2020  t]:..           
-00018b90: 2020 2020 2020 2020 2073 7472 6563 6865           streche
-00018ba0: 6420 3d20 645b 2864 2e4c 6f77 203e 2064  d = d[(d.Low > d
-00018bb0: 5b22 3545 4d41 225d 2920 2620 2864 2e4c  ["5EMA"]) & (d.L
-00018bc0: 6f77 202d 2064 5b22 3545 4d41 225d 203e  ow - d["5EMA"] >
-00018bd0: 2030 2e35 295d 0d0a 2020 2020 2020 2020   0.5)]..        
-00018be0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-00018bf0: 6368 6564 5b22 534c 225d 203d 2073 7472  ched["SL"] = str
-00018c00: 6563 6865 642e 4869 6768 0d0a 2020 2020  eched.High..    
-00018c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c20: 7661 6c69 6461 7465 203d 2064 5b0d 0a20  validate = d[.. 
-00018c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c40: 2020 2020 2020 2028 642e 4c6f 772e 7368         (d.Low.sh
-00018c50: 6966 7428 3129 203e 2064 5b22 3545 4d41  ift(1) > d["5EMA
-00018c60: 225d 2e73 6869 6674 2831 2929 0d0a 2020  "].shift(1))..  
-00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c80: 2020 2020 2020 2620 2864 2e4c 6f77 2e73        & (d.Low.s
-00018c90: 6869 6674 2831 2920 2d20 645b 2235 454d  hift(1) - d["5EM
-00018ca0: 4122 5d2e 7368 6966 7428 3129 203e 2030  A"].shift(1) > 0
-00018cb0: 2e35 290d 0a20 2020 2020 2020 2020 2020  .5)..           
-00018cc0: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 6f6c 645f 696e 6465 7820 3d20 7661 6c69  old_index = vali
-00018cf0: 6461 7465 2e69 6e64 6578 0d0a 2020 2020  date.index..    
-00018d00: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00018d10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018d20: 2020 2020 2020 206d 6173 6b20 3d20 2864         mask = (d
-00018d30: 2e48 6967 6820 3c20 645b 2235 454d 4122  .High < d["5EMA"
-00018d40: 5d29 2026 2028 645b 2235 454d 4122 5d20  ]) & (d["5EMA"] 
-00018d50: 2d20 642e 4869 6768 203e 2030 2e35 2920  - d.High > 0.5) 
-00018d60: 2023 2042 7579 0d0a 2020 2020 2020 2020   # Buy..        
-00018d70: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-00018d80: 6368 6564 203d 2064 5b6d 6173 6b5d 0d0a  ched = d[mask]..
+00016970: 206c 6174 6573 745f 6d66 6461 7465 203d   latest_mfdate =
+00016980: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
+00016990: 6d65 2e66 726f 6d74 696d 6573 7461 6d70  me.fromtimestamp
+000169a0: 286c 6174 6573 745f 6d66 6461 7465 292e  (latest_mfdate).
+000169b0: 7374 7266 7469 6d65 2827 2559 2d25 6d2d  strftime('%Y-%m-
+000169c0: 2564 2729 0d0a 2020 2020 2020 2020 2020  %d')..          
+000169d0: 2020 2020 2020 6578 6365 7074 2028 4b65        except (Ke
+000169e0: 7945 7272 6f72 2c49 6e64 6578 4572 726f  yError,IndexErro
+000169f0: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
+00016a00: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
+00016a10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00016a20: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00016a30: 2020 2020 2020 2020 206c 6174 6573 745f           latest_
+00016a40: 696e 7374 6461 7465 203d 2068 6f73 7444  instdate = hostD
+00016a50: 6174 612e 6c6f 635b 686f 7374 4461 7461  ata.loc[hostData
+00016a60: 2e69 6e64 6578 5b2d 315d 2c22 4649 495f  .index[-1],"FII_
+00016a70: 4461 7465 225d 0d0a 2020 2020 2020 2020  Date"]..        
+00016a80: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00016a90: 7369 6e73 7461 6e63 6528 6c61 7465 7374  sinstance(latest
+00016aa0: 5f69 6e73 7464 6174 652c 2066 6c6f 6174  _instdate, float
+00016ab0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016ac0: 2020 2020 2020 2020 2020 2020 6c61 7465              late
+00016ad0: 7374 5f69 6e73 7464 6174 6520 3d20 6461  st_instdate = da
+00016ae0: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00016af0: 6672 6f6d 7469 6d65 7374 616d 7028 6c61  fromtimestamp(la
+00016b00: 7465 7374 5f69 6e73 7464 6174 6529 2e73  test_instdate).s
+00016b10: 7472 6674 696d 6528 2725 592d 256d 2d25  trftime('%Y-%m-%
+00016b20: 6427 290d 0a20 2020 2020 2020 2020 2020  d')..           
+00016b30: 2020 2020 2065 7863 6570 7420 284b 6579       except (Key
+00016b40: 4572 726f 722c 496e 6465 7845 7272 6f72  Error,IndexError
+00016b50: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016b60: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+00016b70: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016b80: 206c 6174 6573 745f 6d66 6461 7465 2069   latest_mfdate i
+00016b90: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00016ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bb0: 2073 6176 6564 5f6d 6664 6174 6520 3d20   saved_mfdate = 
+00016bc0: 504b 4461 7465 5574 696c 6974 6965 732e  PKDateUtilities.
+00016bd0: 6461 7465 4672 6f6d 596d 6453 7472 696e  dateFromYmdStrin
+00016be0: 6728 6c61 7465 7374 5f6d 6664 6174 652e  g(latest_mfdate.
+00016bf0: 7370 6c69 7428 2254 2229 5b30 5d29 0d0a  split("T")[0])..
+00016c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c10: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00016c20: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00016c30: 5f6d 6664 6174 6520 3d20 6c61 7374 4461  _mfdate = lastDa
+00016c40: 794c 6173 744d 6f6e 7468 202d 2064 6174  yLastMonth - dat
+00016c50: 6574 696d 652e 7469 6d65 6465 6c74 6128  etime.timedelta(
+00016c60: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+00016c70: 2020 2020 6966 206c 6174 6573 745f 696e      if latest_in
+00016c80: 7374 6461 7465 2069 7320 6e6f 7420 4e6f  stdate is not No
+00016c90: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00016ca0: 2020 2020 2020 2020 2073 6176 6564 5f69           saved_i
+00016cb0: 6e73 7464 6174 6520 3d20 504b 4461 7465  nstdate = PKDate
+00016cc0: 5574 696c 6974 6965 732e 6461 7465 4672  Utilities.dateFr
+00016cd0: 6f6d 596d 6453 7472 696e 6728 6c61 7465  omYmdString(late
+00016ce0: 7374 5f69 6e73 7464 6174 652e 7370 6c69  st_instdate.spli
+00016cf0: 7428 2254 2229 5b30 5d29 0d0a 2020 2020  t("T")[0])..    
+00016d00: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00016d10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00016d20: 2020 2020 2020 2073 6176 6564 5f69 6e73         saved_ins
+00016d30: 7464 6174 6520 3d20 6c61 7374 4461 794c  tdate = lastDayL
+00016d40: 6173 744d 6f6e 7468 202d 2064 6174 6574  astMonth - datet
+00016d50: 696d 652e 7469 6d65 6465 6c74 6128 3129  ime.timedelta(1)
+00016d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016d70: 2020 746f 6461 7920 3d20 504b 4461 7465    today = PKDate
+00016d80: 5574 696c 6974 6965 732e 6375 7272 656e  Utilities.curren
+00016d90: 7444 6174 6554 696d 6528 290d 0a20 2020  tDateTime()..   
+00016da0: 2020 2020 2020 2020 2020 2020 206e 6565               nee
+00016db0: 6473 4672 6573 6855 7064 6174 6520 3d20  dsFreshUpdate = 
+00016dc0: 2873 6176 6564 5f6d 6664 6174 652e 6461  (saved_mfdate.da
+00016dd0: 7465 2829 203c 206c 6173 7444 6179 4c61  te() < lastDayLa
+00016de0: 7374 4d6f 6e74 682e 6461 7465 2829 2920  stMonth.date()) 
+00016df0: 616e 6420 2873 6176 6564 5f69 6e73 7464  and (saved_instd
+00016e00: 6174 652e 6461 7465 2829 203c 206c 6173  ate.date() < las
+00016e10: 7444 6179 4c61 7374 4d6f 6e74 682e 6461  tDayLastMonth.da
+00016e20: 7465 2829 290d 0a20 2020 2020 2020 2020  te())..         
+00016e30: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00016e40: 2020 2020 2020 2020 2020 6e65 6564 7346            needsF
+00016e50: 7265 7368 5570 6461 7465 203d 2054 7275  reshUpdate = Tru
+00016e60: 650d 0a0d 0a20 2020 2020 2020 2069 6620  e....        if 
+00016e70: 6e65 6564 7346 7265 7368 5570 6461 7465  needsFreshUpdate
+00016e80: 2061 6e64 2066 6f72 6365 3a0d 0a20 2020   and force:..   
+00016e90: 2020 2020 2020 2020 206e 6574 4368 616e           netChan
+00016ea0: 6765 4d46 2c20 6e65 7443 6861 6e67 6549  geMF, netChangeI
+00016eb0: 6e73 742c 206c 6174 6573 745f 6d66 6461  nst, latest_mfda
+00016ec0: 7465 2c20 6c61 7465 7374 5f69 6e73 7464  te, latest_instd
+00016ed0: 6174 6520 3d20 7365 6c66 2e67 6574 4672  ate = self.getFr
+00016ee0: 6573 684d 4649 5374 6174 7573 2873 746f  eshMFIStatus(sto
+00016ef0: 636b 2c65 7863 6861 6e67 654e 616d 653d  ck,exchangeName=
+00016f00: 6578 6368 616e 6765 4e61 6d65 290d 0a20  exchangeName).. 
+00016f10: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
+00016f20: 7443 6861 6e67 654d 4620 6973 206e 6f74  tChangeMF is not
+00016f30: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00016f40: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f60: 2020 686f 7374 4461 7461 2e6c 6f63 5b68    hostData.loc[h
+00016f70: 6f73 7444 6174 612e 696e 6465 785b 2d31  ostData.index[-1
+00016f80: 5d2c 224d 4622 5d20 3d20 6e65 7443 6861  ],"MF"] = netCha
+00016f90: 6e67 654d 460d 0a20 2020 2020 2020 2020  ngeMF..         
+00016fa0: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
+00016fb0: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
+00016fc0: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
+00016fd0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00016fe0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00016ff0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017000: 2020 206e 6574 4368 616e 6765 4d46 203d     netChangeMF =
+00017010: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+00017020: 6966 206c 6174 6573 745f 6d66 6461 7465  if latest_mfdate
+00017030: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00017040: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00017050: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00017060: 2020 2020 2020 2020 2068 6f73 7444 6174           hostDat
+00017070: 612e 6c6f 635b 686f 7374 4461 7461 2e69  a.loc[hostData.i
+00017080: 6e64 6578 5b2d 315d 2c22 4d46 5f44 6174  ndex[-1],"MF_Dat
+00017090: 6522 5d20 3d20 6c61 7465 7374 5f6d 6664  e"] = latest_mfd
+000170a0: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
+000170b0: 2020 2020 2065 7863 6570 7420 284b 6579       except (Key
+000170c0: 4572 726f 722c 496e 6465 7845 7272 6f72  Error,IndexError
+000170d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000170e0: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+000170f0: 2020 2020 2020 2020 2020 6966 206e 6574            if net
+00017100: 4368 616e 6765 496e 7374 2069 7320 6e6f  ChangeInst is no
+00017110: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00017120: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00017130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017140: 2020 2068 6f73 7444 6174 612e 6c6f 635b     hostData.loc[
+00017150: 686f 7374 4461 7461 2e69 6e64 6578 5b2d  hostData.index[-
+00017160: 315d 2c22 4649 4922 5d20 3d20 6e65 7443  1],"FII"] = netC
+00017170: 6861 6e67 6549 6e73 740d 0a20 2020 2020  hangeInst..     
+00017180: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00017190: 7420 284b 6579 4572 726f 722c 496e 6465  t (KeyError,Inde
+000171a0: 7845 7272 6f72 293a 0d0a 2020 2020 2020  xError):..      
+000171b0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+000171c0: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
+000171d0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000171e0: 2020 2020 2020 206e 6574 4368 616e 6765         netChange
+000171f0: 496e 7374 203d 2030 0d0a 2020 2020 2020  Inst = 0..      
+00017200: 2020 2020 2020 6966 206c 6174 6573 745f        if latest_
+00017210: 696e 7374 6461 7465 2069 7320 6e6f 7420  instdate is not 
+00017220: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00017230: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2068 6f73 7444 6174 612e 6c6f 635b 686f   hostData.loc[ho
+00017260: 7374 4461 7461 2e69 6e64 6578 5b2d 315d  stData.index[-1]
+00017270: 2c22 4649 495f 4461 7465 225d 203d 206c  ,"FII_Date"] = l
+00017280: 6174 6573 745f 696e 7374 6461 7465 0d0a  atest_instdate..
+00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172a0: 6578 6365 7074 2028 4b65 7945 7272 6f72  except (KeyError
+000172b0: 2c49 6e64 6578 4572 726f 7229 3a0d 0a20  ,IndexError):.. 
+000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172d0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+000172e0: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
+000172f0: 6820 3d20 6c61 7374 4461 794c 6173 744d  h = lastDayLastM
+00017300: 6f6e 7468 2e73 7472 6674 696d 6528 2225  onth.strftime("%
+00017310: 592d 256d 2d25 6454 3030 3a30 303a 3030  Y-%m-%dT00:00:00
+00017320: 2e30 3030 2229 0d0a 2020 2020 2020 2020  .000")..        
+00017330: 6966 206f 6e6c 794d 463a 0d0a 2020 2020  if onlyMF:..    
+00017340: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00017350: 6574 4368 616e 6765 4d46 0d0a 2020 2020  etChangeMF..    
+00017360: 2020 2020 6966 206c 6174 6573 745f 696e      if latest_in
+00017370: 7374 6461 7465 203d 3d20 6c61 7465 7374  stdate == latest
+00017380: 5f6d 6664 6174 653a 0d0a 2020 2020 2020  _mfdate:..      
+00017390: 2020 2020 2020 7265 7475 726e 2028 6e65        return (ne
+000173a0: 7443 6861 6e67 654d 4620 2b20 6e65 7443  tChangeMF + netC
+000173b0: 6861 6e67 6549 6e73 7429 0d0a 2020 2020  hangeInst)..    
+000173c0: 2020 2020 656c 6966 206c 6174 6573 745f      elif latest_
+000173d0: 6d66 6461 7465 203d 3d20 6c61 7374 4461  mfdate == lastDa
+000173e0: 794c 6173 744d 6f6e 7468 3a0d 0a20 2020  yLastMonth:..   
+000173f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00017400: 6e65 7443 6861 6e67 654d 460d 0a20 2020  netChangeMF..   
+00017410: 2020 2020 2065 6c69 6620 6c61 7465 7374       elif latest
+00017420: 5f69 6e73 7464 6174 6520 3d3d 206c 6173  _instdate == las
+00017430: 7444 6179 4c61 7374 4d6f 6e74 683a 0d0a  tDayLastMonth:..
+00017440: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017450: 726e 206e 6574 4368 616e 6765 496e 7374  rn netChangeInst
+00017460: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00017470: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
+00017480: 696e 6420 7468 6520 6c61 7465 7374 2064  ind the latest d
+00017490: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
+000174a0: 2069 6620 6c61 7465 7374 5f6d 6664 6174   if latest_mfdat
+000174b0: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+000174c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174d0: 6c61 7465 7374 5f6d 6664 6174 6520 3d20  latest_mfdate = 
+000174e0: 504b 4461 7465 5574 696c 6974 6965 732e  PKDateUtilities.
+000174f0: 6461 7465 4672 6f6d 596d 6453 7472 696e  dateFromYmdStrin
+00017500: 6728 6c61 7465 7374 5f6d 6664 6174 652e  g(latest_mfdate.
+00017510: 7370 6c69 7428 2254 2229 5b30 5d29 0d0a  split("T")[0])..
+00017520: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00017530: 6174 6573 745f 696e 7374 6461 7465 2069  atest_instdate i
+00017540: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00017550: 2020 2020 2020 2020 2020 2020 206c 6174               lat
+00017560: 6573 745f 696e 7374 6461 7465 203d 2050  est_instdate = P
+00017570: 4b44 6174 6555 7469 6c69 7469 6573 2e64  KDateUtilities.d
+00017580: 6174 6546 726f 6d59 6d64 5374 7269 6e67  ateFromYmdString
+00017590: 286c 6174 6573 745f 696e 7374 6461 7465  (latest_instdate
+000175a0: 2e73 706c 6974 2822 5422 295b 305d 290d  .split("T")[0]).
+000175b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000175c0: 7572 6e20 6e65 7443 6861 6e67 654d 4620  urn netChangeMF 
+000175d0: 6966 2028 286c 6174 6573 745f 6d66 6461  if ((latest_mfda
+000175e0: 7465 2069 7320 6e6f 7420 4e6f 6e65 2920  te is not None) 
+000175f0: 616e 6420 6c61 7465 7374 5f6d 6664 6174  and latest_mfdat
+00017600: 6520 3e20 286c 6174 6573 745f 696e 7374  e > (latest_inst
+00017610: 6461 7465 2069 6620 6c61 7465 7374 5f69  date if latest_i
+00017620: 6e73 7464 6174 6520 6973 206e 6f74 204e  nstdate is not N
+00017630: 6f6e 6520 656c 7365 2028 6c61 7465 7374  one else (latest
+00017640: 5f6d 6664 6174 6520 2d20 6461 7465 7469  _mfdate - dateti
+00017650: 6d65 2e74 696d 6564 656c 7461 2831 2929  me.timedelta(1))
+00017660: 2929 2065 6c73 6520 6e65 7443 6861 6e67  )) else netChang
+00017670: 6549 6e73 740d 0a0d 0a20 2020 2064 6566  eInst....    def
+00017680: 2067 6574 4672 6573 684d 4649 5374 6174   getFreshMFIStat
+00017690: 7573 2873 656c 662c 2073 746f 636b 2c65  us(self, stock,e
+000176a0: 7863 6861 6e67 654e 616d 653d 2249 4e44  xchangeName="IND
+000176b0: 4941 2229 3a0d 0a20 2020 2020 2020 2063  IA"):..        c
+000176c0: 6861 6e67 6553 7461 7475 7344 6174 614d  hangeStatusDataM
+000176d0: 4620 3d20 4e6f 6e65 0d0a 2020 2020 2020  F = None..      
+000176e0: 2020 6368 616e 6765 5374 6174 7573 4461    changeStatusDa
+000176f0: 7461 496e 7374 203d 204e 6f6e 650d 0a20  taInst = None.. 
+00017700: 2020 2020 2020 206e 6574 4368 616e 6765         netChange
+00017710: 4d46 203d 2030 0d0a 2020 2020 2020 2020  MF = 0..        
+00017720: 6e65 7443 6861 6e67 6549 6e73 7420 3d20  netChangeInst = 
+00017730: 300d 0a20 2020 2020 2020 206c 6174 6573  0..        lates
+00017740: 745f 6d66 6461 7465 203d 204e 6f6e 650d  t_mfdate = None.
+00017750: 0a20 2020 2020 2020 206c 6174 6573 745f  .        latest_
+00017760: 696e 7374 6461 7465 203d 204e 6f6e 650d  instdate = None.
+00017770: 0a20 2020 2020 2020 2073 6563 7572 6974  .        securit
+00017780: 7920 3d20 4e6f 6e65 0d0a 2020 2020 2020  y = None..      
+00017790: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+000177a0: 2020 2020 7769 7468 2053 7570 7072 6573      with Suppres
+000177b0: 734f 7574 7075 7428 7375 7070 7265 7373  sOutput(suppress
+000177c0: 5f73 7464 6572 723d 5472 7565 2c20 7375  _stderr=True, su
+000177d0: 7070 7265 7373 5f73 7464 6f75 743d 5472  ppress_stdout=Tr
+000177e0: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
+000177f0: 2020 2020 2020 7365 6375 7269 7479 203d        security =
+00017800: 2053 746f 636b 2873 746f 636b 2c65 7863   Stock(stock,exc
+00017810: 6861 6e67 653d 6578 6368 616e 6765 4e61  hange=exchangeNa
+00017820: 6d65 290d 0a20 2020 2020 2020 2065 7863  me)..        exc
+00017830: 6570 7420 5661 6c75 6545 7272 6f72 3a0d  ept ValueError:.
+00017840: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+00017850: 6520 6469 6420 6e6f 7420 6669 6e64 2074  e did not find t
+00017860: 6865 2073 746f 636b 3f20 4974 2773 206f  he stock? It's o
+00017870: 6b61 792e 204d 6f76 6520 6f6e 2074 6f20  kay. Move on to 
+00017880: 7468 6520 6e65 7874 206f 6e65 2e0d 0a20  the next one... 
+00017890: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+000178a0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000178b0: 2854 696d 656f 7574 4572 726f 722c 2043  (TimeoutError, C
+000178c0: 6f6e 6e65 6374 696f 6e45 7272 6f72 2920  onnectionError) 
+000178d0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
+000178e0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+000178f0: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+00017900: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
+00017910: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00017920: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00017930: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00017940: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00017950: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
+00017960: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
+00017970: 6e66 6f3d 5472 7565 290d 0a20 2020 2020  nfo=True)..     
+00017980: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
+00017990: 2020 2020 2069 6620 7365 6375 7269 7479       if security
+000179a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+000179b0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+000179c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000179d0: 2077 6974 6820 5375 7070 7265 7373 4f75   with SuppressOu
+000179e0: 7470 7574 2873 7570 7072 6573 735f 7374  tput(suppress_st
+000179f0: 6465 7272 3d54 7275 652c 2073 7570 7072  derr=True, suppr
+00017a00: 6573 735f 7374 646f 7574 3d54 7275 6529  ess_stdout=True)
+00017a10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017a20: 2020 2020 2020 2063 6861 6e67 6553 7461         changeSta
+00017a30: 7475 7352 6f77 734d 4620 3d20 7365 6375  tusRowsMF = secu
+00017a40: 7269 7479 2e6d 7574 7561 6c46 756e 644f  rity.mutualFundO
+00017a50: 776e 6572 7368 6970 2874 6f70 3d35 290d  wnership(top=5).
+00017a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017a70: 2020 2020 2063 6861 6e67 6553 7461 7475       changeStatu
+00017a80: 7352 6f77 7349 6e73 7420 3d20 7365 6375  sRowsInst = secu
+00017a90: 7269 7479 2e69 6e73 7469 7475 7469 6f6e  rity.institution
+00017aa0: 4f77 6e65 7273 6869 7028 746f 703d 3529  Ownership(top=5)
+00017ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017ac0: 2020 2020 2020 6368 616e 6765 5374 6174        changeStat
+00017ad0: 7573 4461 7461 4d46 203d 2073 6563 7572  usDataMF = secur
+00017ae0: 6974 792e 6d75 7475 616c 4675 6e64 4649  ity.mutualFundFI
+00017af0: 4943 6861 6e67 6544 6174 6128 6368 616e  IChangeData(chan
+00017b00: 6765 5374 6174 7573 526f 7773 4d46 290d  geStatusRowsMF).
+00017b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b20: 2020 2020 2063 6861 6e67 6553 7461 7475       changeStatu
+00017b30: 7344 6174 6149 6e73 7420 3d20 7365 6375  sDataInst = secu
+00017b40: 7269 7479 2e6d 7574 7561 6c46 756e 6446  rity.mutualFundF
+00017b50: 4949 4368 616e 6765 4461 7461 2863 6861  IIChangeData(cha
+00017b60: 6e67 6553 7461 7475 7352 6f77 7349 6e73  ngeStatusRowsIns
+00017b70: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00017b80: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00017b90: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00017ba0: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+00017bb0: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+00017bc0: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+00017bd0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+00017be0: 2020 2020 2023 2054 7970 6545 7272 6f72       # TypeError
+00017bf0: 206f 7220 436f 6e6e 6563 7469 6f6e 4572   or ConnectionEr
+00017c00: 726f 7220 6265 6361 7573 6520 7765 2063  ror because we c
+00017c10: 6f75 6c64 206e 6f74 2066 696e 6420 7468  ould not find th
+00017c20: 6520 7374 6f63 6b20 6f72 204d 4649 2064  e stock or MFI d
+00017c30: 6174 6120 6973 6e27 7420 6176 6169 6c61  ata isn't availa
+00017c40: 626c 653f 0d0a 2020 2020 2020 2020 2020  ble?..          
+00017c50: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+00017c60: 2020 2020 2020 2020 6c61 7374 4461 794c          lastDayL
+00017c70: 6173 744d 6f6e 7468 203d 2050 4b44 6174  astMonth = PKDat
+00017c80: 6555 7469 6c69 7469 6573 2e6c 6173 745f  eUtilities.last_
+00017c90: 6461 795f 6f66 5f70 7265 7669 6f75 735f  day_of_previous_
+00017ca0: 6d6f 6e74 6828 504b 4461 7465 5574 696c  month(PKDateUtil
+00017cb0: 6974 6965 732e 6375 7272 656e 7444 6174  ities.currentDat
+00017cc0: 6554 696d 6528 2929 0d0a 2020 2020 2020  eTime())..      
+00017cd0: 2020 2020 2020 6c61 7374 4461 794c 6173        lastDayLas
+00017ce0: 744d 6f6e 7468 203d 206c 6173 7444 6179  tMonth = lastDay
+00017cf0: 4c61 7374 4d6f 6e74 682e 7374 7266 7469  LastMonth.strfti
+00017d00: 6d65 2822 2559 2d25 6d2d 2564 5430 303a  me("%Y-%m-%dT00:
+00017d10: 3030 3a30 302e 3030 3022 290d 0a20 2020  00:00.000")..   
+00017d20: 2020 2020 2020 2020 2069 6620 6368 616e           if chan
+00017d30: 6765 5374 6174 7573 4461 7461 4d46 2069  geStatusDataMF i
+00017d40: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
+00017d50: 656e 2863 6861 6e67 6553 7461 7475 7344  en(changeStatusD
+00017d60: 6174 614d 4629 203e 2030 3a0d 0a20 2020  ataMF) > 0:..   
+00017d70: 2020 2020 2020 2020 2020 2020 2064 665f               df_
+00017d80: 6772 6f75 7065 644d 4620 3d20 6368 616e  groupedMF = chan
+00017d90: 6765 5374 6174 7573 4461 7461 4d46 2e67  geStatusDataMF.g
+00017da0: 726f 7570 6279 2822 6461 7465 222c 2073  roupby("date", s
+00017db0: 6f72 743d 4661 6c73 6529 0d0a 2020 2020  ort=False)..    
+00017dc0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00017dd0: 6d66 6461 7465 2c20 6466 5f67 726f 7570  mfdate, df_group
+00017de0: 4d46 2069 6e20 6466 5f67 726f 7570 6564  MF in df_grouped
+00017df0: 4d46 3a0d 0a20 2020 2020 2020 2020 2020  MF:..           
+00017e00: 2020 2020 2020 2020 206e 6574 4368 616e           netChan
+00017e10: 6765 4d46 203d 2064 665f 6772 6f75 704d  geMF = df_groupM
+00017e20: 465b 2263 6861 6e67 6541 6d6f 756e 7422  F["changeAmount"
+00017e30: 5d2e 7375 6d28 290d 0a20 2020 2020 2020  ].sum()..       
+00017e40: 2020 2020 2020 2020 2020 2020 206c 6174               lat
+00017e50: 6573 745f 6d66 6461 7465 203d 206d 6664  est_mfdate = mfd
+00017e60: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
+00017e70: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
+00017e80: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00017e90: 6861 6e67 6553 7461 7475 7344 6174 6149  hangeStatusDataI
+00017ea0: 6e73 7420 6973 206e 6f74 204e 6f6e 6520  nst is not None 
+00017eb0: 616e 6420 6c65 6e28 6368 616e 6765 5374  and len(changeSt
+00017ec0: 6174 7573 4461 7461 496e 7374 2920 3e20  atusDataInst) > 
+00017ed0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00017ee0: 2020 2020 6466 5f67 726f 7570 6564 496e      df_groupedIn
+00017ef0: 7374 203d 2063 6861 6e67 6553 7461 7475  st = changeStatu
+00017f00: 7344 6174 6149 6e73 742e 6772 6f75 7062  sDataInst.groupb
+00017f10: 7928 2264 6174 6522 2c20 736f 7274 3d46  y("date", sort=F
+00017f20: 616c 7365 290d 0a20 2020 2020 2020 2020  alse)..         
+00017f30: 2020 2020 2020 2066 6f72 2069 6e73 7464         for instd
+00017f40: 6174 652c 2064 665f 6772 6f75 7049 6e73  ate, df_groupIns
+00017f50: 7420 696e 2064 665f 6772 6f75 7065 6449  t in df_groupedI
+00017f60: 6e73 743a 0d0a 2020 2020 2020 2020 2020  nst:..          
+00017f70: 2020 2020 2020 2020 2020 6966 2028 6c61            if (la
+00017f80: 7465 7374 5f6d 6664 6174 6520 6973 206e  test_mfdate is n
+00017f90: 6f74 204e 6f6e 6520 616e 6420 6c61 7465  ot None and late
+00017fa0: 7374 5f6d 6664 6174 6520 3d3d 2069 6e73  st_mfdate == ins
+00017fb0: 7464 6174 6529 206f 7220 286c 6174 6573  tdate) or (lates
+00017fc0: 745f 6d66 6461 7465 2069 7320 4e6f 6e65  t_mfdate is None
+00017fd0: 2920 6f72 2028 696e 7374 6461 7465 203d  ) or (instdate =
+00017fe0: 3d20 6c61 7374 4461 794c 6173 744d 6f6e  = lastDayLastMon
+00017ff0: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+00018000: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00018010: 7443 6861 6e67 6549 6e73 7420 3d20 6466  tChangeInst = df
+00018020: 5f67 726f 7570 496e 7374 5b22 6368 616e  _groupInst["chan
+00018030: 6765 416d 6f75 6e74 225d 2e73 756d 2829  geAmount"].sum()
+00018040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018050: 2020 2020 2020 2020 2020 6c61 7465 7374            latest
+00018060: 5f69 6e73 7464 6174 6520 3d20 696e 7374  _instdate = inst
+00018070: 6461 7465 0d0a 2020 2020 2020 2020 2020  date..          
+00018080: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
+00018090: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000180a0: 6e65 7443 6861 6e67 654d 462c 6e65 7443  netChangeMF,netC
+000180b0: 6861 6e67 6549 6e73 742c 6c61 7465 7374  hangeInst,latest
+000180c0: 5f6d 6664 6174 652c 6c61 7465 7374 5f69  _mfdate,latest_i
+000180d0: 6e73 7464 6174 650d 0a0d 0a0d 0a20 2020  nstdate......   
+000180e0: 2064 6566 2067 6574 4e69 6674 7950 7265   def getNiftyPre
+000180f0: 6469 6374 696f 6e28 7365 6c66 2c20 6466  diction(self, df
+00018100: 293a 0d0a 2020 2020 2020 2020 696d 706f  ):..        impo
+00018110: 7274 2077 6172 6e69 6e67 730d 0a0d 0a20  rt warnings.... 
+00018120: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+00018130: 6669 6c74 6572 7761 726e 696e 6773 2822  filterwarnings("
+00018140: 6967 6e6f 7265 2229 0d0a 2020 2020 2020  ignore")..      
+00018150: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+00018160: 2829 0d0a 2020 2020 2020 2020 6d6f 6465  ()..        mode
+00018170: 6c2c 2070 6b6c 203d 2055 7469 6c69 7479  l, pkl = Utility
+00018180: 2e74 6f6f 6c73 2e67 6574 4e69 6674 794d  .tools.getNiftyM
+00018190: 6f64 656c 2829 0d0a 2020 2020 2020 2020  odel()..        
+000181a0: 6966 206d 6f64 656c 2069 7320 4e6f 6e65  if model is None
+000181b0: 206f 7220 706b 6c20 6973 204e 6f6e 653a   or pkl is None:
+000181c0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000181d0: 7475 726e 2030 2c20 2255 6e6b 6e6f 776e  turn 0, "Unknown
+000181e0: 222c 2022 556e 6b6e 6f77 6e22 0d0a 2020  ", "Unknown"..  
+000181f0: 2020 2020 2020 7769 7468 2053 7570 7072        with Suppr
+00018200: 6573 734f 7574 7075 7428 7375 7070 7265  essOutput(suppre
+00018210: 7373 5f73 7464 6572 723d 5472 7565 2c20  ss_stderr=True, 
+00018220: 7375 7070 7265 7373 5f73 7464 6f75 743d  suppress_stdout=
+00018230: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
+00018240: 2020 2020 6461 7461 203d 2064 6174 615b      data = data[
+00018250: 706b 6c5b 2263 6f6c 756d 6e73 225d 5d0d  pkl["columns"]].
+00018260: 0a20 2020 2020 2020 2020 2020 2023 2323  .            ###
+00018270: 2076 3220 5072 6570 726f 6365 7373 696e   v2 Preprocessin
+00018280: 670d 0a20 2020 2020 2020 2020 2020 2064  g..            d
+00018290: 6174 615b 2248 6967 6822 5d20 3d20 6461  ata["High"] = da
+000182a0: 7461 5b22 4869 6768 225d 2e70 6374 5f63  ta["High"].pct_c
+000182b0: 6861 6e67 6528 2920 2a20 3130 300d 0a20  hange() * 100.. 
+000182c0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+000182d0: 224c 6f77 225d 203d 2064 6174 615b 224c  "Low"] = data["L
+000182e0: 6f77 225d 2e70 6374 5f63 6861 6e67 6528  ow"].pct_change(
+000182f0: 2920 2a20 3130 300d 0a20 2020 2020 2020  ) * 100..       
+00018300: 2020 2020 2064 6174 615b 224f 7065 6e22       data["Open"
+00018310: 5d20 3d20 6461 7461 5b22 4f70 656e 225d  ] = data["Open"]
+00018320: 2e70 6374 5f63 6861 6e67 6528 2920 2a20  .pct_change() * 
+00018330: 3130 300d 0a20 2020 2020 2020 2020 2020  100..           
+00018340: 2064 6174 615b 2243 6c6f 7365 225d 203d   data["Close"] =
+00018350: 2064 6174 615b 2243 6c6f 7365 225d 2e70   data["Close"].p
+00018360: 6374 5f63 6861 6e67 6528 2920 2a20 3130  ct_change() * 10
+00018370: 300d 0a20 2020 2020 2020 2020 2020 2064  0..            d
+00018380: 6174 6120 3d20 6461 7461 2e69 6c6f 635b  ata = data.iloc[
+00018390: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
+000183a0: 2023 2323 0d0a 2020 2020 2020 2020 2020   ###..          
+000183b0: 2020 6461 7461 203d 2070 6b6c 5b22 7363    data = pkl["sc
+000183c0: 616c 6572 225d 2e74 7261 6e73 666f 726d  aler"].transform
+000183d0: 285b 6461 7461 5d29 0d0a 2020 2020 2020  ([data])..      
+000183e0: 2020 2020 2020 7769 7468 2053 7570 7072        with Suppr
+000183f0: 6573 734f 7574 7075 7428 7375 7070 7265  essOutput(suppre
+00018400: 7373 5f73 7464 6f75 743d 5472 7565 2c20  ss_stdout=True, 
+00018410: 7375 7070 7265 7373 5f73 7464 6572 723d  suppress_stderr=
+00018420: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
+00018430: 2020 2020 2020 2020 7072 6564 203d 206d          pred = m
+00018440: 6f64 656c 2e70 7265 6469 6374 2864 6174  odel.predict(dat
+00018450: 6129 5b30 5d0d 0a20 2020 2020 2020 2069  a)[0]..        i
+00018460: 6620 7072 6564 203e 2030 2e35 3a0d 0a20  f pred > 0.5:.. 
+00018470: 2020 2020 2020 2020 2020 206f 7574 5465             outTe
+00018480: 7874 203d 2022 4245 4152 4953 4822 0d0a  xt = "BEARISH"..
+00018490: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
+000184a0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+000184b0: 2020 2020 2063 6f6c 6f72 5465 7874 2e42       colorText.B
+000184c0: 4f4c 440d 0a20 2020 2020 2020 2020 2020  OLD..           
+000184d0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+000184e0: 2e46 4149 4c0d 0a20 2020 2020 2020 2020  .FAIL..         
+000184f0: 2020 2020 2020 202b 206f 7574 5465 7874         + outText
+00018500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018510: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+00018520: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+00018530: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+00018540: 4f4c 440d 0a20 2020 2020 2020 2020 2020  OLD..           
+00018550: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00018560: 7375 6720 3d20 2248 6f6c 6420 796f 7572  sug = "Hold your
+00018570: 2053 686f 7274 2070 6f73 6974 696f 6e21   Short position!
+00018580: 220d 0a20 2020 2020 2020 2065 6c73 653a  "..        else:
+00018590: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
+000185a0: 7454 6578 7420 3d20 2242 554c 4c49 5348  tText = "BULLISH
+000185b0: 220d 0a20 2020 2020 2020 2020 2020 206f  "..            o
+000185c0: 7574 203d 2028 0d0a 2020 2020 2020 2020  ut = (..        
+000185d0: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
+000185e0: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
+000185f0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00018600: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
+00018610: 2020 2020 2020 2020 2020 202b 206f 7574             + out
+00018620: 5465 7874 0d0a 2020 2020 2020 2020 2020  Text..          
+00018630: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00018640: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+00018650: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+00018660: 7874 2e42 4f4c 440d 0a20 2020 2020 2020  xt.BOLD..       
+00018670: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00018680: 2020 2020 7375 6720 3d20 2253 7461 7920      sug = "Stay 
+00018690: 4275 6c6c 6973 6821 220d 0a20 2020 2020  Bullish!"..     
+000186a0: 2020 2069 6620 504b 4461 7465 5574 696c     if PKDateUtil
+000186b0: 6974 6965 732e 6973 436c 6f73 696e 6748  ities.isClosingH
+000186c0: 6f75 7228 293a 0d0a 2020 2020 2020 2020  our():..        
+000186d0: 2020 2020 4f75 7470 7574 436f 6e74 726f      OutputContro
+000186e0: 6c73 2829 2e70 7269 6e74 4f75 7470 7574  ls().printOutput
+000186f0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00018700: 2020 2063 6f6c 6f72 5465 7874 2e42 4f4c     colorText.BOL
+00018710: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+00018720: 2020 202b 2063 6f6c 6f72 5465 7874 2e57     + colorText.W
+00018730: 4152 4e0d 0a20 2020 2020 2020 2020 2020  ARN..           
+00018740: 2020 2020 202b 2022 4e6f 7465 3a20 5468       + "Note: Th
+00018750: 6520 4149 2070 7265 6469 6374 696f 6e20  e AI prediction 
+00018760: 7368 6f75 6c64 2062 6520 6578 6563 7574  should be execut
+00018770: 6564 2041 6674 6572 2033 2050 4d20 6f72  ed After 3 PM or
+00018780: 204e 6561 7220 746f 2043 6c6f 7369 6e67   Near to Closing
+00018790: 2074 696d 6520 6173 2074 6865 2050 7265   time as the Pre
+000187a0: 6469 6374 696f 6e20 4163 6375 7261 6379  diction Accuracy
+000187b0: 2069 7320 6261 7365 6420 6f6e 2074 6865   is based on the
+000187c0: 2043 6c6f 7369 6e67 2070 7269 6365 2122   Closing price!"
+000187d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000187e0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+000187f0: 440d 0a20 2020 2020 2020 2020 2020 2029  D..            )
+00018800: 0d0a 2020 2020 2020 2020 7072 6564 6963  ..        predic
+00018810: 7469 6f6e 5465 7874 203d 2022 4d61 726b  tionText = "Mark
+00018820: 6574 206d 6179 204f 7065 6e20 7b7d 206e  et may Open {} n
+00018830: 6578 7420 6461 7921 207b 7d22 2e66 6f72  ext day! {}".for
+00018840: 6d61 7428 6f75 742c 2073 7567 290d 0a20  mat(out, sug).. 
+00018850: 2020 2020 2020 2073 7472 656e 6774 6854         strengthT
+00018860: 6578 7420 3d20 2250 726f 6261 6269 6c69  ext = "Probabili
+00018870: 7479 2f53 7472 656e 6774 6820 6f66 2050  ty/Strength of P
+00018880: 7265 6469 6374 696f 6e20 3d20 7b7d 2522  rediction = {}%"
+00018890: 2e66 6f72 6d61 7428 0d0a 2020 2020 2020  .format(..      
+000188a0: 2020 2020 2020 5574 696c 6974 792e 746f        Utility.to
+000188b0: 6f6c 732e 6765 7453 6967 6d6f 6964 436f  ols.getSigmoidCo
+000188c0: 6e66 6964 656e 6365 2870 7265 645b 305d  nfidence(pred[0]
+000188d0: 290d 0a20 2020 2020 2020 2029 0d0a 2020  )..        )..  
+000188e0: 2020 2020 2020 4f75 7470 7574 436f 6e74        OutputCont
+000188f0: 726f 6c73 2829 2e70 7269 6e74 4f75 7470  rols().printOutp
+00018900: 7574 280d 0a20 2020 2020 2020 2020 2020  ut(..           
+00018910: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
+00018920: 0a20 2020 2020 2020 2020 2020 202b 2063  .            + c
+00018930: 6f6c 6f72 5465 7874 2e42 4c55 450d 0a20  olorText.BLUE.. 
+00018940: 2020 2020 2020 2020 2020 202b 2022 5c6e             + "\n
+00018950: 220d 0a20 2020 2020 2020 2020 2020 202b  "..            +
+00018960: 2022 5b2b 5d20 4e69 6674 7920 4149 2050   "[+] Nifty AI P
+00018970: 7265 6469 6374 696f 6e20 2d3e 2022 0d0a  rediction -> "..
+00018980: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+00018990: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+000189a0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+000189b0: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
+000189c0: 2020 2020 2020 202b 2070 7265 6469 6374         + predict
+000189d0: 696f 6e54 6578 740d 0a20 2020 2020 2020  ionText..       
+000189e0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+000189f0: 2e45 4e44 0d0a 2020 2020 2020 2020 290d  .END..        ).
+00018a00: 0a20 2020 2020 2020 204f 7574 7075 7443  .        OutputC
+00018a10: 6f6e 7472 6f6c 7328 292e 7072 696e 744f  ontrols().printO
+00018a20: 7574 7075 7428 0d0a 2020 2020 2020 2020  utput(..        
+00018a30: 2020 2020 636f 6c6f 7254 6578 742e 424f      colorText.BO
+00018a40: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
+00018a50: 2b20 636f 6c6f 7254 6578 742e 424c 5545  + colorText.BLUE
+00018a60: 0d0a 2020 2020 2020 2020 2020 2020 2b20  ..            + 
+00018a70: 225c 6e22 0d0a 2020 2020 2020 2020 2020  "\n"..          
+00018a80: 2020 2b20 225b 2b5d 204e 6966 7479 2041    + "[+] Nifty A
+00018a90: 4920 5072 6564 6963 7469 6f6e 202d 3e20  I Prediction -> 
+00018aa0: 220d 0a20 2020 2020 2020 2020 2020 202b  "..            +
+00018ab0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
+00018ac0: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
+00018ad0: 7265 6e67 7468 5465 7874 0d0a 2020 2020  rengthText..    
+00018ae0: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+00018af0: 2072 6574 7572 6e20 7072 6564 2c20 7072   return pred, pr
+00018b00: 6564 6963 7469 6f6e 5465 7874 2e72 6570  edictionText.rep
+00018b10: 6c61 6365 286f 7574 2c20 6f75 7454 6578  lace(out, outTex
+00018b20: 7429 2c20 7374 7265 6e67 7468 5465 7874  t), strengthText
+00018b30: 0d0a 0d0a 2020 2020 6465 6620 6d6f 6e69  ....    def moni
+00018b40: 746f 7246 6976 6545 6d61 2873 656c 662c  torFiveEma(self,
+00018b50: 2066 6574 6368 6572 2c20 7265 7375 6c74   fetcher, result
+00018b60: 5f64 662c 206c 6173 745f 7369 676e 616c  _df, last_signal
+00018b70: 2c20 7269 736b 5f72 6577 6172 643d 3329  , risk_reward=3)
+00018b80: 3a0d 0a20 2020 2020 2020 2063 6f6c 5f6e  :..        col_n
+00018b90: 616d 6573 203d 205b 2248 6967 6822 2c20  ames = ["High", 
+00018ba0: 224c 6f77 222c 2022 436c 6f73 6522 2c20  "Low", "Close", 
+00018bb0: 2235 454d 4122 5d0d 0a20 2020 2020 2020  "5EMA"]..       
+00018bc0: 2064 6174 615f 6c69 7374 203d 205b 226e   data_list = ["n
+00018bd0: 6966 7479 5f62 7579 222c 2022 6261 6e6b  ifty_buy", "bank
+00018be0: 6e69 6674 795f 6275 7922 2c20 226e 6966  nifty_buy", "nif
+00018bf0: 7479 5f73 656c 6c22 2c20 2262 616e 6b6e  ty_sell", "bankn
+00018c00: 6966 7479 5f73 656c 6c22 5d0d 0a0d 0a20  ifty_sell"].... 
+00018c10: 2020 2020 2020 2064 6174 615f 7475 706c         data_tupl
+00018c20: 6520 3d20 6665 7463 6865 722e 6665 7463  e = fetcher.fetc
+00018c30: 6846 6976 6545 6d61 4461 7461 2829 0d0a  hFiveEmaData()..
+00018c40: 2020 2020 2020 2020 666f 7220 636e 7420          for cnt 
+00018c50: 696e 2072 616e 6765 286c 656e 2864 6174  in range(len(dat
+00018c60: 615f 7475 706c 6529 293a 0d0a 2020 2020  a_tuple)):..    
+00018c70: 2020 2020 2020 2020 6420 3d20 6461 7461          d = data
+00018c80: 5f74 7570 6c65 5b63 6e74 5d0d 0a20 2020  _tuple[cnt]..   
+00018c90: 2020 2020 2020 2020 2064 5b22 3545 4d41           d["5EMA
+00018ca0: 225d 203d 2070 6b74 616c 6962 2e45 4d41  "] = pktalib.EMA
+00018cb0: 2864 5b22 436c 6f73 6522 5d2c 2074 696d  (d["Close"], tim
+00018cc0: 6570 6572 696f 643d 3529 0d0a 2020 2020  eperiod=5)..    
+00018cd0: 2020 2020 2020 2020 6420 3d20 645b 636f          d = d[co
+00018ce0: 6c5f 6e61 6d65 735d 0d0a 2020 2020 2020  l_names]..      
+00018cf0: 2020 2020 2020 6420 3d20 642e 6472 6f70        d = d.drop
+00018d00: 6e61 2829 2e72 6f75 6e64 2832 290d 0a0d  na().round(2)...
+00018d10: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00018d20: 6820 5375 7070 7265 7373 4f75 7470 7574  h SuppressOutput
+00018d30: 2873 7570 7072 6573 735f 7374 6465 7272  (suppress_stderr
+00018d40: 3d54 7275 652c 2073 7570 7072 6573 735f  =True, suppress_
+00018d50: 7374 646f 7574 3d54 7275 6529 3a0d 0a20  stdout=True):.. 
+00018d60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00018d70: 6620 2273 656c 6c22 2069 6e20 6461 7461  f "sell" in data
+00018d80: 5f6c 6973 745b 636e 745d 3a0d 0a20 2020  _list[cnt]:..   
 00018d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018da0: 2020 2020 7374 7265 6368 6564 5b22 534c      streched["SL
-00018db0: 225d 203d 2073 7472 6563 6865 642e 4c6f  "] = streched.Lo
-00018dc0: 770d 0a20 2020 2020 2020 2020 2020 2020  w..             
-00018dd0: 2020 2020 2020 2076 616c 6964 6174 6520         validate 
-00018de0: 3d20 642e 6c6f 635b 6d61 736b 2e73 6869  = d.loc[mask.shi
-00018df0: 6674 2831 292e 6669 6c6c 6e61 2846 616c  ft(1).fillna(Fal
-00018e00: 7365 295d 0d0a 2020 2020 2020 2020 2020  se)]..          
-00018e10: 2020 2020 2020 2020 2020 6f6c 645f 696e            old_in
-00018e20: 6465 7820 3d20 7661 6c69 6461 7465 2e69  dex = validate.i
-00018e30: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-00018e40: 2020 7467 7420 3d20 7064 2e44 6174 6146    tgt = pd.DataF
-00018e50: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
-00018e60: 2020 2020 2020 2028 0d0a 2020 2020 2020         (..      
-00018e70: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00018e80: 6c69 6461 7465 2e43 6c6f 7365 2e72 6573  lidate.Close.res
-00018e90: 6574 5f69 6e64 6578 2864 726f 703d 5472  et_index(drop=Tr
-00018ea0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00018eb0: 2020 2020 2020 2020 202d 2028 0d0a 2020           - (..  
+00018da0: 2073 7472 6563 6865 6420 3d20 645b 2864   streched = d[(d
+00018db0: 2e4c 6f77 203e 2064 5b22 3545 4d41 225d  .Low > d["5EMA"]
+00018dc0: 2920 2620 2864 2e4c 6f77 202d 2064 5b22  ) & (d.Low - d["
+00018dd0: 3545 4d41 225d 203e 2030 2e35 295d 0d0a  5EMA"] > 0.5)]..
+00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018df0: 2020 2020 7374 7265 6368 6564 5b22 534c      streched["SL
+00018e00: 225d 203d 2073 7472 6563 6865 642e 4869  "] = streched.Hi
+00018e10: 6768 0d0a 2020 2020 2020 2020 2020 2020  gh..            
+00018e20: 2020 2020 2020 2020 7661 6c69 6461 7465          validate
+00018e30: 203d 2064 5b0d 0a20 2020 2020 2020 2020   = d[..         
+00018e40: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00018e50: 642e 4c6f 772e 7368 6966 7428 3129 203e  d.Low.shift(1) >
+00018e60: 2064 5b22 3545 4d41 225d 2e73 6869 6674   d["5EMA"].shift
+00018e70: 2831 2929 0d0a 2020 2020 2020 2020 2020  (1))..          
+00018e80: 2020 2020 2020 2020 2020 2020 2020 2620                & 
+00018e90: 2864 2e4c 6f77 2e73 6869 6674 2831 2920  (d.Low.shift(1) 
+00018ea0: 2d20 645b 2235 454d 4122 5d2e 7368 6966  - d["5EMA"].shif
+00018eb0: 7428 3129 203e 2030 2e35 290d 0a20 2020  t(1) > 0.5)..   
 00018ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ed0: 2020 2020 2020 280d 0a20 2020 2020 2020        (..       
-00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ef0: 2020 2020 2073 7472 6563 6865 642e 534c       streched.SL
-00018f00: 2e72 6573 6574 5f69 6e64 6578 2864 726f  .reset_index(dro
-00018f10: 703d 5472 7565 290d 0a20 2020 2020 2020  p=True)..       
-00018f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f30: 2020 2020 202d 2076 616c 6964 6174 652e       - validate.
-00018f40: 436c 6f73 652e 7265 7365 745f 696e 6465  Close.reset_inde
-00018f50: 7828 6472 6f70 3d54 7275 6529 0d0a 2020  x(drop=True)..  
-00018f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f70: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f90: 202a 2072 6973 6b5f 7265 7761 7264 0d0a   * risk_reward..
-00018fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fb0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00018fc0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-00018fd0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-00018fe0: 6e73 3d5b 2254 6172 6765 7422 5d2c 0d0a  ns=["Target"],..
-00018ff0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00019000: 2020 2020 2020 2020 2020 2076 616c 6964             valid
-00019010: 6174 6520 3d20 7064 2e63 6f6e 6361 7428  ate = pd.concat(
-00019020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019030: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
-00019040: 2020 2020 2020 2020 2076 616c 6964 6174           validat
-00019050: 652e 7265 7365 745f 696e 6465 7828 6472  e.reset_index(dr
-00019060: 6f70 3d54 7275 6529 2c0d 0a20 2020 2020  op=True),..     
-00019070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019080: 7472 6563 6865 645b 2253 4c22 5d2e 7265  treched["SL"].re
-00019090: 7365 745f 696e 6465 7828 6472 6f70 3d54  set_index(drop=T
-000190a0: 7275 6529 2c0d 0a20 2020 2020 2020 2020  rue),..         
-000190b0: 2020 2020 2020 2020 2020 2074 6774 2c0d             tgt,.
-000190c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000190d0: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
-000190e0: 2020 2020 2061 7869 733d 312c 0d0a 2020       axis=1,..  
-000190f0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00019100: 2020 2020 2020 2020 2076 616c 6964 6174           validat
-00019110: 6520 3d20 7661 6c69 6461 7465 2e74 6169  e = validate.tai
-00019120: 6c28 6c65 6e28 6f6c 645f 696e 6465 7829  l(len(old_index)
-00019130: 290d 0a20 2020 2020 2020 2020 2020 2076  )..            v
-00019140: 616c 6964 6174 6520 3d20 7661 6c69 6461  alidate = valida
-00019150: 7465 2e73 6574 5f69 6e64 6578 286f 6c64  te.set_index(old
-00019160: 5f69 6e64 6578 290d 0a20 2020 2020 2020  _index)..       
-00019170: 2020 2020 2069 6620 2273 656c 6c22 2069       if "sell" i
-00019180: 6e20 6461 7461 5f6c 6973 745b 636e 745d  n data_list[cnt]
-00019190: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000191a0: 2020 2066 696e 616c 203d 2076 616c 6964     final = valid
-000191b0: 6174 655b 7661 6c69 6461 7465 2e43 6c6f  ate[validate.Clo
-000191c0: 7365 203c 2076 616c 6964 6174 655b 2235  se < validate["5
-000191d0: 454d 4122 5d5d 2e74 6169 6c28 3129 0d0a  EMA"]].tail(1)..
-000191e0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000191f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019200: 2020 2066 696e 616c 203d 2076 616c 6964     final = valid
-00019210: 6174 655b 7661 6c69 6461 7465 2e43 6c6f  ate[validate.Clo
-00019220: 7365 203e 2076 616c 6964 6174 655b 2235  se > validate["5
-00019230: 454d 4122 5d5d 2e74 6169 6c28 3129 0d0a  EMA"]].tail(1)..
-00019240: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00019250: 2064 6174 615f 6c69 7374 5b63 6e74 5d20   data_list[cnt] 
-00019260: 6e6f 7420 696e 206c 6173 745f 7369 676e  not in last_sign
-00019270: 616c 3a0d 0a20 2020 2020 2020 2020 2020  al:..           
-00019280: 2020 2020 206c 6173 745f 7369 676e 616c       last_signal
-00019290: 5b64 6174 615f 6c69 7374 5b63 6e74 5d5d  [data_list[cnt]]
-000192a0: 203d 2066 696e 616c 0d0a 2020 2020 2020   = final..      
-000192b0: 2020 2020 2020 656c 6966 2064 6174 615f        elif data_
-000192c0: 6c69 7374 5b63 6e74 5d20 696e 206c 6173  list[cnt] in las
-000192d0: 745f 7369 676e 616c 3a0d 0a20 2020 2020  t_signal:..     
-000192e0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-000192f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019300: 2020 2020 2063 6f6e 6469 7469 6f6e 203d       condition =
-00019310: 206c 6173 745f 7369 676e 616c 5b64 6174   last_signal[dat
-00019320: 615f 6c69 7374 5b63 6e74 5d5d 5b30 5d5b  a_list[cnt]][0][
-00019330: 2253 4c22 5d5b 305d 0d0a 2020 2020 2020  "SL"][0]..      
-00019340: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00019350: 204b 6579 4572 726f 7220 6173 2065 3a20   KeyError as e: 
-00019360: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-00019370: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
-00019380: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
-00019390: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
-000193a0: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
-000193b0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-000193c0: 2020 2020 2020 2020 2063 6f6e 6469 7469           conditi
-000193d0: 6f6e 203d 206c 6173 745f 7369 676e 616c  on = last_signal
-000193e0: 5b64 6174 615f 6c69 7374 5b63 6e74 5d5d  [data_list[cnt]]
-000193f0: 5b22 534c 225d 5b30 5d0d 0a20 2020 2020  ["SL"][0]..     
-00019400: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-00019410: 6c61 7374 5f73 6967 6e61 6c5b 6461 7461  last_signal[data
-00019420: 5f6c 6973 745b 636e 745d 5d20 6973 206e  _list[cnt]] is n
-00019430: 6f74 2066 696e 616c 3a20 2020 2020 2020  ot final:       
-00019440: 2020 2023 2044 6562 7567 202d 2053 686f     # Debug - Sho
-00019450: 7773 2061 6c6c 2063 6f6e 6469 7469 6f6e  ws all condition
-00019460: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00019470: 2020 2069 6620 6c65 6e28 6669 6e61 6c5b     if len(final[
-00019480: 2253 4c22 5d29 203e 2030 2061 6e64 2063  "SL"]) > 0 and c
-00019490: 6f6e 6469 7469 6f6e 2021 3d20 6669 6e61  ondition != fina
-000194a0: 6c5b 2253 4c22 5d2e 696c 6f63 5b30 5d3a  l["SL"].iloc[0]:
-000194b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000194c0: 2020 2020 2020 2320 446f 2073 6f6d 6574        # Do somet
-000194d0: 6869 6e67 2077 6974 6820 7265 7375 6c74  hing with result
-000194e0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-000194f0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00019500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019510: 2020 2020 2072 6573 756c 745f 6466 203d       result_df =
-00019520: 2070 642e 636f 6e63 6174 280d 0a20 2020   pd.concat(..   
-00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019540: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-00019550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019560: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00019570: 6c74 5f64 662c 0d0a 2020 2020 2020 2020  lt_df,..        
+00018ed0: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
+00018ee0: 2020 2020 2020 2020 6f6c 645f 696e 6465          old_inde
+00018ef0: 7820 3d20 7661 6c69 6461 7465 2e69 6e64  x = validate.ind
+00018f00: 6578 0d0a 2020 2020 2020 2020 2020 2020  ex..            
+00018f10: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00018f20: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00018f30: 6173 6b20 3d20 2864 2e48 6967 6820 3c20  ask = (d.High < 
+00018f40: 645b 2235 454d 4122 5d29 2026 2028 645b  d["5EMA"]) & (d[
+00018f50: 2235 454d 4122 5d20 2d20 642e 4869 6768  "5EMA"] - d.High
+00018f60: 203e 2030 2e35 2920 2023 2042 7579 0d0a   > 0.5)  # Buy..
+00018f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f80: 2020 2020 7374 7265 6368 6564 203d 2064      streched = d
+00018f90: 5b6d 6173 6b5d 0d0a 2020 2020 2020 2020  [mask]..        
+00018fa0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+00018fb0: 6368 6564 5b22 534c 225d 203d 2073 7472  ched["SL"] = str
+00018fc0: 6563 6865 642e 4c6f 770d 0a20 2020 2020  eched.Low..     
+00018fd0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00018fe0: 616c 6964 6174 6520 3d20 642e 6c6f 635b  alidate = d.loc[
+00018ff0: 6d61 736b 2e73 6869 6674 2831 292e 6669  mask.shift(1).fi
+00019000: 6c6c 6e61 2846 616c 7365 295d 0d0a 2020  llna(False)]..  
+00019010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019020: 2020 6f6c 645f 696e 6465 7820 3d20 7661    old_index = va
+00019030: 6c69 6461 7465 2e69 6e64 6578 0d0a 2020  lidate.index..  
+00019040: 2020 2020 2020 2020 2020 7467 7420 3d20            tgt = 
+00019050: 7064 2e44 6174 6146 7261 6d65 280d 0a20  pd.DataFrame(.. 
+00019060: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00019070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019080: 2020 2020 2020 7661 6c69 6461 7465 2e43        validate.C
+00019090: 6c6f 7365 2e72 6573 6574 5f69 6e64 6578  lose.reset_index
+000190a0: 2864 726f 703d 5472 7565 290d 0a20 2020  (drop=True)..   
+000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190c0: 202d 2028 0d0a 2020 2020 2020 2020 2020   - (..          
+000190d0: 2020 2020 2020 2020 2020 2020 2020 280d                (.
+000190e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000190f0: 2020 2020 2020 2020 2020 2020 2073 7472               str
+00019100: 6563 6865 642e 534c 2e72 6573 6574 5f69  eched.SL.reset_i
+00019110: 6e64 6578 2864 726f 703d 5472 7565 290d  ndex(drop=True).
+00019120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019130: 2020 2020 2020 2020 2020 2020 202d 2076               - v
+00019140: 616c 6964 6174 652e 436c 6f73 652e 7265  alidate.Close.re
+00019150: 7365 745f 696e 6465 7828 6472 6f70 3d54  set_index(drop=T
+00019160: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+00019170: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+00019180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019190: 2020 2020 2020 2020 202a 2072 6973 6b5f           * risk_
+000191a0: 7265 7761 7264 0d0a 2020 2020 2020 2020  reward..        
+000191b0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+000191c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000191d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000191e0: 2020 2063 6f6c 756d 6e73 3d5b 2254 6172     columns=["Tar
+000191f0: 6765 7422 5d2c 0d0a 2020 2020 2020 2020  get"],..        
+00019200: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00019210: 2020 2076 616c 6964 6174 6520 3d20 7064     validate = pd
+00019220: 2e63 6f6e 6361 7428 0d0a 2020 2020 2020  .concat(..      
+00019230: 2020 2020 2020 2020 2020 5b0d 0a20 2020            [..   
+00019240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019250: 2076 616c 6964 6174 652e 7265 7365 745f   validate.reset_
+00019260: 696e 6465 7828 6472 6f70 3d54 7275 6529  index(drop=True)
+00019270: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00019280: 2020 2020 2020 2073 7472 6563 6865 645b         streched[
+00019290: 2253 4c22 5d2e 7265 7365 745f 696e 6465  "SL"].reset_inde
+000192a0: 7828 6472 6f70 3d54 7275 6529 2c0d 0a20  x(drop=True),.. 
+000192b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192c0: 2020 2074 6774 2c0d 0a20 2020 2020 2020     tgt,..       
+000192d0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+000192e0: 2020 2020 2020 2020 2020 2020 2061 7869               axi
+000192f0: 733d 312c 0d0a 2020 2020 2020 2020 2020  s=1,..          
+00019300: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00019310: 2076 616c 6964 6174 6520 3d20 7661 6c69   validate = vali
+00019320: 6461 7465 2e74 6169 6c28 6c65 6e28 6f6c  date.tail(len(ol
+00019330: 645f 696e 6465 7829 290d 0a20 2020 2020  d_index))..     
+00019340: 2020 2020 2020 2076 616c 6964 6174 6520         validate 
+00019350: 3d20 7661 6c69 6461 7465 2e73 6574 5f69  = validate.set_i
+00019360: 6e64 6578 286f 6c64 5f69 6e64 6578 290d  ndex(old_index).
+00019370: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00019380: 2273 656c 6c22 2069 6e20 6461 7461 5f6c  "sell" in data_l
+00019390: 6973 745b 636e 745d 3a0d 0a20 2020 2020  ist[cnt]:..     
+000193a0: 2020 2020 2020 2020 2020 2066 696e 616c             final
+000193b0: 203d 2076 616c 6964 6174 655b 7661 6c69   = validate[vali
+000193c0: 6461 7465 2e43 6c6f 7365 203c 2076 616c  date.Close < val
+000193d0: 6964 6174 655b 2235 454d 4122 5d5d 2e74  idate["5EMA"]].t
+000193e0: 6169 6c28 3129 0d0a 2020 2020 2020 2020  ail(1)..        
+000193f0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00019400: 2020 2020 2020 2020 2020 2066 696e 616c             final
+00019410: 203d 2076 616c 6964 6174 655b 7661 6c69   = validate[vali
+00019420: 6461 7465 2e43 6c6f 7365 203e 2076 616c  date.Close > val
+00019430: 6964 6174 655b 2235 454d 4122 5d5d 2e74  idate["5EMA"]].t
+00019440: 6169 6c28 3129 0d0a 0d0a 2020 2020 2020  ail(1)....      
+00019450: 2020 2020 2020 6966 2064 6174 615f 6c69        if data_li
+00019460: 7374 5b63 6e74 5d20 6e6f 7420 696e 206c  st[cnt] not in l
+00019470: 6173 745f 7369 676e 616c 3a0d 0a20 2020  ast_signal:..   
+00019480: 2020 2020 2020 2020 2020 2020 206c 6173               las
+00019490: 745f 7369 676e 616c 5b64 6174 615f 6c69  t_signal[data_li
+000194a0: 7374 5b63 6e74 5d5d 203d 2066 696e 616c  st[cnt]] = final
+000194b0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000194c0: 6966 2064 6174 615f 6c69 7374 5b63 6e74  if data_list[cnt
+000194d0: 5d20 696e 206c 6173 745f 7369 676e 616c  ] in last_signal
+000194e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000194f0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00019500: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00019510: 6469 7469 6f6e 203d 206c 6173 745f 7369  dition = last_si
+00019520: 676e 616c 5b64 6174 615f 6c69 7374 5b63  gnal[data_list[c
+00019530: 6e74 5d5d 5b30 5d5b 2253 4c22 5d5b 305d  nt]][0]["SL"][0]
+00019540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019550: 2020 6578 6365 7074 204b 6579 4572 726f    except KeyErro
+00019560: 7220 6173 2065 3a20 2320 7072 6167 6d61  r as e: # pragma
+00019570: 3a20 6e6f 2063 6f76 6572 0d0a 2020 2020  : no cover..    
 00019580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019590: 2020 2020 2020 2020 7064 2e44 6174 6146          pd.DataF
-000195a0: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
-000195b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195c0: 2020 2020 2020 2020 2020 205b 0d0a 2020             [..  
-000195d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195f0: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
-00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019620: 2020 2020 2063 6f6c 6f72 5465 7874 2e42       colorText.B
-00019630: 4c55 450d 0a20 2020 2020 2020 2020 2020  LUE..           
-00019640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019660: 202b 2073 7472 2866 696e 616c 2e69 6e64   + str(final.ind
-00019670: 6578 5b30 5d29 0d0a 2020 2020 2020 2020  ex[0])..        
-00019680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196a0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-000196b0: 454e 442c 0d0a 2020 2020 2020 2020 2020  END,..          
-000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196e0: 2020 636f 6c6f 7254 6578 742e 424f 4c44    colorText.BOLD
-000196f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019710: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00019720: 636f 6c6f 7254 6578 742e 5741 524e 0d0a  colorText.WARN..
-00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019590: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+000195a0: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
+000195b0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
+000195c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195d0: 2063 6f6e 6469 7469 6f6e 203d 206c 6173   condition = las
+000195e0: 745f 7369 676e 616c 5b64 6174 615f 6c69  t_signal[data_li
+000195f0: 7374 5b63 6e74 5d5d 5b22 534c 225d 5b30  st[cnt]]["SL"][0
+00019600: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00019610: 2020 2023 2069 6620 6c61 7374 5f73 6967     # if last_sig
+00019620: 6e61 6c5b 6461 7461 5f6c 6973 745b 636e  nal[data_list[cn
+00019630: 745d 5d20 6973 206e 6f74 2066 696e 616c  t]] is not final
+00019640: 3a20 2020 2020 2020 2020 2023 2044 6562  :          # Deb
+00019650: 7567 202d 2053 686f 7773 2061 6c6c 2063  ug - Shows all c
+00019660: 6f6e 6469 7469 6f6e 730d 0a20 2020 2020  onditions..     
+00019670: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00019680: 6e28 6669 6e61 6c5b 2253 4c22 5d29 203e  n(final["SL"]) >
+00019690: 2030 2061 6e64 2063 6f6e 6469 7469 6f6e   0 and condition
+000196a0: 2021 3d20 6669 6e61 6c5b 2253 4c22 5d2e   != final["SL"].
+000196b0: 696c 6f63 5b30 5d3a 0d0a 2020 2020 2020  iloc[0]:..      
+000196c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000196d0: 446f 2073 6f6d 6574 6869 6e67 2077 6974  Do something wit
+000196e0: 6820 7265 7375 6c74 730d 0a20 2020 2020  h results..     
+000196f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00019700: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00019710: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00019720: 756c 745f 6466 203d 2070 642e 636f 6e63  ult_df = pd.conc
+00019730: 6174 280d 0a20 2020 2020 2020 2020 2020  at(..           
 00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019750: 2020 2020 2020 2020 2020 2020 2b20 6461              + da
-00019760: 7461 5f6c 6973 745b 636e 745d 2e73 706c  ta_list[cnt].spl
-00019770: 6974 2822 5f22 295b 305d 2e75 7070 6572  it("_")[0].upper
-00019780: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00019750: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+00019760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019770: 2020 2020 7265 7375 6c74 5f64 662c 0d0a      result_df,..
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197b0: 2b20 636f 6c6f 7254 6578 742e 454e 442c  + colorText.END,
-000197c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197e0: 2020 2020 2020 2020 2020 2020 2020 280d                (.
-000197f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197a0: 7064 2e44 6174 6146 7261 6d65 280d 0a20  pd.DataFrame(.. 
+000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197d0: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
+000197e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197f0: 2020 2020 2020 2020 2020 2020 2020 5b0d                [.
+00019800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00019810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019820: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
-00019830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019820: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00019830: 6f72 5465 7874 2e42 4c55 450d 0a20 2020  orText.BLUE..   
 00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019860: 202b 2063 6f6c 6f72 5465 7874 2e46 4149   + colorText.FAI
-00019870: 4c0d 0a20 2020 2020 2020 2020 2020 2020  L..             
+00019860: 2020 2020 2020 2020 202b 2073 7472 2866           + str(f
+00019870: 696e 616c 2e69 6e64 6578 5b30 5d29 0d0a  inal.index[0])..
 00019880: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198a0: 2020 202b 2064 6174 615f 6c69 7374 5b63     + data_list[c
-000198b0: 6e74 5d2e 7370 6c69 7428 225f 2229 5b31  nt].split("_")[1
-000198c0: 5d2e 7570 7065 7228 290d 0a20 2020 2020  ].upper()..     
+000198a0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+000198b0: 6c6f 7254 6578 742e 454e 442c 0d0a 2020  lorText.END,..  
+000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198f0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00019900: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+000198e0: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
+000198f0: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
+00019900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019930: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00019920: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00019930: 742e 5741 524e 0d0a 2020 2020 2020 2020  t.WARN..        
 00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019960: 2020 2020 2020 2069 6620 2273 656c 6c22         if "sell"
-00019970: 2069 6e20 6461 7461 5f6c 6973 745b 636e   in data_list[cn
-00019980: 745d 0d0a 2020 2020 2020 2020 2020 2020  t]..            
+00019960: 2020 2020 2b20 6461 7461 5f6c 6973 745b      + data_list[
+00019970: 636e 745d 2e73 706c 6974 2822 5f22 295b  cnt].split("_")[
+00019980: 305d 2e75 7070 6572 2829 0d0a 2020 2020  0].upper()..    
 00019990: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000199a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199b0: 656c 7365 2028 0d0a 2020 2020 2020 2020  else (..        
-000199c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199b0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+000199c0: 6578 742e 454e 442c 0d0a 2020 2020 2020  ext.END,..      
 000199d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199e0: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
-000199f0: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
+000199e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199f0: 2020 2020 2020 280d 0a20 2020 2020 2020        (..       
 00019a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a20: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00019a30: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
+00019a20: 2020 2020 2020 2020 2063 6f6c 6f72 5465           colorTe
+00019a30: 7874 2e42 4f4c 440d 0a20 2020 2020 2020  xt.BOLD..       
 00019a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a60: 2020 2020 2020 2020 2020 202b 2064 6174             + dat
-00019a70: 615f 6c69 7374 5b63 6e74 5d2e 7370 6c69  a_list[cnt].spli
-00019a80: 7428 225f 2229 5b31 5d2e 7570 7065 7228  t("_")[1].upper(
-00019a90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ac0: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
-00019ad0: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
+00019a60: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00019a70: 5465 7874 2e46 4149 4c0d 0a20 2020 2020  Text.FAIL..     
+00019a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019aa0: 2020 2020 2020 2020 2020 202b 2064 6174             + dat
+00019ab0: 615f 6c69 7374 5b63 6e74 5d2e 7370 6c69  a_list[cnt].spli
+00019ac0: 7428 225f 2229 5b31 5d2e 7570 7065 7228  t("_")[1].upper(
+00019ad0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00019ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b00: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b00: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
+00019b10: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
 00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b30: 636f 6c6f 7254 6578 742e 4641 494c 0d0a  colorText.FAIL..
-00019b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00019b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b60: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
-00019b70: 7228 6669 6e61 6c2e 534c 5b30 5d29 0d0a  r(final.SL[0])..
-00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019b70: 6620 2273 656c 6c22 2069 6e20 6461 7461  f "sell" in data
+00019b80: 5f6c 6973 745b 636e 745d 0d0a 2020 2020  _list[cnt]..    
 00019b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ba0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-00019bb0: 6c6f 7254 6578 742e 454e 442c 0d0a 2020  lorText.END,..  
+00019ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bb0: 2020 2020 2020 2020 656c 7365 2028 0d0a          else (..
 00019bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019be0: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
-00019bf0: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
+00019be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bf0: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
 00019c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c20: 2020 2020 2020 202b 2073 7472 2866 696e         + str(fin
-00019c30: 616c 2e54 6172 6765 745b 305d 290d 0a20  al.Target[0]).. 
-00019c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c30: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00019c40: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
 00019c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c60: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00019c70: 6f72 5465 7874 2e45 4e44 2c0d 0a20 2020  orText.END,..   
-00019c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ca0: 2020 2020 2020 2020 2066 2231 3a7b 7269           f"1:{ri
-00019cb0: 736b 5f72 6577 6172 647d 222c 0d0a 2020  sk_reward}",..  
-00019cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ce0: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+00019c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c70: 2020 202b 2064 6174 615f 6c69 7374 5b63     + data_list[c
+00019c80: 6e74 5d2e 7370 6c69 7428 225f 2229 5b31  nt].split("_")[1
+00019c90: 5d2e 7570 7065 7228 290d 0a20 2020 2020  ].upper()..     
+00019ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cc0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00019cd0: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+00019ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d00: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00019d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019d00: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
+00019d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d30: 2020 2020 2063 6f6c 756d 6e73 3d72 6573       columns=res
-00019d40: 756c 745f 6466 2e63 6f6c 756d 6e73 2c0d  ult_df.columns,.
-00019d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019d30: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
+00019d40: 742e 4641 494c 0d0a 2020 2020 2020 2020  t.FAIL..        
+00019d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d70: 2029 2c0d 0a20 2020 2020 2020 2020 2020   ),..           
-00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d90: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
+00019d70: 2020 2020 2b20 7374 7228 6669 6e61 6c2e      + str(final.
+00019d80: 534c 5b30 5d29 0d0a 2020 2020 2020 2020  SL[0])..        
+00019d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019db0: 2061 7869 733d 302c 0d0a 2020 2020 2020   axis=0,..      
-00019dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019dd0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00019de0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00019df0: 756c 745f 6466 2e72 6573 6574 5f69 6e64  ult_df.reset_ind
-00019e00: 6578 2864 726f 703d 5472 7565 2c20 696e  ex(drop=True, in
-00019e10: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
-00019e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e30: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00019e40: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
-00019e50: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
+00019db0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+00019dc0: 454e 442c 0d0a 2020 2020 2020 2020 2020  END,..          
+00019dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019df0: 2020 636f 6c6f 7254 6578 742e 4752 4545    colorText.GREE
+00019e00: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
+00019e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e20: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00019e30: 2073 7472 2866 696e 616c 2e54 6172 6765   str(final.Targe
+00019e40: 745b 305d 290d 0a20 2020 2020 2020 2020  t[0])..         
+00019e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e70: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-00019e80: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
-00019e90: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
-00019ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019eb0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-00019ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ed0: 2020 2020 2320 5468 656e 2075 7064 6174      # Then updat
-00019ee0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00019ef0: 2020 2020 2020 206c 6173 745f 7369 676e         last_sign
-00019f00: 616c 5b64 6174 615f 6c69 7374 5b63 6e74  al[data_list[cnt
-00019f10: 5d5d 203d 205b 6669 6e61 6c5d 0d0a 2020  ]] = [final]..  
-00019f20: 2020 2020 2020 6966 2072 6573 756c 745f        if result_
-00019f30: 6466 2069 7320 6e6f 7420 4e6f 6e65 3a0d  df is not None:.
-00019f40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00019f50: 756c 745f 6466 2e64 726f 705f 6475 706c  ult_df.drop_dupl
-00019f60: 6963 6174 6573 286b 6565 703d 226c 6173  icates(keep="las
-00019f70: 7422 2c20 696e 706c 6163 653d 5472 7565  t", inplace=True
-00019f80: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00019f90: 6573 756c 745f 6466 2e73 6f72 745f 7661  esult_df.sort_va
-00019fa0: 6c75 6573 2862 793d 2254 696d 6522 2c20  lues(by="Time", 
-00019fb0: 696e 706c 6163 653d 5472 7565 290d 0a20  inplace=True).. 
-00019fc0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00019fd0: 7375 6c74 5f64 665b 3a3a 2d31 5d0d 0a0d  sult_df[::-1]...
-00019fe0: 0a20 2020 2023 2050 7265 7072 6f63 6573  .    # Preproces
-00019ff0: 7320 7468 6520 6163 7175 6972 6564 2064  s the acquired d
-0001a000: 6174 610d 0a20 2020 2064 6566 2070 7265  ata..    def pre
-0001a010: 7072 6f63 6573 7344 6174 6128 7365 6c66  processData(self
-0001a020: 2c20 6466 2c20 6461 7973 546f 4c6f 6f6b  , df, daysToLook
-0001a030: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
-0001a040: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
-0001a050: 7374 616e 6365 2864 662c 2070 642e 4461  stance(df, pd.Da
-0001a060: 7461 4672 616d 6529 0d0a 2020 2020 2020  taFrame)..      
-0001a070: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-0001a080: 2829 0d0a 2020 2020 2020 2020 7472 793a  ()..        try:
-0001a090: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-0001a0a0: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
-0001a0b0: 6528 6e70 2e69 6e66 2c20 6e70 2e6e 616e  e(np.inf, np.nan
-0001a0c0: 292e 7265 706c 6163 6528 2d6e 702e 696e  ).replace(-np.in
-0001a0d0: 662c 206e 702e 6e61 6e29 2e64 726f 706e  f, np.nan).dropn
-0001a0e0: 6128 686f 773d 2261 6c6c 2229 0d0a 2020  a(how="all")..  
-0001a0f0: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-0001a100: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
-0001a110: 696e 666f 2866 2250 7265 7072 6f63 6573  info(f"Preproces
-0001a120: 7369 6e67 2064 6174 613a 5c6e 7b64 6174  sing data:\n{dat
-0001a130: 612e 6865 6164 2831 297d 5c6e 2229 0d0a  a.head(1)}\n")..
-0001a140: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0001a150: 6179 7354 6f4c 6f6f 6b62 6163 6b20 6973  aysToLookback is
-0001a160: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0001a170: 2020 2020 2020 2020 6461 7973 546f 4c6f          daysToLo
-0001a180: 6f6b 6261 636b 203d 2073 656c 662e 636f  okback = self.co
-0001a190: 6e66 6967 4d61 6e61 6765 722e 6461 7973  nfigManager.days
-0001a1a0: 546f 4c6f 6f6b 6261 636b 0d0a 2020 2020  ToLookback..    
-0001a1b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001a1c0: 636f 6e66 6967 4d61 6e61 6765 722e 7573  configManager.us
-0001a1d0: 6545 4d41 3a0d 0a20 2020 2020 2020 2020  eEMA:..         
-0001a1e0: 2020 2020 2020 2073 6d61 203d 2070 6b74         sma = pkt
-0001a1f0: 616c 6962 2e45 4d41 2864 6174 615b 2243  alib.EMA(data["C
-0001a200: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
-0001a210: 6f64 3d35 3029 0d0a 2020 2020 2020 2020  od=50)..        
-0001a220: 2020 2020 2020 2020 6c6d 6120 3d20 706b          lma = pk
-0001a230: 7461 6c69 622e 454d 4128 6461 7461 5b22  talib.EMA(data["
-0001a240: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0001a250: 696f 643d 3230 3029 0d0a 2020 2020 2020  iod=200)..      
-0001a260: 2020 2020 2020 2020 2020 7373 6d61 203d            ssma =
-0001a270: 2070 6b74 616c 6962 2e45 4d41 2864 6174   pktalib.EMA(dat
-0001a280: 615b 2243 6c6f 7365 225d 2c20 7469 6d65  a["Close"], time
-0001a290: 7065 7269 6f64 3d39 290d 0a20 2020 2020  period=9)..     
-0001a2a0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0001a2b0: 696e 7365 7274 286c 656e 2864 6174 612e  insert(len(data.
-0001a2c0: 636f 6c75 6d6e 7329 2c20 2253 4d41 222c  columns), "SMA",
-0001a2d0: 2073 6d61 290d 0a20 2020 2020 2020 2020   sma)..         
-0001a2e0: 2020 2020 2020 2064 6174 612e 696e 7365         data.inse
-0001a2f0: 7274 286c 656e 2864 6174 612e 636f 6c75  rt(len(data.colu
-0001a300: 6d6e 7329 2c20 224c 4d41 222c 206c 6d61  mns), "LMA", lma
-0001a310: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001a320: 2020 2064 6174 612e 696e 7365 7274 286c     data.insert(l
-0001a330: 656e 2864 6174 612e 636f 6c75 6d6e 7329  en(data.columns)
-0001a340: 2c20 2253 534d 4122 2c20 7373 6d61 290d  , "SSMA", ssma).
-0001a350: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001a360: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001a370: 2020 2020 736d 6120 3d20 706b 7461 6c69      sma = pktali
-0001a380: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
-0001a390: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-0001a3a0: 3530 290d 0a20 2020 2020 2020 2020 2020  50)..           
-0001a3b0: 2020 2020 206c 6d61 203d 2070 6b74 616c       lma = pktal
-0001a3c0: 6962 2e53 4d41 2864 6174 615b 2243 6c6f  ib.SMA(data["Clo
-0001a3d0: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
-0001a3e0: 3d32 3030 290d 0a20 2020 2020 2020 2020  =200)..         
-0001a3f0: 2020 2020 2020 2073 736d 6120 3d20 706b         ssma = pk
-0001a400: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
-0001a410: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0001a420: 696f 643d 3929 0d0a 2020 2020 2020 2020  iod=9)..        
-0001a430: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
-0001a440: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
-0001a450: 756d 6e73 292c 2022 534d 4122 2c20 736d  umns), "SMA", sm
-0001a460: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
-0001a470: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-0001a480: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-0001a490: 292c 2022 4c4d 4122 2c20 6c6d 6129 0d0a  ), "LMA", lma)..
-0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4b0: 6461 7461 2e69 6e73 6572 7428 6c65 6e28  data.insert(len(
-0001a4c0: 6461 7461 2e63 6f6c 756d 6e73 292c 2022  data.columns), "
-0001a4d0: 5353 4d41 222c 2073 736d 6129 0d0a 2020  SSMA", ssma)..  
-0001a4e0: 2020 2020 2020 2020 2020 766f 6c20 3d20            vol = 
-0001a4f0: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
-0001a500: 5b22 566f 6c75 6d65 225d 2c20 7469 6d65  ["Volume"], time
-0001a510: 7065 7269 6f64 3d32 3029 0d0a 2020 2020  period=20)..    
-0001a520: 2020 2020 2020 2020 7273 6920 3d20 706b          rsi = pk
-0001a530: 7461 6c69 622e 5253 4928 6461 7461 5b22  talib.RSI(data["
-0001a540: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0001a550: 696f 643d 3134 290d 0a20 2020 2020 2020  iod=14)..       
-0001a560: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
-0001a570: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
-0001a580: 7329 2c20 2256 6f6c 4d41 222c 2076 6f6c  s), "VolMA", vol
-0001a590: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-0001a5a0: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
-0001a5b0: 6174 612e 636f 6c75 6d6e 7329 2c20 2252  ata.columns), "R
-0001a5c0: 5349 222c 2072 7369 290d 0a20 2020 2020  SI", rsi)..     
-0001a5d0: 2020 2020 2020 2063 6369 203d 2070 6b74         cci = pkt
-0001a5e0: 616c 6962 2e43 4349 2864 6174 615b 2248  alib.CCI(data["H
-0001a5f0: 6967 6822 5d2c 2064 6174 615b 224c 6f77  igh"], data["Low
-0001a600: 225d 2c20 6461 7461 5b22 436c 6f73 6522  "], data["Close"
-0001a610: 5d2c 2074 696d 6570 6572 696f 643d 3134  ], timeperiod=14
-0001a620: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-0001a630: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
-0001a640: 6174 612e 636f 6c75 6d6e 7329 2c20 2243  ata.columns), "C
-0001a650: 4349 222c 2063 6369 290d 0a20 2020 2020  CI", cci)..     
-0001a660: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-0001a670: 2020 2020 2020 2020 2020 2020 2066 6173               fas
-0001a680: 746b 2c20 6661 7374 6420 3d20 706b 7461  tk, fastd = pkta
-0001a690: 6c69 622e 5354 4f43 4852 5349 280d 0a20  lib.STOCHRSI(.. 
-0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6b0: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
-0001a6c0: 2c20 7469 6d65 7065 7269 6f64 3d31 342c  , timeperiod=14,
-0001a6d0: 2066 6173 746b 5f70 6572 696f 643d 352c   fastk_period=5,
-0001a6e0: 2066 6173 7464 5f70 6572 696f 643d 332c   fastd_period=3,
-0001a6f0: 2066 6173 7464 5f6d 6174 7970 653d 300d   fastd_matype=0.
-0001a700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a710: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0001a720: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-0001a730: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-0001a740: 292c 2022 4641 5354 4b22 2c20 6661 7374  ), "FASTK", fast
-0001a750: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
-0001a760: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-0001a770: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-0001a780: 292c 2022 4641 5354 4422 2c20 6661 7374  ), "FASTD", fast
-0001a790: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-0001a7a0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0001a7b0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-0001a7c0: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
-0001a7d0: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
-0001a7e0: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
-0001a7f0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-0001a800: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-0001a810: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0001a820: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-0001a830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a840: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-0001a850: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-0001a860: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-0001a870: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
-0001a880: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001a890: 615b 3a3a 2d31 5d20 2023 2052 6576 6572  a[::-1]  # Rever
-0001a8a0: 7365 2074 6865 2064 6174 6166 7261 6d65  se the dataframe
-0001a8b0: 0d0a 2020 2020 2020 2020 2320 6461 7461  ..        # data
-0001a8c0: 203d 2064 6174 612e 6669 6c6c 6e61 2830   = data.fillna(0
-0001a8d0: 290d 0a20 2020 2020 2020 2023 2064 6174  )..        # dat
-0001a8e0: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
-0001a8f0: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
-0001a900: 665d 2c20 3029 0d0a 2020 2020 2020 2020  f], 0)..        
-0001a910: 6675 6c6c 4461 7461 203d 2064 6174 610d  fullData = data.
-0001a920: 0a20 2020 2020 2020 2074 7269 6d6d 6564  .        trimmed
-0001a930: 4461 7461 203d 2064 6174 612e 6865 6164  Data = data.head
-0001a940: 2864 6179 7354 6f4c 6f6f 6b62 6163 6b29  (daysToLookback)
-0001a950: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001a960: 2028 6675 6c6c 4461 7461 2c20 7472 696d   (fullData, trim
-0001a970: 6d65 6444 6174 6129 0d0a 0d0a 2020 2020  medData)....    
-0001a980: 2320 5661 6c69 6461 7465 2069 6620 7468  # Validate if th
-0001a990: 6520 7374 6f63 6b20 6973 2062 756c 6c69  e stock is bulli
-0001a9a0: 7368 2069 6e20 7468 6520 7368 6f72 7420  sh in the short 
-0001a9b0: 7465 726d 0d0a 2020 2020 6465 6620 7661  term..    def va
-0001a9c0: 6c69 6461 7465 3135 4d69 6e75 7465 5072  lidate15MinutePr
-0001a9d0: 6963 6556 6f6c 756d 6542 7265 616b 6f75  iceVolumeBreakou
-0001a9e0: 7428 7365 6c66 2c20 6466 293a 0d0a 2020  t(self, df):..  
-0001a9f0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-0001aa00: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-0001aa10: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-0001aa20: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
-0001aa30: 2020 2020 2020 2020 2320 6874 7470 733a          # https:
-0001aa40: 2f2f 6368 6172 7469 6e6b 2e63 6f6d 2f73  //chartink.com/s
-0001aa50: 6372 6565 6e65 722f 3135 2d6d 696e 2d70  creener/15-min-p
-0001aa60: 7269 6365 2d76 6f6c 756d 652d 6272 6561  rice-volume-brea
-0001aa70: 6b6f 7574 0d0a 2020 2020 2020 2020 6461  kout..        da
-0001aa80: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001aa90: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001aaa0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-0001aab0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001aac0: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-0001aad0: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-0001aae0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-0001aaf0: 2064 6174 615b 3a3a 2d31 5d20 2023 2052   data[::-1]  # R
-0001ab00: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
-0001ab10: 7261 6d65 2073 6f20 7468 6174 2069 7473  rame so that its
-0001ab20: 2074 6865 206f 6c64 6573 7420 6461 7465   the oldest date
-0001ab30: 2066 6972 7374 0d0a 2020 2020 2020 2020   first..        
-0001ab40: 6461 7461 5b22 534d 4132 3022 5d20 3d20  data["SMA20"] = 
-0001ab50: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
-0001ab60: 5b22 436c 6f73 6522 5d2c 2032 3029 0d0a  ["Close"], 20)..
-0001ab70: 2020 2020 2020 2020 6461 7461 5b22 534d          data["SM
-0001ab80: 4132 3056 225d 203d 2070 6b74 616c 6962  A20V"] = pktalib
-0001ab90: 2e53 4d41 2864 6174 615b 2256 6f6c 756d  .SMA(data["Volum
-0001aba0: 6522 5d2c 2032 3029 0d0a 2020 2020 2020  e"], 20)..      
-0001abb0: 2020 6461 7461 203d 2064 6174 615b 0d0a    data = data[..
-0001abc0: 2020 2020 2020 2020 2020 2020 3a3a 2d31              ::-1
-0001abd0: 0d0a 2020 2020 2020 2020 5d20 2023 2052  ..        ]  # R
-0001abe0: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
-0001abf0: 7261 6d65 2073 6f20 7468 6174 2069 7427  rame so that it'
-0001ac00: 7320 7468 6520 6d6f 7374 2072 6563 656e  s the most recen
-0001ac10: 7420 6461 7465 2066 6972 7374 0d0a 2020  t date first..  
-0001ac20: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
-0001ac30: 6174 612e 6865 6164 2833 290d 0a20 2020  ata.head(3)..   
-0001ac40: 2020 2020 2069 6620 6c65 6e28 7265 6365       if len(rece
-0001ac50: 6e74 2920 3c20 333a 0d0a 2020 2020 2020  nt) < 3:..      
-0001ac60: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001ac70: 7365 0d0a 2020 2020 2020 2020 636f 6e64  se..        cond
-0001ac80: 3120 3d20 7265 6365 6e74 5b22 436c 6f73  1 = recent["Clos
-0001ac90: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
-0001aca0: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
-0001acb0: 6f63 5b31 5d0d 0a20 2020 2020 2020 2063  oc[1]..        c
-0001acc0: 6f6e 6432 203d 2063 6f6e 6431 2061 6e64  ond2 = cond1 and
-0001acd0: 2028 7265 6365 6e74 5b22 436c 6f73 6522   (recent["Close"
-0001ace0: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
-0001acf0: 6e74 5b22 534d 4132 3022 5d2e 696c 6f63  nt["SMA20"].iloc
-0001ad00: 5b30 5d29 0d0a 2020 2020 2020 2020 636f  [0])..        co
-0001ad10: 6e64 3320 3d20 636f 6e64 3220 616e 6420  nd3 = cond2 and 
-0001ad20: 2872 6563 656e 745b 2243 6c6f 7365 225d  (recent["Close"]
-0001ad30: 2e69 6c6f 635b 315d 203e 2072 6563 656e  .iloc[1] > recen
-0001ad40: 745b 2248 6967 6822 5d2e 696c 6f63 5b32  t["High"].iloc[2
-0001ad50: 5d29 0d0a 2020 2020 2020 2020 636f 6e64  ])..        cond
-0001ad60: 3420 3d20 636f 6e64 3320 616e 6420 2872  4 = cond3 and (r
-0001ad70: 6563 656e 745b 2256 6f6c 756d 6522 5d2e  ecent["Volume"].
-0001ad80: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
-0001ad90: 5b22 534d 4132 3056 225d 2e69 6c6f 635b  ["SMA20V"].iloc[
-0001ada0: 305d 290d 0a20 2020 2020 2020 2063 6f6e  0])..        con
-0001adb0: 6435 203d 2063 6f6e 6434 2061 6e64 2028  d5 = cond4 and (
-0001adc0: 7265 6365 6e74 5b22 566f 6c75 6d65 225d  recent["Volume"]
-0001add0: 2e69 6c6f 635b 315d 203e 2072 6563 656e  .iloc[1] > recen
-0001ade0: 745b 2253 4d41 3230 5622 5d2e 696c 6f63  t["SMA20V"].iloc
-0001adf0: 5b30 5d29 0d0a 2020 2020 2020 2020 7265  [0])..        re
-0001ae00: 7475 726e 2063 6f6e 6435 0d0a 0d0a 2020  turn cond5....  
-0001ae10: 2020 6465 6620 7661 6c69 6461 7465 4275    def validateBu
-0001ae20: 6c6c 6973 6846 6f72 546f 6d6f 7272 6f77  llishForTomorrow
-0001ae30: 2873 656c 662c 2064 6629 3a0d 0a20 2020  (self, df):..   
-0001ae40: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-0001ae50: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-0001ae60: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-0001ae70: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-0001ae80: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-0001ae90: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-0001aea0: 2023 2068 7474 7073 3a2f 2f63 6861 7274   # https://chart
-0001aeb0: 696e 6b2e 636f 6d2f 7363 7265 656e 6572  ink.com/screener
-0001aec0: 2f62 756c 6c69 7368 2d66 6f72 2d74 6f6d  /bullish-for-tom
-0001aed0: 6f72 726f 770d 0a20 2020 2020 2020 2064  orrow..        d
-0001aee0: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
-0001aef0: 6128 3029 0d0a 2020 2020 2020 2020 6461  a(0)..        da
-0001af00: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
-0001af10: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
-0001af20: 6e66 5d2c 2030 290d 0a20 2020 2020 2020  nf], 0)..       
-0001af30: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
-0001af40: 315d 2020 2320 5265 7665 7273 6520 7468  1]  # Reverse th
-0001af50: 6520 6461 7461 6672 616d 6520 736f 2074  e dataframe so t
-0001af60: 6861 7420 6974 7320 7468 6520 6f6c 6465  hat its the olde
-0001af70: 7374 2064 6174 6520 6669 7273 740d 0a20  st date first.. 
-0001af80: 2020 2020 2020 206d 6163 644c 696e 6520         macdLine 
-0001af90: 3d20 706b 7461 6c69 622e 4d41 4344 2864  = pktalib.MACD(d
-0001afa0: 6174 615b 2243 6c6f 7365 225d 2c20 3132  ata["Close"], 12
-0001afb0: 2c20 3236 2c20 3929 5b30 5d2e 7461 696c  , 26, 9)[0].tail
-0001afc0: 2833 290d 0a20 2020 2020 2020 206d 6163  (3)..        mac
-0001afd0: 6453 6967 6e61 6c20 3d20 706b 7461 6c69  dSignal = pktali
-0001afe0: 622e 4d41 4344 2864 6174 615b 2243 6c6f  b.MACD(data["Clo
-0001aff0: 7365 225d 2c20 3132 2c20 3236 2c20 3929  se"], 12, 26, 9)
-0001b000: 5b31 5d2e 7461 696c 2833 290d 0a20 2020  [1].tail(3)..   
-0001b010: 2020 2020 206d 6163 6448 6973 7420 3d20       macdHist = 
-0001b020: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
-0001b030: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
-0001b040: 3236 2c20 3929 5b32 5d2e 7461 696c 2833  26, 9)[2].tail(3
-0001b050: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
-0001b060: 7572 6e20 280d 0a20 2020 2020 2020 2020  urn (..         
-0001b070: 2020 2028 6d61 6364 4869 7374 2e69 6c6f     (macdHist.ilo
-0001b080: 635b 3a31 5d2e 696c 6f63 5b30 5d20 3c20  c[:1].iloc[0] < 
-0001b090: 6d61 6364 4869 7374 2e69 6c6f 635b 3a32  macdHist.iloc[:2
-0001b0a0: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
-0001b0b0: 2020 2020 2020 2020 616e 6420 286d 6163          and (mac
-0001b0c0: 6448 6973 742e 696c 6f63 5b3a 335d 2e69  dHist.iloc[:3].i
-0001b0d0: 6c6f 635b 325d 203e 206d 6163 6448 6973  loc[2] > macdHis
-0001b0e0: 742e 696c 6f63 5b3a 325d 2e69 6c6f 635b  t.iloc[:2].iloc[
-0001b0f0: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
-0001b100: 2061 6e64 2028 0d0a 2020 2020 2020 2020   and (..        
-0001b110: 2020 2020 2020 2020 286d 6163 644c 696e          (macdLin
-0001b120: 652e 696c 6f63 5b3a 335d 2e69 6c6f 635b  e.iloc[:3].iloc[
-0001b130: 325d 202d 206d 6163 6453 6967 6e61 6c2e  2] - macdSignal.
-0001b140: 696c 6f63 5b3a 335d 2e69 6c6f 635b 325d  iloc[:3].iloc[2]
-0001b150: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001b160: 2020 202d 2028 6d61 6364 4c69 6e65 2e69     - (macdLine.i
-0001b170: 6c6f 635b 3a32 5d2e 696c 6f63 5b31 5d20  loc[:2].iloc[1] 
-0001b180: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
-0001b190: 635b 3a32 5d2e 696c 6f63 5b31 5d29 0d0a  c[:2].iloc[1])..
-0001b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1b0: 3e3d 2030 2e34 0d0a 2020 2020 2020 2020  >= 0.4..        
-0001b1c0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0001b1d0: 2020 2061 6e64 2028 0d0a 2020 2020 2020     and (..      
-0001b1e0: 2020 2020 2020 2020 2020 286d 6163 644c            (macdL
-0001b1f0: 696e 652e 696c 6f63 5b3a 325d 2e69 6c6f  ine.iloc[:2].ilo
-0001b200: 635b 315d 202d 206d 6163 6453 6967 6e61  c[1] - macdSigna
-0001b210: 6c2e 696c 6f63 5b3a 325d 2e69 6c6f 635b  l.iloc[:2].iloc[
-0001b220: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
-0001b230: 2020 2020 202d 2028 6d61 6364 4c69 6e65       - (macdLine
-0001b240: 2e69 6c6f 635b 3a31 5d2e 696c 6f63 5b30  .iloc[:1].iloc[0
-0001b250: 5d20 2d20 6d61 6364 5369 676e 616c 2e69  ] - macdSignal.i
-0001b260: 6c6f 635b 3a31 5d2e 696c 6f63 5b30 5d29  loc[:1].iloc[0])
-0001b270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b280: 2020 3c3d 2030 2e32 0d0a 2020 2020 2020    <= 0.2..      
-0001b290: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001b2a0: 2020 2020 2061 6e64 2028 6d61 6364 4c69       and (macdLi
-0001b2b0: 6e65 2e69 6c6f 635b 3a33 5d2e 696c 6f63  ne.iloc[:3].iloc
-0001b2c0: 5b32 5d20 3e20 6d61 6364 5369 676e 616c  [2] > macdSignal
-0001b2d0: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
-0001b2e0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-0001b2f0: 616e 6420 280d 0a20 2020 2020 2020 2020  and (..         
-0001b300: 2020 2020 2020 2028 6d61 6364 4c69 6e65         (macdLine
-0001b310: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
-0001b320: 5d20 2d20 6d61 6364 5369 676e 616c 2e69  ] - macdSignal.i
-0001b330: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d29  loc[:3].iloc[2])
-0001b340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b350: 2020 2d20 286d 6163 644c 696e 652e 696c    - (macdLine.il
-0001b360: 6f63 5b3a 325d 2e69 6c6f 635b 315d 202d  oc[:2].iloc[1] -
-0001b370: 206d 6163 6453 6967 6e61 6c2e 696c 6f63   macdSignal.iloc
-0001b380: 5b3a 325d 2e69 6c6f 635b 315d 290d 0a20  [:2].iloc[1]).. 
-0001b390: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0001b3a0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-0001b3b0: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
-0001b3c0: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-0001b3d0: 6d65 0d0a 2020 2020 2320 7661 6c69 6461  me..    # valida
-0001b3e0: 7465 2069 6620 4343 4920 6973 2077 6974  te if CCI is wit
-0001b3f0: 6869 6e20 6769 7665 6e20 7261 6e67 650d  hin given range.
-0001b400: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0001b410: 6543 4349 2873 656c 662c 2064 662c 2073  eCCI(self, df, s
-0001b420: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001b430: 6963 742c 206d 696e 4343 492c 206d 6178  ict, minCCI, max
-0001b440: 4343 4929 3a0d 0a20 2020 2020 2020 2069  CCI):..        i
-0001b450: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
-0001b460: 6c65 6e28 6466 2920 3d3d 2030 3a0d 0a20  len(df) == 0:.. 
-0001b470: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001b480: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
-0001b490: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-0001b4a0: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
-0001b4b0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
-0001b4c0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-0001b4d0: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
-0001b4e0: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
-0001b4f0: 2030 290d 0a20 2020 2020 2020 2063 6369   0)..        cci
-0001b500: 203d 2069 6e74 2864 6174 612e 6865 6164   = int(data.head
-0001b510: 2831 295b 2243 4349 225d 2e69 6c6f 635b  (1)["CCI"].iloc[
-0001b520: 305d 290d 0a20 2020 2020 2020 2073 6176  0])..        sav
-0001b530: 6544 6963 745b 2243 4349 225d 203d 2063  eDict["CCI"] = c
-0001b540: 6369 0d0a 2020 2020 2020 2020 6966 2028  ci..        if (
-0001b550: 6363 6920 3e3d 206d 696e 4343 4920 616e  cci >= minCCI an
-0001b560: 6420 6363 6920 3c3d 206d 6178 4343 4929  d cci <= maxCCI)
-0001b570: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0001b580: 6620 2822 5570 2220 696e 2073 6176 6544  f ("Up" in saveD
-0001b590: 6963 745b 2254 7265 6e64 225d 293a 0d0a  ict["Trend"]):..
-0001b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b5b0: 7363 7265 656e 4469 6374 5b22 4343 4922  screenDict["CCI"
-0001b5c0: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
-0001b5d0: 2020 2020 2020 2020 2020 2028 636f 6c6f             (colo
-0001b5e0: 7254 6578 742e 424f 4c44 2069 6620 2822  rText.BOLD if ("
-0001b5f0: 5374 726f 6e67 2220 696e 2073 6176 6544  Strong" in saveD
-0001b600: 6963 745b 2254 7265 6e64 225d 2920 656c  ict["Trend"]) el
-0001b610: 7365 2022 2229 202b 2063 6f6c 6f72 5465  se "") + colorTe
-0001b620: 7874 2e47 5245 454e 202b 2073 7472 2863  xt.GREEN + str(c
-0001b630: 6369 2920 2b20 636f 6c6f 7254 6578 742e  ci) + colorText.
-0001b640: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-0001b650: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0001b660: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001b670: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001b680: 6e44 6963 745b 2243 4349 225d 203d 2028  nDict["CCI"] = (
-0001b690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b6a0: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
-0001b6b0: 2e42 4f4c 4420 6966 2028 2253 7472 6f6e  .BOLD if ("Stron
-0001b6c0: 6722 2069 6e20 7361 7665 4469 6374 5b22  g" in saveDict["
-0001b6d0: 5472 656e 6422 5d29 2065 6c73 6520 2222  Trend"]) else ""
-0001b6e0: 2920 2b20 636f 6c6f 7254 6578 742e 4641  ) + colorText.FA
-0001b6f0: 494c 202b 2073 7472 2863 6369 2920 2b20  IL + str(cci) + 
-0001b700: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-0001b710: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001b720: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001b730: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-0001b740: 2020 2073 6372 6565 6e44 6963 745b 2243     screenDict["C
-0001b750: 4349 225d 203d 2063 6f6c 6f72 5465 7874  CI"] = colorText
-0001b760: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-0001b770: 742e 4641 494c 202b 2073 7472 2863 6369  t.FAIL + str(cci
-0001b780: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
-0001b790: 440d 0a20 2020 2020 2020 2072 6574 7572  D..        retur
-0001b7a0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2023  n False....    #
-0001b7b0: 2046 696e 6420 436f 6e66 6c75 6365 6e63   Find Conflucenc
-0001b7c0: 650d 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
-0001b7d0: 6174 6543 6f6e 666c 7565 6e63 6528 7365  ateConfluence(se
-0001b7e0: 6c66 2c20 7374 6f63 6b2c 2064 662c 2073  lf, stock, df, s
-0001b7f0: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001b800: 6963 742c 2070 6572 6365 6e74 6167 653d  ict, percentage=
-0001b810: 302e 312c 636f 6e66 4669 6c74 6572 3d33  0.1,confFilter=3
-0001b820: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-0001b830: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001b840: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-0001b850: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001b860: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-0001b870: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001b880: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
-0001b890: 2064 6174 612e 6865 6164 2832 290d 0a20   data.head(2).. 
-0001b8a0: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
-0001b8b0: 6365 6e74 2920 3c20 323a 0d0a 2020 2020  cent) < 2:..    
-0001b8c0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001b8d0: 616c 7365 0d0a 2020 2020 2020 2020 6973  alse..        is
-0001b8e0: 3530 444d 4155 7054 7265 6e64 203d 2028  50DMAUpTrend = (
-0001b8f0: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
-0001b900: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b22  oc[0] > recent["
-0001b910: 534d 4122 5d2e 696c 6f63 5b31 5d29 0d0a  SMA"].iloc[1])..
-0001b920: 2020 2020 2020 2020 6973 3530 444d 4144          is50DMAD
-0001b930: 6f77 6e54 7265 6e64 203d 2028 7265 6365  ownTrend = (rece
-0001b940: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
-0001b950: 5d20 3c20 7265 6365 6e74 5b22 534d 4122  ] < recent["SMA"
-0001b960: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
-0001b970: 2020 2020 6973 476f 6c64 656e 4372 6f73      isGoldenCros
-0001b980: 734f 7665 7220 3d20 2872 6563 656e 745b  sOver = (recent[
-0001b990: 2253 4d41 225d 2e69 6c6f 635b 305d 203e  "SMA"].iloc[0] >
-0001b9a0: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
-0001b9b0: 696c 6f63 5b30 5d29 2061 6e64 205c 0d0a  iloc[0]) and \..
-0001b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b9d0: 2020 2020 2020 2020 2020 2020 2872 6563              (rec
-0001b9e0: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
-0001b9f0: 315d 203c 3d20 7265 6365 6e74 5b22 4c4d  1] <= recent["LM
-0001ba00: 4122 5d2e 696c 6f63 5b31 5d29 0d0a 2020  A"].iloc[1])..  
-0001ba10: 2020 2020 2020 6973 4465 6164 4372 6f73        isDeadCros
-0001ba20: 734f 7665 7220 3d20 2872 6563 656e 745b  sOver = (recent[
-0001ba30: 2253 4d41 225d 2e69 6c6f 635b 305d 203c  "SMA"].iloc[0] <
-0001ba40: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
-0001ba50: 696c 6f63 5b30 5d29 2061 6e64 205c 0d0a  iloc[0]) and \..
-0001ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba70: 2020 2020 2020 2020 2020 2020 2872 6563              (rec
-0001ba80: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
-0001ba90: 315d 203e 3d20 7265 6365 6e74 5b22 4c4d  1] >= recent["LM
-0001baa0: 4122 5d2e 696c 6f63 5b31 5d29 0d0a 2020  A"].iloc[1])..  
-0001bab0: 2020 2020 2020 6973 3530 444d 4120 3d20        is50DMA = 
-0001bac0: 2872 6563 656e 745b 2253 4d41 225d 2e69  (recent["SMA"].i
-0001bad0: 6c6f 635b 305d 203c 3d20 7265 6365 6e74  loc[0] <= recent
-0001bae0: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-0001baf0: 5d29 0d0a 2020 2020 2020 2020 6973 3230  ])..        is20
-0001bb00: 3044 4d41 203d 2028 7265 6365 6e74 5b22  0DMA = (recent["
-0001bb10: 4c4d 4122 5d2e 696c 6f63 5b30 5d20 3c3d  LMA"].iloc[0] <=
-0001bb20: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
-0001bb30: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
-0001bb40: 2020 2064 6966 6665 7265 6e63 6520 3d20     difference = 
-0001bb50: 726f 756e 6428 2872 6563 656e 745b 2253  round((recent["S
-0001bb60: 4d41 225d 2e69 6c6f 635b 305d 202d 2072  MA"].iloc[0] - r
-0001bb70: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
-0001bb80: 635b 305d 290d 0a20 2020 2020 2020 2020  c[0])..         
-0001bb90: 2020 2020 2020 202f 2072 6563 656e 745b         / recent[
-0001bba0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-0001bbb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001bbc0: 2020 2a20 3130 302c 0d0a 2020 2020 2020    * 100,..      
-0001bbd0: 2020 2020 2020 2020 2020 322c 0d0a 2020            2,..  
-0001bbe0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001bbf0: 2020 2020 2073 6176 6544 6963 745b 2243       saveDict["C
-0001bc00: 6f6e 6644 4d41 4469 6666 6572 656e 6365  onfDMADifference
-0001bc10: 225d 203d 2064 6966 6665 7265 6e63 650d  "] = difference.
-0001bc20: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
-0001bc30: 6963 745b 2243 6f6e 6644 4d41 4469 6666  ict["ConfDMADiff
-0001bc40: 6572 656e 6365 225d 203d 2064 6966 6665  erence"] = diffe
-0001bc50: 7265 6e63 650d 0a20 2020 2020 2020 2073  rence..        s
-0001bc60: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
-0001bc70: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
-0001bc80: 6528 7363 7265 656e 4469 6374 2c73 6176  e(screenDict,sav
-0001bc90: 6544 6963 742c 224d 412d 5369 676e 616c  eDict,"MA-Signal
-0001bca0: 2229 0d0a 2020 2020 2020 2020 2320 6469  ")..        # di
-0001bcb0: 6666 6572 656e 6365 203d 2061 6273 2864  fference = abs(d
-0001bcc0: 6966 6665 7265 6e63 6529 0d0a 2020 2020  ifference)..    
-0001bcd0: 2020 2020 636f 6e66 5465 7874 203d 2066      confText = f
-0001bce0: 227b 2747 6f6c 6465 6e43 726f 7373 6f76  "{'GoldenCrossov
-0001bcf0: 6572 2720 6966 2069 7347 6f6c 6465 6e43  er' if isGoldenC
-0001bd00: 726f 7373 4f76 6572 2065 6c73 6520 2827  rossOver else ('
-0001bd10: 4465 6164 4372 6f73 736f 7665 7227 2069  DeadCrossover' i
-0001bd20: 6620 6973 4465 6164 4372 6f73 734f 7665  f isDeadCrossOve
-0001bd30: 7220 656c 7365 2028 2743 6f6e 662e 5570  r else ('Conf.Up
-0001bd40: 2720 6966 2069 7335 3044 4d41 5570 5472  ' if is50DMAUpTr
-0001bd50: 656e 6420 656c 7365 2028 2743 6f6e 662e  end else ('Conf.
-0001bd60: 446f 776e 2720 6966 2069 7335 3044 4d41  Down' if is50DMA
-0001bd70: 446f 776e 5472 656e 6420 656c 7365 2028  DownTrend else (
-0001bd80: 2735 3044 4d41 2720 6966 2069 7335 3044  '50DMA' if is50D
-0001bd90: 4d41 2065 6c73 6520 2827 3230 3044 4d41  MA else ('200DMA
-0001bda0: 2720 6966 2069 7332 3030 444d 4120 656c  ' if is200DMA el
-0001bdb0: 7365 2027 556e 6b6e 6f77 6e27 2929 2929  se 'Unknown'))))
-0001bdc0: 297d 220d 0a20 2020 2020 2020 2069 6620  )}"..        if 
-0001bdd0: 6162 7328 7265 6365 6e74 5b22 534d 4122  abs(recent["SMA"
-0001bde0: 5d2e 696c 6f63 5b30 5d20 2d20 7265 6365  ].iloc[0] - rece
-0001bdf0: 6e74 5b22 4c4d 4122 5d2e 696c 6f63 5b30  nt["LMA"].iloc[0
-0001be00: 5d29 203c 3d20 280d 0a20 2020 2020 2020  ]) <= (..       
-0001be10: 2020 2020 2072 6563 656e 745b 2253 4d41       recent["SMA
-0001be20: 225d 2e69 6c6f 635b 305d 202a 2070 6572  "].iloc[0] * per
-0001be30: 6365 6e74 6167 650d 0a20 2020 2020 2020  centage..       
-0001be40: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-0001be50: 2069 6620 7265 6365 6e74 5b22 534d 4122   if recent["SMA"
-0001be60: 5d2e 696c 6f63 5b30 5d20 3e3d 2072 6563  ].iloc[0] >= rec
-0001be70: 656e 745b 224c 4d41 225d 2e69 6c6f 635b  ent["LMA"].iloc[
-0001be80: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
-0001be90: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001bea0: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
-0001beb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001bec0: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
-0001bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bee0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001bef0: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
-0001bf00: 2020 2020 2020 2020 2020 202b 2028 636f             + (co
-0001bf10: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
-0001bf20: 2069 7335 3044 4d41 5570 5472 656e 6420   is50DMAUpTrend 
-0001bf30: 656c 7365 2028 636f 6c6f 7254 6578 742e  else (colorText.
-0001bf40: 4641 494c 2069 6620 6973 3530 444d 4144  FAIL if is50DMAD
-0001bf50: 6f77 6e54 7265 6e64 2065 6c73 6520 636f  ownTrend else co
-0001bf60: 6c6f 7254 6578 742e 5741 524e 2929 0d0a  lorText.WARN))..
-0001bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf80: 2020 2020 2b20 6622 7b63 6f6e 6654 6578      + f"{confTex
-0001bf90: 747d 2028 7b64 6966 6665 7265 6e63 657d  t} ({difference}
-0001bfa0: 2529 220d 0a20 2020 2020 2020 2020 2020  %)"..           
-0001bfb0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0001bfc0: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-0001bfd0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001bfe0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001bff0: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-0001c000: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-0001c010: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
-0001c020: 6966 6665 7265 6e63 657d 2529 220d 0a20  ifference}%)".. 
-0001c030: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001c040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c050: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
-0001c060: 2d53 6967 6e61 6c22 5d20 3d20 280d 0a20  -Signal"] = (.. 
-0001c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c080: 2020 2073 6176 6564 5b30 5d20 0d0a 2020     saved[0] ..  
-0001c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0a0: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
-0001c0b0: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
-0001c0c0: 2020 2020 2020 2020 2b20 2863 6f6c 6f72          + (color
-0001c0d0: 5465 7874 2e47 5245 454e 2069 6620 6973  Text.GREEN if is
-0001c0e0: 3530 444d 4155 7054 7265 6e64 2065 6c73  50DMAUpTrend els
-0001c0f0: 6520 2863 6f6c 6f72 5465 7874 2e46 4149  e (colorText.FAI
-0001c100: 4c20 6966 2069 7335 3044 4d41 446f 776e  L if is50DMADown
-0001c110: 5472 656e 6420 656c 7365 2063 6f6c 6f72  Trend else color
-0001c120: 5465 7874 2e57 4152 4e29 290d 0a20 2020  Text.WARN))..   
-0001c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c140: 202b 2066 227b 636f 6e66 5465 7874 7d20   + f"{confText} 
-0001c150: 287b 6469 6666 6572 656e 6365 7d25 2922  ({difference}%)"
-0001c160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c170: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001c180: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-0001c190: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0001c1a0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-0001c1b0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-0001c1c0: 3d20 7361 7665 645b 315d 202b 2066 227b  = saved[1] + f"{
-0001c1d0: 636f 6e66 5465 7874 7d20 287b 6469 6666  confText} ({diff
-0001c1e0: 6572 656e 6365 7d25 2922 0d0a 2020 2020  erence}%)"..    
-0001c1f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-0001c200: 6f6e 6646 696c 7465 7220 3d3d 2033 206f  onfFilter == 3 o
-0001c210: 7220 5c0d 0a20 2020 2020 2020 2020 2020  r \..           
-0001c220: 2020 2020 2028 636f 6e66 4669 6c74 6572       (confFilter
-0001c230: 203d 3d20 3120 616e 6420 2869 7335 3044   == 1 and (is50D
-0001c240: 4d41 5570 5472 656e 6420 6f72 2028 6973  MAUpTrend or (is
-0001c250: 476f 6c64 656e 4372 6f73 734f 7665 7220  GoldenCrossOver 
-0001c260: 6f72 2027 5570 2720 696e 2063 6f6e 6654  or 'Up' in confT
-0001c270: 6578 7429 2929 206f 7220 5c0d 0a20 2020  ext))) or \..   
-0001c280: 2020 2020 2020 2020 2020 2020 2028 636f               (co
-0001c290: 6e66 4669 6c74 6572 203d 3d20 3220 616e  nfFilter == 2 an
-0001c2a0: 6420 2869 7335 3044 4d41 446f 776e 5472  d (is50DMADownTr
-0001c2b0: 656e 6420 6f72 2069 7344 6561 6443 726f  end or isDeadCro
-0001c2c0: 7373 4f76 6572 206f 7220 2744 6f77 6e27  ssOver or 'Down'
-0001c2d0: 2069 6e20 636f 6e66 5465 7874 2929 0d0a   in confText))..
-0001c2e0: 2020 2020 2020 2020 2320 4d61 7962 6520          # Maybe 
-0001c2f0: 7468 6520 6469 6666 6572 656e 6365 2069  the difference i
-0001c300: 7320 6e6f 7420 7769 7468 696e 2074 6865  s not within the
-0001c310: 2072 616e 6765 2c20 6275 7420 7765 2764   range, but we'd
-0001c320: 2073 7469 6c6c 206c 696b 6520 746f 206b   still like to k
-0001c330: 6565 7020 7468 6520 7374 6f63 6b20 696e  eep the stock in
-0001c340: 0d0a 2020 2020 2020 2020 2320 7468 6520  ..        # the 
-0001c350: 6c69 7374 2069 6620 6974 2773 2061 2067  list if it's a g
-0001c360: 6f6c 6465 6e20 6372 6f73 736f 7665 7220  olden crossover 
-0001c370: 6f72 2064 6561 6420 6372 6f73 736f 7665  or dead crossove
-0001c380: 720d 0a20 2020 2020 2020 2069 6620 6973  r..        if is
-0001c390: 476f 6c64 656e 4372 6f73 734f 7665 7220  GoldenCrossOver 
-0001c3a0: 6f72 2069 7344 6561 6443 726f 7373 4f76  or isDeadCrossOv
-0001c3b0: 6572 3a0d 0a20 2020 2020 2020 2020 2020  er:..           
-0001c3c0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
-0001c3d0: 5369 676e 616c 225d 203d 2028 0d0a 2020  Signal"] = (..  
-0001c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3f0: 2020 7361 7665 645b 305d 200d 0a20 2020    saved[0] ..   
-0001c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c410: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-0001c420: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-0001c430: 2020 2020 2020 202b 2028 636f 6c6f 7254         + (colorT
-0001c440: 6578 742e 4752 4545 4e20 6966 2069 7335  ext.GREEN if is5
-0001c450: 3044 4d41 5570 5472 656e 6420 656c 7365  0DMAUpTrend else
-0001c460: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
-0001c470: 2069 6620 6973 3530 444d 4144 6f77 6e54   if is50DMADownT
-0001c480: 7265 6e64 2065 6c73 6520 636f 6c6f 7254  rend else colorT
-0001c490: 6578 742e 5741 524e 2929 0d0a 2020 2020  ext.WARN))..    
-0001c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c4b0: 2b20 6622 7b63 6f6e 6654 6578 747d 2028  + f"{confText} (
-0001c4c0: 7b64 6966 6665 7265 6e63 657d 2529 220d  {difference}%)".
-0001c4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c4e0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001c4f0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-0001c500: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001c510: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
-0001c520: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
-0001c530: 6564 5b31 5d20 2b20 6622 7b63 6f6e 6654  ed[1] + f"{confT
-0001c540: 6578 747d 2028 7b64 6966 6665 7265 6e63  ext} ({differenc
-0001c550: 657d 2529 220d 0a20 2020 2020 2020 2020  e}%)"..         
-0001c560: 2020 2072 6574 7572 6e20 636f 6e66 4669     return confFi
-0001c570: 6c74 6572 203d 3d20 3320 6f72 205c 0d0a  lter == 3 or \..
-0001c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c590: 2863 6f6e 6646 696c 7465 7220 3d3d 2031  (confFilter == 1
-0001c5a0: 2061 6e64 2069 7347 6f6c 6465 6e43 726f   and isGoldenCro
-0001c5b0: 7373 4f76 6572 2920 6f72 205c 0d0a 2020  ssOver) or \..  
-0001c5c0: 2020 2020 2020 2020 2020 2020 2020 2863                (c
-0001c5d0: 6f6e 6646 696c 7465 7220 3d3d 2032 2061  onfFilter == 2 a
-0001c5e0: 6e64 2069 7344 6561 6443 726f 7373 4f76  nd isDeadCrossOv
-0001c5f0: 6572 290d 0a20 2020 2020 2020 2072 6574  er)..        ret
-0001c600: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-0001c610: 2023 406d 6561 7375 7265 5f74 696d 650d   #@measure_time.
-0001c620: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
-0001c630: 6966 2073 6861 7265 2070 7269 6365 7320  if share prices 
-0001c640: 6172 6520 636f 6e73 6f6c 6964 6174 696e  are consolidatin
-0001c650: 670d 0a20 2020 2064 6566 2076 616c 6964  g..    def valid
-0001c660: 6174 6543 6f6e 736f 6c69 6461 7469 6f6e  ateConsolidation
-0001c670: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
-0001c680: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-0001c690: 2070 6572 6365 6e74 6167 653d 3130 293a   percentage=10):
-0001c6a0: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
-0001c6b0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-0001c6c0: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
-0001c6d0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001c6e0: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
-0001c6f0: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
-0001c700: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001c710: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
-0001c720: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001c730: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-0001c740: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
-0001c750: 2020 2020 2020 2020 6863 203d 2064 6174          hc = dat
-0001c760: 612e 6465 7363 7269 6265 2829 5b22 436c  a.describe()["Cl
-0001c770: 6f73 6522 5d5b 226d 6178 225d 0d0a 2020  ose"]["max"]..  
-0001c780: 2020 2020 2020 6c63 203d 2064 6174 612e        lc = data.
-0001c790: 6465 7363 7269 6265 2829 5b22 436c 6f73  describe()["Clos
-0001c7a0: 6522 5d5b 226d 696e 225d 0d0a 2020 2020  e"]["min"]..    
-0001c7b0: 2020 2020 6966 2028 6863 202d 206c 6329      if (hc - lc)
-0001c7c0: 203c 3d20 2868 6320 2a20 7065 7263 656e   <= (hc * percen
-0001c7d0: 7461 6765 202f 2031 3030 2920 616e 6420  tage / 100) and 
-0001c7e0: 2868 6320 2d20 6c63 2021 3d20 3029 3a0d  (hc - lc != 0):.
-0001c7f0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-0001c800: 6565 6e44 6963 745b 2243 6f6e 736f 6c2e  eenDict["Consol.
-0001c810: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-0001c820: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
-0001c830: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
-0001c840: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001c850: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
-0001c860: 2020 2020 2020 2020 2020 202b 2022 5261             + "Ra
-0001c870: 6e67 653a 220d 0a20 2020 2020 2020 2020  nge:"..         
-0001c880: 2020 2020 2020 202b 2073 7472 2872 6f75         + str(rou
-0001c890: 6e64 2828 6162 7328 2868 6320 2d20 6c63  nd((abs((hc - lc
-0001c8a0: 2920 2f20 6863 2920 2a20 3130 3029 2c20  ) / hc) * 100), 
-0001c8b0: 3129 290d 0a20 2020 2020 2020 2020 2020  1))..           
-0001c8c0: 2020 2020 202b 2022 2522 0d0a 2020 2020       + "%"..    
-0001c8d0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001c8e0: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-0001c8f0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0001c900: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001c910: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001c920: 745b 2243 6f6e 736f 6c2e 225d 203d 2028  t["Consol."] = (
-0001c930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c940: 2020 636f 6c6f 7254 6578 742e 424f 4c44    colorText.BOLD
-0001c950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c960: 2020 2b20 636f 6c6f 7254 6578 742e 4641    + colorText.FA
-0001c970: 494c 0d0a 2020 2020 2020 2020 2020 2020  IL..            
-0001c980: 2020 2020 2b20 2252 616e 6765 3a22 0d0a      + "Range:"..
-0001c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9a0: 2b20 7374 7228 726f 756e 6428 2861 6273  + str(round((abs
-0001c9b0: 2828 6863 202d 206c 6329 202f 2068 6329  ((hc - lc) / hc)
-0001c9c0: 202a 2031 3030 292c 2031 2929 0d0a 2020   * 100), 1))..  
-0001c9d0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001c9e0: 2225 220d 0a20 2020 2020 2020 2020 2020  "%"..           
-0001c9f0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001ca00: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-0001ca10: 2020 290d 0a20 2020 2020 2020 2073 6176    )..        sav
-0001ca20: 6544 6963 745b 2243 6f6e 736f 6c2e 225d  eDict["Consol."]
-0001ca30: 203d 2066 2752 616e 6765 3a7b 7374 7228   = f'Range:{str(
-0001ca40: 726f 756e 6428 2861 6273 2828 6863 2d6c  round((abs((hc-l
-0001ca50: 6329 2f68 6329 2a31 3030 292c 3129 292b  c)/hc)*100),1))+
-0001ca60: 2225 227d 270d 0a20 2020 2020 2020 2072  "%"}'..        r
-0001ca70: 6574 7572 6e20 726f 756e 6428 2861 6273  eturn round((abs
-0001ca80: 2828 6863 202d 206c 6329 202f 2068 6329  ((hc - lc) / hc)
-0001ca90: 202a 2031 3030 292c 2031 290d 0a0d 0a20   * 100), 1).... 
-0001caa0: 2020 2023 2076 616c 6964 6174 6520 6966     # validate if
-0001cab0: 2074 6865 2073 746f 636b 2068 6173 2062   the stock has b
-0001cac0: 6565 6e20 6861 7669 6e67 2068 6967 6865  een having highe
-0001cad0: 7220 6869 6768 732c 2068 6967 6865 7220  r highs, higher 
-0001cae0: 6c6f 7773 0d0a 2020 2020 2320 616e 6420  lows..    # and 
-0001caf0: 6869 6768 6572 2063 6c6f 7365 2077 6974  higher close wit
-0001cb00: 6820 6c61 7465 7374 2063 6c6f 7365 203e  h latest close >
-0001cb10: 2073 7570 6572 7472 656e 6420 616e 6420   supertrend and 
-0001cb20: 382d 454d 412e 0d0a 2020 2020 6465 6620  8-EMA...    def 
-0001cb30: 7661 6c69 6461 7465 4869 6768 6572 4869  validateHigherHi
-0001cb40: 6768 7348 6967 6865 724c 6f77 7348 6967  ghsHigherLowsHig
-0001cb50: 6865 7243 6c6f 7365 2873 656c 662c 2064  herClose(self, d
-0001cb60: 6629 3a0d 0a20 2020 2020 2020 2069 6620  f):..        if 
-0001cb70: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-0001cb80: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
-0001cb90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001cba0: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
-0001cbb0: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
-0001cbc0: 0a20 2020 2020 2020 2064 6179 3020 3d20  .        day0 = 
-0001cbd0: 6461 7461 0d0a 2020 2020 2020 2020 6461  data..        da
-0001cbe0: 7931 203d 2064 6174 615b 313a 5d0d 0a20  y1 = data[1:].. 
-0001cbf0: 2020 2020 2020 2064 6179 3220 3d20 6461         day2 = da
-0001cc00: 7461 5b32 3a5d 0d0a 2020 2020 2020 2020  ta[2:]..        
-0001cc10: 6461 7933 203d 2064 6174 615b 333a 5d0d  day3 = data[3:].
-0001cc20: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0001cc30: 6461 7931 2920 3c20 3120 6f72 206c 656e  day1) < 1 or len
-0001cc40: 2864 6179 3229 203c 2031 206f 7220 6c65  (day2) < 1 or le
-0001cc50: 6e28 6461 7933 2920 3c20 313a 0d0a 2020  n(day3) < 1:..  
-0001cc60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001cc70: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0001cc80: 6869 6768 6572 4869 6768 7320 3d20 280d  higherHighs = (.
-0001cc90: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
-0001cca0: 7930 5b22 4869 6768 225d 2e69 6c6f 635b  y0["High"].iloc[
-0001ccb0: 305d 203e 2064 6179 315b 2248 6967 6822  0] > day1["High"
-0001ccc0: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
-0001ccd0: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
-0001cce0: 315b 2248 6967 6822 5d2e 696c 6f63 5b30  1["High"].iloc[0
-0001ccf0: 5d20 3e20 6461 7932 5b22 4869 6768 225d  ] > day2["High"]
-0001cd00: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
-0001cd10: 2020 2020 2020 2061 6e64 2028 6461 7932         and (day2
-0001cd20: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
-0001cd30: 203e 2064 6179 335b 2248 6967 6822 5d2e   > day3["High"].
-0001cd40: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
-0001cd50: 2020 290d 0a20 2020 2020 2020 2068 6967    )..        hig
-0001cd60: 6865 724c 6f77 7320 3d20 280d 0a20 2020  herLows = (..   
-0001cd70: 2020 2020 2020 2020 2028 6461 7930 5b22           (day0["
-0001cd80: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3e20  Low"].iloc[0] > 
-0001cd90: 6461 7931 5b22 4c6f 7722 5d2e 696c 6f63  day1["Low"].iloc
-0001cda0: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
-0001cdb0: 2020 616e 6420 2864 6179 315b 224c 6f77    and (day1["Low
-0001cdc0: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
-0001cdd0: 325b 224c 6f77 225d 2e69 6c6f 635b 305d  2["Low"].iloc[0]
-0001cde0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-0001cdf0: 6e64 2028 6461 7932 5b22 4c6f 7722 5d2e  nd (day2["Low"].
-0001ce00: 696c 6f63 5b30 5d20 3e20 6461 7933 5b22  iloc[0] > day3["
-0001ce10: 4c6f 7722 5d2e 696c 6f63 5b30 5d29 0d0a  Low"].iloc[0])..
-0001ce20: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001ce30: 2020 2068 6967 6865 7243 6c6f 7365 203d     higherClose =
-0001ce40: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0001ce50: 2864 6179 305b 2243 6c6f 7365 225d 2e69  (day0["Close"].i
-0001ce60: 6c6f 635b 305d 203e 2064 6179 315b 2243  loc[0] > day1["C
-0001ce70: 6c6f 7365 225d 2e69 6c6f 635b 305d 290d  lose"].iloc[0]).
-0001ce80: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001ce90: 2028 6461 7931 5b22 436c 6f73 6522 5d2e   (day1["Close"].
-0001cea0: 696c 6f63 5b30 5d20 3e20 6461 7932 5b22  iloc[0] > day2["
-0001ceb0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d29  Close"].iloc[0])
-0001cec0: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
-0001ced0: 6420 2864 6179 325b 2243 6c6f 7365 225d  d (day2["Close"]
-0001cee0: 2e69 6c6f 635b 305d 203e 2064 6179 335b  .iloc[0] > day3[
-0001cef0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-0001cf00: 290d 0a20 2020 2020 2020 2029 0d0a 2020  )..        )..  
-0001cf10: 2020 2020 2020 2320 6869 6768 6572 5253        # higherRS
-0001cf20: 4920 3d20 2864 6179 305b 2252 5349 225d  I = (day0["RSI"]
-0001cf30: 2e69 6c6f 635b 305d 203e 2064 6179 315b  .iloc[0] > day1[
-0001cf40: 2252 5349 225d 2e69 6c6f 635b 305d 2920  "RSI"].iloc[0]) 
-0001cf50: 616e 6420 5c0d 0a20 2020 2020 2020 2023  and \..        #
-0001cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf70: 2028 6461 7931 5b22 5253 4922 5d2e 696c   (day1["RSI"].il
-0001cf80: 6f63 5b30 5d20 3e20 6461 7932 5b22 5253  oc[0] > day2["RS
-0001cf90: 4922 5d2e 696c 6f63 5b30 5d29 2061 6e64  I"].iloc[0]) and
-0001cfa0: 205c 0d0a 2020 2020 2020 2020 2320 2020   \..        #   
-0001cfb0: 2020 2020 2020 2020 2020 2020 2020 2864                (d
-0001cfc0: 6179 325b 2252 5349 225d 2e69 6c6f 635b  ay2["RSI"].iloc[
-0001cfd0: 305d 203e 2064 6179 335b 2252 5349 225d  0] > day3["RSI"]
-0001cfe0: 2e69 6c6f 635b 305d 2920 616e 6420 5c0d  .iloc[0]) and \.
-0001cff0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0001d000: 2020 2020 2020 2020 2020 2064 6179 335b             day3[
-0001d010: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
-0001d020: 3d20 3530 2061 6e64 2064 6179 305b 2252  = 50 and day0["R
-0001d030: 5349 225d 2e69 6c6f 635b 305d 203e 3d20  SI"].iloc[0] >= 
-0001d040: 3635 0d0a 2020 2020 2020 2020 7265 7665  65..        reve
-0001d050: 7273 6564 4461 7461 203d 2064 6174 615b  rsedData = data[
-0001d060: 3a3a 2d31 5d2e 636f 7079 2829 0d0a 2020  ::-1].copy()..  
-0001d070: 2020 2020 2020 7265 7665 7273 6564 4461        reversedDa
-0001d080: 7461 5b22 5355 5045 5254 225d 203d 2070  ta["SUPERT"] = p
-0001d090: 6b74 616c 6962 2e73 7570 6572 7472 656e  ktalib.supertren
-0001d0a0: 6428 7265 7665 7273 6564 4461 7461 2c20  d(reversedData, 
-0001d0b0: 372c 2033 295b 2253 5550 4552 545f 375f  7, 3)["SUPERT_7_
-0001d0c0: 332e 3022 5d0d 0a20 2020 2020 2020 2072  3.0"]..        r
-0001d0d0: 6576 6572 7365 6444 6174 615b 2245 4d41  eversedData["EMA
-0001d0e0: 3822 5d20 3d20 706b 7461 6c69 622e 454d  8"] = pktalib.EM
-0001d0f0: 4128 7265 7665 7273 6564 4461 7461 5b22  A(reversedData["
-0001d100: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0001d110: 696f 643d 3929 0d0a 2020 2020 2020 2020  iod=9)..        
-0001d120: 6869 6768 6572 436c 6f73 6520 3d20 280d  higherClose = (.
-0001d130: 0a20 2020 2020 2020 2020 2020 2068 6967  .            hig
-0001d140: 6865 7243 6c6f 7365 0d0a 2020 2020 2020  herClose..      
-0001d150: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
-0001d160: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-0001d170: 3e20 7265 7665 7273 6564 4461 7461 2e74  > reversedData.t
-0001d180: 6169 6c28 3129 5b22 5355 5045 5254 225d  ail(1)["SUPERT"]
-0001d190: 2e69 6c6f 635b 305d 0d0a 2020 2020 2020  .iloc[0]..      
-0001d1a0: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
-0001d1b0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-0001d1c0: 3e20 7265 7665 7273 6564 4461 7461 2e74  > reversedData.t
-0001d1d0: 6169 6c28 3129 5b22 454d 4138 225d 2e69  ail(1)["EMA8"].i
-0001d1e0: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
-0001d1f0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0001d200: 6e20 6869 6768 6572 4869 6768 7320 616e  n higherHighs an
-0001d210: 6420 6869 6768 6572 4c6f 7773 2061 6e64  d higherLows and
-0001d220: 2068 6967 6865 7243 6c6f 7365 0d0a 0d0a   higherClose....
-0001d230: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-0001d240: 6d65 0d0a 2020 2020 2320 5661 6c69 6461  me..    # Valida
-0001d250: 7465 2027 496e 7369 6465 2042 6172 2720  te 'Inside Bar' 
-0001d260: 7374 7275 6374 7572 6520 666f 7220 7265  structure for re
-0001d270: 6365 6e74 2064 6179 730d 0a20 2020 2064  cent days..    d
-0001d280: 6566 2076 616c 6964 6174 6549 6e73 6964  ef validateInsid
-0001d290: 6542 6172 280d 0a20 2020 2020 2020 2073  eBar(..        s
-0001d2a0: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
-0001d2b0: 6963 742c 2073 6176 6544 6963 742c 2063  ict, saveDict, c
-0001d2c0: 6861 7274 5061 7474 6572 6e3d 312c 2064  hartPattern=1, d
-0001d2d0: 6179 7354 6f4c 6f6f 6b62 6163 6b3d 350d  aysToLookback=5.
-0001d2e0: 0a20 2020 2029 3a0d 0a20 2020 2020 2020  .    ):..       
-0001d2f0: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-0001d300: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0d  r len(df) == 0:.
-0001d310: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001d320: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
-0001d330: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-0001d340: 7928 290d 0a20 2020 2020 2020 206f 7267  y()..        org
-0001d350: 4461 7461 203d 2064 6174 610d 0a20 2020  Data = data..   
-0001d360: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-0001d370: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-0001d380: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-0001d390: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
-0001d3a0: 6174 7465 726e 2229 0d0a 2020 2020 2020  attern")..      
-0001d3b0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0001d3c0: 2869 6e74 2864 6179 7354 6f4c 6f6f 6b62  (int(daysToLookb
-0001d3d0: 6163 6b29 2c20 696e 7428 726f 756e 6428  ack), int(round(
-0001d3e0: 6461 7973 546f 4c6f 6f6b 6261 636b 202a  daysToLookback *
-0001d3f0: 2030 2e35 2929 202d 2031 2c20 2d31 293a   0.5)) - 1, -1):
-0001d400: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001d410: 2069 203d 3d20 323a 0d0a 2020 2020 2020   i == 2:..      
-0001d420: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001d430: 2030 2020 2320 4578 6974 2069 6620 6f6e   0  # Exit if on
-0001d440: 6c79 206c 6173 7420 3220 6361 6e64 6c65  ly last 2 candle
-0001d450: 7320 6172 6520 6c65 6674 0d0a 2020 2020  s are left..    
-0001d460: 2020 2020 2020 2020 6966 2063 6861 7274          if chart
-0001d470: 5061 7474 6572 6e20 3d3d 2031 3a0d 0a20  Pattern == 1:.. 
-0001d480: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001d490: 6620 2255 7022 2069 6e20 7361 7665 4469  f "Up" in saveDi
-0001d4a0: 6374 5b22 5472 656e 6422 5d20 616e 6420  ct["Trend"] and 
-0001d4b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0001d4c0: 2020 2020 2020 2022 4275 6c6c 2220 696e         "Bull" in
-0001d4d0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-0001d4e0: 676e 616c 225d 0d0a 2020 2020 2020 2020  gnal"]..        
-0001d4f0: 2020 2020 2020 2020 2020 2020 6f72 2022              or "
-0001d500: 5375 7070 6f72 7422 2069 6e20 7361 7665  Support" in save
-0001d510: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-0001d520: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001d530: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-0001d540: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-0001d550: 3d20 6f72 6744 6174 612e 6865 6164 2869  = orgData.head(i
-0001d560: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001d570: 2020 2020 2020 2072 6566 4361 6e64 6c65         refCandle
-0001d580: 203d 2064 6174 612e 7461 696c 2831 290d   = data.tail(1).
-0001d590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d5a0: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-0001d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5c0: 2020 2028 6c65 6e28 6461 7461 2e48 6967     (len(data.Hig
-0001d5d0: 685b 6461 7461 2e48 6967 6820 3e20 7265  h[data.High > re
-0001d5e0: 6643 616e 646c 652e 4869 6768 2e69 7465  fCandle.High.ite
-0001d5f0: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
-0001d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d610: 2020 2020 2061 6e64 2028 6c65 6e28 6461       and (len(da
-0001d620: 7461 2e4c 6f77 5b64 6174 612e 4c6f 7720  ta.Low[data.Low 
-0001d630: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
-0001d640: 6974 656d 2829 5d29 203d 3d20 3029 0d0a  item()]) == 0)..
-0001d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d660: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
-0001d670: 2864 6174 612e 4f70 656e 5b64 6174 612e  (data.Open[data.
-0001d680: 4f70 656e 203e 2072 6566 4361 6e64 6c65  Open > refCandle
-0001d690: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
-0001d6a0: 3d20 3029 0d0a 2020 2020 2020 2020 2020  = 0)..          
-0001d6b0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0001d6c0: 6420 286c 656e 2864 6174 612e 436c 6f73  d (len(data.Clos
-0001d6d0: 655b 6461 7461 2e43 6c6f 7365 203c 2072  e[data.Close < r
-0001d6e0: 6566 4361 6e64 6c65 2e4c 6f77 2e69 7465  efCandle.Low.ite
-0001d6f0: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
-0001d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d710: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-0001d720: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-0001d730: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
-0001d740: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-0001d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d760: 2020 2020 7361 7665 645b 305d 0d0a 2020      saved[0]..  
-0001d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d780: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001d790: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
-0001d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7b0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001d7c0: 6578 742e 5741 524e 0d0a 2020 2020 2020  ext.WARN..      
-0001d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7e0: 2020 2020 2020 2b20 2822 496e 7369 6465        + ("Inside
-0001d7f0: 2042 6172 2028 2564 2922 2025 2069 290d   Bar (%d)" % i).
-0001d800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d810: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001d820: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-0001d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d840: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d860: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
-0001d870: 726e 225d 203d 2073 6176 6564 5b31 5d20  rn"] = saved[1] 
-0001d880: 2b20 2249 6e73 6964 6520 4261 7220 2825  + "Inside Bar (%
-0001d890: 6429 2220 2520 690d 0a20 2020 2020 2020  d)" % i..       
-0001d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8b0: 2072 6574 7572 6e20 690d 0a20 2020 2020   return i..     
-0001d8c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001d8d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d8e0: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
-0001d8f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001d900: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001d910: 2020 2069 6620 2244 6f77 6e22 2069 6e20     if "Down" in 
-0001d920: 7361 7665 4469 6374 5b22 5472 656e 6422  saveDict["Trend"
-0001d930: 5d20 616e 6420 280d 0a20 2020 2020 2020  ] and (..       
-0001d940: 2020 2020 2020 2020 2020 2020 2022 4265               "Be
-0001d950: 6172 2220 696e 2073 6176 6544 6963 745b  ar" in saveDict[
-0001d960: 224d 412d 5369 676e 616c 225d 206f 7220  "MA-Signal"] or 
-0001d970: 2252 6573 6973 7422 2069 6e20 7361 7665  "Resist" in save
-0001d980: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-0001d990: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001d9a0: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-0001d9b0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-0001d9c0: 3d20 6f72 6744 6174 612e 6865 6164 2869  = orgData.head(i
-0001d9d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001d9e0: 2020 2020 2020 2072 6566 4361 6e64 6c65         refCandle
-0001d9f0: 203d 2064 6174 612e 7461 696c 2831 290d   = data.tail(1).
-0001da00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001da10: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-0001da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da30: 2020 2028 6c65 6e28 6461 7461 2e48 6967     (len(data.Hig
-0001da40: 685b 6461 7461 2e48 6967 6820 3e20 7265  h[data.High > re
-0001da50: 6643 616e 646c 652e 4869 6768 2e69 7465  fCandle.High.ite
-0001da60: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
-0001da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da80: 2020 2020 2061 6e64 2028 6c65 6e28 6461       and (len(da
-0001da90: 7461 2e4c 6f77 5b64 6174 612e 4c6f 7720  ta.Low[data.Low 
-0001daa0: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
-0001dab0: 6974 656d 2829 5d29 203d 3d20 3029 0d0a  item()]) == 0)..
-0001dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dad0: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
-0001dae0: 2864 6174 612e 4f70 656e 5b64 6174 612e  (data.Open[data.
-0001daf0: 4f70 656e 203e 2072 6566 4361 6e64 6c65  Open > refCandle
-0001db00: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
-0001db10: 3d20 3029 0d0a 2020 2020 2020 2020 2020  = 0)..          
-0001db20: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0001db30: 6420 286c 656e 2864 6174 612e 436c 6f73  d (len(data.Clos
-0001db40: 655b 6461 7461 2e43 6c6f 7365 203c 2072  e[data.Close < r
-0001db50: 6566 4361 6e64 6c65 2e4c 6f77 2e69 7465  efCandle.Low.ite
-0001db60: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
-0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db80: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-0001db90: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-0001dba0: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
-0001dbb0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-0001dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbd0: 2020 2020 7361 7665 645b 305d 0d0a 2020      saved[0]..  
-0001dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbf0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001dc00: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
-0001dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc20: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001dc30: 6578 742e 5741 524e 0d0a 2020 2020 2020  ext.WARN..      
-0001dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc50: 2020 2020 2020 2b20 2822 496e 7369 6465        + ("Inside
-0001dc60: 2042 6172 2028 2564 2922 2025 2069 290d   Bar (%d)" % i).
-0001dc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dc80: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001dc90: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-0001dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcb0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcd0: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
-0001dce0: 726e 225d 203d 2073 6176 6564 5b31 5d20  rn"] = saved[1] 
-0001dcf0: 2b20 2249 6e73 6964 6520 4261 7220 2825  + "Inside Bar (%
-0001dd00: 6429 2220 2520 690d 0a20 2020 2020 2020  d)" % i..       
-0001dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd20: 2072 6574 7572 6e20 690d 0a20 2020 2020   return i..     
-0001dd30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001dd40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dd50: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
-0001dd60: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
-0001dd70: 0d0a 0d0a 2020 2020 2320 4669 6e64 2049  ....    # Find I
-0001dd80: 504f 2062 6173 650d 0a20 2020 2064 6566  PO base..    def
-0001dd90: 2076 616c 6964 6174 6549 706f 4261 7365   validateIpoBase
-0001dda0: 2873 656c 662c 2073 746f 636b 2c20 6466  (self, stock, df
-0001ddb0: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
-0001ddc0: 7665 4469 6374 2c20 7065 7263 656e 7461  veDict, percenta
-0001ddd0: 6765 3d30 2e33 293a 0d0a 2020 2020 2020  ge=0.3):..      
-0001dde0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-0001ddf0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-0001de00: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001de10: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
-0001de20: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-0001de30: 7079 2829 0d0a 2020 2020 2020 2020 6c69  py()..        li
-0001de40: 7374 696e 6750 7269 6365 203d 2064 6174  stingPrice = dat
-0001de50: 615b 3a3a 2d31 5d2e 6865 6164 2831 295b  a[::-1].head(1)[
-0001de60: 224f 7065 6e22 5d2e 696c 6f63 5b30 5d0d  "Open"].iloc[0].
-0001de70: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
-0001de80: 5072 6963 6520 3d20 6461 7461 2e68 6561  Price = data.hea
-0001de90: 6428 3129 5b22 436c 6f73 6522 5d2e 696c  d(1)["Close"].il
-0001dea0: 6f63 5b30 5d0d 0a20 2020 2020 2020 2041  oc[0]..        A
-0001deb0: 5448 203d 2064 6174 612e 6465 7363 7269  TH = data.descri
-0001dec0: 6265 2829 5b22 4869 6768 225d 5b22 6d61  be()["High"]["ma
-0001ded0: 7822 5d0d 0a20 2020 2020 2020 2069 6620  x"]..        if 
-0001dee0: 4154 4820 3e20 286c 6973 7469 6e67 5072  ATH > (listingPr
-0001def0: 6963 6520 2b20 286c 6973 7469 6e67 5072  ice + (listingPr
-0001df00: 6963 6520 2a20 7065 7263 656e 7461 6765  ice * percentage
-0001df10: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-0001df20: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-0001df30: 2020 2020 2020 2061 7761 7920 3d20 726f         away = ro
-0001df40: 756e 6428 2828 6375 7272 656e 7450 7269  und(((currentPri
-0001df50: 6365 202d 206c 6973 7469 6e67 5072 6963  ce - listingPric
-0001df60: 6529 202f 206c 6973 7469 6e67 5072 6963  e) / listingPric
-0001df70: 6529 202a 2031 3030 2c20 3129 0d0a 2020  e) * 100, 1)..  
-0001df80: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
-0001df90: 2020 2020 2020 2020 286c 6973 7469 6e67          (listing
-0001dfa0: 5072 6963 6520 2d20 286c 6973 7469 6e67  Price - (listing
-0001dfb0: 5072 6963 6520 2a20 7065 7263 656e 7461  Price * percenta
-0001dfc0: 6765 2929 0d0a 2020 2020 2020 2020 2020  ge))..          
-0001dfd0: 2020 3c3d 2063 7572 7265 6e74 5072 6963    <= currentPric
-0001dfe0: 650d 0a20 2020 2020 2020 2020 2020 203c  e..            <
-0001dff0: 3d20 286c 6973 7469 6e67 5072 6963 6520  = (listingPrice 
-0001e000: 2b20 286c 6973 7469 6e67 5072 6963 6520  + (listingPrice 
-0001e010: 2a20 7065 7263 656e 7461 6765 2929 0d0a  * percentage))..
-0001e020: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-0001e030: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
-0001e040: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
-0001e050: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
-0001e060: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-0001e070: 2022 5061 7474 6572 6e22 290d 0a20 2020   "Pattern")..   
-0001e080: 2020 2020 2020 2020 2069 6620 6177 6179           if away
-0001e090: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-0001e0a0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001e0b0: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-0001e0c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e0d0: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
-0001e0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e0f0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001e100: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
-0001e110: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001e120: 6f72 5465 7874 2e47 5245 454e 0d0a 2020  orText.GREEN..  
-0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e140: 2020 2b20 6622 4950 4f20 4261 7365 2028    + f"IPO Base (
-0001e150: 7b61 7761 797d 2025 2922 0d0a 2020 2020  {away} %)"..    
-0001e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e170: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-0001e180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e190: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0001e1a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0001e1b0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001e1c0: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-0001e1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e1e0: 2020 2020 2020 7361 7665 645b 305d 0d0a        saved[0]..
-0001e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e200: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-0001e210: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
-0001e220: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001e230: 7254 6578 742e 4752 4545 4e0d 0a20 2020  rText.GREEN..   
-0001e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e250: 202b 2022 4950 4f20 4261 7365 2022 0d0a   + "IPO Base "..
-0001e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e270: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-0001e280: 4641 494c 0d0a 2020 2020 2020 2020 2020  FAIL..          
-0001e290: 2020 2020 2020 2020 2020 2b20 6622 287b            + f"({
-0001e2a0: 6177 6179 7d20 2529 220d 0a20 2020 2020  away} %)"..     
-0001e2b0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001e2c0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
-0001e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2e0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0001e2f0: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-0001e300: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-0001e310: 6622 4950 4f20 4261 7365 2028 7b61 7761  f"IPO Base ({awa
-0001e320: 797d 2025 2922 0d0a 2020 2020 2020 2020  y} %)"..        
-0001e330: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
-0001e340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001e350: 4661 6c73 650d 0a0d 0a20 2020 2023 406d  False....    #@m
-0001e360: 6561 7375 7265 5f74 696d 650d 0a20 2020  easure_time..   
-0001e370: 2023 2056 616c 6964 6174 6520 4c6f 7265   # Validate Lore
-0001e380: 6e74 7a69 616e 2043 6c61 7373 6966 6963  ntzian Classific
-0001e390: 6174 696f 6e20 7369 676e 616c 0d0a 2020  ation signal..  
-0001e3a0: 2020 6465 6620 7661 6c69 6461 7465 4c6f    def validateLo
-0001e3b0: 7265 6e74 7a69 616e 2873 656c 662c 2064  rentzian(self, d
-0001e3c0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-0001e3d0: 6176 6544 6963 742c 206c 6f6f 6b46 6f72  aveDict, lookFor
-0001e3e0: 3d33 293a 0d0a 2020 2020 2020 2020 6966  =3):..        if
-0001e3f0: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
-0001e400: 656e 2864 6629 203d 3d20 303a 0d0a 2020  en(df) == 0:..  
-0001e410: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001e420: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0001e430: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-0001e440: 0d0a 2020 2020 2020 2020 2320 6c6f 6f6b  ..        # look
-0001e450: 466f 723a 2031 2d42 7579 2c20 322d 5365  For: 1-Buy, 2-Se
-0001e460: 6c6c 2c20 332d 416e 790d 0a20 2020 2020  ll, 3-Any..     
-0001e470: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
-0001e480: 3a2d 315d 2020 2320 5265 7665 7273 6520  :-1]  # Reverse 
-0001e490: 7468 6520 6461 7461 6672 616d 650d 0a20  the dataframe.. 
-0001e4a0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001e4b0: 7461 2e72 656e 616d 6528 0d0a 2020 2020  ta.rename(..    
-0001e4c0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-0001e4d0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-0001e4e0: 2020 2022 4f70 656e 223a 2022 6f70 656e     "Open": "open
-0001e4f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0001e500: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
-0001e510: 6f73 6522 2c0d 0a20 2020 2020 2020 2020  ose",..         
-0001e520: 2020 2020 2020 2022 4869 6768 223a 2022         "High": "
-0001e530: 6869 6768 222c 0d0a 2020 2020 2020 2020  high",..        
-0001e540: 2020 2020 2020 2020 224c 6f77 223a 2022          "Low": "
-0001e550: 6c6f 7722 2c0d 0a20 2020 2020 2020 2020  low",..         
-0001e560: 2020 2020 2020 2022 566f 6c75 6d65 223a         "Volume":
-0001e570: 2022 766f 6c75 6d65 222c 0d0a 2020 2020   "volume",..    
-0001e580: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-0001e590: 2020 2029 0d0a 2020 2020 2020 2020 7472     )..        tr
-0001e5a0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-0001e5b0: 7769 7468 2053 7570 7072 6573 734f 7574  with SuppressOut
-0001e5c0: 7075 7428 7375 7070 7265 7373 5f73 7464  put(suppress_std
-0001e5d0: 6f75 743d 5472 7565 2c20 7375 7070 7265  out=True, suppre
-0001e5e0: 7373 5f73 7464 6572 723d 5472 7565 293a  ss_stderr=True):
-0001e5f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e600: 2020 6c63 203d 2061 7461 2e4c 6f72 656e    lc = ata.Loren
-0001e610: 747a 6961 6e43 6c61 7373 6966 6963 6174  tzianClassificat
-0001e620: 696f 6e28 6461 7461 3d64 6174 6129 0d0a  ion(data=data)..
-0001e630: 2020 2020 2020 2020 2020 2020 7361 7665              save
-0001e640: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
-0001e650: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
-0001e660: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001e670: 6963 742c 2022 5061 7474 6572 6e22 290d  ict, "Pattern").
-0001e680: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001e690: 6c63 2e64 662e 696c 6f63 5b2d 315d 5b22  lc.df.iloc[-1]["
-0001e6a0: 6973 4e65 7742 7579 5369 676e 616c 225d  isNewBuySignal"]
-0001e6b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001e6c0: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-0001e6d0: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
-0001e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6f0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-0001e700: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-0001e710: 6c6f 7254 6578 742e 4752 4545 4e20 2b20  lorText.GREEN + 
-0001e720: 224c 6f72 656e 747a 6961 6e2d 4275 7922  "Lorentzian-Buy"
-0001e730: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-0001e740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e750: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-0001e760: 2020 2020 2073 6176 6544 6963 745b 2250       saveDict["P
-0001e770: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
-0001e780: 5b31 5d20 2b20 224c 6f72 656e 747a 6961  [1] + "Lorentzia
-0001e790: 6e2d 4275 7922 0d0a 2020 2020 2020 2020  n-Buy"..        
-0001e7a0: 2020 2020 2020 2020 6966 206c 6f6f 6b46          if lookF
-0001e7b0: 6f72 2021 3d20 323a 2023 204e 6f74 2053  or != 2: # Not S
-0001e7c0: 656c 6c0d 0a20 2020 2020 2020 2020 2020  ell..           
-0001e7d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001e7e0: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
-0001e7f0: 2020 656c 6966 206c 632e 6466 2e69 6c6f    elif lc.df.ilo
-0001e800: 635b 2d31 5d5b 2269 734e 6577 5365 6c6c  c[-1]["isNewSell
-0001e810: 5369 676e 616c 225d 3a0d 0a20 2020 2020  Signal"]:..     
-0001e820: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001e830: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-0001e840: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001e850: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-0001e860: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
-0001e870: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-0001e880: 4641 494c 202b 2022 4c6f 7265 6e74 7a69  FAIL + "Lorentzi
-0001e890: 616e 2d53 656c 6c22 202b 2063 6f6c 6f72  an-Sell" + color
-0001e8a0: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-0001e8b0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001e8c0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001e8d0: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
-0001e8e0: 203d 2073 6176 6564 5b31 5d20 2b20 224c   = saved[1] + "L
-0001e8f0: 6f72 656e 747a 6961 6e2d 5365 6c6c 220d  orentzian-Sell".
-0001e900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e910: 2069 6620 6c6f 6f6b 466f 7220 213d 2031   if lookFor != 1
-0001e920: 3a20 2320 4e6f 7420 4275 790d 0a20 2020  : # Not Buy..   
-0001e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e940: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
-0001e950: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-0001e960: 6570 7469 6f6e 3a20 2023 2070 7261 676d  eption:  # pragm
-0001e970: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
-0001e980: 2020 2020 2020 2020 2023 2056 616c 7565           # Value
-0001e990: 4572 726f 723a 206f 7065 7261 6e64 7320  Error: operands 
-0001e9a0: 636f 756c 6420 6e6f 7420 6265 2062 726f  could not be bro
-0001e9b0: 6164 6361 7374 2074 6f67 6574 6865 7220  adcast together 
-0001e9c0: 7769 7468 2073 6861 7065 7320 2832 302c  with shapes (20,
-0001e9d0: 2920 2832 362c 290d 0a20 2020 2020 2020  ) (26,)..       
-0001e9e0: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
-0001e9f0: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
-0001ea00: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
-0001ea10: 6163 6b61 6765 732f 6164 7661 6e63 6564  ackages/advanced
-0001ea20: 5f74 612f 4c6f 7265 6e74 7a69 616e 436c  _ta/LorentzianCl
-0001ea30: 6173 7369 6669 6361 7469 6f6e 2f43 6c61  assification/Cla
-0001ea40: 7373 6966 6965 722e 7079 222c 206c 696e  ssifier.py", lin
-0001ea50: 6520 3138 362c 2069 6e20 5f5f 696e 6974  e 186, in __init
-0001ea60: 5f5f 0d0a 2020 2020 2020 2020 2020 2020  __..            
-0001ea70: 2320 4669 6c65 2022 2f6f 7074 2f68 6f6d  # File "/opt/hom
-0001ea80: 6562 7265 772f 6c69 622f 7079 7468 6f6e  ebrew/lib/python
-0001ea90: 332e 3131 2f73 6974 652d 7061 636b 6167  3.11/site-packag
-0001eaa0: 6573 2f61 6476 616e 6365 645f 7461 2f4c  es/advanced_ta/L
-0001eab0: 6f72 656e 747a 6961 6e43 6c61 7373 6966  orentzianClassif
-0001eac0: 6963 6174 696f 6e2f 436c 6173 7369 6669  ication/Classifi
-0001ead0: 6572 2e70 7922 2c20 6c69 6e65 2033 3935  er.py", line 395
-0001eae0: 2c20 696e 205f 5f63 6c61 7373 6966 790d  , in __classify.
-0001eaf0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
-0001eb00: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
-0001eb10: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
-0001eb20: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
-0001eb30: 7061 6e64 6173 2f63 6f72 652f 6f70 732f  pandas/core/ops/
-0001eb40: 636f 6d6d 6f6e 2e70 7922 2c20 6c69 6e65  common.py", line
-0001eb50: 2037 362c 2069 6e20 6e65 775f 6d65 7468   76, in new_meth
-0001eb60: 6f64 0d0a 2020 2020 2020 2020 2020 2020  od..            
-0001eb70: 2320 4669 6c65 2022 2f6f 7074 2f68 6f6d  # File "/opt/hom
-0001eb80: 6562 7265 772f 6c69 622f 7079 7468 6f6e  ebrew/lib/python
-0001eb90: 332e 3131 2f73 6974 652d 7061 636b 6167  3.11/site-packag
-0001eba0: 6573 2f70 616e 6461 732f 636f 7265 2f61  es/pandas/core/a
-0001ebb0: 7272 6179 6c69 6b65 2e70 7922 2c20 6c69  rraylike.py", li
-0001ebc0: 6e65 2037 302c 2069 6e20 5f5f 616e 645f  ne 70, in __and_
-0001ebd0: 5f0d 0a20 2020 2020 2020 2020 2020 2023  _..            #
-0001ebe0: 2046 696c 6520 222f 6f70 742f 686f 6d65   File "/opt/home
-0001ebf0: 6272 6577 2f6c 6962 2f70 7974 686f 6e33  brew/lib/python3
-0001ec00: 2e31 312f 7369 7465 2d70 6163 6b61 6765  .11/site-package
-0001ec10: 732f 7061 6e64 6173 2f63 6f72 652f 7365  s/pandas/core/se
-0001ec20: 7269 6573 2e70 7922 2c20 6c69 6e65 2035  ries.py", line 5
-0001ec30: 3831 302c 2069 6e20 5f6c 6f67 6963 616c  810, in _logical
-0001ec40: 5f6d 6574 686f 640d 0a20 2020 2020 2020  _method..       
-0001ec50: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
-0001ec60: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
-0001ec70: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
-0001ec80: 6163 6b61 6765 732f 7061 6e64 6173 2f63  ackages/pandas/c
-0001ec90: 6f72 652f 6f70 732f 6172 7261 795f 6f70  ore/ops/array_op
-0001eca0: 732e 7079 222c 206c 696e 6520 3435 362c  s.py", line 456,
-0001ecb0: 2069 6e20 6c6f 6769 6361 6c5f 6f70 0d0a   in logical_op..
-0001ecc0: 2020 2020 2020 2020 2020 2020 2320 4669              # Fi
-0001ecd0: 6c65 2022 2f6f 7074 2f68 6f6d 6562 7265  le "/opt/homebre
-0001ece0: 772f 6c69 622f 7079 7468 6f6e 332e 3131  w/lib/python3.11
-0001ecf0: 2f73 6974 652d 7061 636b 6167 6573 2f70  /site-packages/p
-0001ed00: 616e 6461 732f 636f 7265 2f6f 7073 2f61  andas/core/ops/a
-0001ed10: 7272 6179 5f6f 7073 2e70 7922 2c20 6c69  rray_ops.py", li
-0001ed20: 6e65 2033 3634 2c20 696e 206e 615f 6c6f  ne 364, in na_lo
-0001ed30: 6769 6361 6c5f 6f70 0d0a 2020 2020 2020  gical_op..      
-0001ed40: 2020 2020 2020 2320 7365 6c66 2e64 6566        # self.def
-0001ed50: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
-0001ed60: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
-0001ed70: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-0001ed80: 2070 6173 730d 0a20 2020 2020 2020 2072   pass..        r
-0001ed90: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
-0001eda0: 2020 2023 2076 616c 6964 6174 6520 6966     # validate if
-0001edb0: 2074 6865 2073 746f 636b 2068 6173 2062   the stock has b
-0001edc0: 6565 6e20 6861 7669 6e67 206c 6f77 6572  een having lower
-0001edd0: 206c 6f77 732c 206c 6f77 6572 2068 6967   lows, lower hig
-0001ede0: 6873 0d0a 2020 2020 6465 6620 7661 6c69  hs..    def vali
-0001edf0: 6461 7465 4c6f 7765 7248 6967 6873 4c6f  dateLowerHighsLo
-0001ee00: 7765 724c 6f77 7328 7365 6c66 2c20 6466  werLows(self, df
-0001ee10: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-0001ee20: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001ee30: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-0001ee40: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001ee50: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-0001ee60: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001ee70: 2020 2020 2020 2020 6461 7930 203d 2064          day0 = d
-0001ee80: 6174 610d 0a20 2020 2020 2020 2064 6179  ata..        day
-0001ee90: 3120 3d20 6461 7461 5b31 3a5d 0d0a 2020  1 = data[1:]..  
-0001eea0: 2020 2020 2020 6461 7932 203d 2064 6174        day2 = dat
-0001eeb0: 615b 323a 5d0d 0a20 2020 2020 2020 2064  a[2:]..        d
-0001eec0: 6179 3320 3d20 6461 7461 5b33 3a5d 0d0a  ay3 = data[3:]..
-0001eed0: 2020 2020 2020 2020 6c6f 7765 7248 6967          lowerHig
-0001eee0: 6873 203d 2028 0d0a 2020 2020 2020 2020  hs = (..        
-0001eef0: 2020 2020 2864 6179 305b 2248 6967 6822      (day0["High"
-0001ef00: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7931  ].iloc[0] < day1
-0001ef10: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
-0001ef20: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-0001ef30: 6e64 2028 6461 7931 5b22 4869 6768 225d  nd (day1["High"]
-0001ef40: 2e69 6c6f 635b 305d 203c 2064 6179 325b  .iloc[0] < day2[
-0001ef50: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
-0001ef60: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
-0001ef70: 6420 2864 6179 325b 2248 6967 6822 5d2e  d (day2["High"].
-0001ef80: 696c 6f63 5b30 5d20 3c20 6461 7933 5b22  iloc[0] < day3["
-0001ef90: 4869 6768 225d 2e69 6c6f 635b 305d 290d  High"].iloc[0]).
-0001efa0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-0001efb0: 2020 2020 6c6f 7765 724c 6f77 7320 3d20      lowerLows = 
-0001efc0: 280d 0a20 2020 2020 2020 2020 2020 2028  (..            (
-0001efd0: 6461 7930 5b22 4c6f 7722 5d2e 696c 6f63  day0["Low"].iloc
-0001efe0: 5b30 5d20 3c20 6461 7931 5b22 4c6f 7722  [0] < day1["Low"
-0001eff0: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
-0001f000: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
-0001f010: 315b 224c 6f77 225d 2e69 6c6f 635b 305d  1["Low"].iloc[0]
-0001f020: 203c 2064 6179 325b 224c 6f77 225d 2e69   < day2["Low"].i
-0001f030: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
-0001f040: 2020 2020 2061 6e64 2028 6461 7932 5b22       and (day2["
-0001f050: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3c20  Low"].iloc[0] < 
-0001f060: 6461 7933 5b22 4c6f 7722 5d2e 696c 6f63  day3["Low"].iloc
-0001f070: 5b30 5d29 0d0a 2020 2020 2020 2020 290d  [0])..        ).
-0001f080: 0a20 2020 2020 2020 2068 6967 6865 7252  .        higherR
-0001f090: 5349 203d 2028 0d0a 2020 2020 2020 2020  SI = (..        
-0001f0a0: 2020 2020 2864 6179 305b 2252 5349 225d      (day0["RSI"]
-0001f0b0: 2e69 6c6f 635b 305d 203c 2064 6179 315b  .iloc[0] < day1[
-0001f0c0: 2252 5349 225d 2e69 6c6f 635b 305d 290d  "RSI"].iloc[0]).
-0001f0d0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001f0e0: 2028 6461 7931 5b22 5253 4922 5d2e 696c   (day1["RSI"].il
-0001f0f0: 6f63 5b30 5d20 3c20 6461 7932 5b22 5253  oc[0] < day2["RS
-0001f100: 4922 5d2e 696c 6f63 5b30 5d29 0d0a 2020  I"].iloc[0])..  
-0001f110: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
-0001f120: 6179 325b 2252 5349 225d 2e69 6c6f 635b  ay2["RSI"].iloc[
-0001f130: 305d 203c 2064 6179 335b 2252 5349 225d  0] < day3["RSI"]
-0001f140: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
-0001f150: 2020 2020 2020 2061 6e64 2064 6179 305b         and day0[
-0001f160: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
-0001f170: 3d20 3530 0d0a 2020 2020 2020 2020 290d  = 50..        ).
-0001f180: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001f190: 6c6f 7765 7248 6967 6873 2061 6e64 206c  lowerHighs and l
-0001f1a0: 6f77 6572 4c6f 7773 2061 6e64 2068 6967  owerLows and hig
-0001f1b0: 6865 7252 5349 0d0a 0d0a 2020 2020 2320  herRSI....    # 
-0001f1c0: 5661 6c69 6461 7465 2069 6620 7265 6365  Validate if rece
-0001f1d0: 6e74 2076 6f6c 756d 6520 6973 206c 6f77  nt volume is low
-0001f1e0: 6573 7420 6f66 206c 6173 7420 274e 2720  est of last 'N' 
-0001f1f0: 4461 7973 0d0a 2020 2020 6465 6620 7661  Days..    def va
-0001f200: 6c69 6461 7465 4c6f 7765 7374 566f 6c75  lidateLowestVolu
-0001f210: 6d65 2873 656c 662c 2064 662c 2064 6179  me(self, df, day
-0001f220: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
-0001f230: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-0001f240: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001f250: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-0001f260: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001f270: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-0001f280: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001f290: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001f2a0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-0001f2b0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001f2c0: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-0001f2d0: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-0001f2e0: 0d0a 2020 2020 2020 2020 6966 2064 6179  ..        if day
-0001f2f0: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
-0001f300: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-0001f310: 2020 2020 2020 2064 6179 7346 6f72 4c6f         daysForLo
-0001f320: 7765 7374 566f 6c75 6d65 203d 2033 300d  westVolume = 30.
-0001f330: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0001f340: 6461 7461 2920 3c20 6461 7973 466f 724c  data) < daysForL
-0001f350: 6f77 6573 7456 6f6c 756d 653a 0d0a 2020  owestVolume:..  
-0001f360: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001f370: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0001f380: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
-0001f390: 2864 6179 7346 6f72 4c6f 7765 7374 566f  (daysForLowestVo
-0001f3a0: 6c75 6d65 290d 0a20 2020 2020 2020 2072  lume)..        r
-0001f3b0: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
-0001f3c0: 6428 3129 0d0a 2020 2020 2020 2020 6966  d(1)..        if
-0001f3d0: 206c 656e 2872 6563 656e 7429 203c 2031   len(recent) < 1
-0001f3e0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0001f3f0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-0001f400: 2020 2020 2069 6620 2872 6563 656e 745b       if (recent[
-0001f410: 2256 6f6c 756d 6522 5d2e 696c 6f63 5b30  "Volume"].iloc[0
-0001f420: 5d20 3c3d 2064 6174 612e 6465 7363 7269  ] <= data.descri
-0001f430: 6265 2829 5b22 566f 6c75 6d65 225d 5b22  be()["Volume"]["
-0001f440: 6d69 6e22 5d29 2061 6e64 2072 6563 656e  min"]) and recen
-0001f450: 745b 0d0a 2020 2020 2020 2020 2020 2020  t[..            
-0001f460: 2256 6f6c 756d 6522 0d0a 2020 2020 2020  "Volume"..      
-0001f470: 2020 5d5b 305d 2021 3d20 6e70 2e6e 616e    ][0] != np.nan
-0001f480: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0001f490: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
-0001f4a0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0001f4b0: 0d0a 0d0a 2020 2020 2320 5661 6c69 6461  ....    # Valida
-0001f4c0: 7465 204c 5450 2077 6974 6869 6e20 6c69  te LTP within li
-0001f4d0: 6d69 7473 0d0a 2020 2020 6465 6620 7661  mits..    def va
-0001f4e0: 6c69 6461 7465 4c54 5028 7365 6c66 2c20  lidateLTP(self, 
-0001f4f0: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
-0001f500: 7361 7665 4469 6374 2c20 6d69 6e4c 5450  saveDict, minLTP
-0001f510: 3d4e 6f6e 652c 206d 6178 4c54 503d 4e6f  =None, maxLTP=No
-0001f520: 6e65 2c6d 696e 4368 616e 6765 3d30 293a  ne,minChange=0):
-0001f530: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-0001f540: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
-0001f550: 2020 2020 6c74 7056 616c 6964 203d 2046      ltpValid = F
-0001f560: 616c 7365 0d0a 2020 2020 2020 2020 6966  alse..        if
-0001f570: 206d 696e 4c54 5020 6973 204e 6f6e 653a   minLTP is None:
-0001f580: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-0001f590: 6e4c 5450 203d 2073 656c 662e 636f 6e66  nLTP = self.conf
-0001f5a0: 6967 4d61 6e61 6765 722e 6d69 6e4c 5450  igManager.minLTP
-0001f5b0: 0d0a 2020 2020 2020 2020 6966 206d 6178  ..        if max
-0001f5c0: 4c54 5020 6973 204e 6f6e 653a 0d0a 2020  LTP is None:..  
-0001f5d0: 2020 2020 2020 2020 2020 6d61 784c 5450            maxLTP
-0001f5e0: 203d 2073 656c 662e 636f 6e66 6967 4d61   = self.configMa
-0001f5f0: 6e61 6765 722e 6d61 784c 5450 0d0a 2020  nager.maxLTP..  
-0001f600: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001f610: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
-0001f620: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001f630: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-0001f640: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
-0001f650: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
-0001f660: 2064 6174 612e 6865 6164 2831 290d 0a0d   data.head(1)...
-0001f670: 0a20 2020 2020 2020 2070 6374 5f63 6861  .        pct_cha
-0001f680: 6e67 6520 3d20 2864 6174 615b 3a3a 2d31  nge = (data[::-1
-0001f690: 5d5b 2243 6c6f 7365 225d 2e70 6374 5f63  ]["Close"].pct_c
-0001f6a0: 6861 6e67 6528 2920 2a20 3130 3029 2e69  hange() * 100).i
-0001f6b0: 6c6f 635b 2d31 5d0d 0a20 2020 2020 2020  loc[-1]..       
-0001f6c0: 2069 6620 7063 745f 6368 616e 6765 203d   if pct_change =
-0001f6d0: 3d20 6e70 2e69 6e66 206f 7220 7063 745f  = np.inf or pct_
-0001f6e0: 6368 616e 6765 203d 3d20 2d6e 702e 696e  change == -np.in
-0001f6f0: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
-0001f700: 7063 745f 6368 616e 6765 203d 2030 0d0a  pct_change = 0..
-0001f710: 2020 2020 2020 2020 7063 745f 7361 7665          pct_save
-0001f720: 203d 2022 252e 3166 2525 2220 2520 7063   = "%.1f%%" % pc
-0001f730: 745f 6368 616e 6765 0d0a 2020 2020 2020  t_change..      
-0001f740: 2020 6966 2070 6374 5f63 6861 6e67 6520    if pct_change 
-0001f750: 3e20 302e 323a 0d0a 2020 2020 2020 2020  > 0.2:..        
-0001f760: 2020 2020 7063 745f 6368 616e 6765 203d      pct_change =
-0001f770: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-0001f780: 202b 2028 2225 2e31 6625 2522 2025 2070   + ("%.1f%%" % p
-0001f790: 6374 5f63 6861 6e67 6529 202b 2063 6f6c  ct_change) + col
-0001f7a0: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
-0001f7b0: 2020 2020 656c 6966 2070 6374 5f63 6861      elif pct_cha
-0001f7c0: 6e67 6520 3c20 2d30 2e32 3a0d 0a20 2020  nge < -0.2:..   
-0001f7d0: 2020 2020 2020 2020 2070 6374 5f63 6861           pct_cha
-0001f7e0: 6e67 6520 3d20 636f 6c6f 7254 6578 742e  nge = colorText.
-0001f7f0: 4641 494c 202b 2028 2225 2e31 6625 2522  FAIL + ("%.1f%%"
-0001f800: 2025 2070 6374 5f63 6861 6e67 6529 202b   % pct_change) +
-0001f810: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
-0001f820: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0001f830: 2020 2020 2020 2020 2020 2070 6374 5f63             pct_c
-0001f840: 6861 6e67 6520 3d20 636f 6c6f 7254 6578  hange = colorTex
-0001f850: 742e 5741 524e 202b 2028 2225 2e31 6625  t.WARN + ("%.1f%
-0001f860: 2522 2025 2070 6374 5f63 6861 6e67 6529  %" % pct_change)
-0001f870: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-0001f880: 0d0a 2020 2020 2020 2020 7361 7665 4469  ..        saveDi
-0001f890: 6374 5b22 2543 686e 6722 5d20 3d20 7063  ct["%Chng"] = pc
-0001f8a0: 745f 7361 7665 0d0a 2020 2020 2020 2020  t_save..        
-0001f8b0: 7363 7265 656e 4469 6374 5b22 2543 686e  screenDict["%Chn
-0001f8c0: 6722 5d20 3d20 7063 745f 6368 616e 6765  g"] = pct_change
-0001f8d0: 0d0a 2020 2020 2020 2020 6c74 7020 3d20  ..        ltp = 
-0001f8e0: 726f 756e 6428 7265 6365 6e74 5b22 436c  round(recent["Cl
-0001f8f0: 6f73 6522 5d2e 696c 6f63 5b30 5d2c 2032  ose"].iloc[0], 2
-0001f900: 290d 0a20 2020 2020 2020 2076 6572 6966  )..        verif
-0001f910: 7953 7461 6765 5477 6f20 3d20 5472 7565  yStageTwo = True
-0001f920: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0001f930: 2864 6174 6129 203e 2032 3530 3a0d 0a20  (data) > 250:.. 
-0001f940: 2020 2020 2020 2020 2020 2079 6561 726c             yearl
-0001f950: 794c 6f77 203d 2064 6174 612e 6865 6164  yLow = data.head
-0001f960: 2832 3530 295b 2243 6c6f 7365 225d 2e6d  (250)["Close"].m
-0001f970: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
-0001f980: 2020 7965 6172 6c79 4869 6768 203d 2064    yearlyHigh = d
-0001f990: 6174 612e 6865 6164 2832 3530 295b 2243  ata.head(250)["C
-0001f9a0: 6c6f 7365 225d 2e6d 6178 2829 0d0a 2020  lose"].max()..  
-0001f9b0: 2020 2020 2020 2020 2020 6966 206c 7470            if ltp
-0001f9c0: 203c 2028 3220 2a20 7965 6172 6c79 4c6f   < (2 * yearlyLo
-0001f9d0: 7729 2061 6e64 206c 7470 203c 2028 302e  w) and ltp < (0.
-0001f9e0: 3735 202a 2079 6561 726c 7948 6967 6829  75 * yearlyHigh)
-0001f9f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001fa00: 2020 2076 6572 6966 7953 7461 6765 5477     verifyStageTw
-0001fa10: 6f20 3d20 4661 6c73 650d 0a20 2020 2020  o = False..     
-0001fa20: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001fa30: 6e44 6963 745b 2253 746f 636b 225d 203d  nDict["Stock"] =
-0001fa40: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
-0001fa50: 2b20 7361 7665 4469 6374 5b22 5374 6f63  + saveDict["Stoc
-0001fa60: 6b22 5d20 2b20 636f 6c6f 7254 6578 742e  k"] + colorText.
-0001fa70: 454e 440d 0a20 2020 2020 2020 2069 6620  END..        if 
-0001fa80: 6c74 7020 3e3d 206d 696e 4c54 5020 616e  ltp >= minLTP an
-0001fa90: 6420 6c74 7020 3c3d 206d 6178 4c54 503a  d ltp <= maxLTP:
-0001faa0: 0d0a 2020 2020 2020 2020 2020 2020 6c74  ..            lt
-0001fab0: 7056 616c 6964 203d 2054 7275 650d 0a20  pValid = True.. 
-0001fac0: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
-0001fad0: 6e43 6861 6e67 6520 213d 2030 3a0d 0a20  nChange != 0:.. 
-0001fae0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001faf0: 2055 7365 7220 6861 7320 7375 7070 6c69   User has suppli
-0001fb00: 6564 2073 6f6d 6520 6669 6c74 6572 2066  ed some filter f
-0001fb10: 6f72 2070 6572 6365 6e74 6167 6520 6368  or percentage ch
-0001fb20: 616e 6765 0d0a 2020 2020 2020 2020 2020  ange..          
-0001fb30: 2020 2020 2020 6c74 7056 616c 6964 203d        ltpValid =
-0001fb40: 2066 6c6f 6174 2873 7472 2870 6374 5f73   float(str(pct_s
-0001fb50: 6176 6529 2e72 6570 6c61 6365 2822 2522  ave).replace("%"
-0001fb60: 2c22 2229 2920 3e3d 206d 696e 4368 616e  ,"")) >= minChan
-0001fb70: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
-0001fb80: 7361 7665 4469 6374 5b22 4c54 5022 5d20  saveDict["LTP"] 
-0001fb90: 3d20 726f 756e 6428 6c74 702c 2032 290d  = round(ltp, 2).
-0001fba0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-0001fbb0: 6565 6e44 6963 745b 224c 5450 225d 203d  eenDict["LTP"] =
-0001fbc0: 2028 636f 6c6f 7254 6578 742e 4752 4545   (colorText.GREE
-0001fbd0: 4e20 6966 206c 7470 5661 6c69 6420 656c  N if ltpValid el
-0001fbe0: 7365 2063 6f6c 6f72 5465 7874 2e46 4149  se colorText.FAI
-0001fbf0: 4c29 202b 2028 2225 2e32 6622 2025 206c  L) + ("%.2f" % l
-0001fc00: 7470 2920 2b20 636f 6c6f 7254 6578 742e  tp) + colorText.
-0001fc10: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-0001fc20: 2072 6574 7572 6e20 6c74 7056 616c 6964   return ltpValid
-0001fc30: 2c20 7665 7269 6679 5374 6167 6554 776f  , verifyStageTwo
-0001fc40: 0d0a 2020 2020 2020 2020 7363 7265 656e  ..        screen
-0001fc50: 4469 6374 5b22 4c54 5022 5d20 3d20 636f  Dict["LTP"] = co
-0001fc60: 6c6f 7254 6578 742e 4641 494c 202b 2028  lorText.FAIL + (
-0001fc70: 2225 2e32 6622 2025 206c 7470 2920 2b20  "%.2f" % ltp) + 
-0001fc80: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-0001fc90: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-0001fca0: 224c 5450 225d 203d 2072 6f75 6e64 286c  "LTP"] = round(l
-0001fcb0: 7470 2c20 3229 0d0a 2020 2020 2020 2020  tp, 2)..        
-0001fcc0: 7265 7475 726e 206c 7470 5661 6c69 642c  return ltpValid,
-0001fcd0: 2076 6572 6966 7953 7461 6765 5477 6f0d   verifyStageTwo.
-0001fce0: 0a0d 0a20 2020 2064 6566 2076 616c 6964  ...    def valid
-0001fcf0: 6174 654c 5450 466f 7250 6f72 7466 6f6c  ateLTPForPortfol
-0001fd00: 696f 4361 6c63 2873 656c 662c 2064 662c  ioCalc(self, df,
-0001fd10: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-0001fd20: 6544 6963 742c 7265 7175 6573 7465 6450  eDict,requestedP
-0001fd30: 6572 696f 643d 3029 3a0d 0a20 2020 2020  eriod=0):..     
-0001fd40: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-0001fd50: 7928 290d 0a20 2020 2020 2020 2070 6572  y()..        per
-0001fd60: 696f 6473 203d 2073 656c 662e 636f 6e66  iods = self.conf
-0001fd70: 6967 4d61 6e61 6765 722e 7065 7269 6f64  igManager.period
-0001fd80: 7352 616e 6765 0d0a 2020 2020 2020 2020  sRange..        
-0001fd90: 6966 2072 6571 7565 7374 6564 5065 7269  if requestedPeri
-0001fda0: 6f64 203e 2030 2061 6e64 2072 6571 7565  od > 0 and reque
-0001fdb0: 7374 6564 5065 7269 6f64 206e 6f74 2069  stedPeriod not i
-0001fdc0: 6e20 7065 7269 6f64 733a 0d0a 2020 2020  n periods:..    
-0001fdd0: 2020 2020 2020 2020 7065 7269 6f64 732e          periods.
-0001fde0: 6170 7065 6e64 2872 6571 7565 7374 6564  append(requested
-0001fdf0: 5065 7269 6f64 290d 0a20 2020 2020 2020  Period)..       
-0001fe00: 2070 7265 7669 6f75 735f 7265 6365 6e74   previous_recent
-0001fe10: 203d 2064 6174 612e 6865 6164 2831 290d   = data.head(1).
-0001fe20: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
-0001fe30: 735f 7265 6365 6e74 2e72 6573 6574 5f69  s_recent.reset_i
-0001fe40: 6e64 6578 2869 6e70 6c61 6365 3d54 7275  ndex(inplace=Tru
-0001fe50: 6529 0d0a 2020 2020 2020 2020 6361 6c63  e)..        calc
-0001fe60: 5f64 6174 6520 3d20 7374 7228 7072 6576  _date = str(prev
-0001fe70: 696f 7573 5f72 6563 656e 742e 696c 6f63  ious_recent.iloc
-0001fe80: 5b3a 2c20 305d 5b30 5d29 2e73 706c 6974  [:, 0][0]).split
-0001fe90: 2822 2022 295b 305d 0d0a 2020 2020 2020  (" ")[0]..      
-0001fea0: 2020 666f 7220 7072 6420 696e 2070 6572    for prd in per
-0001feb0: 696f 6473 3a0d 0a20 2020 2020 2020 2020  iods:..         
-0001fec0: 2020 2069 6620 6c65 6e28 6461 7461 2920     if len(data) 
-0001fed0: 3e3d 2070 7264 202b 2031 3a0d 0a20 2020  >= prd + 1:..   
-0001fee0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-0001fef0: 764c 7470 203d 2064 6174 615b 2243 6c6f  vLtp = data["Clo
-0001ff00: 7365 225d 2e69 6c6f 635b 305d 0d0a 2020  se"].iloc[0]..  
-0001ff10: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
-0001ff20: 7054 6479 203d 2064 6174 615b 2243 6c6f  pTdy = data["Clo
-0001ff30: 7365 225d 2e69 6c6f 635b 7072 645d 0d0a  se"].iloc[prd]..
-0001ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff50: 6966 2069 7369 6e73 7461 6e63 6528 7072  if isinstance(pr
-0001ff60: 6576 4c74 702c 7064 2e53 6572 6965 7329  evLtp,pd.Series)
-0001ff70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001ff80: 2020 2020 2020 2070 7265 764c 7470 203d         prevLtp =
-0001ff90: 2070 7265 764c 7470 5b30 5d0d 0a20 2020   prevLtp[0]..   
-0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ffb0: 206c 7470 5464 7920 3d20 6c74 7054 6479   ltpTdy = ltpTdy
-0001ffc0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-0001ffd0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001ffe0: 6622 4c54 507b 7072 647d 225d 203d 2028  f"LTP{prd}"] = (
-0001fff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020000: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
-00020010: 2e47 5245 454e 2069 6620 286c 7470 5464  .GREEN if (ltpTd
-00020020: 7920 3e3d 2070 7265 764c 7470 2920 656c  y >= prevLtp) el
-00020030: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
-00020040: 494c 2929 0d0a 2020 2020 2020 2020 2020  IL))..          
-00020050: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
-00020060: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
-00020070: 6c74 7054 6479 2929 0d0a 2020 2020 2020  ltpTdy))..      
-00020080: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00020090: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-000200a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000200b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000200c0: 2020 7363 7265 656e 4469 6374 5b66 2247    screenDict[f"G
-000200d0: 726f 7774 687b 7072 647d 225d 203d 2028  rowth{prd}"] = (
-000200e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000200f0: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
-00020100: 2e47 5245 454e 2069 6620 286c 7470 5464  .GREEN if (ltpTd
-00020110: 7920 3e3d 2070 7265 764c 7470 2920 656c  y >= prevLtp) el
-00020120: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
-00020130: 494c 2929 0d0a 2020 2020 2020 2020 2020  IL))..          
-00020140: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
-00020150: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
-00020160: 6c74 7054 6479 202d 2070 7265 764c 7470  ltpTdy - prevLtp
-00020170: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00020180: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00020190: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-000201a0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-000201b0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000201c0: 4469 6374 5b66 224c 5450 7b70 7264 7d22  Dict[f"LTP{prd}"
-000201d0: 5d20 3d20 726f 756e 6428 6c74 7054 6479  ] = round(ltpTdy
-000201e0: 2c20 3229 0d0a 2020 2020 2020 2020 2020  , 2)..          
-000201f0: 2020 2020 2020 7361 7665 4469 6374 5b66        saveDict[f
-00020200: 2247 726f 7774 687b 7072 647d 225d 203d  "Growth{prd}"] =
-00020210: 2072 6f75 6e64 286c 7470 5464 7920 2d20   round(ltpTdy - 
-00020220: 7072 6576 4c74 702c 2032 290d 0a20 2020  prevLtp, 2)..   
-00020230: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00020240: 7072 6420 3d3d 2032 3220 6f72 2028 7072  prd == 22 or (pr
-00020250: 6420 3d3d 2072 6571 7565 7374 6564 5065  d == requestedPe
-00020260: 7269 6f64 293a 0d0a 2020 2020 2020 2020  riod):..        
-00020270: 2020 2020 2020 2020 2020 2020 6368 616e              chan
-00020280: 6765 5065 7263 656e 7420 3d20 726f 756e  gePercent = roun
-00020290: 6428 2828 7072 6576 4c74 702d 6c74 7054  d(((prevLtp-ltpT
-000202a0: 6479 2920 6966 2072 6571 7565 7374 6564  dy) if requested
-000202b0: 5065 7269 6f64 203d 3d30 2065 6c73 6520  Period ==0 else 
-000202c0: 286c 7470 5464 7920 2d20 7072 6576 4c74  (ltpTdy - prevLt
-000202d0: 7029 292a 3130 302f 6c74 7054 6479 2c20  p))*100/ltpTdy, 
-000202e0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-000202f0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00020300: 5b66 227b 7072 647d 2d50 6420 2522 5d20  [f"{prd}-Pd %"] 
-00020310: 3d20 6622 7b63 6861 6e67 6550 6572 6365  = f"{changePerce
-00020320: 6e74 7d25 2220 6966 206e 6f74 2070 642e  nt}%" if not pd.
-00020330: 6973 6e61 2863 6861 6e67 6550 6572 6365  isna(changePerce
-00020340: 6e74 2920 656c 7365 2027 2d27 0d0a 2020  nt) else '-'..  
-00020350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020360: 2020 7363 7265 656e 4469 6374 5b66 227b    screenDict[f"{
-00020370: 7072 647d 2d50 6420 2522 5d20 3d20 2828  prd}-Pd %"] = ((
-00020380: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
-00020390: 6966 2063 6861 6e67 6550 6572 6365 6e74  if changePercent
-000203a0: 203e 3d30 2065 6c73 6520 636f 6c6f 7254   >=0 else colorT
-000203b0: 6578 742e 4641 494c 2920 2b20 6622 7b63  ext.FAIL) + f"{c
-000203c0: 6861 6e67 6550 6572 6365 6e74 7d25 2220  hangePercent}%" 
-000203d0: 2b20 636f 6c6f 7254 6578 742e 454e 4429  + colorText.END)
-000203e0: 2069 6620 6e6f 7420 7064 2e69 736e 6128   if not pd.isna(
-000203f0: 6368 616e 6765 5065 7263 656e 7429 2065  changePercent) e
-00020400: 6c73 6520 272d 270d 0a20 2020 2020 2020  lse '-'..       
-00020410: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00020420: 6963 745b 2244 6174 6522 5d20 3d20 6361  ict["Date"] = ca
-00020430: 6c63 5f64 6174 650d 0a20 2020 2020 2020  lc_date..       
-00020440: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00020450: 745b 2244 6174 6522 5d20 3d20 6361 6c63  t["Date"] = calc
-00020460: 5f64 6174 650d 0a20 2020 2020 2020 2020  _date..         
-00020470: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00020480: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00020490: 6374 5b66 224c 5450 7b70 7264 7d22 5d20  ct[f"LTP{prd}"] 
-000204a0: 3d20 6e70 2e6e 616e 0d0a 2020 2020 2020  = np.nan..      
-000204b0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-000204c0: 6374 5b66 2247 726f 7774 687b 7072 647d  ct[f"Growth{prd}
-000204d0: 225d 203d 206e 702e 6e61 6e0d 0a20 2020  "] = np.nan..   
-000204e0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-000204f0: 6565 6e44 6963 745b 2244 6174 6522 5d20  eenDict["Date"] 
-00020500: 3d20 6361 6c63 5f64 6174 650d 0a20 2020  = calc_date..   
-00020510: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00020520: 6544 6963 745b 2244 6174 6522 5d20 3d20  eDict["Date"] = 
-00020530: 6361 6c63 5f64 6174 650d 0a0d 0a20 2020  calc_date....   
-00020540: 2023 2046 696e 6420 7374 6f63 6b73 2074   # Find stocks t
-00020550: 6861 7420 6172 6520 6265 6172 6973 6820  hat are bearish 
-00020560: 696e 7472 6164 6179 3a20 4d61 6364 2048  intraday: Macd H
-00020570: 6973 746f 6772 616d 206e 6567 6174 6976  istogram negativ
-00020580: 650d 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
-00020590: 6174 654d 4143 4448 6973 746f 6772 616d  ateMACDHistogram
-000205a0: 4265 6c6f 7730 2873 656c 662c 2064 6629  Below0(self, df)
-000205b0: 3a0d 0a20 2020 2020 2020 2069 6620 6466  :..        if df
-000205c0: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-000205d0: 6466 2920 3d3d 2030 3a0d 0a20 2020 2020  df) == 0:..     
-000205e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000205f0: 6c73 650d 0a20 2020 2020 2020 2064 6174  lse..        dat
-00020600: 6120 3d20 6466 2e63 6f70 7928 290d 0a20  a = df.copy().. 
-00020610: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00020620: 7461 2e66 696c 6c6e 6128 3029 0d0a 2020  ta.fillna(0)..  
-00020630: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00020640: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
-00020650: 662c 202d 6e70 2e69 6e66 5d2c 2030 290d  f, -np.inf], 0).
-00020660: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00020670: 6461 7461 5b3a 3a2d 315d 2020 2320 5265  data[::-1]  # Re
-00020680: 7665 7273 6520 7468 6520 6461 7461 6672  verse the datafr
-00020690: 616d 6520 736f 2074 6861 7420 6974 7320  ame so that its 
-000206a0: 7468 6520 6f6c 6465 7374 2064 6174 6520  the oldest date 
-000206b0: 6669 7273 740d 0a20 2020 2020 2020 206d  first..        m
-000206c0: 6163 6420 3d20 706b 7461 6c69 622e 4d41  acd = pktalib.MA
-000206d0: 4344 2864 6174 615b 2243 6c6f 7365 225d  CD(data["Close"]
-000206e0: 2c20 3132 2c20 3236 2c20 3929 5b32 5d2e  , 12, 26, 9)[2].
-000206f0: 7461 696c 2831 290d 0a20 2020 2020 2020  tail(1)..       
-00020700: 2072 6574 7572 6e20 6d61 6364 2e69 6c6f   return macd.ilo
-00020710: 635b 3a31 5d5b 305d 203c 2030 0d0a 0d0a  c[:1][0] < 0....
-00020720: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-00020730: 6d65 0d0a 2020 2020 2320 4669 6e64 2069  me..    # Find i
-00020740: 6620 7374 6f63 6b20 6761 696e 696e 6720  f stock gaining 
-00020750: 6275 6c6c 6973 6820 6d6f 6d65 6e74 756d  bullish momentum
-00020760: 0d0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00020770: 7465 4d6f 6d65 6e74 756d 2873 656c 662c  teMomentum(self,
-00020780: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-00020790: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
-000207a0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-000207b0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-000207c0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000207d0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-000207e0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-000207f0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00020800: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00020810: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00020820: 6561 6428 3329 0d0a 2020 2020 2020 2020  ead(3)..        
-00020830: 2020 2020 6966 206c 656e 2864 6174 6129      if len(data)
-00020840: 203c 2033 3a0d 0a20 2020 2020 2020 2020   < 3:..         
-00020850: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00020860: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00020870: 2066 6f72 2072 6f77 2069 6e20 6461 7461   for row in data
-00020880: 2e69 7465 7272 6f77 7328 293a 0d0a 2020  .iterrows():..  
-00020890: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000208a0: 416c 6c20 3320 6361 6e64 6c65 7320 7368  All 3 candles sh
-000208b0: 6f75 6c64 2062 6520 4772 6565 6e20 616e  ould be Green an
-000208c0: 6420 4e4f 5420 4369 7263 7569 7473 0d0a  d NOT Circuits..
-000208d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208e0: 7963 203d 2072 6f77 5b31 5d5b 2243 6c6f  yc = row[1]["Clo
-000208f0: 7365 225d 0d0a 2020 2020 2020 2020 2020  se"]..          
-00020900: 2020 2020 2020 796f 203d 2072 6f77 5b31        yo = row[1
-00020910: 5d5b 224f 7065 6e22 5d0d 0a20 2020 2020  ]["Open"]..     
-00020920: 2020 2020 2020 2020 2020 2069 6620 7963             if yc
-00020930: 203c 3d20 796f 3a0d 0a20 2020 2020 2020   <= yo:..       
-00020940: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00020950: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
-00020960: 6572 2e69 6e66 6f28 0d0a 2020 2020 2020  er.info(..      
-00020970: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00020980: 2020 2020 6627 5374 6f63 6b3a 7b73 6176      f'Stock:{sav
-00020990: 6544 6963 745b 2253 746f 636b 225d 7d2c  eDict["Stock"]},
-000209a0: 2069 7320 6e6f 7420 6120 6d6f 6d65 6e74   is not a moment
-000209b0: 756d 2d67 6169 6e65 7220 6265 6361 7573  um-gainer becaus
-000209c0: 6520 7965 7374 6572 6461 792d 636c 6f73  e yesterday-clos
-000209d0: 6520 287b 7963 7d29 203c 3d20 7965 7374  e ({yc}) <= yest
-000209e0: 6572 6461 792d 6f70 656e 2028 7b79 6f7d  erday-open ({yo}
-000209f0: 2927 0d0a 2020 2020 2020 2020 2020 2020  )'..            
-00020a00: 2020 2020 2020 2020 2320 290d 0a20 2020          # )..   
-00020a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a20: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00020a30: 2020 2020 2020 2020 2020 206f 7065 6e44             openD
-00020a40: 6573 6320 3d20 6461 7461 2e73 6f72 745f  esc = data.sort_
-00020a50: 7661 6c75 6573 2862 793d 5b22 4f70 656e  values(by=["Open
-00020a60: 225d 2c20 6173 6365 6e64 696e 673d 4661  "], ascending=Fa
-00020a70: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
-00020a80: 2020 636c 6f73 6544 6573 6320 3d20 6461    closeDesc = da
-00020a90: 7461 2e73 6f72 745f 7661 6c75 6573 2862  ta.sort_values(b
-00020aa0: 793d 5b22 436c 6f73 6522 5d2c 2061 7363  y=["Close"], asc
-00020ab0: 656e 6469 6e67 3d46 616c 7365 290d 0a20  ending=False).. 
-00020ac0: 2020 2020 2020 2020 2020 2076 6f6c 4465             volDe
-00020ad0: 7363 203d 2064 6174 612e 736f 7274 5f76  sc = data.sort_v
-00020ae0: 616c 7565 7328 6279 3d5b 2256 6f6c 756d  alues(by=["Volum
-00020af0: 6522 5d2c 2061 7363 656e 6469 6e67 3d46  e"], ascending=F
-00020b00: 616c 7365 290d 0a20 2020 2020 2020 2020  alse)..         
-00020b10: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00020b20: 2020 2020 2020 2020 2069 6620 280d 0a20           if (.. 
-00020b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b40: 2020 2064 6174 612e 6571 7561 6c73 286f     data.equals(o
-00020b50: 7065 6e44 6573 6329 0d0a 2020 2020 2020  penDesc)..      
-00020b60: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00020b70: 6420 6461 7461 2e65 7175 616c 7328 636c  d data.equals(cl
-00020b80: 6f73 6544 6573 6329 0d0a 2020 2020 2020  oseDesc)..      
-00020b90: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00020ba0: 6420 6461 7461 2e65 7175 616c 7328 766f  d data.equals(vo
-00020bb0: 6c44 6573 6329 0d0a 2020 2020 2020 2020  lDesc)..        
-00020bc0: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-00020bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020be0: 2320 7365 6c66 2e64 6566 6175 6c74 5f6c  # self.default_l
-00020bf0: 6f67 6765 722e 696e 666f 280d 0a20 2020  ogger.info(..   
+00019e70: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
+00019e80: 4e44 2c0d 0a20 2020 2020 2020 2020 2020  ND,..           
+00019e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019eb0: 2066 2231 3a7b 7269 736b 5f72 6577 6172   f"1:{risk_rewar
+00019ec0: 647d 222c 0d0a 2020 2020 2020 2020 2020  d}",..          
+00019ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ee0: 2020 2020 2020 2020 2020 2020 2020 5d0d                ].
+00019ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f10: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
+00019f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f30: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00019f40: 756d 6e73 3d72 6573 756c 745f 6466 2e63  umns=result_df.c
+00019f50: 6f6c 756d 6e73 2c0d 0a20 2020 2020 2020  olumns,..       
+00019f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f70: 2020 2020 2020 2020 2029 2c0d 0a20 2020           ),..   
+00019f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f90: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00019fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fb0: 2020 2020 2020 2020 2061 7869 733d 302c           axis=0,
+00019fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019fd0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00019fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ff0: 2020 2020 2072 6573 756c 745f 6466 2e72       result_df.r
+0001a000: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
+0001a010: 5472 7565 2c20 696e 706c 6163 653d 5472  True, inplace=Tr
+0001a020: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+0001a030: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+0001a040: 4578 6365 7074 696f 6e20 6173 2065 3a20  Exception as e: 
+0001a050: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+0001a060: 7665 720d 0a20 2020 2020 2020 2020 2020  ver..           
+0001a070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001a080: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+0001a090: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
+0001a0a0: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
+0001a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0c0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+0001a0d0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+0001a0e0: 656e 2075 7064 6174 650d 0a20 2020 2020  en update..     
+0001a0f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0001a100: 6173 745f 7369 676e 616c 5b64 6174 615f  ast_signal[data_
+0001a110: 6c69 7374 5b63 6e74 5d5d 203d 205b 6669  list[cnt]] = [fi
+0001a120: 6e61 6c5d 0d0a 2020 2020 2020 2020 6966  nal]..        if
+0001a130: 2072 6573 756c 745f 6466 2069 7320 6e6f   result_df is no
+0001a140: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0001a150: 2020 2020 2072 6573 756c 745f 6466 2e64       result_df.d
+0001a160: 726f 705f 6475 706c 6963 6174 6573 286b  rop_duplicates(k
+0001a170: 6565 703d 226c 6173 7422 2c20 696e 706c  eep="last", inpl
+0001a180: 6163 653d 5472 7565 290d 0a20 2020 2020  ace=True)..     
+0001a190: 2020 2020 2020 2072 6573 756c 745f 6466         result_df
+0001a1a0: 2e73 6f72 745f 7661 6c75 6573 2862 793d  .sort_values(by=
+0001a1b0: 2254 696d 6522 2c20 696e 706c 6163 653d  "Time", inplace=
+0001a1c0: 5472 7565 290d 0a20 2020 2020 2020 2072  True)..        r
+0001a1d0: 6574 7572 6e20 7265 7375 6c74 5f64 665b  eturn result_df[
+0001a1e0: 3a3a 2d31 5d0d 0a0d 0a20 2020 2023 2050  ::-1]....    # P
+0001a1f0: 7265 7072 6f63 6573 7320 7468 6520 6163  reprocess the ac
+0001a200: 7175 6972 6564 2064 6174 610d 0a20 2020  quired data..   
+0001a210: 2064 6566 2070 7265 7072 6f63 6573 7344   def preprocessD
+0001a220: 6174 6128 7365 6c66 2c20 6466 2c20 6461  ata(self, df, da
+0001a230: 7973 546f 4c6f 6f6b 6261 636b 3d4e 6f6e  ysToLookback=Non
+0001a240: 6529 3a0d 0a20 2020 2020 2020 2061 7373  e):..        ass
+0001a250: 6572 7420 6973 696e 7374 616e 6365 2864  ert isinstance(d
+0001a260: 662c 2070 642e 4461 7461 4672 616d 6529  f, pd.DataFrame)
+0001a270: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+0001a280: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
+0001a290: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+0001a2a0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+0001a2b0: 612e 7265 706c 6163 6528 6e70 2e69 6e66  a.replace(np.inf
+0001a2c0: 2c20 6e70 2e6e 616e 292e 7265 706c 6163  , np.nan).replac
+0001a2d0: 6528 2d6e 702e 696e 662c 206e 702e 6e61  e(-np.inf, np.na
+0001a2e0: 6e29 2e64 726f 706e 6128 686f 773d 2261  n).dropna(how="a
+0001a2f0: 6c6c 2229 0d0a 2020 2020 2020 2020 2020  ll")..          
+0001a300: 2020 2320 7365 6c66 2e64 6566 6175 6c74    # self.default
+0001a310: 5f6c 6f67 6765 722e 696e 666f 2866 2250  _logger.info(f"P
+0001a320: 7265 7072 6f63 6573 7369 6e67 2064 6174  reprocessing dat
+0001a330: 613a 5c6e 7b64 6174 612e 6865 6164 2831  a:\n{data.head(1
+0001a340: 297d 5c6e 2229 0d0a 2020 2020 2020 2020  )}\n")..        
+0001a350: 2020 2020 6966 2064 6179 7354 6f4c 6f6f      if daysToLoo
+0001a360: 6b62 6163 6b20 6973 204e 6f6e 653a 0d0a  kback is None:..
+0001a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a380: 6461 7973 546f 4c6f 6f6b 6261 636b 203d  daysToLookback =
+0001a390: 2073 656c 662e 636f 6e66 6967 4d61 6e61   self.configMana
+0001a3a0: 6765 722e 6461 7973 546f 4c6f 6f6b 6261  ger.daysToLookba
+0001a3b0: 636b 0d0a 2020 2020 2020 2020 2020 2020  ck..            
+0001a3c0: 6966 2073 656c 662e 636f 6e66 6967 4d61  if self.configMa
+0001a3d0: 6e61 6765 722e 7573 6545 4d41 3a0d 0a20  nager.useEMA:.. 
+0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a3f0: 6d61 203d 2070 6b74 616c 6962 2e45 4d41  ma = pktalib.EMA
+0001a400: 2864 6174 615b 2243 6c6f 7365 225d 2c20  (data["Close"], 
+0001a410: 7469 6d65 7065 7269 6f64 3d35 3029 0d0a  timeperiod=50)..
+0001a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a430: 6c6d 6120 3d20 706b 7461 6c69 622e 454d  lma = pktalib.EM
+0001a440: 4128 6461 7461 5b22 436c 6f73 6522 5d2c  A(data["Close"],
+0001a450: 2074 696d 6570 6572 696f 643d 3230 3029   timeperiod=200)
+0001a460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a470: 2020 7373 6d61 203d 2070 6b74 616c 6962    ssma = pktalib
+0001a480: 2e45 4d41 2864 6174 615b 2243 6c6f 7365  .EMA(data["Close
+0001a490: 225d 2c20 7469 6d65 7065 7269 6f64 3d39  "], timeperiod=9
+0001a4a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a4b0: 2020 2064 6174 612e 696e 7365 7274 286c     data.insert(l
+0001a4c0: 656e 2864 6174 612e 636f 6c75 6d6e 7329  en(data.columns)
+0001a4d0: 2c20 2253 4d41 222c 2073 6d61 290d 0a20  , "SMA", sma).. 
+0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001a4f0: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
+0001a500: 6174 612e 636f 6c75 6d6e 7329 2c20 224c  ata.columns), "L
+0001a510: 4d41 222c 206c 6d61 290d 0a20 2020 2020  MA", lma)..     
+0001a520: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0001a530: 696e 7365 7274 286c 656e 2864 6174 612e  insert(len(data.
+0001a540: 636f 6c75 6d6e 7329 2c20 2253 534d 4122  columns), "SSMA"
+0001a550: 2c20 7373 6d61 290d 0a20 2020 2020 2020  , ssma)..       
+0001a560: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0001a570: 2020 2020 2020 2020 2020 2020 736d 6120              sma 
+0001a580: 3d20 706b 7461 6c69 622e 534d 4128 6461  = pktalib.SMA(da
+0001a590: 7461 5b22 436c 6f73 6522 5d2c 2074 696d  ta["Close"], tim
+0001a5a0: 6570 6572 696f 643d 3530 290d 0a20 2020  eperiod=50)..   
+0001a5b0: 2020 2020 2020 2020 2020 2020 206c 6d61               lma
+0001a5c0: 203d 2070 6b74 616c 6962 2e53 4d41 2864   = pktalib.SMA(d
+0001a5d0: 6174 615b 2243 6c6f 7365 225d 2c20 7469  ata["Close"], ti
+0001a5e0: 6d65 7065 7269 6f64 3d32 3030 290d 0a20  meperiod=200).. 
+0001a5f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a600: 736d 6120 3d20 706b 7461 6c69 622e 534d  sma = pktalib.SM
+0001a610: 4128 6461 7461 5b22 436c 6f73 6522 5d2c  A(data["Close"],
+0001a620: 2074 696d 6570 6572 696f 643d 3929 0d0a   timeperiod=9)..
+0001a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a640: 6461 7461 2e69 6e73 6572 7428 6c65 6e28  data.insert(len(
+0001a650: 6461 7461 2e63 6f6c 756d 6e73 292c 2022  data.columns), "
+0001a660: 534d 4122 2c20 736d 6129 0d0a 2020 2020  SMA", sma)..    
+0001a670: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0001a680: 2e69 6e73 6572 7428 6c65 6e28 6461 7461  .insert(len(data
+0001a690: 2e63 6f6c 756d 6e73 292c 2022 4c4d 4122  .columns), "LMA"
+0001a6a0: 2c20 6c6d 6129 0d0a 2020 2020 2020 2020  , lma)..        
+0001a6b0: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
+0001a6c0: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
+0001a6d0: 756d 6e73 292c 2022 5353 4d41 222c 2073  umns), "SSMA", s
+0001a6e0: 736d 6129 0d0a 2020 2020 2020 2020 2020  sma)..          
+0001a6f0: 2020 766f 6c20 3d20 706b 7461 6c69 622e    vol = pktalib.
+0001a700: 534d 4128 6461 7461 5b22 566f 6c75 6d65  SMA(data["Volume
+0001a710: 225d 2c20 7469 6d65 7065 7269 6f64 3d32  "], timeperiod=2
+0001a720: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+0001a730: 7273 6920 3d20 706b 7461 6c69 622e 5253  rsi = pktalib.RS
+0001a740: 4928 6461 7461 5b22 436c 6f73 6522 5d2c  I(data["Close"],
+0001a750: 2074 696d 6570 6572 696f 643d 3134 290d   timeperiod=14).
+0001a760: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0001a770: 612e 696e 7365 7274 286c 656e 2864 6174  a.insert(len(dat
+0001a780: 612e 636f 6c75 6d6e 7329 2c20 2256 6f6c  a.columns), "Vol
+0001a790: 4d41 222c 2076 6f6c 290d 0a20 2020 2020  MA", vol)..     
+0001a7a0: 2020 2020 2020 2064 6174 612e 696e 7365         data.inse
+0001a7b0: 7274 286c 656e 2864 6174 612e 636f 6c75  rt(len(data.colu
+0001a7c0: 6d6e 7329 2c20 2252 5349 222c 2072 7369  mns), "RSI", rsi
+0001a7d0: 290d 0a20 2020 2020 2020 2020 2020 2063  )..            c
+0001a7e0: 6369 203d 2070 6b74 616c 6962 2e43 4349  ci = pktalib.CCI
+0001a7f0: 2864 6174 615b 2248 6967 6822 5d2c 2064  (data["High"], d
+0001a800: 6174 615b 224c 6f77 225d 2c20 6461 7461  ata["Low"], data
+0001a810: 5b22 436c 6f73 6522 5d2c 2074 696d 6570  ["Close"], timep
+0001a820: 6572 696f 643d 3134 290d 0a20 2020 2020  eriod=14)..     
+0001a830: 2020 2020 2020 2064 6174 612e 696e 7365         data.inse
+0001a840: 7274 286c 656e 2864 6174 612e 636f 6c75  rt(len(data.colu
+0001a850: 6d6e 7329 2c20 2243 4349 222c 2063 6369  mns), "CCI", cci
+0001a860: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
+0001a870: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+0001a880: 2020 2020 2066 6173 746b 2c20 6661 7374       fastk, fast
+0001a890: 6420 3d20 706b 7461 6c69 622e 5354 4f43  d = pktalib.STOC
+0001a8a0: 4852 5349 280d 0a20 2020 2020 2020 2020  HRSI(..         
+0001a8b0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+0001a8c0: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+0001a8d0: 7269 6f64 3d31 342c 2066 6173 746b 5f70  riod=14, fastk_p
+0001a8e0: 6572 696f 643d 352c 2066 6173 7464 5f70  eriod=5, fastd_p
+0001a8f0: 6572 696f 643d 332c 2066 6173 7464 5f6d  eriod=3, fastd_m
+0001a900: 6174 7970 653d 300d 0a20 2020 2020 2020  atype=0..       
+0001a910: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+0001a920: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0001a930: 2e69 6e73 6572 7428 6c65 6e28 6461 7461  .insert(len(data
+0001a940: 2e63 6f6c 756d 6e73 292c 2022 4641 5354  .columns), "FAST
+0001a950: 4b22 2c20 6661 7374 6b29 0d0a 2020 2020  K", fastk)..    
+0001a960: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0001a970: 2e69 6e73 6572 7428 6c65 6e28 6461 7461  .insert(len(data
+0001a980: 2e63 6f6c 756d 6e73 292c 2022 4641 5354  .columns), "FAST
+0001a990: 4422 2c20 6661 7374 6429 0d0a 2020 2020  D", fastd)..    
+0001a9a0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+0001a9b0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+0001a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9d0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+0001a9e0: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
+0001a9f0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
+0001aa00: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+0001aa10: 730d 0a20 2020 2020 2020 2065 7863 6570  s..        excep
+0001aa20: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0001aa30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001aa40: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+0001aa50: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+0001aa60: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
+0001aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa80: 7061 7373 0d0a 2020 2020 2020 2020 6461  pass..        da
+0001aa90: 7461 203d 2064 6174 615b 3a3a 2d31 5d20  ta = data[::-1] 
+0001aaa0: 2023 2052 6576 6572 7365 2074 6865 2064   # Reverse the d
+0001aab0: 6174 6166 7261 6d65 0d0a 2020 2020 2020  ataframe..      
+0001aac0: 2020 2320 6461 7461 203d 2064 6174 612e    # data = data.
+0001aad0: 6669 6c6c 6e61 2830 290d 0a20 2020 2020  fillna(0)..     
+0001aae0: 2020 2023 2064 6174 6120 3d20 6461 7461     # data = data
+0001aaf0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+0001ab00: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
+0001ab10: 2020 2020 2020 2020 6675 6c6c 4461 7461          fullData
+0001ab20: 203d 2064 6174 610d 0a20 2020 2020 2020   = data..       
+0001ab30: 2074 7269 6d6d 6564 4461 7461 203d 2064   trimmedData = d
+0001ab40: 6174 612e 6865 6164 2864 6179 7354 6f4c  ata.head(daysToL
+0001ab50: 6f6f 6b62 6163 6b29 0d0a 2020 2020 2020  ookback)..      
+0001ab60: 2020 7265 7475 726e 2028 6675 6c6c 4461    return (fullDa
+0001ab70: 7461 2c20 7472 696d 6d65 6444 6174 6129  ta, trimmedData)
+0001ab80: 0d0a 0d0a 2020 2020 2320 5661 6c69 6461  ....    # Valida
+0001ab90: 7465 2069 6620 7468 6520 7374 6f63 6b20  te if the stock 
+0001aba0: 6973 2062 756c 6c69 7368 2069 6e20 7468  is bullish in th
+0001abb0: 6520 7368 6f72 7420 7465 726d 0d0a 2020  e short term..  
+0001abc0: 2020 6465 6620 7661 6c69 6461 7465 3135    def validate15
+0001abd0: 4d69 6e75 7465 5072 6963 6556 6f6c 756d  MinutePriceVolum
+0001abe0: 6542 7265 616b 6f75 7428 7365 6c66 2c20  eBreakout(self, 
+0001abf0: 6466 293a 0d0a 2020 2020 2020 2020 6966  df):..        if
+0001ac00: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+0001ac10: 656e 2864 6629 203d 3d20 303a 0d0a 2020  en(df) == 0:..  
+0001ac20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001ac30: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0001ac40: 2320 6874 7470 733a 2f2f 6368 6172 7469  # https://charti
+0001ac50: 6e6b 2e63 6f6d 2f73 6372 6565 6e65 722f  nk.com/screener/
+0001ac60: 3135 2d6d 696e 2d70 7269 6365 2d76 6f6c  15-min-price-vol
+0001ac70: 756d 652d 6272 6561 6b6f 7574 0d0a 2020  ume-breakout..  
+0001ac80: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+0001ac90: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+0001aca0: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+0001acb0: 6e61 2830 290d 0a20 2020 2020 2020 2064  na(0)..        d
+0001acc0: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
+0001acd0: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
+0001ace0: 696e 665d 2c20 3029 0d0a 2020 2020 2020  inf], 0)..      
+0001acf0: 2020 6461 7461 203d 2064 6174 615b 3a3a    data = data[::
+0001ad00: 2d31 5d20 2023 2052 6576 6572 7365 2074  -1]  # Reverse t
+0001ad10: 6865 2064 6174 6166 7261 6d65 2073 6f20  he dataframe so 
+0001ad20: 7468 6174 2069 7473 2074 6865 206f 6c64  that its the old
+0001ad30: 6573 7420 6461 7465 2066 6972 7374 0d0a  est date first..
+0001ad40: 2020 2020 2020 2020 6461 7461 5b22 534d          data["SM
+0001ad50: 4132 3022 5d20 3d20 706b 7461 6c69 622e  A20"] = pktalib.
+0001ad60: 534d 4128 6461 7461 5b22 436c 6f73 6522  SMA(data["Close"
+0001ad70: 5d2c 2032 3029 0d0a 2020 2020 2020 2020  ], 20)..        
+0001ad80: 6461 7461 5b22 534d 4132 3056 225d 203d  data["SMA20V"] =
+0001ad90: 2070 6b74 616c 6962 2e53 4d41 2864 6174   pktalib.SMA(dat
+0001ada0: 615b 2256 6f6c 756d 6522 5d2c 2032 3029  a["Volume"], 20)
+0001adb0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+0001adc0: 2064 6174 615b 0d0a 2020 2020 2020 2020   data[..        
+0001add0: 2020 2020 3a3a 2d31 0d0a 2020 2020 2020      ::-1..      
+0001ade0: 2020 5d20 2023 2052 6576 6572 7365 2074    ]  # Reverse t
+0001adf0: 6865 2064 6174 6166 7261 6d65 2073 6f20  he dataframe so 
+0001ae00: 7468 6174 2069 7427 7320 7468 6520 6d6f  that it's the mo
+0001ae10: 7374 2072 6563 656e 7420 6461 7465 2066  st recent date f
+0001ae20: 6972 7374 0d0a 2020 2020 2020 2020 7265  irst..        re
+0001ae30: 6365 6e74 203d 2064 6174 612e 6865 6164  cent = data.head
+0001ae40: 2833 290d 0a20 2020 2020 2020 2069 6620  (3)..        if 
+0001ae50: 6c65 6e28 7265 6365 6e74 2920 3c20 333a  len(recent) < 3:
+0001ae60: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0001ae70: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
+0001ae80: 2020 2020 636f 6e64 3120 3d20 7265 6365      cond1 = rece
+0001ae90: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+0001aea0: 5b30 5d20 3e20 7265 6365 6e74 5b22 436c  [0] > recent["Cl
+0001aeb0: 6f73 6522 5d2e 696c 6f63 5b31 5d0d 0a20  ose"].iloc[1].. 
+0001aec0: 2020 2020 2020 2063 6f6e 6432 203d 2063         cond2 = c
+0001aed0: 6f6e 6431 2061 6e64 2028 7265 6365 6e74  ond1 and (recent
+0001aee0: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
+0001aef0: 5d20 3e20 7265 6365 6e74 5b22 534d 4132  ] > recent["SMA2
+0001af00: 3022 5d2e 696c 6f63 5b30 5d29 0d0a 2020  0"].iloc[0])..  
+0001af10: 2020 2020 2020 636f 6e64 3320 3d20 636f        cond3 = co
+0001af20: 6e64 3220 616e 6420 2872 6563 656e 745b  nd2 and (recent[
+0001af30: 2243 6c6f 7365 225d 2e69 6c6f 635b 315d  "Close"].iloc[1]
+0001af40: 203e 2072 6563 656e 745b 2248 6967 6822   > recent["High"
+0001af50: 5d2e 696c 6f63 5b32 5d29 0d0a 2020 2020  ].iloc[2])..    
+0001af60: 2020 2020 636f 6e64 3420 3d20 636f 6e64      cond4 = cond
+0001af70: 3320 616e 6420 2872 6563 656e 745b 2256  3 and (recent["V
+0001af80: 6f6c 756d 6522 5d2e 696c 6f63 5b30 5d20  olume"].iloc[0] 
+0001af90: 3e20 7265 6365 6e74 5b22 534d 4132 3056  > recent["SMA20V
+0001afa0: 225d 2e69 6c6f 635b 305d 290d 0a20 2020  "].iloc[0])..   
+0001afb0: 2020 2020 2063 6f6e 6435 203d 2063 6f6e       cond5 = con
+0001afc0: 6434 2061 6e64 2028 7265 6365 6e74 5b22  d4 and (recent["
+0001afd0: 566f 6c75 6d65 225d 2e69 6c6f 635b 315d  Volume"].iloc[1]
+0001afe0: 203e 2072 6563 656e 745b 2253 4d41 3230   > recent["SMA20
+0001aff0: 5622 5d2e 696c 6f63 5b30 5d29 0d0a 2020  V"].iloc[0])..  
+0001b000: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+0001b010: 6435 0d0a 0d0a 2020 2020 6465 6620 7661  d5....    def va
+0001b020: 6c69 6461 7465 4275 6c6c 6973 6846 6f72  lidateBullishFor
+0001b030: 546f 6d6f 7272 6f77 2873 656c 662c 2064  Tomorrow(self, d
+0001b040: 6629 3a0d 0a20 2020 2020 2020 2069 6620  f):..        if 
+0001b050: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+0001b060: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
+0001b070: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001b080: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
+0001b090: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
+0001b0a0: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
+0001b0b0: 3a2f 2f63 6861 7274 696e 6b2e 636f 6d2f  ://chartink.com/
+0001b0c0: 7363 7265 656e 6572 2f62 756c 6c69 7368  screener/bullish
+0001b0d0: 2d66 6f72 2d74 6f6d 6f72 726f 770d 0a20  -for-tomorrow.. 
+0001b0e0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+0001b0f0: 7461 2e66 696c 6c6e 6128 3029 0d0a 2020  ta.fillna(0)..  
+0001b100: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+0001b110: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
+0001b120: 662c 202d 6e70 2e69 6e66 5d2c 2030 290d  f, -np.inf], 0).
+0001b130: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0001b140: 6461 7461 5b3a 3a2d 315d 2020 2320 5265  data[::-1]  # Re
+0001b150: 7665 7273 6520 7468 6520 6461 7461 6672  verse the datafr
+0001b160: 616d 6520 736f 2074 6861 7420 6974 7320  ame so that its 
+0001b170: 7468 6520 6f6c 6465 7374 2064 6174 6520  the oldest date 
+0001b180: 6669 7273 740d 0a20 2020 2020 2020 206d  first..        m
+0001b190: 6163 644c 696e 6520 3d20 706b 7461 6c69  acdLine = pktali
+0001b1a0: 622e 4d41 4344 2864 6174 615b 2243 6c6f  b.MACD(data["Clo
+0001b1b0: 7365 225d 2c20 3132 2c20 3236 2c20 3929  se"], 12, 26, 9)
+0001b1c0: 5b30 5d2e 7461 696c 2833 290d 0a20 2020  [0].tail(3)..   
+0001b1d0: 2020 2020 206d 6163 6453 6967 6e61 6c20       macdSignal 
+0001b1e0: 3d20 706b 7461 6c69 622e 4d41 4344 2864  = pktalib.MACD(d
+0001b1f0: 6174 615b 2243 6c6f 7365 225d 2c20 3132  ata["Close"], 12
+0001b200: 2c20 3236 2c20 3929 5b31 5d2e 7461 696c  , 26, 9)[1].tail
+0001b210: 2833 290d 0a20 2020 2020 2020 206d 6163  (3)..        mac
+0001b220: 6448 6973 7420 3d20 706b 7461 6c69 622e  dHist = pktalib.
+0001b230: 4d41 4344 2864 6174 615b 2243 6c6f 7365  MACD(data["Close
+0001b240: 225d 2c20 3132 2c20 3236 2c20 3929 5b32  "], 12, 26, 9)[2
+0001b250: 5d2e 7461 696c 2833 290d 0a0d 0a20 2020  ].tail(3)....   
+0001b260: 2020 2020 2072 6574 7572 6e20 280d 0a20       return (.. 
+0001b270: 2020 2020 2020 2020 2020 2028 6d61 6364             (macd
+0001b280: 4869 7374 2e69 6c6f 635b 3a31 5d2e 696c  Hist.iloc[:1].il
+0001b290: 6f63 5b30 5d20 3c20 6d61 6364 4869 7374  oc[0] < macdHist
+0001b2a0: 2e69 6c6f 635b 3a32 5d2e 696c 6f63 5b31  .iloc[:2].iloc[1
+0001b2b0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+0001b2c0: 616e 6420 286d 6163 6448 6973 742e 696c  and (macdHist.il
+0001b2d0: 6f63 5b3a 335d 2e69 6c6f 635b 325d 203e  oc[:3].iloc[2] >
+0001b2e0: 206d 6163 6448 6973 742e 696c 6f63 5b3a   macdHist.iloc[:
+0001b2f0: 325d 2e69 6c6f 635b 315d 290d 0a20 2020  2].iloc[1])..   
+0001b300: 2020 2020 2020 2020 2061 6e64 2028 0d0a           and (..
+0001b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b320: 286d 6163 644c 696e 652e 696c 6f63 5b3a  (macdLine.iloc[:
+0001b330: 335d 2e69 6c6f 635b 325d 202d 206d 6163  3].iloc[2] - mac
+0001b340: 6453 6967 6e61 6c2e 696c 6f63 5b3a 335d  dSignal.iloc[:3]
+0001b350: 2e69 6c6f 635b 325d 290d 0a20 2020 2020  .iloc[2])..     
+0001b360: 2020 2020 2020 2020 2020 202d 2028 6d61             - (ma
+0001b370: 6364 4c69 6e65 2e69 6c6f 635b 3a32 5d2e  cdLine.iloc[:2].
+0001b380: 696c 6f63 5b31 5d20 2d20 6d61 6364 5369  iloc[1] - macdSi
+0001b390: 676e 616c 2e69 6c6f 635b 3a32 5d2e 696c  gnal.iloc[:2].il
+0001b3a0: 6f63 5b31 5d29 0d0a 2020 2020 2020 2020  oc[1])..        
+0001b3b0: 2020 2020 2020 2020 3e3d 2030 2e34 0d0a          >= 0.4..
+0001b3c0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0001b3d0: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
+0001b3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b3f0: 2020 286d 6163 644c 696e 652e 696c 6f63    (macdLine.iloc
+0001b400: 5b3a 325d 2e69 6c6f 635b 315d 202d 206d  [:2].iloc[1] - m
+0001b410: 6163 6453 6967 6e61 6c2e 696c 6f63 5b3a  acdSignal.iloc[:
+0001b420: 325d 2e69 6c6f 635b 315d 290d 0a20 2020  2].iloc[1])..   
+0001b430: 2020 2020 2020 2020 2020 2020 202d 2028               - (
+0001b440: 6d61 6364 4c69 6e65 2e69 6c6f 635b 3a31  macdLine.iloc[:1
+0001b450: 5d2e 696c 6f63 5b30 5d20 2d20 6d61 6364  ].iloc[0] - macd
+0001b460: 5369 676e 616c 2e69 6c6f 635b 3a31 5d2e  Signal.iloc[:1].
+0001b470: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
+0001b480: 2020 2020 2020 2020 2020 3c3d 2030 2e32            <= 0.2
+0001b490: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+0001b4a0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001b4b0: 2028 6d61 6364 4c69 6e65 2e69 6c6f 635b   (macdLine.iloc[
+0001b4c0: 3a33 5d2e 696c 6f63 5b32 5d20 3e20 6d61  :3].iloc[2] > ma
+0001b4d0: 6364 5369 676e 616c 2e69 6c6f 635b 3a33  cdSignal.iloc[:3
+0001b4e0: 5d2e 696c 6f63 5b32 5d29 0d0a 2020 2020  ].iloc[2])..    
+0001b4f0: 2020 2020 2020 2020 616e 6420 280d 0a20          and (.. 
+0001b500: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0001b510: 6d61 6364 4c69 6e65 2e69 6c6f 635b 3a33  macdLine.iloc[:3
+0001b520: 5d2e 696c 6f63 5b32 5d20 2d20 6d61 6364  ].iloc[2] - macd
+0001b530: 5369 676e 616c 2e69 6c6f 635b 3a33 5d2e  Signal.iloc[:3].
+0001b540: 696c 6f63 5b32 5d29 0d0a 2020 2020 2020  iloc[2])..      
+0001b550: 2020 2020 2020 2020 2020 2d20 286d 6163            - (mac
+0001b560: 644c 696e 652e 696c 6f63 5b3a 325d 2e69  dLine.iloc[:2].i
+0001b570: 6c6f 635b 315d 202d 206d 6163 6453 6967  loc[1] - macdSig
+0001b580: 6e61 6c2e 696c 6f63 5b3a 325d 2e69 6c6f  nal.iloc[:2].ilo
+0001b590: 635b 315d 290d 0a20 2020 2020 2020 2020  c[1])..         
+0001b5a0: 2020 2020 2020 203c 2031 0d0a 2020 2020         < 1..    
+0001b5b0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001b5c0: 2020 2029 0d0a 0d0a 2020 2020 2340 6d65     )....    #@me
+0001b5d0: 6173 7572 655f 7469 6d65 0d0a 2020 2020  asure_time..    
+0001b5e0: 2320 7661 6c69 6461 7465 2069 6620 4343  # validate if CC
+0001b5f0: 4920 6973 2077 6974 6869 6e20 6769 7665  I is within give
+0001b600: 6e20 7261 6e67 650d 0a20 2020 2064 6566  n range..    def
+0001b610: 2076 616c 6964 6174 6543 4349 2873 656c   validateCCI(sel
+0001b620: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+0001b630: 742c 2073 6176 6544 6963 742c 206d 696e  t, saveDict, min
+0001b640: 4343 492c 206d 6178 4343 4929 3a0d 0a20  CCI, maxCCI):.. 
+0001b650: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
+0001b660: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
+0001b670: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+0001b680: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+0001b690: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0001b6a0: 6466 2e63 6f70 7928 290d 0a20 2020 2020  df.copy()..     
+0001b6b0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
+0001b6c0: 696c 6c6e 6128 3029 0d0a 2020 2020 2020  illna(0)..      
+0001b6d0: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+0001b6e0: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
+0001b6f0: 6e70 2e69 6e66 5d2c 2030 290d 0a20 2020  np.inf], 0)..   
+0001b700: 2020 2020 2063 6369 203d 2069 6e74 2864       cci = int(d
+0001b710: 6174 612e 6865 6164 2831 295b 2243 4349  ata.head(1)["CCI
+0001b720: 225d 2e69 6c6f 635b 305d 290d 0a20 2020  "].iloc[0])..   
+0001b730: 2020 2020 2073 6176 6544 6963 745b 2243       saveDict["C
+0001b740: 4349 225d 203d 2063 6369 0d0a 2020 2020  CI"] = cci..    
+0001b750: 2020 2020 6966 2028 6363 6920 3e3d 206d      if (cci >= m
+0001b760: 696e 4343 4920 616e 6420 6363 6920 3c3d  inCCI and cci <=
+0001b770: 206d 6178 4343 4929 3a0d 0a20 2020 2020   maxCCI):..     
+0001b780: 2020 2020 2020 2069 6620 2822 5570 2220         if ("Up" 
+0001b790: 696e 2073 6176 6544 6963 745b 2254 7265  in saveDict["Tre
+0001b7a0: 6e64 225d 293a 0d0a 2020 2020 2020 2020  nd"]):..        
+0001b7b0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+0001b7c0: 6374 5b22 4343 4922 5d20 3d20 280d 0a20  ct["CCI"] = (.. 
+0001b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b7e0: 2020 2028 636f 6c6f 7254 6578 742e 424f     (colorText.BO
+0001b7f0: 4c44 2069 6620 2822 5374 726f 6e67 2220  LD if ("Strong" 
+0001b800: 696e 2073 6176 6544 6963 745b 2254 7265  in saveDict["Tre
+0001b810: 6e64 225d 2920 656c 7365 2022 2229 202b  nd"]) else "") +
+0001b820: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+0001b830: 202b 2073 7472 2863 6369 2920 2b20 636f   + str(cci) + co
+0001b840: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+0001b850: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0001b860: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001b870: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001b880: 2020 2073 6372 6565 6e44 6963 745b 2243     screenDict["C
+0001b890: 4349 225d 203d 2028 0d0a 2020 2020 2020  CI"] = (..      
+0001b8a0: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+0001b8b0: 6f6c 6f72 5465 7874 2e42 4f4c 4420 6966  olorText.BOLD if
+0001b8c0: 2028 2253 7472 6f6e 6722 2069 6e20 7361   ("Strong" in sa
+0001b8d0: 7665 4469 6374 5b22 5472 656e 6422 5d29  veDict["Trend"])
+0001b8e0: 2065 6c73 6520 2222 2920 2b20 636f 6c6f   else "") + colo
+0001b8f0: 7254 6578 742e 4641 494c 202b 2073 7472  rText.FAIL + str
+0001b900: 2863 6369 2920 2b20 636f 6c6f 7254 6578  (cci) + colorTex
+0001b910: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+0001b920: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001b930: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0001b940: 650d 0a20 2020 2020 2020 2073 6372 6565  e..        scree
+0001b950: 6e44 6963 745b 2243 4349 225d 203d 2063  nDict["CCI"] = c
+0001b960: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+0001b970: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
+0001b980: 2073 7472 2863 6369 2920 2b20 636f 6c6f   str(cci) + colo
+0001b990: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+0001b9a0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+0001b9b0: 0a0d 0a20 2020 2023 2046 696e 6420 436f  ...    # Find Co
+0001b9c0: 6e66 6c75 6365 6e63 650d 0a20 2020 2064  nflucence..    d
+0001b9d0: 6566 2076 616c 6964 6174 6543 6f6e 666c  ef validateConfl
+0001b9e0: 7565 6e63 6528 7365 6c66 2c20 7374 6f63  uence(self, stoc
+0001b9f0: 6b2c 2064 662c 2073 6372 6565 6e44 6963  k, df, screenDic
+0001ba00: 742c 2073 6176 6544 6963 742c 2070 6572  t, saveDict, per
+0001ba10: 6365 6e74 6167 653d 302e 312c 636f 6e66  centage=0.1,conf
+0001ba20: 4669 6c74 6572 3d33 293a 0d0a 2020 2020  Filter=3):..    
+0001ba30: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+0001ba40: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+0001ba50: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+0001ba60: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+0001ba70: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+0001ba80: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+0001ba90: 7265 6365 6e74 203d 2064 6174 612e 6865  recent = data.he
+0001baa0: 6164 2832 290d 0a20 2020 2020 2020 2069  ad(2)..        i
+0001bab0: 6620 6c65 6e28 7265 6365 6e74 2920 3c20  f len(recent) < 
+0001bac0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
+0001bad0: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+0001bae0: 2020 2020 2020 6973 3530 444d 4155 7054        is50DMAUpT
+0001baf0: 7265 6e64 203d 2028 7265 6365 6e74 5b22  rend = (recent["
+0001bb00: 534d 4122 5d2e 696c 6f63 5b30 5d20 3e20  SMA"].iloc[0] > 
+0001bb10: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
+0001bb20: 6f63 5b31 5d29 0d0a 2020 2020 2020 2020  oc[1])..        
+0001bb30: 6973 3530 444d 4144 6f77 6e54 7265 6e64  is50DMADownTrend
+0001bb40: 203d 2028 7265 6365 6e74 5b22 534d 4122   = (recent["SMA"
+0001bb50: 5d2e 696c 6f63 5b30 5d20 3c20 7265 6365  ].iloc[0] < rece
+0001bb60: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b31  nt["SMA"].iloc[1
+0001bb70: 5d29 0d0a 2020 2020 2020 2020 6973 476f  ])..        isGo
+0001bb80: 6c64 656e 4372 6f73 734f 7665 7220 3d20  ldenCrossOver = 
+0001bb90: 2872 6563 656e 745b 2253 4d41 225d 2e69  (recent["SMA"].i
+0001bba0: 6c6f 635b 305d 203e 3d20 7265 6365 6e74  loc[0] >= recent
+0001bbb0: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d29  ["LMA"].iloc[0])
+0001bbc0: 2061 6e64 205c 0d0a 2020 2020 2020 2020   and \..        
+0001bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbe0: 2020 2020 2872 6563 656e 745b 2253 4d41      (recent["SMA
+0001bbf0: 225d 2e69 6c6f 635b 315d 203c 3d20 7265  "].iloc[1] <= re
+0001bc00: 6365 6e74 5b22 4c4d 4122 5d2e 696c 6f63  cent["LMA"].iloc
+0001bc10: 5b31 5d29 0d0a 2020 2020 2020 2020 6973  [1])..        is
+0001bc20: 4465 6164 4372 6f73 734f 7665 7220 3d20  DeadCrossOver = 
+0001bc30: 2872 6563 656e 745b 2253 4d41 225d 2e69  (recent["SMA"].i
+0001bc40: 6c6f 635b 305d 203c 3d20 7265 6365 6e74  loc[0] <= recent
+0001bc50: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d29  ["LMA"].iloc[0])
+0001bc60: 2061 6e64 205c 0d0a 2020 2020 2020 2020   and \..        
+0001bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc80: 2020 2020 2872 6563 656e 745b 2253 4d41      (recent["SMA
+0001bc90: 225d 2e69 6c6f 635b 315d 203e 3d20 7265  "].iloc[1] >= re
+0001bca0: 6365 6e74 5b22 4c4d 4122 5d2e 696c 6f63  cent["LMA"].iloc
+0001bcb0: 5b31 5d29 0d0a 2020 2020 2020 2020 6973  [1])..        is
+0001bcc0: 3530 444d 4120 3d20 2872 6563 656e 745b  50DMA = (recent[
+0001bcd0: 2253 4d41 225d 2e69 6c6f 635b 305d 203c  "SMA"].iloc[0] <
+0001bce0: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
+0001bcf0: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
+0001bd00: 2020 2020 6973 3230 3044 4d41 203d 2028      is200DMA = (
+0001bd10: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
+0001bd20: 6f63 5b30 5d20 3c3d 2072 6563 656e 745b  oc[0] <= recent[
+0001bd30: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+0001bd40: 290d 0a20 2020 2020 2020 2064 6966 6665  )..        diffe
+0001bd50: 7265 6e63 6520 3d20 726f 756e 6428 2872  rence = round((r
+0001bd60: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
+0001bd70: 635b 305d 202d 2072 6563 656e 745b 224c  c[0] - recent["L
+0001bd80: 4d41 225d 2e69 6c6f 635b 305d 290d 0a20  MA"].iloc[0]).. 
+0001bd90: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+0001bda0: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
+0001bdb0: 2e69 6c6f 635b 305d 0d0a 2020 2020 2020  .iloc[0]..      
+0001bdc0: 2020 2020 2020 2020 2020 2a20 3130 302c            * 100,
+0001bdd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bde0: 2020 322c 0d0a 2020 2020 2020 2020 2020    2,..          
+0001bdf0: 2020 290d 0a20 2020 2020 2020 2073 6176    )..        sav
+0001be00: 6544 6963 745b 2243 6f6e 6644 4d41 4469  eDict["ConfDMADi
+0001be10: 6666 6572 656e 6365 225d 203d 2064 6966  fference"] = dif
+0001be20: 6665 7265 6e63 650d 0a20 2020 2020 2020  ference..       
+0001be30: 2073 6372 6565 6e44 6963 745b 2243 6f6e   screenDict["Con
+0001be40: 6644 4d41 4469 6666 6572 656e 6365 225d  fDMADifference"]
+0001be50: 203d 2064 6966 6665 7265 6e63 650d 0a20   = difference.. 
+0001be60: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
+0001be70: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
+0001be80: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
+0001be90: 4469 6374 2c73 6176 6544 6963 742c 224d  Dict,saveDict,"M
+0001bea0: 412d 5369 676e 616c 2229 0d0a 2020 2020  A-Signal")..    
+0001beb0: 2020 2020 2320 6469 6666 6572 656e 6365      # difference
+0001bec0: 203d 2061 6273 2864 6966 6665 7265 6e63   = abs(differenc
+0001bed0: 6529 0d0a 2020 2020 2020 2020 636f 6e66  e)..        conf
+0001bee0: 5465 7874 203d 2066 227b 2747 6f6c 6465  Text = f"{'Golde
+0001bef0: 6e43 726f 7373 6f76 6572 2720 6966 2069  nCrossover' if i
+0001bf00: 7347 6f6c 6465 6e43 726f 7373 4f76 6572  sGoldenCrossOver
+0001bf10: 2065 6c73 6520 2827 4465 6164 4372 6f73   else ('DeadCros
+0001bf20: 736f 7665 7227 2069 6620 6973 4465 6164  sover' if isDead
+0001bf30: 4372 6f73 734f 7665 7220 656c 7365 2028  CrossOver else (
+0001bf40: 2743 6f6e 662e 5570 2720 6966 2069 7335  'Conf.Up' if is5
+0001bf50: 3044 4d41 5570 5472 656e 6420 656c 7365  0DMAUpTrend else
+0001bf60: 2028 2743 6f6e 662e 446f 776e 2720 6966   ('Conf.Down' if
+0001bf70: 2069 7335 3044 4d41 446f 776e 5472 656e   is50DMADownTren
+0001bf80: 6420 656c 7365 2028 2735 3044 4d41 2720  d else ('50DMA' 
+0001bf90: 6966 2069 7335 3044 4d41 2065 6c73 6520  if is50DMA else 
+0001bfa0: 2827 3230 3044 4d41 2720 6966 2069 7332  ('200DMA' if is2
+0001bfb0: 3030 444d 4120 656c 7365 2027 556e 6b6e  00DMA else 'Unkn
+0001bfc0: 6f77 6e27 2929 2929 297d 220d 0a20 2020  own')))))}"..   
+0001bfd0: 2020 2020 2069 6620 6162 7328 7265 6365       if abs(rece
+0001bfe0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
+0001bff0: 5d20 2d20 7265 6365 6e74 5b22 4c4d 4122  ] - recent["LMA"
+0001c000: 5d2e 696c 6f63 5b30 5d29 203c 3d20 280d  ].iloc[0]) <= (.
+0001c010: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
+0001c020: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
+0001c030: 305d 202a 2070 6572 6365 6e74 6167 650d  0] * percentage.
+0001c040: 0a20 2020 2020 2020 2029 3a0d 0a20 2020  .        ):..   
+0001c050: 2020 2020 2020 2020 2069 6620 7265 6365           if rece
+0001c060: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
+0001c070: 5d20 3e3d 2072 6563 656e 745b 224c 4d41  ] >= recent["LMA
+0001c080: 225d 2e69 6c6f 635b 305d 3a0d 0a20 2020  "].iloc[0]:..   
+0001c090: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+0001c0a0: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
+0001c0b0: 616c 225d 203d 2028 0d0a 2020 2020 2020  al"] = (..      
+0001c0c0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+0001c0d0: 7665 645b 305d 200d 0a20 2020 2020 2020  ved[0] ..       
+0001c0e0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001c0f0: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
+0001c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c110: 2020 202b 2028 636f 6c6f 7254 6578 742e     + (colorText.
+0001c120: 4752 4545 4e20 6966 2069 7335 3044 4d41  GREEN if is50DMA
+0001c130: 5570 5472 656e 6420 656c 7365 2028 636f  UpTrend else (co
+0001c140: 6c6f 7254 6578 742e 4641 494c 2069 6620  lorText.FAIL if 
+0001c150: 6973 3530 444d 4144 6f77 6e54 7265 6e64  is50DMADownTrend
+0001c160: 2065 6c73 6520 636f 6c6f 7254 6578 742e   else colorText.
+0001c170: 5741 524e 2929 0d0a 2020 2020 2020 2020  WARN))..        
+0001c180: 2020 2020 2020 2020 2020 2020 2b20 6622              + f"
+0001c190: 7b63 6f6e 6654 6578 747d 2028 7b64 6966  {confText} ({dif
+0001c1a0: 6665 7265 6e63 657d 2529 220d 0a20 2020  ference}%)"..   
+0001c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1c0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001c1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c1e0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+0001c1f0: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
+0001c200: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
+0001c210: 6564 5b31 5d20 2b20 6622 7b63 6f6e 6654  ed[1] + f"{confT
+0001c220: 6578 747d 2028 7b64 6966 6665 7265 6e63  ext} ({differenc
+0001c230: 657d 2529 220d 0a20 2020 2020 2020 2020  e}%)"..         
+0001c240: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0001c250: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+0001c260: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+0001c270: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
+0001c280: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+0001c290: 5b30 5d20 0d0a 2020 2020 2020 2020 2020  [0] ..          
+0001c2a0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001c2b0: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
+0001c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c2d0: 2b20 2863 6f6c 6f72 5465 7874 2e47 5245  + (colorText.GRE
+0001c2e0: 454e 2069 6620 6973 3530 444d 4155 7054  EN if is50DMAUpT
+0001c2f0: 7265 6e64 2065 6c73 6520 2863 6f6c 6f72  rend else (color
+0001c300: 5465 7874 2e46 4149 4c20 6966 2069 7335  Text.FAIL if is5
+0001c310: 3044 4d41 446f 776e 5472 656e 6420 656c  0DMADownTrend el
+0001c320: 7365 2063 6f6c 6f72 5465 7874 2e57 4152  se colorText.WAR
+0001c330: 4e29 290d 0a20 2020 2020 2020 2020 2020  N))..           
+0001c340: 2020 2020 2020 2020 202b 2066 227b 636f           + f"{co
+0001c350: 6e66 5465 7874 7d20 287b 6469 6666 6572  nfText} ({differ
+0001c360: 656e 6365 7d25 2922 0d0a 2020 2020 2020  ence}%)"..      
+0001c370: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001c380: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+0001c390: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001c3a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c3b0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
+0001c3c0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
+0001c3d0: 315d 202b 2066 227b 636f 6e66 5465 7874  1] + f"{confText
+0001c3e0: 7d20 287b 6469 6666 6572 656e 6365 7d25  } ({difference}%
+0001c3f0: 2922 0d0a 2020 2020 2020 2020 2020 2020  )"..            
+0001c400: 7265 7475 726e 2063 6f6e 6646 696c 7465  return confFilte
+0001c410: 7220 3d3d 2033 206f 7220 5c0d 0a20 2020  r == 3 or \..   
+0001c420: 2020 2020 2020 2020 2020 2020 2028 636f               (co
+0001c430: 6e66 4669 6c74 6572 203d 3d20 3120 616e  nfFilter == 1 an
+0001c440: 6420 2869 7335 3044 4d41 5570 5472 656e  d (is50DMAUpTren
+0001c450: 6420 6f72 2028 6973 476f 6c64 656e 4372  d or (isGoldenCr
+0001c460: 6f73 734f 7665 7220 6f72 2027 5570 2720  ossOver or 'Up' 
+0001c470: 696e 2063 6f6e 6654 6578 7429 2929 206f  in confText))) o
+0001c480: 7220 5c0d 0a20 2020 2020 2020 2020 2020  r \..           
+0001c490: 2020 2020 2028 636f 6e66 4669 6c74 6572       (confFilter
+0001c4a0: 203d 3d20 3220 616e 6420 2869 7335 3044   == 2 and (is50D
+0001c4b0: 4d41 446f 776e 5472 656e 6420 6f72 2069  MADownTrend or i
+0001c4c0: 7344 6561 6443 726f 7373 4f76 6572 206f  sDeadCrossOver o
+0001c4d0: 7220 2744 6f77 6e27 2069 6e20 636f 6e66  r 'Down' in conf
+0001c4e0: 5465 7874 2929 0d0a 2020 2020 2020 2020  Text))..        
+0001c4f0: 2320 4d61 7962 6520 7468 6520 6469 6666  # Maybe the diff
+0001c500: 6572 656e 6365 2069 7320 6e6f 7420 7769  erence is not wi
+0001c510: 7468 696e 2074 6865 2072 616e 6765 2c20  thin the range, 
+0001c520: 6275 7420 7765 2764 2073 7469 6c6c 206c  but we'd still l
+0001c530: 696b 6520 746f 206b 6565 7020 7468 6520  ike to keep the 
+0001c540: 7374 6f63 6b20 696e 0d0a 2020 2020 2020  stock in..      
+0001c550: 2020 2320 7468 6520 6c69 7374 2069 6620    # the list if 
+0001c560: 6974 2773 2061 2067 6f6c 6465 6e20 6372  it's a golden cr
+0001c570: 6f73 736f 7665 7220 6f72 2064 6561 6420  ossover or dead 
+0001c580: 6372 6f73 736f 7665 720d 0a20 2020 2020  crossover..     
+0001c590: 2020 2069 6620 6973 476f 6c64 656e 4372     if isGoldenCr
+0001c5a0: 6f73 734f 7665 7220 6f72 2069 7344 6561  ossOver or isDea
+0001c5b0: 6443 726f 7373 4f76 6572 3a0d 0a20 2020  dCrossOver:..   
+0001c5c0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+0001c5d0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+0001c5e0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+0001c5f0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+0001c600: 305d 200d 0a20 2020 2020 2020 2020 2020  0] ..           
+0001c610: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001c620: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
+0001c630: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001c640: 2028 636f 6c6f 7254 6578 742e 4752 4545   (colorText.GREE
+0001c650: 4e20 6966 2069 7335 3044 4d41 5570 5472  N if is50DMAUpTr
+0001c660: 656e 6420 656c 7365 2028 636f 6c6f 7254  end else (colorT
+0001c670: 6578 742e 4641 494c 2069 6620 6973 3530  ext.FAIL if is50
+0001c680: 444d 4144 6f77 6e54 7265 6e64 2065 6c73  DMADownTrend els
+0001c690: 6520 636f 6c6f 7254 6578 742e 5741 524e  e colorText.WARN
+0001c6a0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0001c6b0: 2020 2020 2020 2020 2b20 6622 7b63 6f6e          + f"{con
+0001c6c0: 6654 6578 747d 2028 7b64 6966 6665 7265  fText} ({differe
+0001c6d0: 6e63 657d 2529 220d 0a20 2020 2020 2020  nce}%)"..       
+0001c6e0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001c6f0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+0001c700: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0001c710: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+0001c720: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
+0001c730: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+0001c740: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
+0001c750: 6966 6665 7265 6e63 657d 2529 220d 0a20  ifference}%)".. 
+0001c760: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001c770: 6e20 636f 6e66 4669 6c74 6572 203d 3d20  n confFilter == 
+0001c780: 3320 6f72 205c 0d0a 2020 2020 2020 2020  3 or \..        
+0001c790: 2020 2020 2020 2020 2863 6f6e 6646 696c          (confFil
+0001c7a0: 7465 7220 3d3d 2031 2061 6e64 2069 7347  ter == 1 and isG
+0001c7b0: 6f6c 6465 6e43 726f 7373 4f76 6572 2920  oldenCrossOver) 
+0001c7c0: 6f72 205c 0d0a 2020 2020 2020 2020 2020  or \..          
+0001c7d0: 2020 2020 2020 2863 6f6e 6646 696c 7465        (confFilte
+0001c7e0: 7220 3d3d 2032 2061 6e64 2069 7344 6561  r == 2 and isDea
+0001c7f0: 6443 726f 7373 4f76 6572 290d 0a20 2020  dCrossOver)..   
+0001c800: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+0001c810: 650d 0a0d 0a20 2020 2023 406d 6561 7375  e....    #@measu
+0001c820: 7265 5f74 696d 650d 0a20 2020 2023 2056  re_time..    # V
+0001c830: 616c 6964 6174 6520 6966 2073 6861 7265  alidate if share
+0001c840: 2070 7269 6365 7320 6172 6520 636f 6e73   prices are cons
+0001c850: 6f6c 6964 6174 696e 670d 0a20 2020 2064  olidating..    d
+0001c860: 6566 2076 616c 6964 6174 6543 6f6e 736f  ef validateConso
+0001c870: 6c69 6461 7469 6f6e 2873 656c 662c 2064  lidation(self, d
+0001c880: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+0001c890: 6176 6544 6963 742c 2070 6572 6365 6e74  aveDict, percent
+0001c8a0: 6167 653d 3130 293a 0d0a 2020 2020 2020  age=10):..      
+0001c8b0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+0001c8c0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+0001c8d0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0001c8e0: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
+0001c8f0: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
+0001c900: 7079 2829 0d0a 2020 2020 2020 2020 6461  py()..        da
+0001c910: 7461 203d 2064 6174 612e 6669 6c6c 6e61  ta = data.fillna
+0001c920: 2830 290d 0a20 2020 2020 2020 2064 6174  (0)..        dat
+0001c930: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
+0001c940: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
+0001c950: 665d 2c20 3029 0d0a 2020 2020 2020 2020  f], 0)..        
+0001c960: 6863 203d 2064 6174 612e 6465 7363 7269  hc = data.descri
+0001c970: 6265 2829 5b22 436c 6f73 6522 5d5b 226d  be()["Close"]["m
+0001c980: 6178 225d 0d0a 2020 2020 2020 2020 6c63  ax"]..        lc
+0001c990: 203d 2064 6174 612e 6465 7363 7269 6265   = data.describe
+0001c9a0: 2829 5b22 436c 6f73 6522 5d5b 226d 696e  ()["Close"]["min
+0001c9b0: 225d 0d0a 2020 2020 2020 2020 6966 2028  "]..        if (
+0001c9c0: 6863 202d 206c 6329 203c 3d20 2868 6320  hc - lc) <= (hc 
+0001c9d0: 2a20 7065 7263 656e 7461 6765 202f 2031  * percentage / 1
+0001c9e0: 3030 2920 616e 6420 2868 6320 2d20 6c63  00) and (hc - lc
+0001c9f0: 2021 3d20 3029 3a0d 0a20 2020 2020 2020   != 0):..       
+0001ca00: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001ca10: 2243 6f6e 736f 6c2e 225d 203d 2028 0d0a  "Consol."] = (..
+0001ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca30: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
+0001ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca50: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+0001ca60: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
+0001ca70: 2020 202b 2022 5261 6e67 653a 220d 0a20     + "Range:".. 
+0001ca80: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001ca90: 2073 7472 2872 6f75 6e64 2828 6162 7328   str(round((abs(
+0001caa0: 2868 6320 2d20 6c63 2920 2f20 6863 2920  (hc - lc) / hc) 
+0001cab0: 2a20 3130 3029 2c20 3129 290d 0a20 2020  * 100), 1))..   
+0001cac0: 2020 2020 2020 2020 2020 2020 202b 2022               + "
+0001cad0: 2522 0d0a 2020 2020 2020 2020 2020 2020  %"..            
+0001cae0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+0001caf0: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+0001cb00: 2029 0d0a 2020 2020 2020 2020 656c 7365   )..        else
+0001cb10: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+0001cb20: 6372 6565 6e44 6963 745b 2243 6f6e 736f  creenDict["Conso
+0001cb30: 6c2e 225d 203d 2028 0d0a 2020 2020 2020  l."] = (..      
+0001cb40: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
+0001cb50: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
+0001cb60: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001cb70: 7254 6578 742e 4641 494c 0d0a 2020 2020  rText.FAIL..    
+0001cb80: 2020 2020 2020 2020 2020 2020 2b20 2252              + "R
+0001cb90: 616e 6765 3a22 0d0a 2020 2020 2020 2020  ange:"..        
+0001cba0: 2020 2020 2020 2020 2b20 7374 7228 726f          + str(ro
+0001cbb0: 756e 6428 2861 6273 2828 6863 202d 206c  und((abs((hc - l
+0001cbc0: 6329 202f 2068 6329 202a 2031 3030 292c  c) / hc) * 100),
+0001cbd0: 2031 2929 0d0a 2020 2020 2020 2020 2020   1))..          
+0001cbe0: 2020 2020 2020 2b20 2225 220d 0a20 2020        + "%"..   
+0001cbf0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001cc00: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+0001cc10: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0001cc20: 2020 2020 2073 6176 6544 6963 745b 2243       saveDict["C
+0001cc30: 6f6e 736f 6c2e 225d 203d 2066 2752 616e  onsol."] = f'Ran
+0001cc40: 6765 3a7b 7374 7228 726f 756e 6428 2861  ge:{str(round((a
+0001cc50: 6273 2828 6863 2d6c 6329 2f68 6329 2a31  bs((hc-lc)/hc)*1
+0001cc60: 3030 292c 3129 292b 2225 227d 270d 0a20  00),1))+"%"}'.. 
+0001cc70: 2020 2020 2020 2072 6574 7572 6e20 726f         return ro
+0001cc80: 756e 6428 2861 6273 2828 6863 202d 206c  und((abs((hc - l
+0001cc90: 6329 202f 2068 6329 202a 2031 3030 292c  c) / hc) * 100),
+0001cca0: 2031 290d 0a0d 0a20 2020 2023 2076 616c   1)....    # val
+0001ccb0: 6964 6174 6520 6966 2074 6865 2073 746f  idate if the sto
+0001ccc0: 636b 2068 6173 2062 6565 6e20 6861 7669  ck has been havi
+0001ccd0: 6e67 2068 6967 6865 7220 6869 6768 732c  ng higher highs,
+0001cce0: 2068 6967 6865 7220 6c6f 7773 0d0a 2020   higher lows..  
+0001ccf0: 2020 2320 616e 6420 6869 6768 6572 2063    # and higher c
+0001cd00: 6c6f 7365 2077 6974 6820 6c61 7465 7374  lose with latest
+0001cd10: 2063 6c6f 7365 203e 2073 7570 6572 7472   close > supertr
+0001cd20: 656e 6420 616e 6420 382d 454d 412e 0d0a  end and 8-EMA...
+0001cd30: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0001cd40: 4869 6768 6572 4869 6768 7348 6967 6865  HigherHighsHighe
+0001cd50: 724c 6f77 7348 6967 6865 7243 6c6f 7365  rLowsHigherClose
+0001cd60: 2873 656c 662c 2064 6629 3a0d 0a20 2020  (self, df):..   
+0001cd70: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+0001cd80: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+0001cd90: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+0001cda0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+0001cdb0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+0001cdc0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+0001cdd0: 2064 6179 3020 3d20 6461 7461 0d0a 2020   day0 = data..  
+0001cde0: 2020 2020 2020 6461 7931 203d 2064 6174        day1 = dat
+0001cdf0: 615b 313a 5d0d 0a20 2020 2020 2020 2064  a[1:]..        d
+0001ce00: 6179 3220 3d20 6461 7461 5b32 3a5d 0d0a  ay2 = data[2:]..
+0001ce10: 2020 2020 2020 2020 6461 7933 203d 2064          day3 = d
+0001ce20: 6174 615b 333a 5d0d 0a20 2020 2020 2020  ata[3:]..       
+0001ce30: 2069 6620 6c65 6e28 6461 7931 2920 3c20   if len(day1) < 
+0001ce40: 3120 6f72 206c 656e 2864 6179 3229 203c  1 or len(day2) <
+0001ce50: 2031 206f 7220 6c65 6e28 6461 7933 2920   1 or len(day3) 
+0001ce60: 3c20 313a 0d0a 2020 2020 2020 2020 2020  < 1:..          
+0001ce70: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+0001ce80: 2020 2020 2020 2020 6869 6768 6572 4869          higherHi
+0001ce90: 6768 7320 3d20 280d 0a20 2020 2020 2020  ghs = (..       
+0001cea0: 2020 2020 2028 6461 7930 5b22 4869 6768       (day0["High
+0001ceb0: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
+0001cec0: 315b 2248 6967 6822 5d2e 696c 6f63 5b30  1["High"].iloc[0
+0001ced0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+0001cee0: 616e 6420 2864 6179 315b 2248 6967 6822  and (day1["High"
+0001cef0: 5d2e 696c 6f63 5b30 5d20 3e20 6461 7932  ].iloc[0] > day2
+0001cf00: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
+0001cf10: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+0001cf20: 6e64 2028 6461 7932 5b22 4869 6768 225d  nd (day2["High"]
+0001cf30: 2e69 6c6f 635b 305d 203e 2064 6179 335b  .iloc[0] > day3[
+0001cf40: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
+0001cf50: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+0001cf60: 2020 2020 2068 6967 6865 724c 6f77 7320       higherLows 
+0001cf70: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+0001cf80: 2028 6461 7930 5b22 4c6f 7722 5d2e 696c   (day0["Low"].il
+0001cf90: 6f63 5b30 5d20 3e20 6461 7931 5b22 4c6f  oc[0] > day1["Lo
+0001cfa0: 7722 5d2e 696c 6f63 5b30 5d29 0d0a 2020  w"].iloc[0])..  
+0001cfb0: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
+0001cfc0: 6179 315b 224c 6f77 225d 2e69 6c6f 635b  ay1["Low"].iloc[
+0001cfd0: 305d 203e 2064 6179 325b 224c 6f77 225d  0] > day2["Low"]
+0001cfe0: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
+0001cff0: 2020 2020 2020 2061 6e64 2028 6461 7932         and (day2
+0001d000: 5b22 4c6f 7722 5d2e 696c 6f63 5b30 5d20  ["Low"].iloc[0] 
+0001d010: 3e20 6461 7933 5b22 4c6f 7722 5d2e 696c  > day3["Low"].il
+0001d020: 6f63 5b30 5d29 0d0a 2020 2020 2020 2020  oc[0])..        
+0001d030: 290d 0a20 2020 2020 2020 2068 6967 6865  )..        highe
+0001d040: 7243 6c6f 7365 203d 2028 0d0a 2020 2020  rClose = (..    
+0001d050: 2020 2020 2020 2020 2864 6179 305b 2243          (day0["C
+0001d060: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
+0001d070: 2064 6179 315b 2243 6c6f 7365 225d 2e69   day1["Close"].i
+0001d080: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
+0001d090: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
+0001d0a0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+0001d0b0: 3e20 6461 7932 5b22 436c 6f73 6522 5d2e  > day2["Close"].
+0001d0c0: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
+0001d0d0: 2020 2020 2020 616e 6420 2864 6179 325b        and (day2[
+0001d0e0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+0001d0f0: 203e 2064 6179 335b 2243 6c6f 7365 225d   > day3["Close"]
+0001d100: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
+0001d110: 2020 2029 0d0a 2020 2020 2020 2020 2320     )..        # 
+0001d120: 6869 6768 6572 5253 4920 3d20 2864 6179  higherRSI = (day
+0001d130: 305b 2252 5349 225d 2e69 6c6f 635b 305d  0["RSI"].iloc[0]
+0001d140: 203e 2064 6179 315b 2252 5349 225d 2e69   > day1["RSI"].i
+0001d150: 6c6f 635b 305d 2920 616e 6420 5c0d 0a20  loc[0]) and \.. 
+0001d160: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001d170: 2020 2020 2020 2020 2028 6461 7931 5b22           (day1["
+0001d180: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
+0001d190: 6461 7932 5b22 5253 4922 5d2e 696c 6f63  day2["RSI"].iloc
+0001d1a0: 5b30 5d29 2061 6e64 205c 0d0a 2020 2020  [0]) and \..    
+0001d1b0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0001d1c0: 2020 2020 2020 2864 6179 325b 2252 5349        (day2["RSI
+0001d1d0: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
+0001d1e0: 335b 2252 5349 225d 2e69 6c6f 635b 305d  3["RSI"].iloc[0]
+0001d1f0: 2920 616e 6420 5c0d 0a20 2020 2020 2020  ) and \..       
+0001d200: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0001d210: 2020 2064 6179 335b 2252 5349 225d 2e69     day3["RSI"].i
+0001d220: 6c6f 635b 305d 203e 3d20 3530 2061 6e64  loc[0] >= 50 and
+0001d230: 2064 6179 305b 2252 5349 225d 2e69 6c6f   day0["RSI"].ilo
+0001d240: 635b 305d 203e 3d20 3635 0d0a 2020 2020  c[0] >= 65..    
+0001d250: 2020 2020 7265 7665 7273 6564 4461 7461      reversedData
+0001d260: 203d 2064 6174 615b 3a3a 2d31 5d2e 636f   = data[::-1].co
+0001d270: 7079 2829 0d0a 2020 2020 2020 2020 7265  py()..        re
+0001d280: 7665 7273 6564 4461 7461 5b22 5355 5045  versedData["SUPE
+0001d290: 5254 225d 203d 2070 6b74 616c 6962 2e73  RT"] = pktalib.s
+0001d2a0: 7570 6572 7472 656e 6428 7265 7665 7273  upertrend(revers
+0001d2b0: 6564 4461 7461 2c20 372c 2033 295b 2253  edData, 7, 3)["S
+0001d2c0: 5550 4552 545f 375f 332e 3022 5d0d 0a20  UPERT_7_3.0"].. 
+0001d2d0: 2020 2020 2020 2072 6576 6572 7365 6444         reversedD
+0001d2e0: 6174 615b 2245 4d41 3822 5d20 3d20 706b  ata["EMA8"] = pk
+0001d2f0: 7461 6c69 622e 454d 4128 7265 7665 7273  talib.EMA(revers
+0001d300: 6564 4461 7461 5b22 436c 6f73 6522 5d2c  edData["Close"],
+0001d310: 2074 696d 6570 6572 696f 643d 3929 0d0a   timeperiod=9)..
+0001d320: 2020 2020 2020 2020 6869 6768 6572 436c          higherCl
+0001d330: 6f73 6520 3d20 280d 0a20 2020 2020 2020  ose = (..       
+0001d340: 2020 2020 2068 6967 6865 7243 6c6f 7365       higherClose
+0001d350: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+0001d360: 6420 6461 7930 5b22 436c 6f73 6522 5d2e  d day0["Close"].
+0001d370: 696c 6f63 5b30 5d20 3e20 7265 7665 7273  iloc[0] > revers
+0001d380: 6564 4461 7461 2e74 6169 6c28 3129 5b22  edData.tail(1)["
+0001d390: 5355 5045 5254 225d 2e69 6c6f 635b 305d  SUPERT"].iloc[0]
+0001d3a0: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+0001d3b0: 6420 6461 7930 5b22 436c 6f73 6522 5d2e  d day0["Close"].
+0001d3c0: 696c 6f63 5b30 5d20 3e20 7265 7665 7273  iloc[0] > revers
+0001d3d0: 6564 4461 7461 2e74 6169 6c28 3129 5b22  edData.tail(1)["
+0001d3e0: 454d 4138 225d 2e69 6c6f 635b 305d 0d0a  EMA8"].iloc[0]..
+0001d3f0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001d400: 2020 2072 6574 7572 6e20 6869 6768 6572     return higher
+0001d410: 4869 6768 7320 616e 6420 6869 6768 6572  Highs and higher
+0001d420: 4c6f 7773 2061 6e64 2068 6967 6865 7243  Lows and higherC
+0001d430: 6c6f 7365 0d0a 0d0a 2020 2020 2340 6d65  lose....    #@me
+0001d440: 6173 7572 655f 7469 6d65 0d0a 2020 2020  asure_time..    
+0001d450: 2320 5661 6c69 6461 7465 2027 496e 7369  # Validate 'Insi
+0001d460: 6465 2042 6172 2720 7374 7275 6374 7572  de Bar' structur
+0001d470: 6520 666f 7220 7265 6365 6e74 2064 6179  e for recent day
+0001d480: 730d 0a20 2020 2064 6566 2076 616c 6964  s..    def valid
+0001d490: 6174 6549 6e73 6964 6542 6172 280d 0a20  ateInsideBar(.. 
+0001d4a0: 2020 2020 2020 2073 656c 662c 2064 662c         self, df,
+0001d4b0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+0001d4c0: 6544 6963 742c 2063 6861 7274 5061 7474  eDict, chartPatt
+0001d4d0: 6572 6e3d 312c 2064 6179 7354 6f4c 6f6f  ern=1, daysToLoo
+0001d4e0: 6b62 6163 6b3d 350d 0a20 2020 2029 3a0d  kback=5..    ):.
+0001d4f0: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
+0001d500: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+0001d510: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
+0001d520: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+0001d530: 650d 0a20 2020 2020 2020 2064 6174 6120  e..        data 
+0001d540: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
+0001d550: 2020 2020 206f 7267 4461 7461 203d 2064       orgData = d
+0001d560: 6174 610d 0a20 2020 2020 2020 2073 6176  ata..        sav
+0001d570: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+0001d580: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+0001d590: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+0001d5a0: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
+0001d5b0: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
+0001d5c0: 696e 2072 616e 6765 2869 6e74 2864 6179  in range(int(day
+0001d5d0: 7354 6f4c 6f6f 6b62 6163 6b29 2c20 696e  sToLookback), in
+0001d5e0: 7428 726f 756e 6428 6461 7973 546f 4c6f  t(round(daysToLo
+0001d5f0: 6f6b 6261 636b 202a 2030 2e35 2929 202d  okback * 0.5)) -
+0001d600: 2031 2c20 2d31 293a 0d0a 2020 2020 2020   1, -1):..      
+0001d610: 2020 2020 2020 6966 2069 203d 3d20 323a        if i == 2:
+0001d620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d630: 2020 7265 7475 726e 2030 2020 2320 4578    return 0  # Ex
+0001d640: 6974 2069 6620 6f6e 6c79 206c 6173 7420  it if only last 
+0001d650: 3220 6361 6e64 6c65 7320 6172 6520 6c65  2 candles are le
+0001d660: 6674 0d0a 2020 2020 2020 2020 2020 2020  ft..            
+0001d670: 6966 2063 6861 7274 5061 7474 6572 6e20  if chartPattern 
+0001d680: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
+0001d690: 2020 2020 2020 2069 6620 2255 7022 2069         if "Up" i
+0001d6a0: 6e20 7361 7665 4469 6374 5b22 5472 656e  n saveDict["Tren
+0001d6b0: 6422 5d20 616e 6420 280d 0a20 2020 2020  d"] and (..     
+0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001d6d0: 4275 6c6c 2220 696e 2073 6176 6544 6963  Bull" in saveDic
+0001d6e0: 745b 224d 412d 5369 676e 616c 225d 0d0a  t["MA-Signal"]..
+0001d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d700: 2020 2020 6f72 2022 5375 7070 6f72 7422      or "Support"
+0001d710: 2069 6e20 7361 7665 4469 6374 5b22 4d41   in saveDict["MA
+0001d720: 2d53 6967 6e61 6c22 5d0d 0a20 2020 2020  -Signal"]..     
+0001d730: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
+0001d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d750: 2020 2064 6174 6120 3d20 6f72 6744 6174     data = orgDat
+0001d760: 612e 6865 6164 2869 290d 0a20 2020 2020  a.head(i)..     
+0001d770: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001d780: 6566 4361 6e64 6c65 203d 2064 6174 612e  efCandle = data.
+0001d790: 7461 696c 2831 290d 0a20 2020 2020 2020  tail(1)..       
+0001d7a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001d7b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001d7c0: 2020 2020 2020 2020 2020 2028 6c65 6e28             (len(
+0001d7d0: 6461 7461 2e48 6967 685b 6461 7461 2e48  data.High[data.H
+0001d7e0: 6967 6820 3e20 7265 6643 616e 646c 652e  igh > refCandle.
+0001d7f0: 4869 6768 2e69 7465 6d28 295d 2920 3d3d  High.item()]) ==
+0001d800: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
+0001d810: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+0001d820: 2028 6c65 6e28 6461 7461 2e4c 6f77 5b64   (len(data.Low[d
+0001d830: 6174 612e 4c6f 7720 3c20 7265 6643 616e  ata.Low < refCan
+0001d840: 646c 652e 4c6f 772e 6974 656d 2829 5d29  dle.Low.item()])
+0001d850: 203d 3d20 3029 0d0a 2020 2020 2020 2020   == 0)..        
+0001d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d870: 616e 6420 286c 656e 2864 6174 612e 4f70  and (len(data.Op
+0001d880: 656e 5b64 6174 612e 4f70 656e 203e 2072  en[data.Open > r
+0001d890: 6566 4361 6e64 6c65 2e48 6967 682e 6974  efCandle.High.it
+0001d8a0: 656d 2829 5d29 203d 3d20 3029 0d0a 2020  em()]) == 0)..  
+0001d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8c0: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
+0001d8d0: 6174 612e 436c 6f73 655b 6461 7461 2e43  ata.Close[data.C
+0001d8e0: 6c6f 7365 203c 2072 6566 4361 6e64 6c65  lose < refCandle
+0001d8f0: 2e4c 6f77 2e69 7465 6d28 295d 2920 3d3d  .Low.item()]) ==
+0001d900: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
+0001d910: 2020 2020 2020 2020 2029 3a0d 0a20 2020           ):..   
+0001d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d930: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001d940: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
+0001d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d960: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0001d970: 645b 305d 0d0a 2020 2020 2020 2020 2020  d[0]..          
+0001d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d990: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
+0001d9a0: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
+0001d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9c0: 2b20 636f 6c6f 7254 6578 742e 5741 524e  + colorText.WARN
+0001d9d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d9e0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001d9f0: 2822 496e 7369 6465 2042 6172 2028 2564  ("Inside Bar (%d
+0001da00: 2922 2025 2069 290d 0a20 2020 2020 2020  )" % i)..       
+0001da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da20: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001da30: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+0001da40: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0001da50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001da60: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+0001da70: 745b 2250 6174 7465 726e 225d 203d 2073  t["Pattern"] = s
+0001da80: 6176 6564 5b31 5d20 2b20 2249 6e73 6964  aved[1] + "Insid
+0001da90: 6520 4261 7220 2825 6429 2220 2520 690d  e Bar (%d)" % i.
+0001daa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001dab0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001dac0: 690d 0a20 2020 2020 2020 2020 2020 2020  i..             
+0001dad0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0001dae0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001daf0: 7475 726e 2030 0d0a 2020 2020 2020 2020  turn 0..        
+0001db00: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0001db10: 2020 2020 2020 2020 2020 2069 6620 2244             if "D
+0001db20: 6f77 6e22 2069 6e20 7361 7665 4469 6374  own" in saveDict
+0001db30: 5b22 5472 656e 6422 5d20 616e 6420 280d  ["Trend"] and (.
+0001db40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001db50: 2020 2020 2022 4265 6172 2220 696e 2073       "Bear" in s
+0001db60: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+0001db70: 616c 225d 206f 7220 2252 6573 6973 7422  al"] or "Resist"
+0001db80: 2069 6e20 7361 7665 4469 6374 5b22 4d41   in saveDict["MA
+0001db90: 2d53 6967 6e61 6c22 5d0d 0a20 2020 2020  -Signal"]..     
+0001dba0: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
+0001dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbc0: 2020 2064 6174 6120 3d20 6f72 6744 6174     data = orgDat
+0001dbd0: 612e 6865 6164 2869 290d 0a20 2020 2020  a.head(i)..     
+0001dbe0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001dbf0: 6566 4361 6e64 6c65 203d 2064 6174 612e  efCandle = data.
+0001dc00: 7461 696c 2831 290d 0a20 2020 2020 2020  tail(1)..       
+0001dc10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001dc20: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001dc30: 2020 2020 2020 2020 2020 2028 6c65 6e28             (len(
+0001dc40: 6461 7461 2e48 6967 685b 6461 7461 2e48  data.High[data.H
+0001dc50: 6967 6820 3e20 7265 6643 616e 646c 652e  igh > refCandle.
+0001dc60: 4869 6768 2e69 7465 6d28 295d 2920 3d3d  High.item()]) ==
+0001dc70: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
+0001dc80: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+0001dc90: 2028 6c65 6e28 6461 7461 2e4c 6f77 5b64   (len(data.Low[d
+0001dca0: 6174 612e 4c6f 7720 3c20 7265 6643 616e  ata.Low < refCan
+0001dcb0: 646c 652e 4c6f 772e 6974 656d 2829 5d29  dle.Low.item()])
+0001dcc0: 203d 3d20 3029 0d0a 2020 2020 2020 2020   == 0)..        
+0001dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dce0: 616e 6420 286c 656e 2864 6174 612e 4f70  and (len(data.Op
+0001dcf0: 656e 5b64 6174 612e 4f70 656e 203e 2072  en[data.Open > r
+0001dd00: 6566 4361 6e64 6c65 2e48 6967 682e 6974  efCandle.High.it
+0001dd10: 656d 2829 5d29 203d 3d20 3029 0d0a 2020  em()]) == 0)..  
+0001dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dd30: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
+0001dd40: 6174 612e 436c 6f73 655b 6461 7461 2e43  ata.Close[data.C
+0001dd50: 6c6f 7365 203c 2072 6566 4361 6e64 6c65  lose < refCandle
+0001dd60: 2e4c 6f77 2e69 7465 6d28 295d 2920 3d3d  .Low.item()]) ==
+0001dd70: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
+0001dd80: 2020 2020 2020 2020 2029 3a0d 0a20 2020           ):..   
+0001dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dda0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001ddb0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
+0001ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddd0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0001dde0: 645b 305d 0d0a 2020 2020 2020 2020 2020  d[0]..          
+0001ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de00: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
+0001de10: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
+0001de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de30: 2b20 636f 6c6f 7254 6578 742e 5741 524e  + colorText.WARN
+0001de40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001de50: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001de60: 2822 496e 7369 6465 2042 6172 2028 2564  ("Inside Bar (%d
+0001de70: 2922 2025 2069 290d 0a20 2020 2020 2020  )" % i)..       
+0001de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de90: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001dea0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+0001deb0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0001dec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ded0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+0001dee0: 745b 2250 6174 7465 726e 225d 203d 2073  t["Pattern"] = s
+0001def0: 6176 6564 5b31 5d20 2b20 2249 6e73 6964  aved[1] + "Insid
+0001df00: 6520 4261 7220 2825 6429 2220 2520 690d  e Bar (%d)" % i.
+0001df10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001df20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001df30: 690d 0a20 2020 2020 2020 2020 2020 2020  i..             
+0001df40: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0001df50: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001df60: 7475 726e 2030 0d0a 2020 2020 2020 2020  turn 0..        
+0001df70: 7265 7475 726e 2030 0d0a 0d0a 2020 2020  return 0....    
+0001df80: 2320 4669 6e64 2049 504f 2062 6173 650d  # Find IPO base.
+0001df90: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0001dfa0: 6549 706f 4261 7365 2873 656c 662c 2073  eIpoBase(self, s
+0001dfb0: 746f 636b 2c20 6466 2c20 7363 7265 656e  tock, df, screen
+0001dfc0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+0001dfd0: 7065 7263 656e 7461 6765 3d30 2e33 293a  percentage=0.3):
+0001dfe0: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+0001dff0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+0001e000: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+0001e010: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001e020: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
+0001e030: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+0001e040: 2020 2020 2020 6c69 7374 696e 6750 7269        listingPri
+0001e050: 6365 203d 2064 6174 615b 3a3a 2d31 5d2e  ce = data[::-1].
+0001e060: 6865 6164 2831 295b 224f 7065 6e22 5d2e  head(1)["Open"].
+0001e070: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
+0001e080: 2063 7572 7265 6e74 5072 6963 6520 3d20   currentPrice = 
+0001e090: 6461 7461 2e68 6561 6428 3129 5b22 436c  data.head(1)["Cl
+0001e0a0: 6f73 6522 5d2e 696c 6f63 5b30 5d0d 0a20  ose"].iloc[0].. 
+0001e0b0: 2020 2020 2020 2041 5448 203d 2064 6174         ATH = dat
+0001e0c0: 612e 6465 7363 7269 6265 2829 5b22 4869  a.describe()["Hi
+0001e0d0: 6768 225d 5b22 6d61 7822 5d0d 0a20 2020  gh"]["max"]..   
+0001e0e0: 2020 2020 2069 6620 4154 4820 3e20 286c       if ATH > (l
+0001e0f0: 6973 7469 6e67 5072 6963 6520 2b20 286c  istingPrice + (l
+0001e100: 6973 7469 6e67 5072 6963 6520 2a20 7065  istingPrice * pe
+0001e110: 7263 656e 7461 6765 2929 3a0d 0a20 2020  rcentage)):..   
+0001e120: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001e130: 4661 6c73 650d 0a20 2020 2020 2020 2061  False..        a
+0001e140: 7761 7920 3d20 726f 756e 6428 2828 6375  way = round(((cu
+0001e150: 7272 656e 7450 7269 6365 202d 206c 6973  rrentPrice - lis
+0001e160: 7469 6e67 5072 6963 6529 202f 206c 6973  tingPrice) / lis
+0001e170: 7469 6e67 5072 6963 6529 202a 2031 3030  tingPrice) * 100
+0001e180: 2c20 3129 0d0a 2020 2020 2020 2020 6966  , 1)..        if
+0001e190: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0001e1a0: 286c 6973 7469 6e67 5072 6963 6520 2d20  (listingPrice - 
+0001e1b0: 286c 6973 7469 6e67 5072 6963 6520 2a20  (listingPrice * 
+0001e1c0: 7065 7263 656e 7461 6765 2929 0d0a 2020  percentage))..  
+0001e1d0: 2020 2020 2020 2020 2020 3c3d 2063 7572            <= cur
+0001e1e0: 7265 6e74 5072 6963 650d 0a20 2020 2020  rentPrice..     
+0001e1f0: 2020 2020 2020 203c 3d20 286c 6973 7469         <= (listi
+0001e200: 6e67 5072 6963 6520 2b20 286c 6973 7469  ngPrice + (listi
+0001e210: 6e67 5072 6963 6520 2a20 7065 7263 656e  ngPrice * percen
+0001e220: 7461 6765 2929 0d0a 2020 2020 2020 2020  tage))..        
+0001e230: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001e240: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
+0001e250: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
+0001e260: 7565 2873 6372 6565 6e44 6963 742c 2073  ue(screenDict, s
+0001e270: 6176 6544 6963 742c 2022 5061 7474 6572  aveDict, "Patter
+0001e280: 6e22 290d 0a20 2020 2020 2020 2020 2020  n")..           
+0001e290: 2069 6620 6177 6179 203e 2030 3a0d 0a20   if away > 0:.. 
+0001e2a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001e2b0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+0001e2c0: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
+0001e2d0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+0001e2e0: 7665 645b 305d 200d 0a20 2020 2020 2020  ved[0] ..       
+0001e2f0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001e300: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
+0001e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e320: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
+0001e330: 5245 454e 0d0a 2020 2020 2020 2020 2020  REEN..          
+0001e340: 2020 2020 2020 2020 2020 2b20 6622 4950            + f"IP
+0001e350: 4f20 4261 7365 2028 7b61 7761 797d 2025  O Base ({away} %
+0001e360: 2922 0d0a 2020 2020 2020 2020 2020 2020  )"..            
+0001e370: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001e380: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
+0001e390: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+0001e3a0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001e3b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001e3c0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+0001e3d0: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
+0001e3e0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+0001e3f0: 7665 645b 305d 0d0a 2020 2020 2020 2020  ved[0]..        
+0001e400: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+0001e410: 6c6f 7254 6578 742e 424f 4c44 0d0a 2020  lorText.BOLD..  
+0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e430: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
+0001e440: 4545 4e0d 0a20 2020 2020 2020 2020 2020  EEN..           
+0001e450: 2020 2020 2020 2020 202b 2022 4950 4f20           + "IPO 
+0001e460: 4261 7365 2022 0d0a 2020 2020 2020 2020  Base "..        
+0001e470: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+0001e480: 6c6f 7254 6578 742e 4641 494c 0d0a 2020  lorText.FAIL..  
+0001e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4a0: 2020 2b20 6622 287b 6177 6179 7d20 2529    + f"({away} %)
+0001e4b0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+0001e4c0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+0001e4d0: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+0001e4e0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001e4f0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
+0001e500: 2250 6174 7465 726e 225d 203d 2073 6176  "Pattern"] = sav
+0001e510: 6564 5b31 5d20 2b20 6622 4950 4f20 4261  ed[1] + f"IPO Ba
+0001e520: 7365 2028 7b61 7761 797d 2025 2922 0d0a  se ({away} %)"..
+0001e530: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001e540: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
+0001e550: 2072 6574 7572 6e20 4661 6c73 650d 0a0d   return False...
+0001e560: 0a20 2020 2023 406d 6561 7375 7265 5f74  .    #@measure_t
+0001e570: 696d 650d 0a20 2020 2023 2056 616c 6964  ime..    # Valid
+0001e580: 6174 6520 4c6f 7265 6e74 7a69 616e 2043  ate Lorentzian C
+0001e590: 6c61 7373 6966 6963 6174 696f 6e20 7369  lassification si
+0001e5a0: 676e 616c 0d0a 2020 2020 6465 6620 7661  gnal..    def va
+0001e5b0: 6c69 6461 7465 4c6f 7265 6e74 7a69 616e  lidateLorentzian
+0001e5c0: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
+0001e5d0: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+0001e5e0: 206c 6f6f 6b46 6f72 3d33 293a 0d0a 2020   lookFor=3):..  
+0001e5f0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+0001e600: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+0001e610: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+0001e620: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+0001e630: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001e640: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
+0001e650: 2020 2320 6c6f 6f6b 466f 723a 2031 2d42    # lookFor: 1-B
+0001e660: 7579 2c20 322d 5365 6c6c 2c20 332d 416e  uy, 2-Sell, 3-An
+0001e670: 790d 0a20 2020 2020 2020 2064 6174 6120  y..        data 
+0001e680: 3d20 6461 7461 5b3a 3a2d 315d 2020 2320  = data[::-1]  # 
+0001e690: 5265 7665 7273 6520 7468 6520 6461 7461  Reverse the data
+0001e6a0: 6672 616d 650d 0a20 2020 2020 2020 2064  frame..        d
+0001e6b0: 6174 6120 3d20 6461 7461 2e72 656e 616d  ata = data.renam
+0001e6c0: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+0001e6d0: 636f 6c75 6d6e 733d 7b0d 0a20 2020 2020  columns={..     
+0001e6e0: 2020 2020 2020 2020 2020 2022 4f70 656e             "Open
+0001e6f0: 223a 2022 6f70 656e 222c 0d0a 2020 2020  ": "open",..    
+0001e700: 2020 2020 2020 2020 2020 2020 2243 6c6f              "Clo
+0001e710: 7365 223a 2022 636c 6f73 6522 2c0d 0a20  se": "close",.. 
+0001e720: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001e730: 4869 6768 223a 2022 6869 6768 222c 0d0a  High": "high",..
+0001e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e750: 224c 6f77 223a 2022 6c6f 7722 2c0d 0a20  "Low": "low",.. 
+0001e760: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001e770: 566f 6c75 6d65 223a 2022 766f 6c75 6d65  Volume": "volume
+0001e780: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001e790: 7d0d 0a20 2020 2020 2020 2029 0d0a 2020  }..        )..  
+0001e7a0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+0001e7b0: 2020 2020 2020 2020 7769 7468 2053 7570          with Sup
+0001e7c0: 7072 6573 734f 7574 7075 7428 7375 7070  pressOutput(supp
+0001e7d0: 7265 7373 5f73 7464 6f75 743d 5472 7565  ress_stdout=True
+0001e7e0: 2c20 7375 7070 7265 7373 5f73 7464 6572  , suppress_stder
+0001e7f0: 723d 5472 7565 293a 0d0a 2020 2020 2020  r=True):..      
+0001e800: 2020 2020 2020 2020 2020 6c63 203d 2061            lc = a
+0001e810: 7461 2e4c 6f72 656e 747a 6961 6e43 6c61  ta.LorentzianCla
+0001e820: 7373 6966 6963 6174 696f 6e28 6461 7461  ssification(data
+0001e830: 3d64 6174 6129 0d0a 2020 2020 2020 2020  =data)..        
+0001e840: 2020 2020 7361 7665 6420 3d20 7365 6c66      saved = self
+0001e850: 2e66 696e 6443 7572 7265 6e74 5361 7665  .findCurrentSave
+0001e860: 6456 616c 7565 2873 6372 6565 6e44 6963  dValue(screenDic
+0001e870: 742c 2073 6176 6544 6963 742c 2022 5061  t, saveDict, "Pa
+0001e880: 7474 6572 6e22 290d 0a20 2020 2020 2020  ttern")..       
+0001e890: 2020 2020 2069 6620 6c63 2e64 662e 696c       if lc.df.il
+0001e8a0: 6f63 5b2d 315d 5b22 6973 4e65 7742 7579  oc[-1]["isNewBuy
+0001e8b0: 5369 676e 616c 225d 3a0d 0a20 2020 2020  Signal"]:..     
+0001e8c0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001e8d0: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+0001e8e0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+0001e8f0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+0001e900: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
+0001e910: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+0001e920: 4752 4545 4e20 2b20 224c 6f72 656e 747a  GREEN + "Lorentz
+0001e930: 6961 6e2d 4275 7922 202b 2063 6f6c 6f72  ian-Buy" + color
+0001e940: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+0001e950: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0001e960: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+0001e970: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
+0001e980: 203d 2073 6176 6564 5b31 5d20 2b20 224c   = saved[1] + "L
+0001e990: 6f72 656e 747a 6961 6e2d 4275 7922 0d0a  orentzian-Buy"..
+0001e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9b0: 6966 206c 6f6f 6b46 6f72 2021 3d20 323a  if lookFor != 2:
+0001e9c0: 2023 204e 6f74 2053 656c 6c0d 0a20 2020   # Not Sell..   
+0001e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9e0: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
+0001e9f0: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+0001ea00: 632e 6466 2e69 6c6f 635b 2d31 5d5b 2269  c.df.iloc[-1]["i
+0001ea10: 734e 6577 5365 6c6c 5369 676e 616c 225d  sNewSellSignal"]
+0001ea20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001ea30: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+0001ea40: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
+0001ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea60: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
+0001ea70: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+0001ea80: 6c6f 7254 6578 742e 4641 494c 202b 2022  lorText.FAIL + "
+0001ea90: 4c6f 7265 6e74 7a69 616e 2d53 656c 6c22  Lorentzian-Sell"
+0001eaa0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001eab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001eac0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+0001ead0: 2020 2020 2073 6176 6544 6963 745b 2250       saveDict["P
+0001eae0: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
+0001eaf0: 5b31 5d20 2b20 224c 6f72 656e 747a 6961  [1] + "Lorentzia
+0001eb00: 6e2d 5365 6c6c 220d 0a20 2020 2020 2020  n-Sell"..       
+0001eb10: 2020 2020 2020 2020 2069 6620 6c6f 6f6b           if look
+0001eb20: 466f 7220 213d 2031 3a20 2320 4e6f 7420  For != 1: # Not 
+0001eb30: 4275 790d 0a20 2020 2020 2020 2020 2020  Buy..           
+0001eb40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001eb50: 5472 7565 0d0a 2020 2020 2020 2020 6578  True..        ex
+0001eb60: 6365 7074 2045 7863 6570 7469 6f6e 3a20  cept Exception: 
+0001eb70: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+0001eb80: 7665 720d 0a20 2020 2020 2020 2020 2020  ver..           
+0001eb90: 2023 2056 616c 7565 4572 726f 723a 206f   # ValueError: o
+0001eba0: 7065 7261 6e64 7320 636f 756c 6420 6e6f  perands could no
+0001ebb0: 7420 6265 2062 726f 6164 6361 7374 2074  t be broadcast t
+0001ebc0: 6f67 6574 6865 7220 7769 7468 2073 6861  ogether with sha
+0001ebd0: 7065 7320 2832 302c 2920 2832 362c 290d  pes (20,) (26,).
+0001ebe0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0001ebf0: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
+0001ec00: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
+0001ec10: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
+0001ec20: 6164 7661 6e63 6564 5f74 612f 4c6f 7265  advanced_ta/Lore
+0001ec30: 6e74 7a69 616e 436c 6173 7369 6669 6361  ntzianClassifica
+0001ec40: 7469 6f6e 2f43 6c61 7373 6966 6965 722e  tion/Classifier.
+0001ec50: 7079 222c 206c 696e 6520 3138 362c 2069  py", line 186, i
+0001ec60: 6e20 5f5f 696e 6974 5f5f 0d0a 2020 2020  n __init__..    
+0001ec70: 2020 2020 2020 2020 2320 4669 6c65 2022          # File "
+0001ec80: 2f6f 7074 2f68 6f6d 6562 7265 772f 6c69  /opt/homebrew/li
+0001ec90: 622f 7079 7468 6f6e 332e 3131 2f73 6974  b/python3.11/sit
+0001eca0: 652d 7061 636b 6167 6573 2f61 6476 616e  e-packages/advan
+0001ecb0: 6365 645f 7461 2f4c 6f72 656e 747a 6961  ced_ta/Lorentzia
+0001ecc0: 6e43 6c61 7373 6966 6963 6174 696f 6e2f  nClassification/
+0001ecd0: 436c 6173 7369 6669 6572 2e70 7922 2c20  Classifier.py", 
+0001ece0: 6c69 6e65 2033 3935 2c20 696e 205f 5f63  line 395, in __c
+0001ecf0: 6c61 7373 6966 790d 0a20 2020 2020 2020  lassify..       
+0001ed00: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
+0001ed10: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
+0001ed20: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
+0001ed30: 6163 6b61 6765 732f 7061 6e64 6173 2f63  ackages/pandas/c
+0001ed40: 6f72 652f 6f70 732f 636f 6d6d 6f6e 2e70  ore/ops/common.p
+0001ed50: 7922 2c20 6c69 6e65 2037 362c 2069 6e20  y", line 76, in 
+0001ed60: 6e65 775f 6d65 7468 6f64 0d0a 2020 2020  new_method..    
+0001ed70: 2020 2020 2020 2020 2320 4669 6c65 2022          # File "
+0001ed80: 2f6f 7074 2f68 6f6d 6562 7265 772f 6c69  /opt/homebrew/li
+0001ed90: 622f 7079 7468 6f6e 332e 3131 2f73 6974  b/python3.11/sit
+0001eda0: 652d 7061 636b 6167 6573 2f70 616e 6461  e-packages/panda
+0001edb0: 732f 636f 7265 2f61 7272 6179 6c69 6b65  s/core/arraylike
+0001edc0: 2e70 7922 2c20 6c69 6e65 2037 302c 2069  .py", line 70, i
+0001edd0: 6e20 5f5f 616e 645f 5f0d 0a20 2020 2020  n __and__..     
+0001ede0: 2020 2020 2020 2023 2046 696c 6520 222f         # File "/
+0001edf0: 6f70 742f 686f 6d65 6272 6577 2f6c 6962  opt/homebrew/lib
+0001ee00: 2f70 7974 686f 6e33 2e31 312f 7369 7465  /python3.11/site
+0001ee10: 2d70 6163 6b61 6765 732f 7061 6e64 6173  -packages/pandas
+0001ee20: 2f63 6f72 652f 7365 7269 6573 2e70 7922  /core/series.py"
+0001ee30: 2c20 6c69 6e65 2035 3831 302c 2069 6e20  , line 5810, in 
+0001ee40: 5f6c 6f67 6963 616c 5f6d 6574 686f 640d  _logical_method.
+0001ee50: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0001ee60: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
+0001ee70: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
+0001ee80: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
+0001ee90: 7061 6e64 6173 2f63 6f72 652f 6f70 732f  pandas/core/ops/
+0001eea0: 6172 7261 795f 6f70 732e 7079 222c 206c  array_ops.py", l
+0001eeb0: 696e 6520 3435 362c 2069 6e20 6c6f 6769  ine 456, in logi
+0001eec0: 6361 6c5f 6f70 0d0a 2020 2020 2020 2020  cal_op..        
+0001eed0: 2020 2020 2320 4669 6c65 2022 2f6f 7074      # File "/opt
+0001eee0: 2f68 6f6d 6562 7265 772f 6c69 622f 7079  /homebrew/lib/py
+0001eef0: 7468 6f6e 332e 3131 2f73 6974 652d 7061  thon3.11/site-pa
+0001ef00: 636b 6167 6573 2f70 616e 6461 732f 636f  ckages/pandas/co
+0001ef10: 7265 2f6f 7073 2f61 7272 6179 5f6f 7073  re/ops/array_ops
+0001ef20: 2e70 7922 2c20 6c69 6e65 2033 3634 2c20  .py", line 364, 
+0001ef30: 696e 206e 615f 6c6f 6769 6361 6c5f 6f70  in na_logical_op
+0001ef40: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001ef50: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+0001ef60: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
+0001ef70: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
+0001ef80: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
+0001ef90: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0001efa0: 6c73 650d 0a0d 0a20 2020 2023 2076 616c  lse....    # val
+0001efb0: 6964 6174 6520 6966 2074 6865 2073 746f  idate if the sto
+0001efc0: 636b 2068 6173 2062 6565 6e20 6861 7669  ck has been havi
+0001efd0: 6e67 206c 6f77 6572 206c 6f77 732c 206c  ng lower lows, l
+0001efe0: 6f77 6572 2068 6967 6873 0d0a 2020 2020  ower highs..    
+0001eff0: 6465 6620 7661 6c69 6461 7465 4c6f 7765  def validateLowe
+0001f000: 7248 6967 6873 4c6f 7765 724c 6f77 7328  rHighsLowerLows(
+0001f010: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
+0001f020: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+0001f030: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+0001f040: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+0001f050: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+0001f060: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+0001f070: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+0001f080: 6461 7930 203d 2064 6174 610d 0a20 2020  day0 = data..   
+0001f090: 2020 2020 2064 6179 3120 3d20 6461 7461       day1 = data
+0001f0a0: 5b31 3a5d 0d0a 2020 2020 2020 2020 6461  [1:]..        da
+0001f0b0: 7932 203d 2064 6174 615b 323a 5d0d 0a20  y2 = data[2:].. 
+0001f0c0: 2020 2020 2020 2064 6179 3320 3d20 6461         day3 = da
+0001f0d0: 7461 5b33 3a5d 0d0a 2020 2020 2020 2020  ta[3:]..        
+0001f0e0: 6c6f 7765 7248 6967 6873 203d 2028 0d0a  lowerHighs = (..
+0001f0f0: 2020 2020 2020 2020 2020 2020 2864 6179              (day
+0001f100: 305b 2248 6967 6822 5d2e 696c 6f63 5b30  0["High"].iloc[0
+0001f110: 5d20 3c20 6461 7931 5b22 4869 6768 225d  ] < day1["High"]
+0001f120: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
+0001f130: 2020 2020 2020 2061 6e64 2028 6461 7931         and (day1
+0001f140: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
+0001f150: 203c 2064 6179 325b 2248 6967 6822 5d2e   < day2["High"].
+0001f160: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
+0001f170: 2020 2020 2020 616e 6420 2864 6179 325b        and (day2[
+0001f180: 2248 6967 6822 5d2e 696c 6f63 5b30 5d20  "High"].iloc[0] 
+0001f190: 3c20 6461 7933 5b22 4869 6768 225d 2e69  < day3["High"].i
+0001f1a0: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
+0001f1b0: 2029 0d0a 2020 2020 2020 2020 6c6f 7765   )..        lowe
+0001f1c0: 724c 6f77 7320 3d20 280d 0a20 2020 2020  rLows = (..     
+0001f1d0: 2020 2020 2020 2028 6461 7930 5b22 4c6f         (day0["Lo
+0001f1e0: 7722 5d2e 696c 6f63 5b30 5d20 3c20 6461  w"].iloc[0] < da
+0001f1f0: 7931 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y1["Low"].iloc[0
+0001f200: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+0001f210: 616e 6420 2864 6179 315b 224c 6f77 225d  and (day1["Low"]
+0001f220: 2e69 6c6f 635b 305d 203c 2064 6179 325b  .iloc[0] < day2[
+0001f230: 224c 6f77 225d 2e69 6c6f 635b 305d 290d  "Low"].iloc[0]).
+0001f240: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001f250: 2028 6461 7932 5b22 4c6f 7722 5d2e 696c   (day2["Low"].il
+0001f260: 6f63 5b30 5d20 3c20 6461 7933 5b22 4c6f  oc[0] < day3["Lo
+0001f270: 7722 5d2e 696c 6f63 5b30 5d29 0d0a 2020  w"].iloc[0])..  
+0001f280: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001f290: 2068 6967 6865 7252 5349 203d 2028 0d0a   higherRSI = (..
+0001f2a0: 2020 2020 2020 2020 2020 2020 2864 6179              (day
+0001f2b0: 305b 2252 5349 225d 2e69 6c6f 635b 305d  0["RSI"].iloc[0]
+0001f2c0: 203c 2064 6179 315b 2252 5349 225d 2e69   < day1["RSI"].i
+0001f2d0: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
+0001f2e0: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
+0001f2f0: 5253 4922 5d2e 696c 6f63 5b30 5d20 3c20  RSI"].iloc[0] < 
+0001f300: 6461 7932 5b22 5253 4922 5d2e 696c 6f63  day2["RSI"].iloc
+0001f310: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
+0001f320: 2020 616e 6420 2864 6179 325b 2252 5349    and (day2["RSI
+0001f330: 225d 2e69 6c6f 635b 305d 203c 2064 6179  "].iloc[0] < day
+0001f340: 335b 2252 5349 225d 2e69 6c6f 635b 305d  3["RSI"].iloc[0]
+0001f350: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+0001f360: 6e64 2064 6179 305b 2252 5349 225d 2e69  nd day0["RSI"].i
+0001f370: 6c6f 635b 305d 203e 3d20 3530 0d0a 2020  loc[0] >= 50..  
+0001f380: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001f390: 2072 6574 7572 6e20 6c6f 7765 7248 6967   return lowerHig
+0001f3a0: 6873 2061 6e64 206c 6f77 6572 4c6f 7773  hs and lowerLows
+0001f3b0: 2061 6e64 2068 6967 6865 7252 5349 0d0a   and higherRSI..
+0001f3c0: 0d0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
+0001f3d0: 2069 6620 7265 6365 6e74 2076 6f6c 756d   if recent volum
+0001f3e0: 6520 6973 206c 6f77 6573 7420 6f66 206c  e is lowest of l
+0001f3f0: 6173 7420 274e 2720 4461 7973 0d0a 2020  ast 'N' Days..  
+0001f400: 2020 6465 6620 7661 6c69 6461 7465 4c6f    def validateLo
+0001f410: 7765 7374 566f 6c75 6d65 2873 656c 662c  westVolume(self,
+0001f420: 2064 662c 2064 6179 7346 6f72 4c6f 7765   df, daysForLowe
+0001f430: 7374 566f 6c75 6d65 293a 0d0a 2020 2020  stVolume):..    
+0001f440: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+0001f450: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+0001f460: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+0001f470: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+0001f480: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+0001f490: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+0001f4a0: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+0001f4b0: 6e61 2830 290d 0a20 2020 2020 2020 2064  na(0)..        d
+0001f4c0: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
+0001f4d0: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
+0001f4e0: 696e 665d 2c20 3029 0d0a 2020 2020 2020  inf], 0)..      
+0001f4f0: 2020 6966 2064 6179 7346 6f72 4c6f 7765    if daysForLowe
+0001f500: 7374 566f 6c75 6d65 2069 7320 4e6f 6e65  stVolume is None
+0001f510: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+0001f520: 6179 7346 6f72 4c6f 7765 7374 566f 6c75  aysForLowestVolu
+0001f530: 6d65 203d 2033 300d 0a20 2020 2020 2020  me = 30..       
+0001f540: 2069 6620 6c65 6e28 6461 7461 2920 3c20   if len(data) < 
+0001f550: 6461 7973 466f 724c 6f77 6573 7456 6f6c  daysForLowestVol
+0001f560: 756d 653a 0d0a 2020 2020 2020 2020 2020  ume:..          
+0001f570: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+0001f580: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001f590: 6174 612e 6865 6164 2864 6179 7346 6f72  ata.head(daysFor
+0001f5a0: 4c6f 7765 7374 566f 6c75 6d65 290d 0a20  LowestVolume).. 
+0001f5b0: 2020 2020 2020 2072 6563 656e 7420 3d20         recent = 
+0001f5c0: 6461 7461 2e68 6561 6428 3129 0d0a 2020  data.head(1)..  
+0001f5d0: 2020 2020 2020 6966 206c 656e 2872 6563        if len(rec
+0001f5e0: 656e 7429 203c 2031 3a0d 0a20 2020 2020  ent) < 1:..     
+0001f5f0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0001f600: 6c73 650d 0a20 2020 2020 2020 2069 6620  lse..        if 
+0001f610: 2872 6563 656e 745b 2256 6f6c 756d 6522  (recent["Volume"
+0001f620: 5d2e 696c 6f63 5b30 5d20 3c3d 2064 6174  ].iloc[0] <= dat
+0001f630: 612e 6465 7363 7269 6265 2829 5b22 566f  a.describe()["Vo
+0001f640: 6c75 6d65 225d 5b22 6d69 6e22 5d29 2061  lume"]["min"]) a
+0001f650: 6e64 2072 6563 656e 745b 0d0a 2020 2020  nd recent[..    
+0001f660: 2020 2020 2020 2020 2256 6f6c 756d 6522          "Volume"
+0001f670: 0d0a 2020 2020 2020 2020 5d5b 305d 2021  ..        ][0] !
+0001f680: 3d20 6e70 2e6e 616e 3a0d 0a20 2020 2020  = np.nan:..     
+0001f690: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+0001f6a0: 7565 0d0a 2020 2020 2020 2020 7265 7475  ue..        retu
+0001f6b0: 726e 2046 616c 7365 0d0a 0d0a 2020 2020  rn False....    
+0001f6c0: 2320 5661 6c69 6461 7465 204c 5450 2077  # Validate LTP w
+0001f6d0: 6974 6869 6e20 6c69 6d69 7473 0d0a 2020  ithin limits..  
+0001f6e0: 2020 6465 6620 7661 6c69 6461 7465 4c54    def validateLT
+0001f6f0: 5028 7365 6c66 2c20 6466 2c20 7363 7265  P(self, df, scre
+0001f700: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+0001f710: 2c20 6d69 6e4c 5450 3d4e 6f6e 652c 206d  , minLTP=None, m
+0001f720: 6178 4c54 503d 4e6f 6e65 2c6d 696e 4368  axLTP=None,minCh
+0001f730: 616e 6765 3d30 293a 0d0a 2020 2020 2020  ange=0):..      
+0001f740: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+0001f750: 2829 0d0a 2020 2020 2020 2020 6c74 7056  ()..        ltpV
+0001f760: 616c 6964 203d 2046 616c 7365 0d0a 2020  alid = False..  
+0001f770: 2020 2020 2020 6966 206d 696e 4c54 5020        if minLTP 
+0001f780: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+0001f790: 2020 2020 2020 6d69 6e4c 5450 203d 2073        minLTP = s
+0001f7a0: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
+0001f7b0: 722e 6d69 6e4c 5450 0d0a 2020 2020 2020  r.minLTP..      
+0001f7c0: 2020 6966 206d 6178 4c54 5020 6973 204e    if maxLTP is N
+0001f7d0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0001f7e0: 2020 6d61 784c 5450 203d 2073 656c 662e    maxLTP = self.
+0001f7f0: 636f 6e66 6967 4d61 6e61 6765 722e 6d61  configManager.ma
+0001f800: 784c 5450 0d0a 2020 2020 2020 2020 6461  xLTP..        da
+0001f810: 7461 203d 2064 6174 612e 6669 6c6c 6e61  ta = data.fillna
+0001f820: 2830 290d 0a20 2020 2020 2020 2064 6174  (0)..        dat
+0001f830: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
+0001f840: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
+0001f850: 665d 2c20 3029 0d0a 2020 2020 2020 2020  f], 0)..        
+0001f860: 7265 6365 6e74 203d 2064 6174 612e 6865  recent = data.he
+0001f870: 6164 2831 290d 0a0d 0a20 2020 2020 2020  ad(1)....       
+0001f880: 2070 6374 5f63 6861 6e67 6520 3d20 2864   pct_change = (d
+0001f890: 6174 615b 3a3a 2d31 5d5b 2243 6c6f 7365  ata[::-1]["Close
+0001f8a0: 225d 2e70 6374 5f63 6861 6e67 6528 2920  "].pct_change() 
+0001f8b0: 2a20 3130 3029 2e69 6c6f 635b 2d31 5d0d  * 100).iloc[-1].
+0001f8c0: 0a20 2020 2020 2020 2069 6620 7063 745f  .        if pct_
+0001f8d0: 6368 616e 6765 203d 3d20 6e70 2e69 6e66  change == np.inf
+0001f8e0: 206f 7220 7063 745f 6368 616e 6765 203d   or pct_change =
+0001f8f0: 3d20 2d6e 702e 696e 663a 0d0a 2020 2020  = -np.inf:..    
+0001f900: 2020 2020 2020 2020 7063 745f 6368 616e          pct_chan
+0001f910: 6765 203d 2030 0d0a 2020 2020 2020 2020  ge = 0..        
+0001f920: 7063 745f 7361 7665 203d 2022 252e 3166  pct_save = "%.1f
+0001f930: 2525 2220 2520 7063 745f 6368 616e 6765  %%" % pct_change
+0001f940: 0d0a 2020 2020 2020 2020 6966 2070 6374  ..        if pct
+0001f950: 5f63 6861 6e67 6520 3e20 302e 323a 0d0a  _change > 0.2:..
+0001f960: 2020 2020 2020 2020 2020 2020 7063 745f              pct_
+0001f970: 6368 616e 6765 203d 2063 6f6c 6f72 5465  change = colorTe
+0001f980: 7874 2e47 5245 454e 202b 2028 2225 2e31  xt.GREEN + ("%.1
+0001f990: 6625 2522 2025 2070 6374 5f63 6861 6e67  f%%" % pct_chang
+0001f9a0: 6529 202b 2063 6f6c 6f72 5465 7874 2e45  e) + colorText.E
+0001f9b0: 4e44 0d0a 2020 2020 2020 2020 656c 6966  ND..        elif
+0001f9c0: 2070 6374 5f63 6861 6e67 6520 3c20 2d30   pct_change < -0
+0001f9d0: 2e32 3a0d 0a20 2020 2020 2020 2020 2020  .2:..           
+0001f9e0: 2070 6374 5f63 6861 6e67 6520 3d20 636f   pct_change = co
+0001f9f0: 6c6f 7254 6578 742e 4641 494c 202b 2028  lorText.FAIL + (
+0001fa00: 2225 2e31 6625 2522 2025 2070 6374 5f63  "%.1f%%" % pct_c
+0001fa10: 6861 6e67 6529 202b 2063 6f6c 6f72 5465  hange) + colorTe
+0001fa20: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+0001fa30: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0001fa40: 2020 2070 6374 5f63 6861 6e67 6520 3d20     pct_change = 
+0001fa50: 636f 6c6f 7254 6578 742e 5741 524e 202b  colorText.WARN +
+0001fa60: 2028 2225 2e31 6625 2522 2025 2070 6374   ("%.1f%%" % pct
+0001fa70: 5f63 6861 6e67 6529 202b 2063 6f6c 6f72  _change) + color
+0001fa80: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+0001fa90: 2020 7361 7665 4469 6374 5b22 2543 686e    saveDict["%Chn
+0001faa0: 6722 5d20 3d20 7063 745f 7361 7665 0d0a  g"] = pct_save..
+0001fab0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+0001fac0: 6374 5b22 2543 686e 6722 5d20 3d20 7063  ct["%Chng"] = pc
+0001fad0: 745f 6368 616e 6765 0d0a 2020 2020 2020  t_change..      
+0001fae0: 2020 6c74 7020 3d20 726f 756e 6428 7265    ltp = round(re
+0001faf0: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
+0001fb00: 6f63 5b30 5d2c 2032 290d 0a20 2020 2020  oc[0], 2)..     
+0001fb10: 2020 2076 6572 6966 7953 7461 6765 5477     verifyStageTw
+0001fb20: 6f20 3d20 5472 7565 0d0a 2020 2020 2020  o = True..      
+0001fb30: 2020 6966 206c 656e 2864 6174 6129 203e    if len(data) >
+0001fb40: 2032 3530 3a0d 0a20 2020 2020 2020 2020   250:..         
+0001fb50: 2020 2079 6561 726c 794c 6f77 203d 2064     yearlyLow = d
+0001fb60: 6174 612e 6865 6164 2832 3530 295b 2243  ata.head(250)["C
+0001fb70: 6c6f 7365 225d 2e6d 696e 2829 0d0a 2020  lose"].min()..  
+0001fb80: 2020 2020 2020 2020 2020 7965 6172 6c79            yearly
+0001fb90: 4869 6768 203d 2064 6174 612e 6865 6164  High = data.head
+0001fba0: 2832 3530 295b 2243 6c6f 7365 225d 2e6d  (250)["Close"].m
+0001fbb0: 6178 2829 0d0a 2020 2020 2020 2020 2020  ax()..          
+0001fbc0: 2020 6966 206c 7470 203c 2028 3220 2a20    if ltp < (2 * 
+0001fbd0: 7965 6172 6c79 4c6f 7729 2061 6e64 206c  yearlyLow) and l
+0001fbe0: 7470 203c 2028 302e 3735 202a 2079 6561  tp < (0.75 * yea
+0001fbf0: 726c 7948 6967 6829 3a0d 0a20 2020 2020  rlyHigh):..     
+0001fc00: 2020 2020 2020 2020 2020 2076 6572 6966             verif
+0001fc10: 7953 7461 6765 5477 6f20 3d20 4661 6c73  yStageTwo = Fals
+0001fc20: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+0001fc30: 2020 2073 6372 6565 6e44 6963 745b 2253     screenDict["S
+0001fc40: 746f 636b 225d 203d 2063 6f6c 6f72 5465  tock"] = colorTe
+0001fc50: 7874 2e46 4149 4c20 2b20 7361 7665 4469  xt.FAIL + saveDi
+0001fc60: 6374 5b22 5374 6f63 6b22 5d20 2b20 636f  ct["Stock"] + co
+0001fc70: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+0001fc80: 2020 2020 2069 6620 6c74 7020 3e3d 206d       if ltp >= m
+0001fc90: 696e 4c54 5020 616e 6420 6c74 7020 3c3d  inLTP and ltp <=
+0001fca0: 206d 6178 4c54 503a 0d0a 2020 2020 2020   maxLTP:..      
+0001fcb0: 2020 2020 2020 6c74 7056 616c 6964 203d        ltpValid =
+0001fcc0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+0001fcd0: 2020 2069 6620 6d69 6e43 6861 6e67 6520     if minChange 
+0001fce0: 213d 2030 3a0d 0a20 2020 2020 2020 2020  != 0:..         
+0001fcf0: 2020 2020 2020 2023 2055 7365 7220 6861         # User ha
+0001fd00: 7320 7375 7070 6c69 6564 2073 6f6d 6520  s supplied some 
+0001fd10: 6669 6c74 6572 2066 6f72 2070 6572 6365  filter for perce
+0001fd20: 6e74 6167 6520 6368 616e 6765 0d0a 2020  ntage change..  
+0001fd30: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
+0001fd40: 7056 616c 6964 203d 2066 6c6f 6174 2873  pValid = float(s
+0001fd50: 7472 2870 6374 5f73 6176 6529 2e72 6570  tr(pct_save).rep
+0001fd60: 6c61 6365 2822 2522 2c22 2229 2920 3e3d  lace("%","")) >=
+0001fd70: 206d 696e 4368 616e 6765 0d0a 2020 2020   minChange..    
+0001fd80: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+0001fd90: 5b22 4c54 5022 5d20 3d20 726f 756e 6428  ["LTP"] = round(
+0001fda0: 6c74 702c 2032 290d 0a20 2020 2020 2020  ltp, 2)..       
+0001fdb0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001fdc0: 224c 5450 225d 203d 2028 636f 6c6f 7254  "LTP"] = (colorT
+0001fdd0: 6578 742e 4752 4545 4e20 6966 206c 7470  ext.GREEN if ltp
+0001fde0: 5661 6c69 6420 656c 7365 2063 6f6c 6f72  Valid else color
+0001fdf0: 5465 7874 2e46 4149 4c29 202b 2028 2225  Text.FAIL) + ("%
+0001fe00: 2e32 6622 2025 206c 7470 2920 2b20 636f  .2f" % ltp) + co
+0001fe10: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+0001fe20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001fe30: 6c74 7056 616c 6964 2c20 7665 7269 6679  ltpValid, verify
+0001fe40: 5374 6167 6554 776f 0d0a 2020 2020 2020  StageTwo..      
+0001fe50: 2020 7363 7265 656e 4469 6374 5b22 4c54    screenDict["LT
+0001fe60: 5022 5d20 3d20 636f 6c6f 7254 6578 742e  P"] = colorText.
+0001fe70: 4641 494c 202b 2028 2225 2e32 6622 2025  FAIL + ("%.2f" %
+0001fe80: 206c 7470 2920 2b20 636f 6c6f 7254 6578   ltp) + colorTex
+0001fe90: 742e 454e 440d 0a20 2020 2020 2020 2073  t.END..        s
+0001fea0: 6176 6544 6963 745b 224c 5450 225d 203d  aveDict["LTP"] =
+0001feb0: 2072 6f75 6e64 286c 7470 2c20 3229 0d0a   round(ltp, 2)..
+0001fec0: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+0001fed0: 7470 5661 6c69 642c 2076 6572 6966 7953  tpValid, verifyS
+0001fee0: 7461 6765 5477 6f0d 0a0d 0a20 2020 2064  tageTwo....    d
+0001fef0: 6566 2076 616c 6964 6174 654c 5450 466f  ef validateLTPFo
+0001ff00: 7250 6f72 7466 6f6c 696f 4361 6c63 2873  rPortfolioCalc(s
+0001ff10: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
+0001ff20: 6963 742c 2073 6176 6544 6963 742c 7265  ict, saveDict,re
+0001ff30: 7175 6573 7465 6450 6572 696f 643d 3029  questedPeriod=0)
+0001ff40: 3a0d 0a20 2020 2020 2020 2064 6174 6120  :..        data 
+0001ff50: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
+0001ff60: 2020 2020 2070 6572 696f 6473 203d 2073       periods = s
+0001ff70: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
+0001ff80: 722e 7065 7269 6f64 7352 616e 6765 0d0a  r.periodsRange..
+0001ff90: 2020 2020 2020 2020 6966 2072 6571 7565          if reque
+0001ffa0: 7374 6564 5065 7269 6f64 203e 2030 2061  stedPeriod > 0 a
+0001ffb0: 6e64 2072 6571 7565 7374 6564 5065 7269  nd requestedPeri
+0001ffc0: 6f64 206e 6f74 2069 6e20 7065 7269 6f64  od not in period
+0001ffd0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0001ffe0: 7065 7269 6f64 732e 6170 7065 6e64 2872  periods.append(r
+0001fff0: 6571 7565 7374 6564 5065 7269 6f64 290d  equestedPeriod).
+00020000: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
+00020010: 735f 7265 6365 6e74 203d 2064 6174 612e  s_recent = data.
+00020020: 6865 6164 2831 290d 0a20 2020 2020 2020  head(1)..       
+00020030: 2070 7265 7669 6f75 735f 7265 6365 6e74   previous_recent
+00020040: 2e72 6573 6574 5f69 6e64 6578 2869 6e70  .reset_index(inp
+00020050: 6c61 6365 3d54 7275 6529 0d0a 2020 2020  lace=True)..    
+00020060: 2020 2020 6361 6c63 5f64 6174 6520 3d20      calc_date = 
+00020070: 7374 7228 7072 6576 696f 7573 5f72 6563  str(previous_rec
+00020080: 656e 742e 696c 6f63 5b3a 2c20 305d 5b30  ent.iloc[:, 0][0
+00020090: 5d29 2e73 706c 6974 2822 2022 295b 305d  ]).split(" ")[0]
+000200a0: 0d0a 2020 2020 2020 2020 666f 7220 7072  ..        for pr
+000200b0: 6420 696e 2070 6572 696f 6473 3a0d 0a20  d in periods:.. 
+000200c0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+000200d0: 6e28 6461 7461 2920 3e3d 2070 7264 202b  n(data) >= prd +
+000200e0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+000200f0: 2020 2020 2070 7265 764c 7470 203d 2064       prevLtp = d
+00020100: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
+00020110: 635b 305d 0d0a 2020 2020 2020 2020 2020  c[0]..          
+00020120: 2020 2020 2020 6c74 7054 6479 203d 2064        ltpTdy = d
+00020130: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
+00020140: 635b 7072 645d 0d0a 2020 2020 2020 2020  c[prd]..        
+00020150: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00020160: 7461 6e63 6528 7072 6576 4c74 702c 7064  tance(prevLtp,pd
+00020170: 2e53 6572 6965 7329 3a0d 0a20 2020 2020  .Series):..     
+00020180: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00020190: 7265 764c 7470 203d 2070 7265 764c 7470  revLtp = prevLtp
+000201a0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+000201b0: 2020 2020 2020 2020 206c 7470 5464 7920           ltpTdy 
+000201c0: 3d20 6c74 7054 6479 5b30 5d0d 0a20 2020  = ltpTdy[0]..   
+000201d0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+000201e0: 6565 6e44 6963 745b 6622 4c54 507b 7072  eenDict[f"LTP{pr
+000201f0: 647d 225d 203d 2028 0d0a 2020 2020 2020  d}"] = (..      
+00020200: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+00020210: 6f6c 6f72 5465 7874 2e47 5245 454e 2069  olorText.GREEN i
+00020220: 6620 286c 7470 5464 7920 3e3d 2070 7265  f (ltpTdy >= pre
+00020230: 764c 7470 2920 656c 7365 2028 636f 6c6f  vLtp) else (colo
+00020240: 7254 6578 742e 4641 494c 2929 0d0a 2020  rText.FAIL))..  
+00020250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020260: 2020 2b20 7374 7228 227b 3a2e 3266 7d22    + str("{:.2f}"
+00020270: 2e66 6f72 6d61 7428 6c74 7054 6479 2929  .format(ltpTdy))
+00020280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020290: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+000202a0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+000202b0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000202c0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+000202d0: 4469 6374 5b66 2247 726f 7774 687b 7072  Dict[f"Growth{pr
+000202e0: 647d 225d 203d 2028 0d0a 2020 2020 2020  d}"] = (..      
+000202f0: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+00020300: 6f6c 6f72 5465 7874 2e47 5245 454e 2069  olorText.GREEN i
+00020310: 6620 286c 7470 5464 7920 3e3d 2070 7265  f (ltpTdy >= pre
+00020320: 764c 7470 2920 656c 7365 2028 636f 6c6f  vLtp) else (colo
+00020330: 7254 6578 742e 4641 494c 2929 0d0a 2020  rText.FAIL))..  
+00020340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020350: 2020 2b20 7374 7228 227b 3a2e 3266 7d22    + str("{:.2f}"
+00020360: 2e66 6f72 6d61 7428 6c74 7054 6479 202d  .format(ltpTdy -
+00020370: 2070 7265 764c 7470 2929 0d0a 2020 2020   prevLtp))..    
+00020380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020390: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+000203a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000203b0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+000203c0: 2020 2020 7361 7665 4469 6374 5b66 224c      saveDict[f"L
+000203d0: 5450 7b70 7264 7d22 5d20 3d20 726f 756e  TP{prd}"] = roun
+000203e0: 6428 6c74 7054 6479 2c20 3229 0d0a 2020  d(ltpTdy, 2)..  
+000203f0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00020400: 7665 4469 6374 5b66 2247 726f 7774 687b  veDict[f"Growth{
+00020410: 7072 647d 225d 203d 2072 6f75 6e64 286c  prd}"] = round(l
+00020420: 7470 5464 7920 2d20 7072 6576 4c74 702c  tpTdy - prevLtp,
+00020430: 2032 290d 0a20 2020 2020 2020 2020 2020   2)..           
+00020440: 2020 2020 2069 6620 7072 6420 3d3d 2032       if prd == 2
+00020450: 3220 6f72 2028 7072 6420 3d3d 2072 6571  2 or (prd == req
+00020460: 7565 7374 6564 5065 7269 6f64 293a 0d0a  uestedPeriod):..
+00020470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020480: 2020 2020 6368 616e 6765 5065 7263 656e      changePercen
+00020490: 7420 3d20 726f 756e 6428 2828 7072 6576  t = round(((prev
+000204a0: 4c74 702d 6c74 7054 6479 2920 6966 2072  Ltp-ltpTdy) if r
+000204b0: 6571 7565 7374 6564 5065 7269 6f64 203d  equestedPeriod =
+000204c0: 3d30 2065 6c73 6520 286c 7470 5464 7920  =0 else (ltpTdy 
+000204d0: 2d20 7072 6576 4c74 7029 292a 3130 302f  - prevLtp))*100/
+000204e0: 6c74 7054 6479 2c20 3229 0d0a 2020 2020  ltpTdy, 2)..    
+000204f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020500: 7361 7665 4469 6374 5b66 227b 7072 647d  saveDict[f"{prd}
+00020510: 2d50 6420 2522 5d20 3d20 6622 7b63 6861  -Pd %"] = f"{cha
+00020520: 6e67 6550 6572 6365 6e74 7d25 2220 6966  ngePercent}%" if
+00020530: 206e 6f74 2070 642e 6973 6e61 2863 6861   not pd.isna(cha
+00020540: 6e67 6550 6572 6365 6e74 2920 656c 7365  ngePercent) else
+00020550: 2027 2d27 0d0a 2020 2020 2020 2020 2020   '-'..          
+00020560: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+00020570: 4469 6374 5b66 227b 7072 647d 2d50 6420  Dict[f"{prd}-Pd 
+00020580: 2522 5d20 3d20 2828 636f 6c6f 7254 6578  %"] = ((colorTex
+00020590: 742e 4752 4545 4e20 6966 2063 6861 6e67  t.GREEN if chang
+000205a0: 6550 6572 6365 6e74 203e 3d30 2065 6c73  ePercent >=0 els
+000205b0: 6520 636f 6c6f 7254 6578 742e 4641 494c  e colorText.FAIL
+000205c0: 2920 2b20 6622 7b63 6861 6e67 6550 6572  ) + f"{changePer
+000205d0: 6365 6e74 7d25 2220 2b20 636f 6c6f 7254  cent}%" + colorT
+000205e0: 6578 742e 454e 4429 2069 6620 6e6f 7420  ext.END) if not 
+000205f0: 7064 2e69 736e 6128 6368 616e 6765 5065  pd.isna(changePe
+00020600: 7263 656e 7429 2065 6c73 6520 272d 270d  rcent) else '-'.
+00020610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020620: 2073 6372 6565 6e44 6963 745b 2244 6174   screenDict["Dat
+00020630: 6522 5d20 3d20 6361 6c63 5f64 6174 650d  e"] = calc_date.
+00020640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020650: 2073 6176 6544 6963 745b 2244 6174 6522   saveDict["Date"
+00020660: 5d20 3d20 6361 6c63 5f64 6174 650d 0a20  ] = calc_date.. 
+00020670: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00020680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020690: 2020 7361 7665 4469 6374 5b66 224c 5450    saveDict[f"LTP
+000206a0: 7b70 7264 7d22 5d20 3d20 6e70 2e6e 616e  {prd}"] = np.nan
+000206b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000206c0: 2020 7361 7665 4469 6374 5b66 2247 726f    saveDict[f"Gro
+000206d0: 7774 687b 7072 647d 225d 203d 206e 702e  wth{prd}"] = np.
+000206e0: 6e61 6e0d 0a20 2020 2020 2020 2020 2020  nan..           
+000206f0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00020700: 2244 6174 6522 5d20 3d20 6361 6c63 5f64  "Date"] = calc_d
+00020710: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
+00020720: 2020 2020 2073 6176 6544 6963 745b 2244       saveDict["D
+00020730: 6174 6522 5d20 3d20 6361 6c63 5f64 6174  ate"] = calc_dat
+00020740: 650d 0a0d 0a20 2020 2023 2046 696e 6420  e....    # Find 
+00020750: 7374 6f63 6b73 2074 6861 7420 6172 6520  stocks that are 
+00020760: 6265 6172 6973 6820 696e 7472 6164 6179  bearish intraday
+00020770: 3a20 4d61 6364 2048 6973 746f 6772 616d  : Macd Histogram
+00020780: 206e 6567 6174 6976 650d 0a20 2020 2064   negative..    d
+00020790: 6566 2076 616c 6964 6174 654d 4143 4448  ef validateMACDH
+000207a0: 6973 746f 6772 616d 4265 6c6f 7730 2873  istogramBelow0(s
+000207b0: 656c 662c 2064 6629 3a0d 0a20 2020 2020  elf, df):..     
+000207c0: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
+000207d0: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
+000207e0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000207f0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+00020800: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+00020810: 6f70 7928 290d 0a20 2020 2020 2020 2064  opy()..        d
+00020820: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
+00020830: 6128 3029 0d0a 2020 2020 2020 2020 6461  a(0)..        da
+00020840: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+00020850: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
+00020860: 6e66 5d2c 2030 290d 0a20 2020 2020 2020  nf], 0)..       
+00020870: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
+00020880: 315d 2020 2320 5265 7665 7273 6520 7468  1]  # Reverse th
+00020890: 6520 6461 7461 6672 616d 6520 736f 2074  e dataframe so t
+000208a0: 6861 7420 6974 7320 7468 6520 6f6c 6465  hat its the olde
+000208b0: 7374 2064 6174 6520 6669 7273 740d 0a20  st date first.. 
+000208c0: 2020 2020 2020 206d 6163 6420 3d20 706b         macd = pk
+000208d0: 7461 6c69 622e 4d41 4344 2864 6174 615b  talib.MACD(data[
+000208e0: 2243 6c6f 7365 225d 2c20 3132 2c20 3236  "Close"], 12, 26
+000208f0: 2c20 3929 5b32 5d2e 7461 696c 2831 290d  , 9)[2].tail(1).
+00020900: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00020910: 6d61 6364 2e69 6c6f 635b 3a31 5d5b 305d  macd.iloc[:1][0]
+00020920: 203c 2030 0d0a 0d0a 2020 2020 2340 6d65   < 0....    #@me
+00020930: 6173 7572 655f 7469 6d65 0d0a 2020 2020  asure_time..    
+00020940: 2320 4669 6e64 2069 6620 7374 6f63 6b20  # Find if stock 
+00020950: 6761 696e 696e 6720 6275 6c6c 6973 6820  gaining bullish 
+00020960: 6d6f 6d65 6e74 756d 0d0a 2020 2020 6465  momentum..    de
+00020970: 6620 7661 6c69 6461 7465 4d6f 6d65 6e74  f validateMoment
+00020980: 756d 2873 656c 662c 2064 662c 2073 6372  um(self, df, scr
+00020990: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+000209a0: 7429 3a0d 0a20 2020 2020 2020 2069 6620  t):..        if 
+000209b0: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+000209c0: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
+000209d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000209e0: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
+000209f0: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
+00020a00: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00020a10: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00020a20: 3d20 6461 7461 2e68 6561 6428 3329 0d0a  = data.head(3)..
+00020a30: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00020a40: 656e 2864 6174 6129 203c 2033 3a0d 0a20  en(data) < 3:.. 
+00020a50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00020a60: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+00020a70: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
+00020a80: 2069 6e20 6461 7461 2e69 7465 7272 6f77   in data.iterrow
+00020a90: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+00020aa0: 2020 2020 2020 2320 416c 6c20 3320 6361        # All 3 ca
+00020ab0: 6e64 6c65 7320 7368 6f75 6c64 2062 6520  ndles should be 
+00020ac0: 4772 6565 6e20 616e 6420 4e4f 5420 4369  Green and NOT Ci
+00020ad0: 7263 7569 7473 0d0a 2020 2020 2020 2020  rcuits..        
+00020ae0: 2020 2020 2020 2020 7963 203d 2072 6f77          yc = row
+00020af0: 5b31 5d5b 2243 6c6f 7365 225d 0d0a 2020  [1]["Close"]..  
+00020b00: 2020 2020 2020 2020 2020 2020 2020 796f                yo
+00020b10: 203d 2072 6f77 5b31 5d5b 224f 7065 6e22   = row[1]["Open"
+00020b20: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00020b30: 2020 2069 6620 7963 203c 3d20 796f 3a0d     if yc <= yo:.
+00020b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020b50: 2020 2020 2023 2073 656c 662e 6465 6661       # self.defa
+00020b60: 756c 745f 6c6f 6767 6572 2e69 6e66 6f28  ult_logger.info(
+00020b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020b80: 2020 2020 2020 2320 2020 2020 6627 5374        #     f'St
+00020b90: 6f63 6b3a 7b73 6176 6544 6963 745b 2253  ock:{saveDict["S
+00020ba0: 746f 636b 225d 7d2c 2069 7320 6e6f 7420  tock"]}, is not 
+00020bb0: 6120 6d6f 6d65 6e74 756d 2d67 6169 6e65  a momentum-gaine
+00020bc0: 7220 6265 6361 7573 6520 7965 7374 6572  r because yester
+00020bd0: 6461 792d 636c 6f73 6520 287b 7963 7d29  day-close ({yc})
+00020be0: 203c 3d20 7965 7374 6572 6461 792d 6f70   <= yesterday-op
+00020bf0: 656e 2028 7b79 6f7d 2927 0d0a 2020 2020  en ({yo})'..    
 00020c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c10: 2023 2020 2020 2066 2753 746f 636b 3a7b   #     f'Stock:{
-00020c20: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
-00020c30: 5d7d 2c20 6f70 656e 2c63 6c6f 7365 2061  ]}, open,close a
-00020c40: 6e64 2076 6f6c 756d 6520 6571 7561 6c20  nd volume equal 
-00020c50: 6672 6f6d 2064 6179 2062 6566 6f72 6520  from day before 
-00020c60: 7965 7374 6572 6461 792e 2041 2070 6f74  yesterday. A pot
-00020c70: 656e 7469 616c 206d 6f6d 656e 7475 6d2d  ential momentum-
-00020c80: 6761 696e 6572 2127 0d0a 2020 2020 2020  gainer!'..      
-00020c90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00020ca0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00020cb0: 2020 2020 2020 2074 6f20 3d20 6461 7461         to = data
-00020cc0: 5b22 4f70 656e 225d 2e69 6c6f 635b 305d  ["Open"].iloc[0]
-00020cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020ce0: 2020 2020 2020 7963 203d 2064 6174 615b        yc = data[
-00020cf0: 2243 6c6f 7365 225d 2e69 6c6f 635b 315d  "Close"].iloc[1]
-00020d00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020d10: 2020 2020 2020 796f 203d 2064 6174 615b        yo = data[
-00020d20: 224f 7065 6e22 5d2e 696c 6f63 5b31 5d0d  "Open"].iloc[1].
-00020d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020d40: 2020 2020 2064 7963 203d 2064 6174 615b       dyc = data[
-00020d50: 2243 6c6f 7365 225d 2e69 6c6f 635b 325d  "Close"].iloc[2]
+00020c10: 2320 290d 0a20 2020 2020 2020 2020 2020  # )..           
+00020c20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00020c30: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+00020c40: 2020 206f 7065 6e44 6573 6320 3d20 6461     openDesc = da
+00020c50: 7461 2e73 6f72 745f 7661 6c75 6573 2862  ta.sort_values(b
+00020c60: 793d 5b22 4f70 656e 225d 2c20 6173 6365  y=["Open"], asce
+00020c70: 6e64 696e 673d 4661 6c73 6529 0d0a 2020  nding=False)..  
+00020c80: 2020 2020 2020 2020 2020 636c 6f73 6544            closeD
+00020c90: 6573 6320 3d20 6461 7461 2e73 6f72 745f  esc = data.sort_
+00020ca0: 7661 6c75 6573 2862 793d 5b22 436c 6f73  values(by=["Clos
+00020cb0: 6522 5d2c 2061 7363 656e 6469 6e67 3d46  e"], ascending=F
+00020cc0: 616c 7365 290d 0a20 2020 2020 2020 2020  alse)..         
+00020cd0: 2020 2076 6f6c 4465 7363 203d 2064 6174     volDesc = dat
+00020ce0: 612e 736f 7274 5f76 616c 7565 7328 6279  a.sort_values(by
+00020cf0: 3d5b 2256 6f6c 756d 6522 5d2c 2061 7363  =["Volume"], asc
+00020d00: 656e 6469 6e67 3d46 616c 7365 290d 0a20  ending=False).. 
+00020d10: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+00020d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020d30: 2069 6620 280d 0a20 2020 2020 2020 2020   if (..         
+00020d40: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+00020d50: 6571 7561 6c73 286f 7065 6e44 6573 6329  equals(openDesc)
 00020d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020d70: 2020 2020 2020 6966 2028 746f 203e 3d20        if (to >= 
-00020d80: 7963 2920 616e 6420 2879 6f20 3e3d 2064  yc) and (yo >= d
-00020d90: 7963 293a 0d0a 2020 2020 2020 2020 2020  yc):..          
-00020da0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00020db0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-00020dc0: 6765 722e 696e 666f 280d 0a20 2020 2020  ger.info(..     
-00020dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020de0: 2020 2023 2020 2020 2066 2753 746f 636b     #     f'Stock
-00020df0: 3a7b 7361 7665 4469 6374 5b22 5374 6f63  :{saveDict["Stoc
-00020e00: 6b22 5d7d 2c20 6973 2061 206d 6f6d 656e  k"]}, is a momen
-00020e10: 7475 6d2d 6761 696e 6572 2062 6563 6175  tum-gainer becau
-00020e20: 7365 2074 6f64 6179 2d6f 7065 6e20 287b  se today-open ({
-00020e30: 746f 7d29 203e 3d20 7965 7374 6572 6461  to}) >= yesterda
-00020e40: 792d 636c 6f73 6520 287b 7963 7d29 2061  y-close ({yc}) a
-00020e50: 6e64 2079 6573 7465 7264 6179 2d6f 7065  nd yesterday-ope
-00020e60: 6e28 7b79 6f7d 2920 3e3d 2064 6179 2d62  n({yo}) >= day-b
-00020e70: 6566 6f72 652d 636c 6f73 6528 7b64 7963  efore-close({dyc
-00020e80: 7d29 270d 0a20 2020 2020 2020 2020 2020  })'..           
-00020e90: 2020 2020 2020 2020 2020 2020 2023 2029               # )
-00020ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020eb0: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
-00020ec0: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
-00020ed0: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
-00020ee0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-00020ef0: 742c 2022 5061 7474 6572 6e22 290d 0a20  t, "Pattern").. 
-00020f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f10: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00020f20: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-00020f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020f40: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00020f50: 7665 645b 305d 0d0a 2020 2020 2020 2020  ved[0]..        
-00020f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f70: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-00020f80: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
-00020f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020fa0: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
-00020fb0: 4545 4e0d 0a20 2020 2020 2020 2020 2020  EEN..           
-00020fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020fd0: 202b 2022 4d6f 6d65 6e74 756d 2047 6169   + "Momentum Gai
-00020fe0: 6e65 7222 0d0a 2020 2020 2020 2020 2020  ner"..          
-00020ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021000: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-00021010: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-00021020: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00021030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021040: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-00021050: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
-00021060: 645b 315d 202b 2022 4d6f 6d65 6e74 756d  d[1] + "Momentum
-00021070: 2047 6169 6e65 7222 0d0a 2020 2020 2020   Gainer"..      
-00021080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021090: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
-000210a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000210b0: 2020 2023 2073 656c 662e 6465 6661 756c     # self.defaul
-000210c0: 745f 6c6f 6767 6572 2e69 6e66 6f28 0d0a  t_logger.info(..
-000210d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000210e0: 2020 2020 2320 2020 2020 6627 5374 6f63      #     f'Stoc
-000210f0: 6b3a 7b73 6176 6544 6963 745b 2253 746f  k:{saveDict["Sto
-00021100: 636b 225d 7d2c 2069 7320 6e6f 7420 6120  ck"]}, is not a 
-00021110: 6d6f 6d65 6e74 756d 2d67 6169 6e65 7220  momentum-gainer 
-00021120: 6265 6361 7573 6520 6569 7468 6572 2074  because either t
-00021130: 6f64 6179 2d6f 7065 6e20 287b 746f 7d29  oday-open ({to})
-00021140: 203c 2079 6573 7465 7264 6179 2d63 6c6f   < yesterday-clo
-00021150: 7365 2028 7b79 637d 2920 6f72 2079 6573  se ({yc}) or yes
-00021160: 7465 7264 6179 2d6f 7065 6e28 7b79 6f7d  terday-open({yo}
-00021170: 2920 3c20 6461 792d 6265 666f 7265 2d63  ) < day-before-c
-00021180: 6c6f 7365 287b 6479 637d 2927 0d0a 2020  lose({dyc})'..  
+00020d70: 2020 2020 2020 616e 6420 6461 7461 2e65        and data.e
+00020d80: 7175 616c 7328 636c 6f73 6544 6573 6329  quals(closeDesc)
+00020d90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020da0: 2020 2020 2020 616e 6420 6461 7461 2e65        and data.e
+00020db0: 7175 616c 7328 766f 6c44 6573 6329 0d0a  quals(volDesc)..
+00020dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020dd0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00020de0: 2020 2020 2020 2020 2320 7365 6c66 2e64          # self.d
+00020df0: 6566 6175 6c74 5f6c 6f67 6765 722e 696e  efault_logger.in
+00020e00: 666f 280d 0a20 2020 2020 2020 2020 2020  fo(..           
+00020e10: 2020 2020 2020 2020 2023 2020 2020 2066           #     f
+00020e20: 2753 746f 636b 3a7b 7361 7665 4469 6374  'Stock:{saveDict
+00020e30: 5b22 5374 6f63 6b22 5d7d 2c20 6f70 656e  ["Stock"]}, open
+00020e40: 2c63 6c6f 7365 2061 6e64 2076 6f6c 756d  ,close and volum
+00020e50: 6520 6571 7561 6c20 6672 6f6d 2064 6179  e equal from day
+00020e60: 2062 6566 6f72 6520 7965 7374 6572 6461   before yesterda
+00020e70: 792e 2041 2070 6f74 656e 7469 616c 206d  y. A potential m
+00020e80: 6f6d 656e 7475 6d2d 6761 696e 6572 2127  omentum-gainer!'
+00020e90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020ea0: 2020 2020 2020 2320 290d 0a20 2020 2020        # )..     
+00020eb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00020ec0: 6f20 3d20 6461 7461 5b22 4f70 656e 225d  o = data["Open"]
+00020ed0: 2e69 6c6f 635b 305d 0d0a 2020 2020 2020  .iloc[0]..      
+00020ee0: 2020 2020 2020 2020 2020 2020 2020 7963                yc
+00020ef0: 203d 2064 6174 615b 2243 6c6f 7365 225d   = data["Close"]
+00020f00: 2e69 6c6f 635b 315d 0d0a 2020 2020 2020  .iloc[1]..      
+00020f10: 2020 2020 2020 2020 2020 2020 2020 796f                yo
+00020f20: 203d 2064 6174 615b 224f 7065 6e22 5d2e   = data["Open"].
+00020f30: 696c 6f63 5b31 5d0d 0a20 2020 2020 2020  iloc[1]..       
+00020f40: 2020 2020 2020 2020 2020 2020 2064 7963               dyc
+00020f50: 203d 2064 6174 615b 2243 6c6f 7365 225d   = data["Close"]
+00020f60: 2e69 6c6f 635b 325d 0d0a 2020 2020 2020  .iloc[2]..      
+00020f70: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00020f80: 2028 746f 203e 3d20 7963 2920 616e 6420   (to >= yc) and 
+00020f90: 2879 6f20 3e3d 2064 7963 293a 0d0a 2020  (yo >= dyc):..  
+00020fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020fb0: 2020 2020 2020 2320 7365 6c66 2e64 6566        # self.def
+00020fc0: 6175 6c74 5f6c 6f67 6765 722e 696e 666f  ault_logger.info
+00020fd0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00020fe0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00020ff0: 2066 2753 746f 636b 3a7b 7361 7665 4469   f'Stock:{saveDi
+00021000: 6374 5b22 5374 6f63 6b22 5d7d 2c20 6973  ct["Stock"]}, is
+00021010: 2061 206d 6f6d 656e 7475 6d2d 6761 696e   a momentum-gain
+00021020: 6572 2062 6563 6175 7365 2074 6f64 6179  er because today
+00021030: 2d6f 7065 6e20 287b 746f 7d29 203e 3d20  -open ({to}) >= 
+00021040: 7965 7374 6572 6461 792d 636c 6f73 6520  yesterday-close 
+00021050: 287b 7963 7d29 2061 6e64 2079 6573 7465  ({yc}) and yeste
+00021060: 7264 6179 2d6f 7065 6e28 7b79 6f7d 2920  rday-open({yo}) 
+00021070: 3e3d 2064 6179 2d62 6566 6f72 652d 636c  >= day-before-cl
+00021080: 6f73 6528 7b64 7963 7d29 270d 0a20 2020  ose({dyc})'..   
+00021090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000210a0: 2020 2020 2023 2029 0d0a 2020 2020 2020       # )..      
+000210b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000210c0: 2020 7361 7665 6420 3d20 7365 6c66 2e66    saved = self.f
+000210d0: 696e 6443 7572 7265 6e74 5361 7665 6456  indCurrentSavedV
+000210e0: 616c 7565 2873 6372 6565 6e44 6963 742c  alue(screenDict,
+000210f0: 2073 6176 6544 6963 742c 2022 5061 7474   saveDict, "Patt
+00021100: 6572 6e22 290d 0a20 2020 2020 2020 2020  ern")..         
+00021110: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021120: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+00021130: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
+00021140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021150: 2020 2020 2020 7361 7665 645b 305d 0d0a        saved[0]..
+00021160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021170: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+00021180: 6c6f 7254 6578 742e 424f 4c44 0d0a 2020  lorText.BOLD..  
 00021190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211a0: 2020 2320 290d 0a20 2020 2020 2020 2020    # )..         
-000211b0: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
-000211c0: 7272 6f72 2061 7320 653a 2023 2070 7261  rror as e: # pra
-000211d0: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
-000211e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000211f0: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
-00021200: 6572 2e64 6562 7567 2865 2c20 6578 635f  er.debug(e, exc_
-00021210: 696e 666f 3d54 7275 6529 0d0a 2020 2020  info=True)..    
-00021220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00021230: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
-00021240: 6465 6275 6728 6461 7461 290d 0a20 2020  debug(data)..   
-00021250: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00021260: 730d 0a20 2020 2020 2020 2020 2020 2072  s..            r
-00021270: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-00021280: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00021290: 7074 696f 6e20 6173 2065 3a20 2023 2070  ption as e:  # p
-000212a0: 7261 676d 613a 206e 6f20 636f 7665 720d  ragma: no cover.
-000212b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000211a0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+000211b0: 7254 6578 742e 4752 4545 4e0d 0a20 2020  rText.GREEN..   
+000211c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211d0: 2020 2020 2020 2020 202b 2022 4d6f 6d65           + "Mome
+000211e0: 6e74 756d 2047 6169 6e65 7222 0d0a 2020  ntum Gainer"..  
+000211f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021200: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00021210: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+00021220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021230: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00021240: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00021250: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
+00021260: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
+00021270: 4d6f 6d65 6e74 756d 2047 6169 6e65 7222  Momentum Gainer"
+00021280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00021290: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000212a0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+000212b0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
 000212c0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-000212d0: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
-000212e0: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
-000212f0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00021300: 7365 0d0a 0d0a 2020 2020 2340 6d65 6173  se....    #@meas
-00021310: 7572 655f 7469 6d65 0d0a 2020 2020 2320  ure_time..    # 
-00021320: 5661 6c69 6461 7465 204d 6f76 696e 6720  Validate Moving 
-00021330: 6176 6572 6167 6573 2061 6e64 206c 6f6f  averages and loo
-00021340: 6b20 666f 7220 6275 792f 7365 6c6c 2073  k for buy/sell s
-00021350: 6967 6e61 6c73 0d0a 2020 2020 6465 6620  ignals..    def 
-00021360: 7661 6c69 6461 7465 4d6f 7669 6e67 4176  validateMovingAv
-00021370: 6572 6167 6573 2873 656c 662c 2064 662c  erages(self, df,
-00021380: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-00021390: 6544 6963 742c 206d 6152 616e 6765 3d32  eDict, maRange=2
-000213a0: 2e35 293a 0d0a 2020 2020 2020 2020 6461  .5):..        da
-000213b0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-000213c0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-000213d0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-000213e0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-000213f0: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00021400: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00021410: 0d0a 2020 2020 2020 2020 7265 6365 6e74  ..        recent
-00021420: 203d 2064 6174 612e 6865 6164 2831 290d   = data.head(1).
-00021430: 0a20 2020 2020 2020 2073 6176 6564 203d  .        saved =
-00021440: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-00021450: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-00021460: 656e 4469 6374 2c73 6176 6544 6963 742c  enDict,saveDict,
-00021470: 224d 412d 5369 676e 616c 2229 0d0a 2020  "MA-Signal")..  
-00021480: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
-00021490: 2020 2020 2020 2020 7265 6365 6e74 5b22          recent["
-000214a0: 534d 4122 5d2e 696c 6f63 5b30 5d20 3e20  SMA"].iloc[0] > 
-000214b0: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
-000214c0: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
-000214d0: 2020 2061 6e64 2072 6563 656e 745b 2243     and recent["C
-000214e0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
-000214f0: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
-00021500: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
-00021510: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00021520: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
-00021530: 6967 6e61 6c22 5d20 3d20 280d 0a20 2020  ignal"] = (..   
-00021540: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00021550: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
-00021560: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
-00021570: 7874 2e47 5245 454e 202b 2022 4275 6c6c  xt.GREEN + "Bull
-00021580: 6973 6822 202b 2063 6f6c 6f72 5465 7874  ish" + colorText
-00021590: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-000215a0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-000215b0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-000215c0: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-000215d0: 5d20 2b20 2242 756c 6c69 7368 220d 0a20  ] + "Bullish".. 
-000215e0: 2020 2020 2020 2065 6c69 6620 7265 6365         elif rece
-000215f0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
-00021600: 5d20 3c20 7265 6365 6e74 5b22 4c4d 4122  ] < recent["LMA"
-00021610: 5d2e 696c 6f63 5b30 5d3a 0d0a 2020 2020  ].iloc[0]:..    
-00021620: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00021630: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-00021640: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-00021650: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-00021660: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-00021670: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
-00021680: 2b20 2242 6561 7269 7368 2220 2b20 636f  + "Bearish" + co
-00021690: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-000216a0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-000216b0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-000216c0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
-000216d0: 7361 7665 645b 315d 202b 2022 4265 6172  saved[1] + "Bear
-000216e0: 6973 6822 0d0a 2020 2020 2020 2020 656c  ish"..        el
-000216f0: 6966 2072 6563 656e 745b 2253 4d41 225d  if recent["SMA"]
-00021700: 2e69 6c6f 635b 305d 203d 3d20 303a 0d0a  .iloc[0] == 0:..
-00021710: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00021720: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
-00021730: 6c22 5d20 3d20 280d 0a20 2020 2020 2020  l"] = (..       
-00021740: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00021750: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00021760: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
-00021770: 4152 4e20 2b20 2255 6e6b 6e6f 776e 2220  ARN + "Unknown" 
-00021780: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-00021790: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-000217a0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000217b0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-000217c0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
-000217d0: 556e 6b6e 6f77 6e22 0d0a 2020 2020 2020  Unknown"..      
-000217e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000217f0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00021800: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
-00021810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021820: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-00021830: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00021840: 6c6f 7254 6578 742e 5741 524e 202b 2022  lorText.WARN + "
-00021850: 4e65 7574 7261 6c22 202b 2063 6f6c 6f72  Neutral" + color
-00021860: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-00021870: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00021880: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
-00021890: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
-000218a0: 6564 5b31 5d20 2b20 224e 6575 7472 616c  ed[1] + "Neutral
-000218b0: 220d 0a0d 0a20 2020 2020 2020 2073 6d61  "....        sma
-000218c0: 4465 7620 3d20 6461 7461 5b22 534d 4122  Dev = data["SMA"
-000218d0: 5d2e 696c 6f63 5b30 5d20 2a20 6d61 5261  ].iloc[0] * maRa
-000218e0: 6e67 6520 2f20 3130 300d 0a20 2020 2020  nge / 100..     
-000218f0: 2020 206c 6d61 4465 7620 3d20 6461 7461     lmaDev = data
-00021900: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d20  ["LMA"].iloc[0] 
-00021910: 2a20 6d61 5261 6e67 6520 2f20 3130 300d  * maRange / 100.
-00021920: 0a20 2020 2020 2020 206f 7065 6e2c 2068  .        open, h
-00021930: 6967 682c 206c 6f77 2c20 636c 6f73 652c  igh, low, close,
-00021940: 2073 6d61 2c20 6c6d 6120 3d20 280d 0a20   sma, lma = (.. 
-00021950: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-00021960: 224f 7065 6e22 5d2e 696c 6f63 5b30 5d2c  "Open"].iloc[0],
-00021970: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00021980: 7461 5b22 4869 6768 225d 2e69 6c6f 635b  ta["High"].iloc[
-00021990: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-000219a0: 2064 6174 615b 224c 6f77 225d 2e69 6c6f   data["Low"].ilo
-000219b0: 635b 305d 2c0d 0a20 2020 2020 2020 2020  c[0],..         
-000219c0: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
-000219d0: 2e69 6c6f 635b 305d 2c0d 0a20 2020 2020  .iloc[0],..     
-000219e0: 2020 2020 2020 2064 6174 615b 2253 4d41         data["SMA
-000219f0: 225d 2e69 6c6f 635b 305d 2c0d 0a20 2020  "].iloc[0],..   
-00021a00: 2020 2020 2020 2020 2064 6174 615b 224c           data["L
-00021a10: 4d41 225d 2e69 6c6f 635b 305d 2c0d 0a20  MA"].iloc[0],.. 
-00021a20: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00021a30: 2020 6d61 5265 7665 7273 616c 203d 2030    maReversal = 0
-00021a40: 0d0a 2020 2020 2020 2020 2320 5461 6b69  ..        # Taki
-00021a50: 6e67 2053 7570 706f 7274 2035 300d 0a20  ng Support 50.. 
-00021a60: 2020 2020 2020 2069 6620 636c 6f73 6520         if close 
-00021a70: 3e20 736d 6120 616e 6420 6c6f 7720 3c3d  > sma and low <=
-00021a80: 2028 736d 6120 2b20 736d 6144 6576 293a   (sma + smaDev):
-00021a90: 0d0a 2020 2020 2020 2020 2020 2020 7363  ..            sc
-00021aa0: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
-00021ab0: 6e61 6c22 5d20 3d20 280d 0a20 2020 2020  nal"] = (..     
-00021ac0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00021ad0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
-00021ae0: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
-00021af0: 2e47 5245 454e 202b 2022 3530 4d41 2d53  .GREEN + "50MA-S
-00021b00: 7570 706f 7274 2220 2b20 636f 6c6f 7254  upport" + colorT
-00021b10: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-00021b20: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00021b30: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
-00021b40: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
-00021b50: 645b 315d 202b 2022 3530 4d41 2d53 7570  d[1] + "50MA-Sup
-00021b60: 706f 7274 220d 0a20 2020 2020 2020 2020  port"..         
-00021b70: 2020 206d 6152 6576 6572 7361 6c20 3d20     maReversal = 
-00021b80: 310d 0a20 2020 2020 2020 2023 2056 616c  1..        # Val
-00021b90: 6964 6174 696e 6720 5265 7369 7374 616e  idating Resistan
-00021ba0: 6365 2035 300d 0a20 2020 2020 2020 2065  ce 50..        e
-00021bb0: 6c69 6620 636c 6f73 6520 3c20 736d 6120  lif close < sma 
-00021bc0: 616e 6420 6869 6768 203e 3d20 2873 6d61  and high >= (sma
-00021bd0: 202d 2073 6d61 4465 7629 3a0d 0a20 2020   - smaDev):..   
-00021be0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00021bf0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021c00: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00021c10: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00021c20: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00021c30: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-00021c40: 202b 2022 3530 4d41 2d52 6573 6973 7422   + "50MA-Resist"
-00021c50: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00021c60: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00021c70: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-00021c80: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-00021c90: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00021ca0: 2235 304d 412d 5265 7369 7374 220d 0a20  "50MA-Resist".. 
-00021cb0: 2020 2020 2020 2020 2020 206d 6152 6576             maRev
-00021cc0: 6572 7361 6c20 3d20 2d31 0d0a 2020 2020  ersal = -1..    
-00021cd0: 2020 2020 2320 5461 6b69 6e67 2053 7570      # Taking Sup
-00021ce0: 706f 7274 2032 3030 0d0a 2020 2020 2020  port 200..      
-00021cf0: 2020 656c 6966 2063 6c6f 7365 203e 206c    elif close > l
-00021d00: 6d61 2061 6e64 206c 6f77 203c 3d20 286c  ma and low <= (l
-00021d10: 6d61 202b 206c 6d61 4465 7629 3a0d 0a20  ma + lmaDev):.. 
-00021d20: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00021d30: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
-00021d40: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-00021d50: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00021d60: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00021d70: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-00021d80: 4545 4e20 2b20 2232 3030 4d41 2d53 7570  EEN + "200MA-Sup
-00021d90: 706f 7274 2220 2b20 636f 6c6f 7254 6578  port" + colorTex
-00021da0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-00021db0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00021dc0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00021dd0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-00021de0: 315d 202b 2022 3230 304d 412d 5375 7070  1] + "200MA-Supp
-00021df0: 6f72 7422 0d0a 2020 2020 2020 2020 2020  ort"..          
-00021e00: 2020 6d61 5265 7665 7273 616c 203d 2031    maReversal = 1
-00021e10: 0d0a 2020 2020 2020 2020 2320 5661 6c69  ..        # Vali
-00021e20: 6461 7469 6e67 2052 6573 6973 7461 6e63  dating Resistanc
-00021e30: 6520 3230 300d 0a20 2020 2020 2020 2065  e 200..        e
-00021e40: 6c69 6620 636c 6f73 6520 3c20 6c6d 6120  lif close < lma 
-00021e50: 616e 6420 6869 6768 203e 3d20 286c 6d61  and high >= (lma
-00021e60: 202d 206c 6d61 4465 7629 3a0d 0a20 2020   - lmaDev):..   
-00021e70: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00021e80: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021e90: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00021ea0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00021eb0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00021ec0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-00021ed0: 202b 2022 3230 304d 412d 5265 7369 7374   + "200MA-Resist
-00021ee0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-00021ef0: 440d 0a20 2020 2020 2020 2020 2020 2029  D..            )
-00021f00: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
-00021f10: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
-00021f20: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
-00021f30: 2022 3230 304d 412d 5265 7369 7374 220d   "200MA-Resist".
-00021f40: 0a20 2020 2020 2020 2020 2020 206d 6152  .            maR
-00021f50: 6576 6572 7361 6c20 3d20 2d31 0d0a 2020  eversal = -1..  
-00021f60: 2020 2020 2020 2320 466f 7220 6120 4275        # For a Bu
-00021f70: 6c6c 6973 6820 4361 6e64 6c65 0d0a 2020  llish Candle..  
-00021f80: 2020 2020 2020 6966 2073 656c 662e 6765        if self.ge
-00021f90: 7443 616e 646c 6554 7970 6528 6461 7461  tCandleType(data
-00021fa0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00021fb0: 2320 4372 6f73 7369 6e67 2075 7020 3530  # Crossing up 50
-00021fc0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00021fd0: 206f 7065 6e20 3c20 736d 6120 616e 6420   open < sma and 
-00021fe0: 636c 6f73 6520 3e20 736d 613a 0d0a 2020  close > sma:..  
-00021ff0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00022000: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
-00022010: 6e61 6c22 5d20 3d20 280d 0a20 2020 2020  nal"] = (..     
-00022020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00022030: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
-00022040: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
-00022050: 5465 7874 2e47 5245 454e 202b 2022 4275  Text.GREEN + "Bu
-00022060: 6c6c 4372 6f73 732d 3530 4d41 2220 2b20  llCross-50MA" + 
-00022070: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-00022080: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00022090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000220a0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-000220b0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-000220c0: 315d 202b 2022 4275 6c6c 4372 6f73 732d  1] + "BullCross-
-000220d0: 3530 4d41 220d 0a20 2020 2020 2020 2020  50MA"..         
-000220e0: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
-000220f0: 6c20 3d20 310d 0a20 2020 2020 2020 2020  l = 1..         
-00022100: 2020 2023 2043 726f 7373 696e 6720 7570     # Crossing up
-00022110: 2032 3030 0d0a 2020 2020 2020 2020 2020   200..          
-00022120: 2020 656c 6966 206f 7065 6e20 3c20 6c6d    elif open < lm
-00022130: 6120 616e 6420 636c 6f73 6520 3e20 6c6d  a and close > lm
-00022140: 613a 0d0a 2020 2020 2020 2020 2020 2020  a:..            
-00022150: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-00022160: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280d  MA-Signal"] = (.
-00022170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022180: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-00022190: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-000221a0: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-000221b0: 202b 2022 4275 6c6c 4372 6f73 732d 3230   + "BullCross-20
-000221c0: 304d 4122 202b 2063 6f6c 6f72 5465 7874  0MA" + colorText
-000221d0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-000221e0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-000221f0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00022200: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00022210: 2073 6176 6564 5b31 5d20 2b20 2242 756c   saved[1] + "Bul
-00022220: 6c43 726f 7373 2d32 3030 4d41 220d 0a20  lCross-200MA".. 
-00022230: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00022240: 6152 6576 6572 7361 6c20 3d20 310d 0a20  aReversal = 1.. 
-00022250: 2020 2020 2020 2023 2046 6f72 2061 2042         # For a B
-00022260: 6561 7269 7368 2043 616e 646c 650d 0a20  earish Candle.. 
-00022270: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
-00022280: 7365 6c66 2e67 6574 4361 6e64 6c65 5479  self.getCandleTy
-00022290: 7065 2864 6174 6129 3a0d 0a20 2020 2020  pe(data):..     
-000222a0: 2020 2020 2020 2023 2043 726f 7373 696e         # Crossin
-000222b0: 6720 646f 776e 2035 300d 0a20 2020 2020  g down 50..     
-000222c0: 2020 2020 2020 2069 6620 6f70 656e 203e         if open >
-000222d0: 2073 6d61 2061 6e64 2063 6c6f 7365 203c   sma and close <
-000222e0: 2073 6d61 3a0d 0a20 2020 2020 2020 2020   sma:..         
-000222f0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00022300: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00022310: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00022320: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00022330: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00022340: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
-00022350: 494c 202b 2022 4265 6172 4372 6f73 732d  IL + "BearCross-
-00022360: 3530 4d41 2220 2b20 636f 6c6f 7254 6578  50MA" + colorTex
-00022370: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-00022380: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00022390: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-000223a0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-000223b0: 3d20 7361 7665 645b 315d 202b 2022 4265  = saved[1] + "Be
-000223c0: 6172 4372 6f73 732d 3530 4d41 220d 0a20  arCross-50MA".. 
-000223d0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000223e0: 6152 6576 6572 7361 6c20 3d20 2d31 0d0a  aReversal = -1..
-000223f0: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
-00022400: 6f73 7369 6e67 2075 7020 3230 300d 0a20  ossing up 200.. 
-00022410: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00022420: 6f70 656e 203e 206c 6d61 2061 6e64 2063  open > lma and c
-00022430: 6c6f 7365 203c 206c 6d61 3a0d 0a20 2020  lose < lma:..   
-00022440: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00022450: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
-00022460: 616c 225d 203d 2028 0d0a 2020 2020 2020  al"] = (..      
-00022470: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00022480: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
-00022490: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
-000224a0: 6578 742e 4641 494c 202b 2022 4265 6172  ext.FAIL + "Bear
-000224b0: 4372 6f73 732d 3230 304d 4122 202b 2063  Cross-200MA" + c
-000224c0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-000224d0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-000224e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000224f0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-00022500: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-00022510: 5d20 2b20 2242 6561 7243 726f 7373 2d32  ] + "BearCross-2
-00022520: 3030 4d41 220d 0a20 2020 2020 2020 2020  00MA"..         
-00022530: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
-00022540: 6c20 3d20 2d31 0d0a 2020 2020 2020 2020  l = -1..        
-00022550: 7265 7475 726e 206d 6152 6576 6572 7361  return maReversa
-00022560: 6c0d 0a0d 0a20 2020 2023 2046 696e 6420  l....    # Find 
-00022570: 4e52 7820 7261 6e67 6520 666f 7220 5265  NRx range for Re
-00022580: 7665 7273 616c 0d0a 2020 2020 6465 6620  versal..    def 
-00022590: 7661 6c69 6461 7465 4e61 7272 6f77 5261  validateNarrowRa
-000225a0: 6e67 6528 7365 6c66 2c20 6466 2c20 7363  nge(self, df, sc
-000225b0: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
-000225c0: 6374 2c20 6e72 3d34 293a 0d0a 2020 2020  ct, nr=4):..    
-000225d0: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-000225e0: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-000225f0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00022600: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-00022610: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-00022620: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-00022630: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
-00022640: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
-00022650: 7565 2873 6372 6565 6e44 6963 742c 2073  ue(screenDict, s
-00022660: 6176 6544 6963 742c 2022 5061 7474 6572  aveDict, "Patter
-00022670: 6e22 290d 0a20 2020 2020 2020 2069 6620  n")..        if 
-00022680: 504b 4461 7465 5574 696c 6974 6965 732e  PKDateUtilities.
-00022690: 6973 5472 6164 696e 6754 696d 6528 293a  isTradingTime():
-000226a0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-000226b0: 6e67 6544 6174 6120 3d20 6461 7461 2e68  ngeData = data.h
-000226c0: 6561 6428 6e72 202b 2031 295b 313a 5d0d  ead(nr + 1)[1:].
-000226d0: 0a20 2020 2020 2020 2020 2020 206e 6f77  .            now
-000226e0: 5f63 616e 646c 6520 3d20 6461 7461 2e68  _candle = data.h
-000226f0: 6561 6428 3129 0d0a 2020 2020 2020 2020  ead(1)..        
-00022700: 2020 2020 7261 6e67 6544 6174 615b 2252      rangeData["R
-00022710: 616e 6765 225d 203d 2061 6273 2872 616e  ange"] = abs(ran
-00022720: 6765 4461 7461 5b22 436c 6f73 6522 5d20  geData["Close"] 
-00022730: 2d20 7261 6e67 6544 6174 615b 224f 7065  - rangeData["Ope
-00022740: 6e22 5d29 0d0a 2020 2020 2020 2020 2020  n"])..          
-00022750: 2020 7265 6365 6e74 203d 2072 616e 6765    recent = range
-00022760: 4461 7461 2e68 6561 6428 3129 0d0a 2020  Data.head(1)..  
-00022770: 2020 2020 2020 2020 2020 6966 2028 0d0a            if (..
-00022780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022790: 6c65 6e28 7265 6365 6e74 2920 3d3d 2031  len(recent) == 1
-000227a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000227b0: 2020 616e 6420 7265 6365 6e74 5b22 5261    and recent["Ra
-000227c0: 6e67 6522 5d2e 696c 6f63 5b30 5d20 3d3d  nge"].iloc[0] ==
-000227d0: 2072 616e 6765 4461 7461 2e64 6573 6372   rangeData.descr
-000227e0: 6962 6528 295b 2252 616e 6765 225d 5b22  ibe()["Range"]["
-000227f0: 6d69 6e22 5d0d 0a20 2020 2020 2020 2020  min"]..         
-00022800: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-00022810: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
-00022820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022830: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
-00022840: 7970 6528 7265 6365 6e74 290d 0a20 2020  ype(recent)..   
-00022850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022860: 2061 6e64 206e 6f77 5f63 616e 646c 655b   and now_candle[
-00022870: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-00022880: 203e 3d20 7265 6365 6e74 5b22 436c 6f73   >= recent["Clos
-00022890: 6522 5d2e 696c 6f63 5b30 5d0d 0a20 2020  e"].iloc[0]..   
-000228a0: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
-000228b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000228c0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-000228d0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
-000228e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000228f0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00022900: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00022910: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-00022920: 4545 4e20 2b20 6622 4275 792d 4e52 7b6e  EEN + f"Buy-NR{n
-00022930: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
-00022940: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-00022950: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00022960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022970: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
-00022980: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
-00022990: 2066 2242 7579 2d4e 527b 6e72 7d22 0d0a   f"Buy-NR{nr}"..
-000229a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229b0: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
-000229c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000229d0: 2065 6c69 6620 280d 0a20 2020 2020 2020   elif (..       
-000229e0: 2020 2020 2020 2020 2020 2020 206e 6f74               not
-000229f0: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
-00022a00: 7970 6528 7265 6365 6e74 290d 0a20 2020  ype(recent)..   
-00022a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a20: 2061 6e64 206e 6f77 5f63 616e 646c 655b   and now_candle[
-00022a30: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-00022a40: 203c 3d20 7265 6365 6e74 5b22 436c 6f73   <= recent["Clos
-00022a50: 6522 5d2e 696c 6f63 5b30 5d0d 0a20 2020  e"].iloc[0]..   
-00022a60: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
-00022a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022a80: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00022a90: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
-00022aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022ab0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00022ac0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00022ad0: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
-00022ae0: 494c 202b 2066 2253 656c 6c2d 4e52 7b6e  IL + f"Sell-NR{n
-00022af0: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
-00022b00: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-00022b10: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00022b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b30: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
-00022b40: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
-00022b50: 2066 2253 656c 6c2d 4e52 7b6e 727d 220d   f"Sell-NR{nr}".
-00022b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022b70: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00022b80: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00022b90: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
-00022ba0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00022bb0: 2020 2020 2020 2072 616e 6765 4461 7461         rangeData
-00022bc0: 203d 2064 6174 612e 6865 6164 286e 7229   = data.head(nr)
-00022bd0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00022be0: 6e67 6544 6174 612e 6c6f 635b 3a2c 2752  ngeData.loc[:,'R
-00022bf0: 616e 6765 275d 203d 2061 6273 2872 616e  ange'] = abs(ran
-00022c00: 6765 4461 7461 5b22 436c 6f73 6522 5d20  geData["Close"] 
-00022c10: 2d20 7261 6e67 6544 6174 615b 224f 7065  - rangeData["Ope
-00022c20: 6e22 5d29 0d0a 2020 2020 2020 2020 2020  n"])..          
-00022c30: 2020 7265 6365 6e74 203d 2072 616e 6765    recent = range
-00022c40: 4461 7461 2e68 6561 6428 3129 0d0a 2020  Data.head(1)..  
-00022c50: 2020 2020 2020 2020 2020 6966 2072 6563            if rec
-00022c60: 656e 745b 2252 616e 6765 225d 2e69 6c6f  ent["Range"].ilo
-00022c70: 635b 305d 203d 3d20 7261 6e67 6544 6174  c[0] == rangeDat
-00022c80: 612e 6465 7363 7269 6265 2829 5b22 5261  a.describe()["Ra
-00022c90: 6e67 6522 5d5b 226d 696e 225d 3a0d 0a20  nge"]["min"]:.. 
-00022ca0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00022cb0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
-00022cc0: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
-00022cd0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00022ce0: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
-00022cf0: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
-00022d00: 6578 742e 4752 4545 4e20 2b20 6622 4e52  ext.GREEN + f"NR
-00022d10: 7b6e 727d 2220 2b20 636f 6c6f 7254 6578  {nr}" + colorTex
-00022d20: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-00022d30: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00022d40: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00022d50: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
-00022d60: 7361 7665 645b 315d 202b 2066 224e 527b  saved[1] + f"NR{
-00022d70: 6e72 7d22 0d0a 2020 2020 2020 2020 2020  nr}"..          
-00022d80: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00022d90: 650d 0a20 2020 2020 2020 2020 2020 2072  e..            r
-00022da0: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
-00022db0: 2020 2023 2046 696e 6420 6966 2073 746f     # Find if sto
-00022dc0: 636b 2069 7320 6e65 776c 7920 6c69 7374  ck is newly list
-00022dd0: 6564 0d0a 2020 2020 6465 6620 7661 6c69  ed..    def vali
-00022de0: 6461 7465 4e65 776c 794c 6973 7465 6428  dateNewlyListed(
-00022df0: 7365 6c66 2c20 6466 2c20 6461 7973 546f  self, df, daysTo
-00022e00: 4c6f 6f6b 6261 636b 293a 0d0a 2020 2020  Lookback):..    
-00022e10: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-00022e20: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-00022e30: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00022e40: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-00022e50: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-00022e60: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-00022e70: 6461 7973 546f 4c6f 6f6b 6261 636b 203d  daysToLookback =
-00022e80: 2069 6e74 2864 6179 7354 6f4c 6f6f 6b62   int(daysToLookb
-00022e90: 6163 6b5b 3a2d 315d 290d 0a20 2020 2020  ack[:-1])..     
-00022ea0: 2020 2072 6563 656e 7420 3d20 6461 7461     recent = data
-00022eb0: 2e68 6561 6428 3129 0d0a 2020 2020 2020  .head(1)..      
-00022ec0: 2020 6966 206c 656e 2872 6563 656e 7429    if len(recent)
-00022ed0: 203c 2031 3a0d 0a20 2020 2020 2020 2020   < 1:..         
-00022ee0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00022ef0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00022f00: 6461 7461 2920 3c20 6461 7973 546f 4c6f  data) < daysToLo
-00022f10: 6f6b 6261 636b 2061 6e64 2028 0d0a 2020  okback and (..  
-00022f20: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-00022f30: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-00022f40: 5d20 213d 206e 702e 6e61 6e20 616e 6420  ] != np.nan and 
-00022f50: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
-00022f60: 696c 6f63 5b30 5d20 3e20 300d 0a20 2020  iloc[0] > 0..   
-00022f70: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
-00022f80: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00022f90: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00022fa0: 2046 616c 7365 0d0a 0d0a 2020 2020 2320   False....    # 
-00022fb0: 5661 6c69 6461 7465 2069 6620 7468 6520  Validate if the 
-00022fc0: 7374 6f63 6b20 7072 6963 6573 2061 7265  stock prices are
-00022fd0: 2061 7420 6c65 6173 7420 7269 7369 6e67   at least rising
-00022fe0: 2062 7920 3225 2066 6f72 2074 6865 206c   by 2% for the l
-00022ff0: 6173 7420 3320 7365 7373 696f 6e73 0d0a  ast 3 sessions..
-00023000: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00023010: 5072 6963 6552 6973 696e 6742 7941 744c  PriceRisingByAtL
-00023020: 6561 7374 3250 6572 6365 6e74 2873 656c  east2Percent(sel
-00023030: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-00023040: 742c 2073 6176 6544 6963 7429 3a0d 0a20  t, saveDict):.. 
-00023050: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
-00023060: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
-00023070: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
-00023080: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00023090: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-000230a0: 6466 2e63 6f70 7928 290d 0a20 2020 2020  df.copy()..     
-000230b0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-000230c0: 696c 6c6e 6128 3029 0d0a 2020 2020 2020  illna(0)..      
-000230d0: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-000230e0: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
-000230f0: 6e70 2e69 6e66 5d2c 2030 290d 0a20 2020  np.inf], 0)..   
-00023100: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00023110: 2e68 6561 6428 3429 0d0a 2020 2020 2020  .head(4)..      
-00023120: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
-00023130: 2034 3a0d 0a20 2020 2020 2020 2020 2020   4:..           
-00023140: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00023150: 2020 2020 2020 2064 6179 3020 3d20 6461         day0 = da
-00023160: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
-00023170: 6522 5d2e 6974 656d 2829 0d0a 2020 2020  e"].item()..    
-00023180: 2020 2020 6461 794d 696e 7573 3120 3d20      dayMinus1 = 
-00023190: 6461 7461 2e69 6c6f 635b 315d 5b22 436c  data.iloc[1]["Cl
-000231a0: 6f73 6522 5d2e 6974 656d 2829 0d0a 2020  ose"].item()..  
-000231b0: 2020 2020 2020 6461 794d 696e 7573 3220        dayMinus2 
-000231c0: 3d20 6461 7461 2e69 6c6f 635b 325d 5b22  = data.iloc[2]["
-000231d0: 436c 6f73 6522 5d2e 6974 656d 2829 0d0a  Close"].item()..
-000231e0: 2020 2020 2020 2020 6461 794d 696e 7573          dayMinus
-000231f0: 3320 3d20 6461 7461 2e69 6c6f 635b 335d  3 = data.iloc[3]
-00023200: 5b22 436c 6f73 6522 5d2e 6974 656d 2829  ["Close"].item()
-00023210: 0d0a 2020 2020 2020 2020 7065 7263 656e  ..        percen
-00023220: 7433 203d 2072 6f75 6e64 2828 6461 794d  t3 = round((dayM
-00023230: 696e 7573 3220 2d20 6461 794d 696e 7573  inus2 - dayMinus
-00023240: 3329 202a 2031 3030 202f 2064 6179 4d69  3) * 100 / dayMi
-00023250: 6e75 7333 2c20 3229 0d0a 2020 2020 2020  nus3, 2)..      
-00023260: 2020 7065 7263 656e 7432 203d 2072 6f75    percent2 = rou
-00023270: 6e64 2828 6461 794d 696e 7573 3120 2d20  nd((dayMinus1 - 
-00023280: 6461 794d 696e 7573 3229 202a 2031 3030  dayMinus2) * 100
-00023290: 202f 2064 6179 4d69 6e75 7332 2c20 3229   / dayMinus2, 2)
-000232a0: 0d0a 2020 2020 2020 2020 7065 7263 656e  ..        percen
-000232b0: 7431 203d 2072 6f75 6e64 2828 6461 7930  t1 = round((day0
-000232c0: 202d 2064 6179 4d69 6e75 7331 2920 2a20   - dayMinus1) * 
-000232d0: 3130 3020 2f20 6461 794d 696e 7573 312c  100 / dayMinus1,
-000232e0: 2032 290d 0a0d 0a20 2020 2020 2020 2069   2)....        i
-000232f0: 6620 7065 7263 656e 7431 203e 3d20 3220  f percent1 >= 2 
-00023300: 616e 6420 7065 7263 656e 7432 203e 3d20  and percent2 >= 
-00023310: 3220 616e 6420 7065 7263 656e 7433 203e  2 and percent3 >
-00023320: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
-00023330: 2020 7063 745f 6368 616e 6765 5f74 6578    pct_change_tex
-00023340: 7420 3d20 280d 0a20 2020 2020 2020 2020  t = (..         
-00023350: 2020 2020 2020 2028 2225 2e31 6625 2522         ("%.1f%%"
-00023360: 2025 2070 6572 6365 6e74 3129 0d0a 2020   % percent1)..  
-00023370: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00023380: 2822 2028 252e 3166 2525 2c22 2025 2070  (" (%.1f%%," % p
-00023390: 6572 6365 6e74 3229 0d0a 2020 2020 2020  ercent2)..      
-000233a0: 2020 2020 2020 2020 2020 2b20 2822 2025            + (" %
-000233b0: 2e31 6625 2529 2220 2520 7065 7263 656e  .1f%%)" % percen
-000233c0: 7433 290d 0a20 2020 2020 2020 2020 2020  t3)..           
-000233d0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-000233e0: 7361 7665 4469 6374 5b22 2543 686e 6722  saveDict["%Chng"
-000233f0: 5d20 3d20 7063 745f 6368 616e 6765 5f74  ] = pct_change_t
-00023400: 6578 740d 0a20 2020 2020 2020 2020 2020  ext..           
-00023410: 2073 6372 6565 6e44 6963 745b 2225 4368   screenDict["%Ch
-00023420: 6e67 225d 203d 2063 6f6c 6f72 5465 7874  ng"] = colorText
-00023430: 2e47 5245 454e 202b 2070 6374 5f63 6861  .GREEN + pct_cha
-00023440: 6e67 655f 7465 7874 202b 2063 6f6c 6f72  nge_text + color
-00023450: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-00023460: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00023470: 6520 616e 6420 7365 6c66 2e67 6574 4361  e and self.getCa
-00023480: 6e64 6c65 5479 7065 2864 6174 612e 6865  ndleType(data.he
-00023490: 6164 2831 2929 0d0a 2020 2020 2020 2020  ad(1))..        
-000234a0: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-000234b0: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-000234c0: 6d65 0d0a 2020 2020 2320 7661 6c69 6461  me..    # valida
-000234d0: 7465 2069 6620 5253 4920 6973 2077 6974  te if RSI is wit
-000234e0: 6869 6e20 6769 7665 6e20 7261 6e67 650d  hin given range.
-000234f0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00023500: 6552 5349 2873 656c 662c 2064 662c 2073  eRSI(self, df, s
-00023510: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00023520: 6963 742c 206d 696e 5253 492c 206d 6178  ict, minRSI, max
-00023530: 5253 492c 7273 694b 6579 3d22 5253 4922  RSI,rsiKey="RSI"
-00023540: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-00023550: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-00023560: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-00023570: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00023580: 616c 7365 0d0a 2020 2020 2020 2020 6966  alse..        if
-00023590: 2072 7369 4b65 7920 6e6f 7420 696e 2064   rsiKey not in d
-000235a0: 662e 636f 6c75 6d6e 733a 0d0a 2020 2020  f.columns:..    
-000235b0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-000235c0: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-000235d0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-000235e0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-000235f0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
-00023600: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00023610: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00023620: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00023630: 0d0a 2020 2020 2020 2020 7273 6920 3d20  ..        rsi = 
-00023640: 696e 7428 6461 7461 2e68 6561 6428 3129  int(data.head(1)
-00023650: 5b72 7369 4b65 795d 2e69 6c6f 635b 305d  [rsiKey].iloc[0]
-00023660: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
-00023670: 6963 745b 7273 694b 6579 5d20 3d20 7273  ict[rsiKey] = rs
-00023680: 690d 0a20 2020 2020 2020 2023 2068 7474  i..        # htt
-00023690: 7073 3a2f 2f63 6861 7274 696e 6b2e 636f  ps://chartink.co
-000236a0: 6d2f 7363 7265 656e 6572 2f72 7369 2d73  m/screener/rsi-s
-000236b0: 6372 6565 6e69 6e67 0d0a 2020 2020 2020  creening..      
-000236c0: 2020 6966 2072 7369 3e20 3020 616e 6420    if rsi> 0 and 
-000236d0: 7273 6920 3e3d 206d 696e 5253 4920 616e  rsi >= minRSI an
-000236e0: 6420 7273 6920 3c3d 206d 6178 5253 493a  d rsi <= maxRSI:
-000236f0: 2020 2320 6f72 2028 7273 6920 3c3d 2037    # or (rsi <= 7
-00023700: 3120 616e 6420 7273 6920 3e3d 2036 3729  1 and rsi >= 67)
-00023710: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00023720: 6372 6565 6e44 6963 745b 7273 694b 6579  creenDict[rsiKey
-00023730: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
-00023740: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
-00023750: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-00023760: 742e 4752 4545 4e20 2b20 7374 7228 7273  t.GREEN + str(rs
-00023770: 6929 202b 2063 6f6c 6f72 5465 7874 2e45  i) + colorText.E
-00023780: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-00023790: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-000237a0: 6574 7572 6e20 5472 7565 2069 6620 2872  eturn True if (r
-000237b0: 7369 4b65 7920 3d3d 2022 5253 4969 2229  siKey == "RSIi")
-000237c0: 2065 6c73 6520 2873 656c 662e 7661 6c69   else (self.vali
-000237d0: 6461 7465 5253 4928 6466 2c20 7363 7265  dateRSI(df, scre
-000237e0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-000237f0: 2c20 6d69 6e52 5349 2c20 6d61 7852 5349  , minRSI, maxRSI
-00023800: 2c72 7369 4b65 793d 2252 5349 6922 2920  ,rsiKey="RSIi") 
-00023810: 6f72 2054 7275 6529 0d0a 2020 2020 2020  or True)..      
-00023820: 2020 7363 7265 656e 4469 6374 5b72 7369    screenDict[rsi
-00023830: 4b65 795d 203d 2063 6f6c 6f72 5465 7874  Key] = colorText
-00023840: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-00023850: 742e 4641 494c 202b 2073 7472 2872 7369  t.FAIL + str(rsi
-00023860: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
-00023870: 440d 0a20 2020 2020 2020 2023 2049 6620  D..        # If 
-00023880: 6569 7468 6572 2064 6169 6c79 206f 7220  either daily or 
-00023890: 696e 7472 6164 6179 2052 5349 2063 6f6d  intraday RSI com
-000238a0: 6573 2077 6974 6869 6e20 7261 6e67 653f  es within range?
-000238b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000238c0: 2046 616c 7365 2069 6620 2872 7369 4b65   False if (rsiKe
-000238d0: 7920 3d3d 2022 5253 4969 2229 2065 6c73  y == "RSIi") els
-000238e0: 6520 2873 656c 662e 7661 6c69 6461 7465  e (self.validate
-000238f0: 5253 4928 6466 2c20 7363 7265 656e 4469  RSI(df, screenDi
-00023900: 6374 2c20 7361 7665 4469 6374 2c20 6d69  ct, saveDict, mi
-00023910: 6e52 5349 2c20 6d61 7852 5349 2c72 7369  nRSI, maxRSI,rsi
-00023920: 4b65 793d 2252 5349 6922 2929 0d0a 0d0a  Key="RSIi"))....
-00023930: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
-00023940: 6620 7468 6520 7374 6f63 6b20 6973 2062  f the stock is b
-00023950: 756c 6c69 7368 2069 6e20 7468 6520 7368  ullish in the sh
-00023960: 6f72 7420 7465 726d 0d0a 2020 2020 6465  ort term..    de
-00023970: 6620 7661 6c69 6461 7465 5368 6f72 7454  f validateShortT
-00023980: 6572 6d42 756c 6c69 7368 2873 656c 662c  ermBullish(self,
-00023990: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-000239a0: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
-000239b0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-000239c0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-000239d0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000239e0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-000239f0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-00023a00: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00023a10: 2023 2068 7474 7073 3a2f 2f63 6861 7274   # https://chart
-00023a20: 696e 6b2e 636f 6d2f 7363 7265 656e 6572  ink.com/screener
-00023a30: 2f73 686f 7274 2d74 6572 6d2d 6275 6c6c  /short-term-bull
-00023a40: 6973 680d 0a20 2020 2020 2020 2064 6174  ish..        dat
-00023a50: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
-00023a60: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
-00023a70: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-00023a80: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
-00023a90: 5d2c 2030 290d 0a20 2020 2020 2020 2072  ], 0)..        r
-00023aa0: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
-00023ab0: 6428 3129 0d0a 2020 2020 2020 2020 666b  d(1)..        fk
-00023ac0: 203d 2030 2069 6620 6c65 6e28 6461 7461   = 0 if len(data
-00023ad0: 2920 3c20 3320 656c 7365 206e 702e 726f  ) < 3 else np.ro
-00023ae0: 756e 6428 6461 7461 5b22 4641 5354 4b22  und(data["FASTK"
-00023af0: 5d2e 696c 6f63 5b32 5d2c 2035 290d 0a20  ].iloc[2], 5).. 
-00023b00: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
-00023b10: 2074 6865 2064 6174 6166 7261 6d65 2066   the dataframe f
-00023b20: 6f72 2069 6368 696d 6f6b 7520 6361 6c63  or ichimoku calc
-00023b30: 756c 6174 696f 6e73 2077 6974 6820 6461  ulations with da
-00023b40: 7465 2069 6e20 6173 6365 6e64 696e 6720  te in ascending 
-00023b50: 6f72 6465 720d 0a20 2020 2020 2020 2064  order..        d
-00023b60: 665f 6e65 7720 3d20 6461 7461 5b3a 3a2d  f_new = data[::-
-00023b70: 315d 0d0a 2020 2020 2020 2020 7472 793a  1]..        try:
-00023b80: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-00023b90: 5f69 6368 6920 3d20 6466 5f6e 6577 2e72  _ichi = df_new.r
-00023ba0: 656e 616d 6528 0d0a 2020 2020 2020 2020  ename(..        
-00023bb0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-00023bc0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00023bd0: 2020 2020 2020 2022 4f70 656e 223a 2022         "Open": "
-00023be0: 6f70 656e 222c 0d0a 2020 2020 2020 2020  open",..        
-00023bf0: 2020 2020 2020 2020 2020 2020 2248 6967              "Hig
-00023c00: 6822 3a20 2268 6967 6822 2c0d 0a20 2020  h": "high",..   
-00023c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c20: 2022 4c6f 7722 3a20 226c 6f77 222c 0d0a   "Low": "low",..
-00023c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c40: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
-00023c50: 6f73 6522 2c0d 0a20 2020 2020 2020 2020  ose",..         
-00023c60: 2020 2020 2020 2020 2020 2022 566f 6c75             "Volu
-00023c70: 6d65 223a 2022 766f 6c75 6d65 222c 0d0a  me": "volume",..
-00023c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c90: 7d0d 0a20 2020 2020 2020 2020 2020 2029  }..            )
-00023ca0: 0d0a 2020 2020 2020 2020 2020 2020 6963  ..            ic
-00023cb0: 6869 203d 2070 6b74 616c 6962 2e69 6368  hi = pktalib.ich
-00023cc0: 696d 6f6b 7528 6466 5f69 6368 692c 2039  imoku(df_ichi, 9
-00023cd0: 2c20 3236 2c20 3532 2c20 3236 290d 0a20  , 26, 52, 26).. 
-00023ce0: 2020 2020 2020 2020 2020 2069 6620 6963             if ic
-00023cf0: 6869 2069 7320 4e6f 6e65 3a0d 0a20 2020  hi is None:..   
-00023d00: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00023d10: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
-00023d20: 2020 2020 2020 2064 665f 6e65 7720 3d20         df_new = 
-00023d30: 7064 2e63 6f6e 6361 7428 5b64 665f 6e65  pd.concat([df_ne
-00023d40: 772c 2069 6368 695d 2c20 6178 6973 3d31  w, ichi], axis=1
-00023d50: 290d 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00023d60: 2052 6576 6572 7365 2061 6761 696e 2074   Reverse again t
-00023d70: 6f20 6765 7420 7468 6520 6d6f 7374 2072  o get the most r
-00023d80: 6563 656e 7420 6461 7465 206f 6e20 746f  ecent date on to
-00023d90: 700d 0a20 2020 2020 2020 2020 2020 2064  p..            d
-00023da0: 665f 6e65 7720 3d20 6466 5f6e 6577 5b3a  f_new = df_new[:
-00023db0: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
-00023dc0: 2020 6466 5f6e 6577 203d 2064 665f 6e65    df_new = df_ne
-00023dd0: 772e 6865 6164 2831 290d 0a20 2020 2020  w.head(1)..     
-00023de0: 2020 2020 2020 2064 665f 6e65 775b 2263         df_new["c
-00023df0: 6c6f 7564 5f67 7265 656e 225d 203d 2064  loud_green"] = d
-00023e00: 665f 6e65 775b 2249 5341 5f39 225d 2e69  f_new["ISA_9"].i
-00023e10: 6c6f 635b 305d 203e 2064 665f 6e65 775b  loc[0] > df_new[
-00023e20: 2249 5342 5f32 3622 5d2e 696c 6f63 5b30  "ISB_26"].iloc[0
-00023e30: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
-00023e40: 665f 6e65 775b 2263 6c6f 7564 5f72 6564  f_new["cloud_red
-00023e50: 225d 203d 2064 665f 6e65 775b 2249 5342  "] = df_new["ISB
-00023e60: 5f32 3622 5d2e 696c 6f63 5b30 5d20 3e20  _26"].iloc[0] > 
-00023e70: 6466 5f6e 6577 5b22 4953 415f 3922 5d2e  df_new["ISA_9"].
-00023e80: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
-00023e90: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00023ea0: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
-00023eb0: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
-00023ec0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00023ed0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-00023ee0: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-00023ef0: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-00023f00: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-00023f10: 6162 6f76 6543 6c6f 7564 546f 7020 3d20  aboveCloudTop = 
-00023f20: 4661 6c73 650d 0a20 2020 2020 2020 2023  False..        #
-00023f30: 2062 6173 656c 696e 6520 3e20 636c 6f75   baseline > clou
-00023f40: 6420 746f 7020 2863 6c6f 7564 2069 7320  d top (cloud is 
-00023f50: 626f 756e 6420 6279 2073 7061 6e20 6120  bound by span a 
-00023f60: 616e 6420 7370 616e 2062 2920 616e 6420  and span b) and 
-00023f70: 636c 6f73 6520 6973 203e 2063 6c6f 7564  close is > cloud
-00023f80: 2074 6f70 0d0a 2020 2020 2020 2020 6966   top..        if
-00023f90: 2064 665f 6e65 775b 2263 6c6f 7564 5f67   df_new["cloud_g
-00023fa0: 7265 656e 225d 2e69 6c6f 635b 305d 3a0d  reen"].iloc[0]:.
-00023fb0: 0a20 2020 2020 2020 2020 2020 2061 626f  .            abo
-00023fc0: 7665 436c 6f75 6454 6f70 203d 2028 0d0a  veCloudTop = (..
-00023fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023fe0: 6466 5f6e 6577 5b22 494b 535f 3236 225d  df_new["IKS_26"]
-00023ff0: 2e69 6c6f 635b 305d 203e 2064 665f 6e65  .iloc[0] > df_ne
-00024000: 775b 2249 5341 5f39 225d 2e69 6c6f 635b  w["ISA_9"].iloc[
-00024010: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00024020: 2020 2020 616e 6420 7265 6365 6e74 5b22      and recent["
-00024030: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-00024040: 3e20 6466 5f6e 6577 5b22 4953 415f 3922  > df_new["ISA_9"
-00024050: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
-00024060: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00024070: 2020 656c 6966 2064 665f 6e65 775b 2263    elif df_new["c
-00024080: 6c6f 7564 5f72 6564 225d 2e69 6c6f 635b  loud_red"].iloc[
-00024090: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
-000240a0: 2061 626f 7665 436c 6f75 6454 6f70 203d   aboveCloudTop =
-000240b0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-000240c0: 2020 2020 6466 5f6e 6577 5b22 494b 535f      df_new["IKS_
-000240d0: 3236 225d 2e69 6c6f 635b 305d 203e 2064  26"].iloc[0] > d
-000240e0: 665f 6e65 775b 2249 5342 5f32 3622 5d2e  f_new["ISB_26"].
-000240f0: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
-00024100: 2020 2020 2020 2020 2061 6e64 2072 6563           and rec
-00024110: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
-00024120: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
-00024130: 5342 5f32 3622 5d2e 696c 6f63 5b30 5d0d  SB_26"].iloc[0].
-00024140: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00024150: 0d0a 2020 2020 2020 2020 2320 4c61 7465  ..        # Late
-00024160: 7374 2049 6368 696d 6f6b 7520 6261 7365  st Ichimoku base
-00024170: 6c69 6e65 2069 7320 3c20 6c61 7465 7374  line is < latest
-00024180: 2049 6368 696d 6f6b 7520 636f 6e76 6572   Ichimoku conver
-00024190: 7369 6f6e 206c 696e 650d 0a20 2020 2020  sion line..     
-000241a0: 2020 2069 6620 6162 6f76 6543 6c6f 7564     if aboveCloud
-000241b0: 546f 7020 616e 6420 6466 5f6e 6577 5b22  Top and df_new["
-000241c0: 494b 535f 3236 225d 2e69 6c6f 635b 305d  IKS_26"].iloc[0]
-000241d0: 203c 2064 665f 6e65 775b 2249 5453 5f39   < df_new["ITS_9
-000241e0: 225d 2e69 6c6f 635b 305d 3a0d 0a20 2020  "].iloc[0]:..   
-000241f0: 2020 2020 2020 2020 2023 2053 746f 6368           # Stoch
-00024200: 5253 4920 6372 6f73 7365 6420 3230 2061  RSI crossed 20 a
-00024210: 6e64 2052 5349 203e 2035 300d 0a20 2020  nd RSI > 50..   
-00024220: 2020 2020 2020 2020 2069 6620 666b 203e           if fk >
-00024230: 2032 3020 616e 6420 7265 6365 6e74 5b22   20 and recent["
-00024240: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
-00024250: 3530 3a0d 0a20 2020 2020 2020 2020 2020  50:..           
-00024260: 2020 2020 2023 2063 6f6e 6469 7469 6f6e       # condition
-00024270: 206f 6620 6372 6f73 7369 6e67 2074 6865   of crossing the
-00024280: 2053 746f 6368 5253 4920 6d61 696e 2073   StochRSI main s
-00024290: 6967 6e61 6c20 6c69 6e65 2066 726f 6d20  ignal line from 
-000242a0: 626f 7474 6f6d 2074 6f20 746f 700d 0a20  bottom to top.. 
-000242b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000242c0: 6620 280d 0a20 2020 2020 2020 2020 2020  f (..           
-000242d0: 2020 2020 2020 2020 2064 6174 615b 2246           data["F
-000242e0: 4153 5444 225d 2e69 6c6f 635b 3130 305d  ASTD"].iloc[100]
-000242f0: 203c 2064 6174 615b 2246 4153 544b 225d   < data["FASTK"]
-00024300: 2e69 6c6f 635b 3130 305d 0d0a 2020 2020  .iloc[100]..    
-00024310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024320: 616e 6420 6461 7461 5b22 4641 5354 4422  and data["FASTD"
-00024330: 5d2e 696c 6f63 5b31 3031 5d20 3e20 6461  ].iloc[101] > da
-00024340: 7461 5b22 4641 5354 4b22 5d2e 696c 6f63  ta["FASTK"].iloc
-00024350: 5b31 3031 5d0d 0a20 2020 2020 2020 2020  [101]..         
-00024360: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
-00024370: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00024380: 2063 6c6f 7365 203e 2035 3020 7065 7269   close > 50 peri
-00024390: 6f64 2053 4d41 2f45 4d41 2061 6e64 2032  od SMA/EMA and 2
-000243a0: 3030 2070 6572 696f 6420 534d 412f 454d  00 period SMA/EM
-000243b0: 410d 0a20 2020 2020 2020 2020 2020 2020  A..             
-000243c0: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
-000243d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000243e0: 2020 2020 2072 6563 656e 745b 2253 534d       recent["SSM
-000243f0: 4122 5d2e 696c 6f63 5b30 5d20 3e20 7265  A"].iloc[0] > re
-00024400: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-00024410: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-00024420: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00024430: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
-00024440: 2e69 6c6f 635b 305d 203e 2072 6563 656e  .iloc[0] > recen
-00024450: 745b 2253 534d 4122 5d2e 696c 6f63 5b30  t["SSMA"].iloc[0
-00024460: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00024470: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-00024480: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
-00024490: 6c6f 635b 305d 203e 2072 6563 656e 745b  loc[0] > recent[
-000244a0: 224c 4d41 225d 2e69 6c6f 635b 305d 0d0a  "LMA"].iloc[0]..
-000244b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000244c0: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
+000212d0: 2e69 6e66 6f28 0d0a 2020 2020 2020 2020  .info(..        
+000212e0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+000212f0: 2020 6627 5374 6f63 6b3a 7b73 6176 6544    f'Stock:{saveD
+00021300: 6963 745b 2253 746f 636b 225d 7d2c 2069  ict["Stock"]}, i
+00021310: 7320 6e6f 7420 6120 6d6f 6d65 6e74 756d  s not a momentum
+00021320: 2d67 6169 6e65 7220 6265 6361 7573 6520  -gainer because 
+00021330: 6569 7468 6572 2074 6f64 6179 2d6f 7065  either today-ope
+00021340: 6e20 287b 746f 7d29 203c 2079 6573 7465  n ({to}) < yeste
+00021350: 7264 6179 2d63 6c6f 7365 2028 7b79 637d  rday-close ({yc}
+00021360: 2920 6f72 2079 6573 7465 7264 6179 2d6f  ) or yesterday-o
+00021370: 7065 6e28 7b79 6f7d 2920 3c20 6461 792d  pen({yo}) < day-
+00021380: 6265 666f 7265 2d63 6c6f 7365 287b 6479  before-close({dy
+00021390: 637d 2927 0d0a 2020 2020 2020 2020 2020  c})'..          
+000213a0: 2020 2020 2020 2020 2020 2320 290d 0a20            # ).. 
+000213b0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+000213c0: 7420 496e 6465 7845 7272 6f72 2061 7320  t IndexError as 
+000213d0: 653a 2023 2070 7261 676d 613a 206e 6f20  e: # pragma: no 
+000213e0: 636f 7665 720d 0a20 2020 2020 2020 2020  cover..         
+000213f0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+00021400: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+00021410: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
+00021420: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00021430: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
+00021440: 5f6c 6f67 6765 722e 6465 6275 6728 6461  _logger.debug(da
+00021450: 7461 290d 0a20 2020 2020 2020 2020 2020  ta)..           
+00021460: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
+00021470: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00021480: 6c73 650d 0a20 2020 2020 2020 2065 7863  lse..        exc
+00021490: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+000214a0: 2065 3a20 2023 2070 7261 676d 613a 206e   e:  # pragma: n
+000214b0: 6f20 636f 7665 720d 0a20 2020 2020 2020  o cover..       
+000214c0: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
+000214d0: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
+000214e0: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
+000214f0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00021500: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
+00021510: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
+00021520: 0d0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
+00021530: 204d 6f76 696e 6720 6176 6572 6167 6573   Moving averages
+00021540: 2061 6e64 206c 6f6f 6b20 666f 7220 6275   and look for bu
+00021550: 792f 7365 6c6c 2073 6967 6e61 6c73 0d0a  y/sell signals..
+00021560: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00021570: 4d6f 7669 6e67 4176 6572 6167 6573 2873  MovingAverages(s
+00021580: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
+00021590: 6963 742c 2073 6176 6544 6963 742c 206d  ict, saveDict, m
+000215a0: 6152 616e 6765 3d32 2e35 293a 0d0a 2020  aRange=2.5):..  
+000215b0: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+000215c0: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+000215d0: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+000215e0: 6e61 2830 290d 0a20 2020 2020 2020 2064  na(0)..        d
+000215f0: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
+00021600: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
+00021610: 696e 665d 2c20 3029 0d0a 2020 2020 2020  inf], 0)..      
+00021620: 2020 7265 6365 6e74 203d 2064 6174 612e    recent = data.
+00021630: 6865 6164 2831 290d 0a20 2020 2020 2020  head(1)..       
+00021640: 2073 6176 6564 203d 2073 656c 662e 6669   saved = self.fi
+00021650: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
+00021660: 6c75 6528 7363 7265 656e 4469 6374 2c73  lue(screenDict,s
+00021670: 6176 6544 6963 742c 224d 412d 5369 676e  aveDict,"MA-Sign
+00021680: 616c 2229 0d0a 2020 2020 2020 2020 6966  al")..        if
+00021690: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+000216a0: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
+000216b0: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b22  oc[0] > recent["
+000216c0: 4c4d 4122 5d2e 696c 6f63 5b30 5d0d 0a20  LMA"].iloc[0].. 
+000216d0: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
+000216e0: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
+000216f0: 6c6f 635b 305d 203e 2072 6563 656e 745b  loc[0] > recent[
+00021700: 2253 4d41 225d 2e69 6c6f 635b 305d 0d0a  "SMA"].iloc[0]..
+00021710: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
+00021720: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00021730: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00021740: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+00021750: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
+00021760: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+00021770: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+00021780: 202b 2022 4275 6c6c 6973 6822 202b 2063   + "Bullish" + c
+00021790: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+000217a0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+000217b0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+000217c0: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+000217d0: 2073 6176 6564 5b31 5d20 2b20 2242 756c   saved[1] + "Bul
+000217e0: 6c69 7368 220d 0a20 2020 2020 2020 2065  lish"..        e
+000217f0: 6c69 6620 7265 6365 6e74 5b22 534d 4122  lif recent["SMA"
+00021800: 5d2e 696c 6f63 5b30 5d20 3c20 7265 6365  ].iloc[0] < rece
+00021810: 6e74 5b22 4c4d 4122 5d2e 696c 6f63 5b30  nt["LMA"].iloc[0
+00021820: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+00021830: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
+00021840: 6967 6e61 6c22 5d20 3d20 280d 0a20 2020  ignal"] = (..   
+00021850: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00021860: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
+00021870: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
+00021880: 7874 2e46 4149 4c20 2b20 2242 6561 7269  xt.FAIL + "Beari
+00021890: 7368 2220 2b20 636f 6c6f 7254 6578 742e  sh" + colorText.
+000218a0: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+000218b0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+000218c0: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
+000218d0: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
+000218e0: 202b 2022 4265 6172 6973 6822 0d0a 2020   + "Bearish"..  
+000218f0: 2020 2020 2020 656c 6966 2072 6563 656e        elif recen
+00021900: 745b 2253 4d41 225d 2e69 6c6f 635b 305d  t["SMA"].iloc[0]
+00021910: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00021920: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+00021930: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280d  MA-Signal"] = (.
+00021940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021950: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
+00021960: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
+00021970: 6f72 5465 7874 2e57 4152 4e20 2b20 2255  orText.WARN + "U
+00021980: 6e6b 6e6f 776e 2220 2b20 636f 6c6f 7254  nknown" + colorT
+00021990: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
+000219a0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000219b0: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
+000219c0: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
+000219d0: 645b 315d 202b 2022 556e 6b6e 6f77 6e22  d[1] + "Unknown"
+000219e0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+000219f0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+00021a00: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
+00021a10: 616c 225d 203d 2028 0d0a 2020 2020 2020  al"] = (..      
+00021a20: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+00021a30: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
+00021a40: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+00021a50: 5741 524e 202b 2022 4e65 7574 7261 6c22  WARN + "Neutral"
+00021a60: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+00021a70: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00021a80: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+00021a90: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
+00021aa0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+00021ab0: 224e 6575 7472 616c 220d 0a0d 0a20 2020  "Neutral"....   
+00021ac0: 2020 2020 2073 6d61 4465 7620 3d20 6461       smaDev = da
+00021ad0: 7461 5b22 534d 4122 5d2e 696c 6f63 5b30  ta["SMA"].iloc[0
+00021ae0: 5d20 2a20 6d61 5261 6e67 6520 2f20 3130  ] * maRange / 10
+00021af0: 300d 0a20 2020 2020 2020 206c 6d61 4465  0..        lmaDe
+00021b00: 7620 3d20 6461 7461 5b22 4c4d 4122 5d2e  v = data["LMA"].
+00021b10: 696c 6f63 5b30 5d20 2a20 6d61 5261 6e67  iloc[0] * maRang
+00021b20: 6520 2f20 3130 300d 0a20 2020 2020 2020  e / 100..       
+00021b30: 206f 7065 6e2c 2068 6967 682c 206c 6f77   open, high, low
+00021b40: 2c20 636c 6f73 652c 2073 6d61 2c20 6c6d  , close, sma, lm
+00021b50: 6120 3d20 280d 0a20 2020 2020 2020 2020  a = (..         
+00021b60: 2020 2064 6174 615b 224f 7065 6e22 5d2e     data["Open"].
+00021b70: 696c 6f63 5b30 5d2c 0d0a 2020 2020 2020  iloc[0],..      
+00021b80: 2020 2020 2020 6461 7461 5b22 4869 6768        data["High
+00021b90: 225d 2e69 6c6f 635b 305d 2c0d 0a20 2020  "].iloc[0],..   
+00021ba0: 2020 2020 2020 2020 2064 6174 615b 224c           data["L
+00021bb0: 6f77 225d 2e69 6c6f 635b 305d 2c0d 0a20  ow"].iloc[0],.. 
+00021bc0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00021bd0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+00021be0: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00021bf0: 6174 615b 2253 4d41 225d 2e69 6c6f 635b  ata["SMA"].iloc[
+00021c00: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
+00021c10: 2064 6174 615b 224c 4d41 225d 2e69 6c6f   data["LMA"].ilo
+00021c20: 635b 305d 2c0d 0a20 2020 2020 2020 2029  c[0],..        )
+00021c30: 0d0a 2020 2020 2020 2020 6d61 5265 7665  ..        maReve
+00021c40: 7273 616c 203d 2030 0d0a 2020 2020 2020  rsal = 0..      
+00021c50: 2020 2320 5461 6b69 6e67 2053 7570 706f    # Taking Suppo
+00021c60: 7274 2035 300d 0a20 2020 2020 2020 2069  rt 50..        i
+00021c70: 6620 636c 6f73 6520 3e20 736d 6120 616e  f close > sma an
+00021c80: 6420 6c6f 7720 3c3d 2028 736d 6120 2b20  d low <= (sma + 
+00021c90: 736d 6144 6576 293a 0d0a 2020 2020 2020  smaDev):..      
+00021ca0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00021cb0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+00021cc0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00021cd0: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
+00021ce0: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
+00021cf0: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
+00021d00: 2022 3530 4d41 2d53 7570 706f 7274 2220   "50MA-Support" 
+00021d10: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+00021d20: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00021d30: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00021d40: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+00021d50: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
+00021d60: 3530 4d41 2d53 7570 706f 7274 220d 0a20  50MA-Support".. 
+00021d70: 2020 2020 2020 2020 2020 206d 6152 6576             maRev
+00021d80: 6572 7361 6c20 3d20 310d 0a20 2020 2020  ersal = 1..     
+00021d90: 2020 2023 2056 616c 6964 6174 696e 6720     # Validating 
+00021da0: 5265 7369 7374 616e 6365 2035 300d 0a20  Resistance 50.. 
+00021db0: 2020 2020 2020 2065 6c69 6620 636c 6f73         elif clos
+00021dc0: 6520 3c20 736d 6120 616e 6420 6869 6768  e < sma and high
+00021dd0: 203e 3d20 2873 6d61 202d 2073 6d61 4465   >= (sma - smaDe
+00021de0: 7629 3a0d 0a20 2020 2020 2020 2020 2020  v):..           
+00021df0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
+00021e00: 5369 676e 616c 225d 203d 2028 0d0a 2020  Signal"] = (..  
+00021e10: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00021e20: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
+00021e30: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
+00021e40: 6578 742e 4641 494c 202b 2022 3530 4d41  ext.FAIL + "50MA
+00021e50: 2d52 6573 6973 7422 202b 2063 6f6c 6f72  -Resist" + color
+00021e60: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+00021e70: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00021e80: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
+00021e90: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
+00021ea0: 6564 5b31 5d20 2b20 2235 304d 412d 5265  ed[1] + "50MA-Re
+00021eb0: 7369 7374 220d 0a20 2020 2020 2020 2020  sist"..         
+00021ec0: 2020 206d 6152 6576 6572 7361 6c20 3d20     maReversal = 
+00021ed0: 2d31 0d0a 2020 2020 2020 2020 2320 5461  -1..        # Ta
+00021ee0: 6b69 6e67 2053 7570 706f 7274 2032 3030  king Support 200
+00021ef0: 0d0a 2020 2020 2020 2020 656c 6966 2063  ..        elif c
+00021f00: 6c6f 7365 203e 206c 6d61 2061 6e64 206c  lose > lma and l
+00021f10: 6f77 203c 3d20 286c 6d61 202b 206c 6d61  ow <= (lma + lma
+00021f20: 4465 7629 3a0d 0a20 2020 2020 2020 2020  Dev):..         
+00021f30: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
+00021f40: 412d 5369 676e 616c 225d 203d 2028 0d0a  A-Signal"] = (..
+00021f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f60: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00021f70: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00021f80: 7254 6578 742e 4752 4545 4e20 2b20 2232  rText.GREEN + "2
+00021f90: 3030 4d41 2d53 7570 706f 7274 2220 2b20  00MA-Support" + 
+00021fa0: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00021fb0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00021fc0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00021fd0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00021fe0: 3d20 7361 7665 645b 315d 202b 2022 3230  = saved[1] + "20
+00021ff0: 304d 412d 5375 7070 6f72 7422 0d0a 2020  0MA-Support"..  
+00022000: 2020 2020 2020 2020 2020 6d61 5265 7665            maReve
+00022010: 7273 616c 203d 2031 0d0a 2020 2020 2020  rsal = 1..      
+00022020: 2020 2320 5661 6c69 6461 7469 6e67 2052    # Validating R
+00022030: 6573 6973 7461 6e63 6520 3230 300d 0a20  esistance 200.. 
+00022040: 2020 2020 2020 2065 6c69 6620 636c 6f73         elif clos
+00022050: 6520 3c20 6c6d 6120 616e 6420 6869 6768  e < lma and high
+00022060: 203e 3d20 286c 6d61 202d 206c 6d61 4465   >= (lma - lmaDe
+00022070: 7629 3a0d 0a20 2020 2020 2020 2020 2020  v):..           
+00022080: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
+00022090: 5369 676e 616c 225d 203d 2028 0d0a 2020  Signal"] = (..  
+000220a0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+000220b0: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
+000220c0: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
+000220d0: 6578 742e 4641 494c 202b 2022 3230 304d  ext.FAIL + "200M
+000220e0: 412d 5265 7369 7374 2220 2b20 636f 6c6f  A-Resist" + colo
+000220f0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+00022100: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00022110: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00022120: 4d41 2d53 6967 6e61 6c22 5d20 3d20 7361  MA-Signal"] = sa
+00022130: 7665 645b 315d 202b 2022 3230 304d 412d  ved[1] + "200MA-
+00022140: 5265 7369 7374 220d 0a20 2020 2020 2020  Resist"..       
+00022150: 2020 2020 206d 6152 6576 6572 7361 6c20       maReversal 
+00022160: 3d20 2d31 0d0a 2020 2020 2020 2020 2320  = -1..        # 
+00022170: 466f 7220 6120 4275 6c6c 6973 6820 4361  For a Bullish Ca
+00022180: 6e64 6c65 0d0a 2020 2020 2020 2020 6966  ndle..        if
+00022190: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
+000221a0: 7970 6528 6461 7461 293a 0d0a 2020 2020  ype(data):..    
+000221b0: 2020 2020 2020 2020 2320 4372 6f73 7369          # Crossi
+000221c0: 6e67 2075 7020 3530 0d0a 2020 2020 2020  ng up 50..      
+000221d0: 2020 2020 2020 6966 206f 7065 6e20 3c20        if open < 
+000221e0: 736d 6120 616e 6420 636c 6f73 6520 3e20  sma and close > 
+000221f0: 736d 613a 0d0a 2020 2020 2020 2020 2020  sma:..          
+00022200: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00022210: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+00022220: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00022230: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
+00022240: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+00022250: 202b 2063 6f6c 6f72 5465 7874 2e47 5245   + colorText.GRE
+00022260: 454e 202b 2022 4275 6c6c 4372 6f73 732d  EN + "BullCross-
+00022270: 3530 4d41 2220 2b20 636f 6c6f 7254 6578  50MA" + colorTex
+00022280: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+00022290: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000222a0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+000222b0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+000222c0: 3d20 7361 7665 645b 315d 202b 2022 4275  = saved[1] + "Bu
+000222d0: 6c6c 4372 6f73 732d 3530 4d41 220d 0a20  llCross-50MA".. 
+000222e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000222f0: 6152 6576 6572 7361 6c20 3d20 310d 0a20  aReversal = 1.. 
+00022300: 2020 2020 2020 2020 2020 2023 2043 726f             # Cro
+00022310: 7373 696e 6720 7570 2032 3030 0d0a 2020  ssing up 200..  
+00022320: 2020 2020 2020 2020 2020 656c 6966 206f            elif o
+00022330: 7065 6e20 3c20 6c6d 6120 616e 6420 636c  pen < lma and cl
+00022340: 6f73 6520 3e20 6c6d 613a 0d0a 2020 2020  ose > lma:..    
+00022350: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00022360: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
+00022370: 6c22 5d20 3d20 280d 0a20 2020 2020 2020  l"] = (..       
+00022380: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00022390: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
+000223a0: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
+000223b0: 7874 2e47 5245 454e 202b 2022 4275 6c6c  xt.GREEN + "Bull
+000223c0: 4372 6f73 732d 3230 304d 4122 202b 2063  Cross-200MA" + c
+000223d0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+000223e0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+000223f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022400: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
+00022410: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
+00022420: 5d20 2b20 2242 756c 6c43 726f 7373 2d32  ] + "BullCross-2
+00022430: 3030 4d41 220d 0a20 2020 2020 2020 2020  00MA"..         
+00022440: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
+00022450: 6c20 3d20 310d 0a20 2020 2020 2020 2023  l = 1..        #
+00022460: 2046 6f72 2061 2042 6561 7269 7368 2043   For a Bearish C
+00022470: 616e 646c 650d 0a20 2020 2020 2020 2065  andle..        e
+00022480: 6c69 6620 6e6f 7420 7365 6c66 2e67 6574  lif not self.get
+00022490: 4361 6e64 6c65 5479 7065 2864 6174 6129  CandleType(data)
+000224a0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+000224b0: 2043 726f 7373 696e 6720 646f 776e 2035   Crossing down 5
+000224c0: 300d 0a20 2020 2020 2020 2020 2020 2069  0..            i
+000224d0: 6620 6f70 656e 203e 2073 6d61 2061 6e64  f open > sma and
+000224e0: 2063 6c6f 7365 203c 2073 6d61 3a0d 0a20   close < sma:.. 
+000224f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00022500: 6372 6565 6e44 6963 745b 224d 412d 5369  creenDict["MA-Si
+00022510: 676e 616c 225d 203d 2028 0d0a 2020 2020  gnal"] = (..    
+00022520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022530: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00022540: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00022550: 7254 6578 742e 4641 494c 202b 2022 4265  rText.FAIL + "Be
+00022560: 6172 4372 6f73 732d 3530 4d41 2220 2b20  arCross-50MA" + 
+00022570: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00022580: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00022590: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000225a0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
+000225b0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
+000225c0: 315d 202b 2022 4265 6172 4372 6f73 732d  1] + "BearCross-
+000225d0: 3530 4d41 220d 0a20 2020 2020 2020 2020  50MA"..         
+000225e0: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
+000225f0: 6c20 3d20 2d31 0d0a 2020 2020 2020 2020  l = -1..        
+00022600: 2020 2020 2320 4372 6f73 7369 6e67 2075      # Crossing u
+00022610: 7020 3230 300d 0a20 2020 2020 2020 2020  p 200..         
+00022620: 2020 2065 6c69 6620 6f70 656e 203e 206c     elif open > l
+00022630: 6d61 2061 6e64 2063 6c6f 7365 203c 206c  ma and close < l
+00022640: 6d61 3a0d 0a20 2020 2020 2020 2020 2020  ma:..           
+00022650: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00022660: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
+00022670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00022680: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00022690: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+000226a0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+000226b0: 202b 2022 4265 6172 4372 6f73 732d 3230   + "BearCross-20
+000226c0: 304d 4122 202b 2063 6f6c 6f72 5465 7874  0MA" + colorText
+000226d0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+000226e0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000226f0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00022700: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00022710: 2073 6176 6564 5b31 5d20 2b20 2242 6561   saved[1] + "Bea
+00022720: 7243 726f 7373 2d32 3030 4d41 220d 0a20  rCross-200MA".. 
+00022730: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00022740: 6152 6576 6572 7361 6c20 3d20 2d31 0d0a  aReversal = -1..
+00022750: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+00022760: 6152 6576 6572 7361 6c0d 0a0d 0a20 2020  aReversal....   
+00022770: 2023 2046 696e 6420 4e52 7820 7261 6e67   # Find NRx rang
+00022780: 6520 666f 7220 5265 7665 7273 616c 0d0a  e for Reversal..
+00022790: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000227a0: 4e61 7272 6f77 5261 6e67 6528 7365 6c66  NarrowRange(self
+000227b0: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
+000227c0: 2c20 7361 7665 4469 6374 2c20 6e72 3d34  , saveDict, nr=4
+000227d0: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
+000227e0: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+000227f0: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
+00022800: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00022810: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+00022820: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+00022830: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
+00022840: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
+00022850: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
+00022860: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+00022870: 2022 5061 7474 6572 6e22 290d 0a20 2020   "Pattern")..   
+00022880: 2020 2020 2069 6620 504b 4461 7465 5574       if PKDateUt
+00022890: 696c 6974 6965 732e 6973 5472 6164 696e  ilities.isTradin
+000228a0: 6754 696d 6528 293a 0d0a 2020 2020 2020  gTime():..      
+000228b0: 2020 2020 2020 7261 6e67 6544 6174 6120        rangeData 
+000228c0: 3d20 6461 7461 2e68 6561 6428 6e72 202b  = data.head(nr +
+000228d0: 2031 295b 313a 5d0d 0a20 2020 2020 2020   1)[1:]..       
+000228e0: 2020 2020 206e 6f77 5f63 616e 646c 6520       now_candle 
+000228f0: 3d20 6461 7461 2e68 6561 6428 3129 0d0a  = data.head(1)..
+00022900: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
+00022910: 6544 6174 615b 2252 616e 6765 225d 203d  eData["Range"] =
+00022920: 2061 6273 2872 616e 6765 4461 7461 5b22   abs(rangeData["
+00022930: 436c 6f73 6522 5d20 2d20 7261 6e67 6544  Close"] - rangeD
+00022940: 6174 615b 224f 7065 6e22 5d29 0d0a 2020  ata["Open"])..  
+00022950: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+00022960: 203d 2072 616e 6765 4461 7461 2e68 6561   = rangeData.hea
+00022970: 6428 3129 0d0a 2020 2020 2020 2020 2020  d(1)..          
+00022980: 2020 6966 2028 0d0a 2020 2020 2020 2020    if (..        
+00022990: 2020 2020 2020 2020 6c65 6e28 7265 6365          len(rece
+000229a0: 6e74 2920 3d3d 2031 0d0a 2020 2020 2020  nt) == 1..      
+000229b0: 2020 2020 2020 2020 2020 616e 6420 7265            and re
+000229c0: 6365 6e74 5b22 5261 6e67 6522 5d2e 696c  cent["Range"].il
+000229d0: 6f63 5b30 5d20 3d3d 2072 616e 6765 4461  oc[0] == rangeDa
+000229e0: 7461 2e64 6573 6372 6962 6528 295b 2252  ta.describe()["R
+000229f0: 616e 6765 225d 5b22 6d69 6e22 5d0d 0a20  ange"]["min"].. 
+00022a00: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
+00022a10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00022a20: 6620 280d 0a20 2020 2020 2020 2020 2020  f (..           
+00022a30: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+00022a40: 7443 616e 646c 6554 7970 6528 7265 6365  tCandleType(rece
+00022a50: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
+00022a60: 2020 2020 2020 2020 2061 6e64 206e 6f77           and now
+00022a70: 5f63 616e 646c 655b 2243 6c6f 7365 225d  _candle["Close"]
+00022a80: 2e69 6c6f 635b 305d 203e 3d20 7265 6365  .iloc[0] >= rece
+00022a90: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+00022aa0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00022ab0: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
+00022ac0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00022ad0: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
+00022ae0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+00022af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b00: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00022b10: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00022b20: 7254 6578 742e 4752 4545 4e20 2b20 6622  rText.GREEN + f"
+00022b30: 4275 792d 4e52 7b6e 727d 2220 2b20 636f  Buy-NR{nr}" + co
+00022b40: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+00022b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b60: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00022b70: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00022b80: 5b22 5061 7474 6572 6e22 5d20 3d20 7361  ["Pattern"] = sa
+00022b90: 7665 645b 315d 202b 2066 2242 7579 2d4e  ved[1] + f"Buy-N
+00022ba0: 527b 6e72 7d22 0d0a 2020 2020 2020 2020  R{nr}"..        
+00022bb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00022bc0: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
+00022bd0: 2020 2020 2020 2020 2065 6c69 6620 280d           elif (.
+00022be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022bf0: 2020 2020 206e 6f74 2073 656c 662e 6765       not self.ge
+00022c00: 7443 616e 646c 6554 7970 6528 7265 6365  tCandleType(rece
+00022c10: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
+00022c20: 2020 2020 2020 2020 2061 6e64 206e 6f77           and now
+00022c30: 5f63 616e 646c 655b 2243 6c6f 7365 225d  _candle["Close"]
+00022c40: 2e69 6c6f 635b 305d 203c 3d20 7265 6365  .iloc[0] <= rece
+00022c50: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+00022c60: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00022c70: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
+00022c80: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00022c90: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
+00022ca0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+00022cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022cc0: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00022cd0: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00022ce0: 7254 6578 742e 4641 494c 202b 2066 2253  rText.FAIL + f"S
+00022cf0: 656c 6c2d 4e52 7b6e 727d 2220 2b20 636f  ell-NR{nr}" + co
+00022d00: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+00022d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022d20: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00022d30: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00022d40: 5b22 5061 7474 6572 6e22 5d20 3d20 7361  ["Pattern"] = sa
+00022d50: 7665 645b 315d 202b 2066 2253 656c 6c2d  ved[1] + f"Sell-
+00022d60: 4e52 7b6e 727d 220d 0a20 2020 2020 2020  NR{nr}"..       
+00022d70: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00022d80: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
+00022d90: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00022da0: 7365 0d0a 2020 2020 2020 2020 656c 7365  se..        else
+00022db0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00022dc0: 616e 6765 4461 7461 203d 2064 6174 612e  angeData = data.
+00022dd0: 6865 6164 286e 7229 0d0a 2020 2020 2020  head(nr)..      
+00022de0: 2020 2020 2020 7261 6e67 6544 6174 612e        rangeData.
+00022df0: 6c6f 635b 3a2c 2752 616e 6765 275d 203d  loc[:,'Range'] =
+00022e00: 2061 6273 2872 616e 6765 4461 7461 5b22   abs(rangeData["
+00022e10: 436c 6f73 6522 5d20 2d20 7261 6e67 6544  Close"] - rangeD
+00022e20: 6174 615b 224f 7065 6e22 5d29 0d0a 2020  ata["Open"])..  
+00022e30: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+00022e40: 203d 2072 616e 6765 4461 7461 2e68 6561   = rangeData.hea
+00022e50: 6428 3129 0d0a 2020 2020 2020 2020 2020  d(1)..          
+00022e60: 2020 6966 2072 6563 656e 745b 2252 616e    if recent["Ran
+00022e70: 6765 225d 2e69 6c6f 635b 305d 203d 3d20  ge"].iloc[0] == 
+00022e80: 7261 6e67 6544 6174 612e 6465 7363 7269  rangeData.descri
+00022e90: 6265 2829 5b22 5261 6e67 6522 5d5b 226d  be()["Range"]["m
+00022ea0: 696e 225d 3a0d 0a20 2020 2020 2020 2020  in"]:..         
+00022eb0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00022ec0: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+00022ed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00022ee0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00022ef0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00022f00: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00022f10: 4e20 2b20 6622 4e52 7b6e 727d 2220 2b20  N + f"NR{nr}" + 
+00022f20: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00022f30: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00022f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00022f50: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+00022f60: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
+00022f70: 202b 2066 224e 527b 6e72 7d22 0d0a 2020   + f"NR{nr}"..  
+00022f80: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00022f90: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
+00022fa0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00022fb0: 6c73 650d 0a0d 0a20 2020 2023 2046 696e  lse....    # Fin
+00022fc0: 6420 6966 2073 746f 636b 2069 7320 6e65  d if stock is ne
+00022fd0: 776c 7920 6c69 7374 6564 0d0a 2020 2020  wly listed..    
+00022fe0: 6465 6620 7661 6c69 6461 7465 4e65 776c  def validateNewl
+00022ff0: 794c 6973 7465 6428 7365 6c66 2c20 6466  yListed(self, df
+00023000: 2c20 6461 7973 546f 4c6f 6f6b 6261 636b  , daysToLookback
+00023010: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
+00023020: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+00023030: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
+00023040: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00023050: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+00023060: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+00023070: 2020 2020 2020 2020 6461 7973 546f 4c6f          daysToLo
+00023080: 6f6b 6261 636b 203d 2069 6e74 2864 6179  okback = int(day
+00023090: 7354 6f4c 6f6f 6b62 6163 6b5b 3a2d 315d  sToLookback[:-1]
+000230a0: 290d 0a20 2020 2020 2020 2072 6563 656e  )..        recen
+000230b0: 7420 3d20 6461 7461 2e68 6561 6428 3129  t = data.head(1)
+000230c0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+000230d0: 2872 6563 656e 7429 203c 2031 3a0d 0a20  (recent) < 1:.. 
+000230e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000230f0: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
+00023100: 2069 6620 6c65 6e28 6461 7461 2920 3c20   if len(data) < 
+00023110: 6461 7973 546f 4c6f 6f6b 6261 636b 2061  daysToLookback a
+00023120: 6e64 2028 0d0a 2020 2020 2020 2020 2020  nd (..          
+00023130: 2020 7265 6365 6e74 5b22 436c 6f73 6522    recent["Close"
+00023140: 5d2e 696c 6f63 5b30 5d20 213d 206e 702e  ].iloc[0] != np.
+00023150: 6e61 6e20 616e 6420 7265 6365 6e74 5b22  nan and recent["
+00023160: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+00023170: 3e20 300d 0a20 2020 2020 2020 2029 3a0d  > 0..        ):.
+00023180: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00023190: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
+000231a0: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+000231b0: 0d0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
+000231c0: 2069 6620 7468 6520 7374 6f63 6b20 7072   if the stock pr
+000231d0: 6963 6573 2061 7265 2061 7420 6c65 6173  ices are at leas
+000231e0: 7420 7269 7369 6e67 2062 7920 3225 2066  t rising by 2% f
+000231f0: 6f72 2074 6865 206c 6173 7420 3320 7365  or the last 3 se
+00023200: 7373 696f 6e73 0d0a 2020 2020 6465 6620  ssions..    def 
+00023210: 7661 6c69 6461 7465 5072 6963 6552 6973  validatePriceRis
+00023220: 696e 6742 7941 744c 6561 7374 3250 6572  ingByAtLeast2Per
+00023230: 6365 6e74 2873 656c 662c 2064 662c 2073  cent(self, df, s
+00023240: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00023250: 6963 7429 3a0d 0a20 2020 2020 2020 2069  ict):..        i
+00023260: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
+00023270: 6c65 6e28 6466 2920 3d3d 2030 3a0d 0a20  len(df) == 0:.. 
+00023280: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00023290: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
+000232a0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+000232b0: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+000232c0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+000232d0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+000232e0: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
+000232f0: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
+00023300: 2030 290d 0a20 2020 2020 2020 2064 6174   0)..        dat
+00023310: 6120 3d20 6461 7461 2e68 6561 6428 3429  a = data.head(4)
+00023320: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00023330: 2864 6174 6129 203c 2034 3a0d 0a20 2020  (data) < 4:..   
+00023340: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00023350: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
+00023360: 6179 3020 3d20 6461 7461 2e69 6c6f 635b  ay0 = data.iloc[
+00023370: 305d 5b22 436c 6f73 6522 5d2e 6974 656d  0]["Close"].item
+00023380: 2829 0d0a 2020 2020 2020 2020 6461 794d  ()..        dayM
+00023390: 696e 7573 3120 3d20 6461 7461 2e69 6c6f  inus1 = data.ilo
+000233a0: 635b 315d 5b22 436c 6f73 6522 5d2e 6974  c[1]["Close"].it
+000233b0: 656d 2829 0d0a 2020 2020 2020 2020 6461  em()..        da
+000233c0: 794d 696e 7573 3220 3d20 6461 7461 2e69  yMinus2 = data.i
+000233d0: 6c6f 635b 325d 5b22 436c 6f73 6522 5d2e  loc[2]["Close"].
+000233e0: 6974 656d 2829 0d0a 2020 2020 2020 2020  item()..        
+000233f0: 6461 794d 696e 7573 3320 3d20 6461 7461  dayMinus3 = data
+00023400: 2e69 6c6f 635b 335d 5b22 436c 6f73 6522  .iloc[3]["Close"
+00023410: 5d2e 6974 656d 2829 0d0a 2020 2020 2020  ].item()..      
+00023420: 2020 7065 7263 656e 7433 203d 2072 6f75    percent3 = rou
+00023430: 6e64 2828 6461 794d 696e 7573 3220 2d20  nd((dayMinus2 - 
+00023440: 6461 794d 696e 7573 3329 202a 2031 3030  dayMinus3) * 100
+00023450: 202f 2064 6179 4d69 6e75 7333 2c20 3229   / dayMinus3, 2)
+00023460: 0d0a 2020 2020 2020 2020 7065 7263 656e  ..        percen
+00023470: 7432 203d 2072 6f75 6e64 2828 6461 794d  t2 = round((dayM
+00023480: 696e 7573 3120 2d20 6461 794d 696e 7573  inus1 - dayMinus
+00023490: 3229 202a 2031 3030 202f 2064 6179 4d69  2) * 100 / dayMi
+000234a0: 6e75 7332 2c20 3229 0d0a 2020 2020 2020  nus2, 2)..      
+000234b0: 2020 7065 7263 656e 7431 203d 2072 6f75    percent1 = rou
+000234c0: 6e64 2828 6461 7930 202d 2064 6179 4d69  nd((day0 - dayMi
+000234d0: 6e75 7331 2920 2a20 3130 3020 2f20 6461  nus1) * 100 / da
+000234e0: 794d 696e 7573 312c 2032 290d 0a0d 0a20  yMinus1, 2).... 
+000234f0: 2020 2020 2020 2069 6620 7065 7263 656e         if percen
+00023500: 7431 203e 3d20 3220 616e 6420 7065 7263  t1 >= 2 and perc
+00023510: 656e 7432 203e 3d20 3220 616e 6420 7065  ent2 >= 2 and pe
+00023520: 7263 656e 7433 203e 3d20 323a 0d0a 2020  rcent3 >= 2:..  
+00023530: 2020 2020 2020 2020 2020 7063 745f 6368            pct_ch
+00023540: 616e 6765 5f74 6578 7420 3d20 280d 0a20  ange_text = (.. 
+00023550: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00023560: 2225 2e31 6625 2522 2025 2070 6572 6365  "%.1f%%" % perce
+00023570: 6e74 3129 0d0a 2020 2020 2020 2020 2020  nt1)..          
+00023580: 2020 2020 2020 2b20 2822 2028 252e 3166        + (" (%.1f
+00023590: 2525 2c22 2025 2070 6572 6365 6e74 3229  %%," % percent2)
+000235a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000235b0: 2020 2b20 2822 2025 2e31 6625 2529 2220    + (" %.1f%%)" 
+000235c0: 2520 7065 7263 656e 7433 290d 0a20 2020  % percent3)..   
+000235d0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+000235e0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+000235f0: 5b22 2543 686e 6722 5d20 3d20 7063 745f  ["%Chng"] = pct_
+00023600: 6368 616e 6765 5f74 6578 740d 0a20 2020  change_text..   
+00023610: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00023620: 6963 745b 2225 4368 6e67 225d 203d 2063  ict["%Chng"] = c
+00023630: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
+00023640: 2070 6374 5f63 6861 6e67 655f 7465 7874   pct_change_text
+00023650: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+00023660: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00023670: 7475 726e 2054 7275 6520 616e 6420 7365  turn True and se
+00023680: 6c66 2e67 6574 4361 6e64 6c65 5479 7065  lf.getCandleType
+00023690: 2864 6174 612e 6865 6164 2831 2929 0d0a  (data.head(1))..
+000236a0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000236b0: 616c 7365 0d0a 0d0a 2020 2020 2340 6d65  alse....    #@me
+000236c0: 6173 7572 655f 7469 6d65 0d0a 2020 2020  asure_time..    
+000236d0: 2320 7661 6c69 6461 7465 2069 6620 5253  # validate if RS
+000236e0: 4920 6973 2077 6974 6869 6e20 6769 7665  I is within give
+000236f0: 6e20 7261 6e67 650d 0a20 2020 2064 6566  n range..    def
+00023700: 2076 616c 6964 6174 6552 5349 2873 656c   validateRSI(sel
+00023710: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+00023720: 742c 2073 6176 6544 6963 742c 206d 696e  t, saveDict, min
+00023730: 5253 492c 206d 6178 5253 492c 7273 694b  RSI, maxRSI,rsiK
+00023740: 6579 3d22 5253 4922 293a 0d0a 2020 2020  ey="RSI"):..    
+00023750: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+00023760: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+00023770: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00023780: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+00023790: 2020 2020 2020 6966 2072 7369 4b65 7920        if rsiKey 
+000237a0: 6e6f 7420 696e 2064 662e 636f 6c75 6d6e  not in df.column
+000237b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000237c0: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+000237d0: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+000237e0: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+000237f0: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+00023800: 6e61 2830 290d 0a20 2020 2020 2020 2064  na(0)..        d
+00023810: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
+00023820: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
+00023830: 696e 665d 2c20 3029 0d0a 2020 2020 2020  inf], 0)..      
+00023840: 2020 7273 6920 3d20 696e 7428 6461 7461    rsi = int(data
+00023850: 2e68 6561 6428 3129 5b72 7369 4b65 795d  .head(1)[rsiKey]
+00023860: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
+00023870: 2020 2073 6176 6544 6963 745b 7273 694b     saveDict[rsiK
+00023880: 6579 5d20 3d20 7273 690d 0a20 2020 2020  ey] = rsi..     
+00023890: 2020 2023 2068 7474 7073 3a2f 2f63 6861     # https://cha
+000238a0: 7274 696e 6b2e 636f 6d2f 7363 7265 656e  rtink.com/screen
+000238b0: 6572 2f72 7369 2d73 6372 6565 6e69 6e67  er/rsi-screening
+000238c0: 0d0a 2020 2020 2020 2020 6966 2072 7369  ..        if rsi
+000238d0: 3e20 3020 616e 6420 7273 6920 3e3d 206d  > 0 and rsi >= m
+000238e0: 696e 5253 4920 616e 6420 7273 6920 3c3d  inRSI and rsi <=
+000238f0: 206d 6178 5253 493a 2020 2320 6f72 2028   maxRSI:  # or (
+00023900: 7273 6920 3c3d 2037 3120 616e 6420 7273  rsi <= 71 and rs
+00023910: 6920 3e3d 2036 3729 3a0d 0a20 2020 2020  i >= 67):..     
+00023920: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00023930: 745b 7273 694b 6579 5d20 3d20 280d 0a20  t[rsiKey] = (.. 
+00023940: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00023950: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00023960: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
+00023970: 2b20 7374 7228 7273 6929 202b 2063 6f6c  + str(rsi) + col
+00023980: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+00023990: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+000239a0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000239b0: 7565 2069 6620 2872 7369 4b65 7920 3d3d  ue if (rsiKey ==
+000239c0: 2022 5253 4969 2229 2065 6c73 6520 2873   "RSIi") else (s
+000239d0: 656c 662e 7661 6c69 6461 7465 5253 4928  elf.validateRSI(
+000239e0: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
+000239f0: 7361 7665 4469 6374 2c20 6d69 6e52 5349  saveDict, minRSI
+00023a00: 2c20 6d61 7852 5349 2c72 7369 4b65 793d  , maxRSI,rsiKey=
+00023a10: 2252 5349 6922 2920 6f72 2054 7275 6529  "RSIi") or True)
+00023a20: 0d0a 2020 2020 2020 2020 7363 7265 656e  ..        screen
+00023a30: 4469 6374 5b72 7369 4b65 795d 203d 2063  Dict[rsiKey] = c
+00023a40: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00023a50: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
+00023a60: 2073 7472 2872 7369 2920 2b20 636f 6c6f   str(rsi) + colo
+00023a70: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+00023a80: 2020 2023 2049 6620 6569 7468 6572 2064     # If either d
+00023a90: 6169 6c79 206f 7220 696e 7472 6164 6179  aily or intraday
+00023aa0: 2052 5349 2063 6f6d 6573 2077 6974 6869   RSI comes withi
+00023ab0: 6e20 7261 6e67 653f 0d0a 2020 2020 2020  n range?..      
+00023ac0: 2020 7265 7475 726e 2046 616c 7365 2069    return False i
+00023ad0: 6620 2872 7369 4b65 7920 3d3d 2022 5253  f (rsiKey == "RS
+00023ae0: 4969 2229 2065 6c73 6520 2873 656c 662e  Ii") else (self.
+00023af0: 7661 6c69 6461 7465 5253 4928 6466 2c20  validateRSI(df, 
+00023b00: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+00023b10: 4469 6374 2c20 6d69 6e52 5349 2c20 6d61  Dict, minRSI, ma
+00023b20: 7852 5349 2c72 7369 4b65 793d 2252 5349  xRSI,rsiKey="RSI
+00023b30: 6922 2929 0d0a 0d0a 2020 2020 2320 5661  i"))....    # Va
+00023b40: 6c69 6461 7465 2069 6620 7468 6520 7374  lidate if the st
+00023b50: 6f63 6b20 6973 2062 756c 6c69 7368 2069  ock is bullish i
+00023b60: 6e20 7468 6520 7368 6f72 7420 7465 726d  n the short term
+00023b70: 0d0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00023b80: 7465 5368 6f72 7454 6572 6d42 756c 6c69  teShortTermBulli
+00023b90: 7368 2873 656c 662c 2064 662c 2073 6372  sh(self, df, scr
+00023ba0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+00023bb0: 7429 3a0d 0a20 2020 2020 2020 2069 6620  t):..        if 
+00023bc0: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+00023bd0: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
+00023be0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00023bf0: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
+00023c00: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
+00023c10: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
+00023c20: 3a2f 2f63 6861 7274 696e 6b2e 636f 6d2f  ://chartink.com/
+00023c30: 7363 7265 656e 6572 2f73 686f 7274 2d74  screener/short-t
+00023c40: 6572 6d2d 6275 6c6c 6973 680d 0a20 2020  erm-bullish..   
+00023c50: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00023c60: 2e66 696c 6c6e 6128 3029 0d0a 2020 2020  .fillna(0)..    
+00023c70: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00023c80: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+00023c90: 202d 6e70 2e69 6e66 5d2c 2030 290d 0a20   -np.inf], 0).. 
+00023ca0: 2020 2020 2020 2072 6563 656e 7420 3d20         recent = 
+00023cb0: 6461 7461 2e68 6561 6428 3129 0d0a 2020  data.head(1)..  
+00023cc0: 2020 2020 2020 666b 203d 2030 2069 6620        fk = 0 if 
+00023cd0: 6c65 6e28 6461 7461 2920 3c20 3320 656c  len(data) < 3 el
+00023ce0: 7365 206e 702e 726f 756e 6428 6461 7461  se np.round(data
+00023cf0: 5b22 4641 5354 4b22 5d2e 696c 6f63 5b32  ["FASTK"].iloc[2
+00023d00: 5d2c 2035 290d 0a20 2020 2020 2020 2023  ], 5)..        #
+00023d10: 2052 6576 6572 7365 2074 6865 2064 6174   Reverse the dat
+00023d20: 6166 7261 6d65 2066 6f72 2069 6368 696d  aframe for ichim
+00023d30: 6f6b 7520 6361 6c63 756c 6174 696f 6e73  oku calculations
+00023d40: 2077 6974 6820 6461 7465 2069 6e20 6173   with date in as
+00023d50: 6365 6e64 696e 6720 6f72 6465 720d 0a20  cending order.. 
+00023d60: 2020 2020 2020 2064 665f 6e65 7720 3d20         df_new = 
+00023d70: 6461 7461 5b3a 3a2d 315d 0d0a 2020 2020  data[::-1]..    
+00023d80: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00023d90: 2020 2020 2020 6466 5f69 6368 6920 3d20        df_ichi = 
+00023da0: 6466 5f6e 6577 2e72 656e 616d 6528 0d0a  df_new.rename(..
+00023db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023dc0: 636f 6c75 6d6e 733d 7b0d 0a20 2020 2020  columns={..     
+00023dd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00023de0: 4f70 656e 223a 2022 6f70 656e 222c 0d0a  Open": "open",..
+00023df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e00: 2020 2020 2248 6967 6822 3a20 2268 6967      "High": "hig
+00023e10: 6822 2c0d 0a20 2020 2020 2020 2020 2020  h",..           
+00023e20: 2020 2020 2020 2020 2022 4c6f 7722 3a20           "Low": 
+00023e30: 226c 6f77 222c 0d0a 2020 2020 2020 2020  "low",..        
+00023e40: 2020 2020 2020 2020 2020 2020 2243 6c6f              "Clo
+00023e50: 7365 223a 2022 636c 6f73 6522 2c0d 0a20  se": "close",.. 
+00023e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e70: 2020 2022 566f 6c75 6d65 223a 2022 766f     "Volume": "vo
+00023e80: 6c75 6d65 222c 0d0a 2020 2020 2020 2020  lume",..        
+00023e90: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+00023ea0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00023eb0: 2020 2020 2020 6963 6869 203d 2070 6b74        ichi = pkt
+00023ec0: 616c 6962 2e69 6368 696d 6f6b 7528 6466  alib.ichimoku(df
+00023ed0: 5f69 6368 692c 2039 2c20 3236 2c20 3532  _ichi, 9, 26, 52
+00023ee0: 2c20 3236 290d 0a20 2020 2020 2020 2020  , 26)..         
+00023ef0: 2020 2069 6620 6963 6869 2069 7320 4e6f     if ichi is No
+00023f00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00023f10: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00023f20: 650d 0a20 2020 2020 2020 2020 2020 2064  e..            d
+00023f30: 665f 6e65 7720 3d20 7064 2e63 6f6e 6361  f_new = pd.conca
+00023f40: 7428 5b64 665f 6e65 772c 2069 6368 695d  t([df_new, ichi]
+00023f50: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
+00023f60: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
+00023f70: 2061 6761 696e 2074 6f20 6765 7420 7468   again to get th
+00023f80: 6520 6d6f 7374 2072 6563 656e 7420 6461  e most recent da
+00023f90: 7465 206f 6e20 746f 700d 0a20 2020 2020  te on top..     
+00023fa0: 2020 2020 2020 2064 665f 6e65 7720 3d20         df_new = 
+00023fb0: 6466 5f6e 6577 5b3a 3a2d 315d 0d0a 2020  df_new[::-1]..  
+00023fc0: 2020 2020 2020 2020 2020 6466 5f6e 6577            df_new
+00023fd0: 203d 2064 665f 6e65 772e 6865 6164 2831   = df_new.head(1
+00023fe0: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00023ff0: 665f 6e65 775b 2263 6c6f 7564 5f67 7265  f_new["cloud_gre
+00024000: 656e 225d 203d 2064 665f 6e65 775b 2249  en"] = df_new["I
+00024010: 5341 5f39 225d 2e69 6c6f 635b 305d 203e  SA_9"].iloc[0] >
+00024020: 2064 665f 6e65 775b 2249 5342 5f32 3622   df_new["ISB_26"
+00024030: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
+00024040: 2020 2020 2020 2064 665f 6e65 775b 2263         df_new["c
+00024050: 6c6f 7564 5f72 6564 225d 203d 2064 665f  loud_red"] = df_
+00024060: 6e65 775b 2249 5342 5f32 3622 5d2e 696c  new["ISB_26"].il
+00024070: 6f63 5b30 5d20 3e20 6466 5f6e 6577 5b22  oc[0] > df_new["
+00024080: 4953 415f 3922 5d2e 696c 6f63 5b30 5d0d  ISA_9"].iloc[0].
+00024090: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000240a0: 4578 6365 7074 696f 6e20 6173 2065 3a20  Exception as e: 
+000240b0: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+000240c0: 7665 720d 0a20 2020 2020 2020 2020 2020  ver..           
+000240d0: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
+000240e0: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
+000240f0: 635f 696e 666f 3d54 7275 6529 0d0a 2020  c_info=True)..  
+00024100: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00024110: 2020 2020 2020 2020 6162 6f76 6543 6c6f          aboveClo
+00024120: 7564 546f 7020 3d20 4661 6c73 650d 0a20  udTop = False.. 
+00024130: 2020 2020 2020 2023 2062 6173 656c 696e         # baselin
+00024140: 6520 3e20 636c 6f75 6420 746f 7020 2863  e > cloud top (c
+00024150: 6c6f 7564 2069 7320 626f 756e 6420 6279  loud is bound by
+00024160: 2073 7061 6e20 6120 616e 6420 7370 616e   span a and span
+00024170: 2062 2920 616e 6420 636c 6f73 6520 6973   b) and close is
+00024180: 203e 2063 6c6f 7564 2074 6f70 0d0a 2020   > cloud top..  
+00024190: 2020 2020 2020 6966 2064 665f 6e65 775b        if df_new[
+000241a0: 2263 6c6f 7564 5f67 7265 656e 225d 2e69  "cloud_green"].i
+000241b0: 6c6f 635b 305d 3a0d 0a20 2020 2020 2020  loc[0]:..       
+000241c0: 2020 2020 2061 626f 7665 436c 6f75 6454       aboveCloudT
+000241d0: 6f70 203d 2028 0d0a 2020 2020 2020 2020  op = (..        
+000241e0: 2020 2020 2020 2020 6466 5f6e 6577 5b22          df_new["
+000241f0: 494b 535f 3236 225d 2e69 6c6f 635b 305d  IKS_26"].iloc[0]
+00024200: 203e 2064 665f 6e65 775b 2249 5341 5f39   > df_new["ISA_9
+00024210: 225d 2e69 6c6f 635b 305d 0d0a 2020 2020  "].iloc[0]..    
+00024220: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00024230: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
+00024240: 696c 6f63 5b30 5d20 3e20 6466 5f6e 6577  iloc[0] > df_new
+00024250: 5b22 4953 415f 3922 5d2e 696c 6f63 5b30  ["ISA_9"].iloc[0
+00024260: 5d0d 0a20 2020 2020 2020 2020 2020 2029  ]..            )
+00024270: 0d0a 2020 2020 2020 2020 656c 6966 2064  ..        elif d
+00024280: 665f 6e65 775b 2263 6c6f 7564 5f72 6564  f_new["cloud_red
+00024290: 225d 2e69 6c6f 635b 305d 3a0d 0a20 2020  "].iloc[0]:..   
+000242a0: 2020 2020 2020 2020 2061 626f 7665 436c           aboveCl
+000242b0: 6f75 6454 6f70 203d 2028 0d0a 2020 2020  oudTop = (..    
+000242c0: 2020 2020 2020 2020 2020 2020 6466 5f6e              df_n
+000242d0: 6577 5b22 494b 535f 3236 225d 2e69 6c6f  ew["IKS_26"].ilo
+000242e0: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
+000242f0: 5342 5f32 3622 5d2e 696c 6f63 5b30 5d0d  SB_26"].iloc[0].
+00024300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024310: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
+00024320: 7365 225d 2e69 6c6f 635b 305d 203e 2064  se"].iloc[0] > d
+00024330: 665f 6e65 775b 2249 5342 5f32 3622 5d2e  f_new["ISB_26"].
+00024340: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
+00024350: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+00024360: 2020 2320 4c61 7465 7374 2049 6368 696d    # Latest Ichim
+00024370: 6f6b 7520 6261 7365 6c69 6e65 2069 7320  oku baseline is 
+00024380: 3c20 6c61 7465 7374 2049 6368 696d 6f6b  < latest Ichimok
+00024390: 7520 636f 6e76 6572 7369 6f6e 206c 696e  u conversion lin
+000243a0: 650d 0a20 2020 2020 2020 2069 6620 6162  e..        if ab
+000243b0: 6f76 6543 6c6f 7564 546f 7020 616e 6420  oveCloudTop and 
+000243c0: 6466 5f6e 6577 5b22 494b 535f 3236 225d  df_new["IKS_26"]
+000243d0: 2e69 6c6f 635b 305d 203c 2064 665f 6e65  .iloc[0] < df_ne
+000243e0: 775b 2249 5453 5f39 225d 2e69 6c6f 635b  w["ITS_9"].iloc[
+000243f0: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
+00024400: 2023 2053 746f 6368 5253 4920 6372 6f73   # StochRSI cros
+00024410: 7365 6420 3230 2061 6e64 2052 5349 203e  sed 20 and RSI >
+00024420: 2035 300d 0a20 2020 2020 2020 2020 2020   50..           
+00024430: 2069 6620 666b 203e 2032 3020 616e 6420   if fk > 20 and 
+00024440: 7265 6365 6e74 5b22 5253 4922 5d2e 696c  recent["RSI"].il
+00024450: 6f63 5b30 5d20 3e20 3530 3a0d 0a20 2020  oc[0] > 50:..   
+00024460: 2020 2020 2020 2020 2020 2020 2023 2063               # c
+00024470: 6f6e 6469 7469 6f6e 206f 6620 6372 6f73  ondition of cros
+00024480: 7369 6e67 2074 6865 2053 746f 6368 5253  sing the StochRS
+00024490: 4920 6d61 696e 2073 6967 6e61 6c20 6c69  I main signal li
+000244a0: 6e65 2066 726f 6d20 626f 7474 6f6d 2074  ne from bottom t
+000244b0: 6f20 746f 700d 0a20 2020 2020 2020 2020  o top..         
+000244c0: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
 000244d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000244e0: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
-000244f0: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
-00024500: 7565 2873 6372 6565 6e44 6963 742c 7361  ue(screenDict,sa
-00024510: 7665 4469 6374 2c22 4d41 2d53 6967 6e61  veDict,"MA-Signa
-00024520: 6c22 290d 0a20 2020 2020 2020 2020 2020  l")..           
-00024530: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00024540: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
-00024550: 616c 225d 203d 2028 0d0a 2020 2020 2020  al"] = (..      
-00024560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024570: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00024580: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00024590: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-000245a0: 4e20 2b20 2242 756c 6c69 7368 2220 2b20  N + "Bullish" + 
-000245b0: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-000245c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245d0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000245e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245f0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00024600: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-00024610: 315d 202b 2022 4275 6c6c 6973 6822 0d0a  1] + "Bullish"..
+000244e0: 2064 6174 615b 2246 4153 5444 225d 2e69   data["FASTD"].i
+000244f0: 6c6f 635b 3130 305d 203c 2064 6174 615b  loc[100] < data[
+00024500: 2246 4153 544b 225d 2e69 6c6f 635b 3130  "FASTK"].iloc[10
+00024510: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00024520: 2020 2020 2020 2020 616e 6420 6461 7461          and data
+00024530: 5b22 4641 5354 4422 5d2e 696c 6f63 5b31  ["FASTD"].iloc[1
+00024540: 3031 5d20 3e20 6461 7461 5b22 4641 5354  01] > data["FAST
+00024550: 4b22 5d2e 696c 6f63 5b31 3031 5d0d 0a20  K"].iloc[101].. 
+00024560: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00024570: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00024580: 2020 2020 2020 2023 2063 6c6f 7365 203e         # close >
+00024590: 2035 3020 7065 7269 6f64 2053 4d41 2f45   50 period SMA/E
+000245a0: 4d41 2061 6e64 2032 3030 2070 6572 696f  MA and 200 perio
+000245b0: 6420 534d 412f 454d 410d 0a20 2020 2020  d SMA/EMA..     
+000245c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000245d0: 6620 280d 0a20 2020 2020 2020 2020 2020  f (..           
+000245e0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+000245f0: 656e 745b 2253 534d 4122 5d2e 696c 6f63  ent["SSMA"].iloc
+00024600: 5b30 5d20 3e20 7265 6365 6e74 5b22 534d  [0] > recent["SM
+00024610: 4122 5d2e 696c 6f63 5b30 5d0d 0a20 2020  A"].iloc[0]..   
 00024620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024630: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00024640: 7275 650d 0a20 2020 2020 2020 2072 6574  rue..        ret
-00024650: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-00024660: 2023 2056 616c 6964 6174 6520 5650 430d   # Validate VPC.
-00024670: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00024680: 6556 4350 280d 0a20 2020 2020 2020 2073  eVCP(..        s
-00024690: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
-000246a0: 6963 742c 2073 6176 6544 6963 742c 2073  ict, saveDict, s
-000246b0: 746f 636b 4e61 6d65 3d4e 6f6e 652c 2077  tockName=None, w
-000246c0: 696e 646f 773d 332c 2070 6572 6365 6e74  indow=3, percent
-000246d0: 6167 6546 726f 6d54 6f70 3d33 0d0a 2020  ageFromTop=3..  
-000246e0: 2020 293a 0d0a 2020 2020 2020 2020 6966    ):..        if
-000246f0: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
-00024700: 656e 2864 6629 203d 3d20 303a 0d0a 2020  en(df) == 0:..  
-00024710: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00024720: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00024730: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-00024740: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00024750: 2020 2020 2020 2020 2020 2020 7065 7263              perc
-00024760: 656e 7461 6765 4672 6f6d 546f 7020 2f3d  entageFromTop /=
-00024770: 2031 3030 0d0a 2020 2020 2020 2020 2020   100..          
-00024780: 2020 6461 7461 2e72 6573 6574 5f69 6e64    data.reset_ind
-00024790: 6578 2869 6e70 6c61 6365 3d54 7275 6529  ex(inplace=True)
-000247a0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-000247b0: 7461 2e72 656e 616d 6528 636f 6c75 6d6e  ta.rename(column
-000247c0: 733d 7b22 696e 6465 7822 3a20 2244 6174  s={"index": "Dat
-000247d0: 6522 7d2c 2069 6e70 6c61 6365 3d54 7275  e"}, inplace=Tru
-000247e0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-000247f0: 6461 7461 5b22 746f 7073 225d 203d 2028  data["tops"] = (
-00024800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00024810: 2020 6461 7461 5b22 4869 6768 225d 0d0a    data["High"]..
-00024820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024830: 2e69 6c6f 635b 0d0a 2020 2020 2020 2020  .iloc[..        
-00024840: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00024850: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00024860: 2020 2020 2020 2020 2020 2070 6b74 616c             pktal
-00024870: 6962 2e61 7267 7265 6c65 7874 7265 6d61  ib.argrelextrema
-00024880: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00024890: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000248a0: 702e 6172 7261 7928 6461 7461 5b22 4869  p.array(data["Hi
-000248b0: 6768 225d 292c 206e 702e 6772 6561 7465  gh"]), np.greate
-000248c0: 725f 6571 7561 6c2c 206f 7264 6572 3d77  r_equal, order=w
-000248d0: 696e 646f 770d 0a20 2020 2020 2020 2020  indow..         
-000248e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000248f0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-00024900: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00024910: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-00024920: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-00024930: 6865 6164 2834 290d 0a20 2020 2020 2020  head(4)..       
-00024940: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00024950: 2020 2020 6461 7461 5b22 626f 7473 225d      data["bots"]
-00024960: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00024970: 2020 2020 2020 6461 7461 5b22 4c6f 7722        data["Low"
-00024980: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00024990: 2020 202e 696c 6f63 5b0d 0a20 2020 2020     .iloc[..     
-000249a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000249b0: 6973 7428 0d0a 2020 2020 2020 2020 2020  ist(..          
-000249c0: 2020 2020 2020 2020 2020 2020 2020 706b                pk
-000249d0: 7461 6c69 622e 6172 6772 656c 6578 7472  talib.argrelextr
-000249e0: 656d 6128 0d0a 2020 2020 2020 2020 2020  ema(..          
-000249f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024a00: 2020 6e70 2e61 7272 6179 2864 6174 615b    np.array(data[
-00024a10: 224c 6f77 225d 292c 206e 702e 6c65 7373  "Low"]), np.less
-00024a20: 5f65 7175 616c 2c20 6f72 6465 723d 7769  _equal, order=wi
-00024a30: 6e64 6f77 0d0a 2020 2020 2020 2020 2020  ndow..          
-00024a40: 2020 2020 2020 2020 2020 2020 2020 295b                )[
-00024a50: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00024a60: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00024a70: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-00024a80: 2020 2020 2020 2020 2020 2020 2020 2e68                .h
-00024a90: 6561 6428 3429 0d0a 2020 2020 2020 2020  ead(4)..        
-00024aa0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00024ab0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-00024ac0: 696c 6c6e 6128 3029 0d0a 2020 2020 2020  illna(0)..      
-00024ad0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00024ae0: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
-00024af0: 662c 202d 6e70 2e69 6e66 5d2c 2030 290d  f, -np.inf], 0).
-00024b00: 0a20 2020 2020 2020 2020 2020 2074 6f70  .            top
-00024b10: 7320 3d20 6461 7461 5b64 6174 612e 746f  s = data[data.to
-00024b20: 7073 203e 2030 5d0d 0a20 2020 2020 2020  ps > 0]..       
-00024b30: 2020 2020 2023 2062 6f74 7320 3d20 6461       # bots = da
-00024b40: 7461 5b64 6174 612e 626f 7473 203e 2030  ta[data.bots > 0
-00024b50: 5d0d 0a20 2020 2020 2020 2020 2020 2068  ]..            h
-00024b60: 6967 6865 7374 546f 7020 3d20 726f 756e  ighestTop = roun
-00024b70: 6428 746f 7073 2e64 6573 6372 6962 6528  d(tops.describe(
-00024b80: 295b 2248 6967 6822 5d5b 226d 6178 225d  )["High"]["max"]
-00024b90: 2c20 3129 0d0a 2020 2020 2020 2020 2020  , 1)..          
-00024ba0: 2020 6669 6c74 6572 6564 546f 7073 203d    filteredTops =
-00024bb0: 2074 6f70 735b 0d0a 2020 2020 2020 2020   tops[..        
-00024bc0: 2020 2020 2020 2020 746f 7073 2e74 6f70          tops.top
-00024bd0: 7320 3e20 2868 6967 6865 7374 546f 7020  s > (highestTop 
-00024be0: 2d20 2868 6967 6865 7374 546f 7020 2a20  - (highestTop * 
-00024bf0: 7065 7263 656e 7461 6765 4672 6f6d 546f  percentageFromTo
-00024c00: 7029 290d 0a20 2020 2020 2020 2020 2020  p))..           
-00024c10: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
-00024c20: 6966 2066 696c 7465 7265 6454 6f70 732e  if filteredTops.
-00024c30: 6571 7561 6c73 2874 6f70 7329 3a20 2023  equals(tops):  #
-00024c40: 2054 6f70 7320 6172 6520 696e 2074 6865   Tops are in the
-00024c50: 2072 616e 6765 0d0a 2020 2020 2020 2020   range..        
-00024c60: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
-00024c70: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00024c80: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00024c90: 2072 616e 6765 286c 656e 2874 6f70 7329   range(len(tops)
-00024ca0: 202d 2031 293a 0d0a 2020 2020 2020 2020   - 1):..        
-00024cb0: 2020 2020 2020 2020 2020 2020 656e 6444              endD
-00024cc0: 6174 6520 3d20 746f 7073 2e69 6c6f 635b  ate = tops.iloc[
-00024cd0: 695d 5b22 4461 7465 225d 0d0a 2020 2020  i]["Date"]..    
-00024ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024cf0: 7374 6172 7444 6174 6520 3d20 746f 7073  startDate = tops
-00024d00: 2e69 6c6f 635b 6920 2b20 315d 5b22 4461  .iloc[i + 1]["Da
-00024d10: 7465 225d 0d0a 2020 2020 2020 2020 2020  te"]..          
-00024d20: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
-00024d30: 6e74 732e 6170 7065 6e64 280d 0a20 2020  nts.append(..   
-00024d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024d50: 2020 2020 2064 6174 615b 0d0a 2020 2020       data[..    
-00024d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024d70: 2020 2020 2020 2020 2864 6174 612e 4461          (data.Da
-00024d80: 7465 203e 3d20 7374 6172 7444 6174 6529  te >= startDate)
-00024d90: 2026 2028 6461 7461 2e44 6174 6520 3c3d   & (data.Date <=
-00024da0: 2065 6e64 4461 7465 290d 0a20 2020 2020   endDate)..     
-00024db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024dc0: 2020 205d 2e64 6573 6372 6962 6528 295b     ].describe()[
-00024dd0: 224c 6f77 225d 5b22 6d69 6e22 5d0d 0a20  "Low"]["min"].. 
-00024de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024df0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00024e00: 2020 2020 2020 6c6f 7750 6f69 6e74 734f        lowPointsO
-00024e10: 7267 203d 206c 6f77 506f 696e 7473 0d0a  rg = lowPoints..
-00024e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e30: 6c6f 7750 6f69 6e74 732e 736f 7274 2872  lowPoints.sort(r
-00024e40: 6576 6572 7365 3d54 7275 6529 0d0a 2020  everse=True)..  
-00024e50: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00024e60: 7750 6f69 6e74 7353 6f72 7465 6420 3d20  wPointsSorted = 
-00024e70: 6c6f 7750 6f69 6e74 730d 0a20 2020 2020  lowPoints..     
-00024e80: 2020 2020 2020 2020 2020 2069 6620 6461             if da
-00024e90: 7461 2e65 6d70 7479 206f 7220 6c65 6e28  ta.empty or len(
-00024ea0: 6c6f 7750 6f69 6e74 7329 203c 2031 3a0d  lowPoints) < 1:.
-00024eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024ec0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00024ed0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00024ee0: 2020 206c 7470 203d 2064 6174 612e 6865     ltp = data.he
-00024ef0: 6164 2831 295b 2243 6c6f 7365 225d 2e69  ad(1)["Close"].i
-00024f00: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
-00024f10: 2020 2020 2020 2020 6966 2028 0d0a 2020          if (..  
+00024630: 2020 2020 2061 6e64 2072 6563 656e 745b       and recent[
+00024640: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+00024650: 203e 2072 6563 656e 745b 2253 534d 4122   > recent["SSMA"
+00024660: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
+00024670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024680: 2020 2061 6e64 2072 6563 656e 745b 2243     and recent["C
+00024690: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
+000246a0: 2072 6563 656e 745b 224c 4d41 225d 2e69   recent["LMA"].i
+000246b0: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
+000246c0: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
+000246d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000246e0: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
+000246f0: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
+00024700: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
+00024710: 6e44 6963 742c 7361 7665 4469 6374 2c22  nDict,saveDict,"
+00024720: 4d41 2d53 6967 6e61 6c22 290d 0a20 2020  MA-Signal")..   
+00024730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024740: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00024750: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
+00024760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00024770: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00024780: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
+00024790: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
+000247a0: 6578 742e 4752 4545 4e20 2b20 2242 756c  ext.GREEN + "Bul
+000247b0: 6c69 7368 2220 2b20 636f 6c6f 7254 6578  lish" + colorTex
+000247c0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+000247d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000247e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000247f0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00024800: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00024810: 3d20 7361 7665 645b 315d 202b 2022 4275  = saved[1] + "Bu
+00024820: 6c6c 6973 6822 0d0a 2020 2020 2020 2020  llish"..        
+00024830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024840: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
+00024850: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00024860: 650d 0a0d 0a20 2020 2023 2056 616c 6964  e....    # Valid
+00024870: 6174 6520 5650 430d 0a20 2020 2064 6566  ate VPC..    def
+00024880: 2076 616c 6964 6174 6556 4350 280d 0a20   validateVCP(.. 
+00024890: 2020 2020 2020 2073 656c 662c 2064 662c         self, df,
+000248a0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+000248b0: 6544 6963 742c 2073 746f 636b 4e61 6d65  eDict, stockName
+000248c0: 3d4e 6f6e 652c 2077 696e 646f 773d 332c  =None, window=3,
+000248d0: 2070 6572 6365 6e74 6167 6546 726f 6d54   percentageFromT
+000248e0: 6f70 3d33 0d0a 2020 2020 293a 0d0a 2020  op=3..    ):..  
+000248f0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+00024900: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+00024910: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+00024920: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+00024930: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00024940: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
+00024950: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00024960: 2020 2020 7065 7263 656e 7461 6765 4672      percentageFr
+00024970: 6f6d 546f 7020 2f3d 2031 3030 0d0a 2020  omTop /= 100..  
+00024980: 2020 2020 2020 2020 2020 6461 7461 2e72            data.r
+00024990: 6573 6574 5f69 6e64 6578 2869 6e70 6c61  eset_index(inpla
+000249a0: 6365 3d54 7275 6529 0d0a 2020 2020 2020  ce=True)..      
+000249b0: 2020 2020 2020 6461 7461 2e72 656e 616d        data.renam
+000249c0: 6528 636f 6c75 6d6e 733d 7b22 696e 6465  e(columns={"inde
+000249d0: 7822 3a20 2244 6174 6522 7d2c 2069 6e70  x": "Date"}, inp
+000249e0: 6c61 6365 3d54 7275 6529 0d0a 2020 2020  lace=True)..    
+000249f0: 2020 2020 2020 2020 6461 7461 5b22 746f          data["to
+00024a00: 7073 225d 203d 2028 0d0a 2020 2020 2020  ps"] = (..      
+00024a10: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
+00024a20: 4869 6768 225d 0d0a 2020 2020 2020 2020  High"]..        
+00024a30: 2020 2020 2020 2020 2e69 6c6f 635b 0d0a          .iloc[..
+00024a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024a50: 2020 2020 6c69 7374 280d 0a20 2020 2020      list(..     
+00024a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024a70: 2020 2070 6b74 616c 6962 2e61 7267 7265     pktalib.argre
+00024a80: 6c65 7874 7265 6d61 280d 0a20 2020 2020  lextrema(..     
+00024a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024aa0: 2020 2020 2020 206e 702e 6172 7261 7928         np.array(
+00024ab0: 6461 7461 5b22 4869 6768 225d 292c 206e  data["High"]), n
+00024ac0: 702e 6772 6561 7465 725f 6571 7561 6c2c  p.greater_equal,
+00024ad0: 206f 7264 6572 3d77 696e 646f 770d 0a20   order=window.. 
+00024ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024af0: 2020 2020 2020 2029 5b30 5d0d 0a20 2020         )[0]..   
+00024b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024b10: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00024b20: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
+00024b30: 2020 2020 2020 202e 6865 6164 2834 290d         .head(4).
+00024b40: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00024b50: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00024b60: 5b22 626f 7473 225d 203d 2028 0d0a 2020  ["bots"] = (..  
+00024b70: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00024b80: 7461 5b22 4c6f 7722 5d0d 0a20 2020 2020  ta["Low"]..     
+00024b90: 2020 2020 2020 2020 2020 202e 696c 6f63             .iloc
+00024ba0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00024bb0: 2020 2020 2020 206c 6973 7428 0d0a 2020         list(..  
+00024bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024bd0: 2020 2020 2020 706b 7461 6c69 622e 6172        pktalib.ar
+00024be0: 6772 656c 6578 7472 656d 6128 0d0a 2020  grelextrema(..  
+00024bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024c00: 2020 2020 2020 2020 2020 6e70 2e61 7272            np.arr
+00024c10: 6179 2864 6174 615b 224c 6f77 225d 292c  ay(data["Low"]),
+00024c20: 206e 702e 6c65 7373 5f65 7175 616c 2c20   np.less_equal, 
+00024c30: 6f72 6465 723d 7769 6e64 6f77 0d0a 2020  order=window..  
+00024c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024c50: 2020 2020 2020 295b 305d 0d0a 2020 2020        )[0]..    
+00024c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024c70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00024c80: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
+00024c90: 2020 2020 2020 2e68 6561 6428 3429 0d0a        .head(4)..
+00024ca0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00024cb0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00024cc0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+00024cd0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00024ce0: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+00024cf0: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
+00024d00: 6e66 5d2c 2030 290d 0a20 2020 2020 2020  nf], 0)..       
+00024d10: 2020 2020 2074 6f70 7320 3d20 6461 7461       tops = data
+00024d20: 5b64 6174 612e 746f 7073 203e 2030 5d0d  [data.tops > 0].
+00024d30: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
+00024d40: 6f74 7320 3d20 6461 7461 5b64 6174 612e  ots = data[data.
+00024d50: 626f 7473 203e 2030 5d0d 0a20 2020 2020  bots > 0]..     
+00024d60: 2020 2020 2020 2068 6967 6865 7374 546f         highestTo
+00024d70: 7020 3d20 726f 756e 6428 746f 7073 2e64  p = round(tops.d
+00024d80: 6573 6372 6962 6528 295b 2248 6967 6822  escribe()["High"
+00024d90: 5d5b 226d 6178 225d 2c20 3129 0d0a 2020  ]["max"], 1)..  
+00024da0: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+00024db0: 6564 546f 7073 203d 2074 6f70 735b 0d0a  edTops = tops[..
+00024dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024dd0: 746f 7073 2e74 6f70 7320 3e20 2868 6967  tops.tops > (hig
+00024de0: 6865 7374 546f 7020 2d20 2868 6967 6865  hestTop - (highe
+00024df0: 7374 546f 7020 2a20 7065 7263 656e 7461  stTop * percenta
+00024e00: 6765 4672 6f6d 546f 7029 290d 0a20 2020  geFromTop))..   
+00024e10: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00024e20: 2020 2020 2020 2020 6966 2066 696c 7465          if filte
+00024e30: 7265 6454 6f70 732e 6571 7561 6c73 2874  redTops.equals(t
+00024e40: 6f70 7329 3a20 2023 2054 6f70 7320 6172  ops):  # Tops ar
+00024e50: 6520 696e 2074 6865 2072 616e 6765 0d0a  e in the range..
+00024e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e70: 6c6f 7750 6f69 6e74 7320 3d20 5b5d 0d0a  lowPoints = []..
+00024e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e90: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00024ea0: 656e 2874 6f70 7329 202d 2031 293a 0d0a  en(tops) - 1):..
+00024eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024ec0: 2020 2020 656e 6444 6174 6520 3d20 746f      endDate = to
+00024ed0: 7073 2e69 6c6f 635b 695d 5b22 4461 7465  ps.iloc[i]["Date
+00024ee0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00024ef0: 2020 2020 2020 2020 7374 6172 7444 6174          startDat
+00024f00: 6520 3d20 746f 7073 2e69 6c6f 635b 6920  e = tops.iloc[i 
+00024f10: 2b20 315d 5b22 4461 7465 225d 0d0a 2020  + 1]["Date"]..  
 00024f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f30: 2020 6c6f 7750 6f69 6e74 734f 7267 203d    lowPointsOrg =
-00024f40: 3d20 6c6f 7750 6f69 6e74 7353 6f72 7465  = lowPointsSorte
-00024f50: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
-00024f60: 2020 2020 2020 2061 6e64 206c 7470 203c         and ltp <
-00024f70: 2068 6967 6865 7374 546f 700d 0a20 2020   highestTop..   
-00024f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f90: 2061 6e64 206c 7470 203e 206c 6f77 506f   and ltp > lowPo
-00024fa0: 696e 7473 5b30 5d0d 0a20 2020 2020 2020  ints[0]..       
-00024fb0: 2020 2020 2020 2020 2029 3a0d 0a20 2020           ):..   
-00024fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fd0: 2073 6176 6564 203d 2073 656c 662e 6669   saved = self.fi
-00024fe0: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
-00024ff0: 6c75 6528 7363 7265 656e 4469 6374 2c20  lue(screenDict, 
-00025000: 7361 7665 4469 6374 2c20 2250 6174 7465  saveDict, "Patte
-00025010: 726e 2229 0d0a 2020 2020 2020 2020 2020  rn")..          
-00025020: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-00025030: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-00025040: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-00025050: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00025060: 6564 5b30 5d20 0d0a 2020 2020 2020 2020  ed[0] ..        
-00025070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025080: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
-00025090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000250a0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-000250b0: 7254 6578 742e 4752 4545 4e0d 0a20 2020  rText.GREEN..   
-000250c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000250d0: 2020 2020 202b 2066 2256 4350 2028 424f       + f"VCP (BO
-000250e0: 3a20 7b68 6967 6865 7374 546f 707d 2922  : {highestTop})"
-000250f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025100: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-00025110: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-00025120: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00025130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025140: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-00025150: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
-00025160: 645b 315d 202b 2066 2256 4350 2028 424f  d[1] + f"VCP (BO
-00025170: 3a20 7b68 6967 6865 7374 546f 707d 2922  : {highestTop})"
-00025180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025190: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000251a0: 650d 0a20 2020 2020 2020 2065 7863 6570  e..        excep
-000251b0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-000251c0: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-000251d0: 636f 7665 720d 0a20 2020 2020 2020 2020  cover..         
-000251e0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
-000251f0: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
-00025200: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
-00025210: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00025220: 616c 7365 0d0a 0d0a 2020 2020 2320 5661  alse....    # Va
-00025230: 6c69 6461 7465 2069 6620 766f 6c75 6d65  lidate if volume
-00025240: 206f 6620 6c61 7374 2064 6179 2069 7320   of last day is 
-00025250: 6869 6768 6572 2074 6861 6e20 6176 670d  higher than avg.
-00025260: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00025270: 6556 6f6c 756d 6528 0d0a 2020 2020 2020  eVolume(..      
-00025280: 2020 7365 6c66 2c20 6466 2c20 7363 7265    self, df, scre
-00025290: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-000252a0: 2c20 766f 6c75 6d65 5261 7469 6f3d 322e  , volumeRatio=2.
-000252b0: 352c 206d 696e 566f 6c75 6d65 3d31 3030  5, minVolume=100
-000252c0: 0d0a 2020 2020 293a 0d0a 2020 2020 2020  ..    ):..      
-000252d0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-000252e0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-000252f0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00025300: 7475 726e 2046 616c 7365 2c20 4661 6c73  turn False, Fals
-00025310: 650d 0a20 2020 2020 2020 2064 6174 6120  e..        data 
-00025320: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
-00025330: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00025340: 2e66 696c 6c6e 6128 3029 0d0a 2020 2020  .fillna(0)..    
-00025350: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-00025360: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
-00025370: 202d 6e70 2e69 6e66 5d2c 2030 290d 0a20   -np.inf], 0).. 
-00025380: 2020 2020 2020 2072 6563 656e 7420 3d20         recent = 
-00025390: 6461 7461 2e68 6561 6428 3129 0d0a 2020  data.head(1)..  
-000253a0: 2020 2020 2020 2320 4569 7468 6572 2074        # Either t
-000253b0: 6865 2072 6f6c 6c69 6e67 2076 6f6c 756d  he rolling volum
-000253c0: 6520 6f66 2070 6173 7420 3230 2073 6573  e of past 20 ses
-000253d0: 7369 6f6e 7320 6f72 2074 6f64 6179 2773  sions or today's
-000253e0: 2076 6f6c 756d 6520 7368 6f75 6c64 2062   volume should b
-000253f0: 6520 3e20 6d69 6e20 766f 6c75 6d65 0d0a  e > min volume..
-00025400: 2020 2020 2020 2020 6861 734d 696e 696d          hasMinim
-00025410: 756d 566f 6c75 6d65 203d 2028 0d0a 2020  umVolume = (..  
-00025420: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-00025430: 5b22 566f 6c4d 4122 5d2e 696c 6f63 5b30  ["VolMA"].iloc[0
-00025440: 5d20 3e3d 206d 696e 566f 6c75 6d65 0d0a  ] >= minVolume..
-00025450: 2020 2020 2020 2020 2020 2020 6f72 2072              or r
-00025460: 6563 656e 745b 2256 6f6c 756d 6522 5d2e  ecent["Volume"].
-00025470: 696c 6f63 5b30 5d20 3e3d 206d 696e 566f  iloc[0] >= minVo
-00025480: 6c75 6d65 0d0a 2020 2020 2020 2020 290d  lume..        ).
-00025490: 0a20 2020 2020 2020 2069 6620 7265 6365  .        if rece
-000254a0: 6e74 5b22 566f 6c4d 4122 5d2e 696c 6f63  nt["VolMA"].iloc
-000254b0: 5b30 5d20 3d3d 2030 3a20 2023 2048 616e  [0] == 0:  # Han
-000254c0: 646c 6573 2044 6976 6964 6520 6279 2030  dles Divide by 0
-000254d0: 2077 6172 6e69 6e67 0d0a 2020 2020 2020   warning..      
-000254e0: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-000254f0: 566f 6c75 6d65 225d 203d 2030 2020 2320  Volume"] = 0  # 
-00025500: 2255 6e6b 6e6f 776e 220d 0a20 2020 2020  "Unknown"..     
-00025510: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00025520: 745b 2256 6f6c 756d 6522 5d20 3d20 300d  t["Volume"] = 0.
-00025530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00025540: 7572 6e20 4661 6c73 652c 2068 6173 4d69  urn False, hasMi
-00025550: 6e69 6d75 6d56 6f6c 756d 650d 0a20 2020  nimumVolume..   
-00025560: 2020 2020 2072 6174 696f 203d 2072 6f75       ratio = rou
-00025570: 6e64 2872 6563 656e 745b 2256 6f6c 756d  nd(recent["Volum
-00025580: 6522 5d2e 696c 6f63 5b30 5d20 2f20 7265  e"].iloc[0] / re
-00025590: 6365 6e74 5b22 566f 6c4d 4122 5d2e 696c  cent["VolMA"].il
-000255a0: 6f63 5b30 5d2c 2032 290d 0a20 2020 2020  oc[0], 2)..     
-000255b0: 2020 2073 6176 6544 6963 745b 2256 6f6c     saveDict["Vol
-000255c0: 756d 6522 5d20 3d20 7261 7469 6f0d 0a20  ume"] = ratio.. 
-000255d0: 2020 2020 2020 2069 6620 7261 7469 6f20         if ratio 
-000255e0: 3e3d 2076 6f6c 756d 6552 6174 696f 2061  >= volumeRatio a
-000255f0: 6e64 2072 6174 696f 2021 3d20 6e70 2e6e  nd ratio != np.n
-00025600: 616e 2061 6e64 2028 6e6f 7420 6d61 7468  an and (not math
-00025610: 2e69 7369 6e66 2872 6174 696f 2929 3a0d  .isinf(ratio)):.
-00025620: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-00025630: 6565 6e44 6963 745b 2256 6f6c 756d 6522  eenDict["Volume"
-00025640: 5d20 3d20 7261 7469 6f0d 0a20 2020 2020  ] = ratio..     
-00025650: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00025660: 7565 2c20 6861 734d 696e 696d 756d 566f  ue, hasMinimumVo
-00025670: 6c75 6d65 0d0a 2020 2020 2020 2020 7363  lume..        sc
-00025680: 7265 656e 4469 6374 5b22 566f 6c75 6d65  reenDict["Volume
-00025690: 225d 203d 2072 6174 696f 0d0a 2020 2020  "] = ratio..    
-000256a0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000256b0: 2c20 6861 734d 696e 696d 756d 566f 6c75  , hasMinimumVolu
-000256c0: 6d65 0d0a 0d0a 2020 2020 2320 4669 6e64  me....    # Find
-000256d0: 2069 6620 7374 6f63 6b20 6973 2076 616c   if stock is val
-000256e0: 6964 6174 696e 6720 766f 6c75 6d65 2073  idating volume s
-000256f0: 7072 6561 6420 616e 616c 7973 6973 0d0a  pread analysis..
-00025700: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00025710: 566f 6c75 6d65 5370 7265 6164 416e 616c  VolumeSpreadAnal
-00025720: 7973 6973 2873 656c 662c 2064 662c 2073  ysis(self, df, s
-00025730: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00025740: 6963 7429 3a0d 0a20 2020 2020 2020 2074  ict):..        t
-00025750: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00025760: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-00025770: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0d  r len(df) == 0:.
-00025780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025790: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-000257a0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-000257b0: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
-000257c0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-000257d0: 6461 7461 2e68 6561 6428 3229 0d0a 2020  data.head(2)..  
-000257e0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-000257f0: 2864 6174 6129 203c 2032 3a0d 0a20 2020  (data) < 2:..   
-00025800: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00025810: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
-00025820: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00025830: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-00025840: 6865 636b 2066 6f72 2070 7265 7669 6f75  heck for previou
-00025850: 7320 5245 4420 6361 6e64 6c65 730d 0a20  s RED candles.. 
-00025860: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00025870: 2043 7572 7265 6e74 2063 616e 646c 6520   Current candle 
-00025880: 3d20 3074 682c 2050 7265 7669 6f75 7320  = 0th, Previous 
-00025890: 4361 6e64 6c65 203d 2031 7374 2066 6f72  Candle = 1st for
-000258a0: 2066 6f6c 6c6f 7769 6e67 206c 6f67 6963   following logic
-000258b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000258c0: 2020 6966 2064 6174 612e 696c 6f63 5b31    if data.iloc[1
-000258d0: 5d5b 224f 7065 6e22 5d20 3e3d 2064 6174  ]["Open"] >= dat
-000258e0: 612e 696c 6f63 5b31 5d5b 2243 6c6f 7365  a.iloc[1]["Close
-000258f0: 225d 3a0d 0a20 2020 2020 2020 2020 2020  "]:..           
-00025900: 2020 2020 2020 2020 2073 7072 6561 6431           spread1
-00025910: 203d 2061 6273 2864 6174 612e 696c 6f63   = abs(data.iloc
-00025920: 5b31 5d5b 224f 7065 6e22 5d20 2d20 6461  [1]["Open"] - da
-00025930: 7461 2e69 6c6f 635b 315d 5b22 436c 6f73  ta.iloc[1]["Clos
-00025940: 6522 5d29 0d0a 2020 2020 2020 2020 2020  e"])..          
-00025950: 2020 2020 2020 2020 2020 7370 7265 6164            spread
-00025960: 3020 3d20 6162 7328 6461 7461 2e69 6c6f  0 = abs(data.ilo
-00025970: 635b 305d 5b22 4f70 656e 225d 202d 2064  c[0]["Open"] - d
-00025980: 6174 612e 696c 6f63 5b30 5d5b 2243 6c6f  ata.iloc[0]["Clo
-00025990: 7365 225d 290d 0a20 2020 2020 2020 2020  se"])..         
-000259a0: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
-000259b0: 5f77 6963 6b5f 7370 7265 6164 3020 3d20  _wick_spread0 = 
-000259c0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000259d0: 2020 2020 2020 2020 2020 206d 6178 2864             max(d
-000259e0: 6174 612e 696c 6f63 5b30 5d5b 224f 7065  ata.iloc[0]["Ope
-000259f0: 6e22 5d2c 2064 6174 612e 696c 6f63 5b30  n"], data.iloc[0
-00025a00: 5d5b 2243 6c6f 7365 225d 290d 0a20 2020  ]["Close"])..   
-00025a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a20: 2020 2020 202d 2064 6174 612e 696c 6f63       - data.iloc
-00025a30: 5b30 5d5b 224c 6f77 225d 0d0a 2020 2020  [0]["Low"]..    
-00025a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00025a60: 2020 2020 2020 2076 6f6c 3120 3d20 6461         vol1 = da
-00025a70: 7461 2e69 6c6f 635b 315d 5b22 566f 6c75  ta.iloc[1]["Volu
-00025a80: 6d65 225d 0d0a 2020 2020 2020 2020 2020  me"]..          
-00025a90: 2020 2020 2020 2020 2020 766f 6c30 203d            vol0 =
-00025aa0: 2064 6174 612e 696c 6f63 5b30 5d5b 2256   data.iloc[0]["V
-00025ab0: 6f6c 756d 6522 5d0d 0a20 2020 2020 2020  olume"]..       
-00025ac0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00025ad0: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
-00025ae0: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
-00025af0: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
-00025b00: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
-00025b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025b20: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
-00025b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b40: 2020 2020 7370 7265 6164 3020 3e20 7370      spread0 > sp
-00025b50: 7265 6164 310d 0a20 2020 2020 2020 2020  read1..         
-00025b60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00025b70: 6e64 2076 6f6c 3020 3c20 766f 6c31 0d0a  nd vol0 < vol1..
-00025b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b90: 2020 2020 2020 2020 616e 6420 6461 7461          and data
-00025ba0: 2e69 6c6f 635b 305d 5b22 566f 6c75 6d65  .iloc[0]["Volume
-00025bb0: 225d 203c 2064 6174 612e 696c 6f63 5b30  "] < data.iloc[0
-00025bc0: 5d5b 2256 6f6c 4d41 225d 0d0a 2020 2020  ]["VolMA"]..    
+00024f30: 2020 6c6f 7750 6f69 6e74 732e 6170 7065    lowPoints.appe
+00024f40: 6e64 280d 0a20 2020 2020 2020 2020 2020  nd(..           
+00024f50: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00024f60: 615b 0d0a 2020 2020 2020 2020 2020 2020  a[..            
+00024f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024f80: 2864 6174 612e 4461 7465 203e 3d20 7374  (data.Date >= st
+00024f90: 6172 7444 6174 6529 2026 2028 6461 7461  artDate) & (data
+00024fa0: 2e44 6174 6520 3c3d 2065 6e64 4461 7465  .Date <= endDate
+00024fb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00024fc0: 2020 2020 2020 2020 2020 205d 2e64 6573             ].des
+00024fd0: 6372 6962 6528 295b 224c 6f77 225d 5b22  cribe()["Low"]["
+00024fe0: 6d69 6e22 5d0d 0a20 2020 2020 2020 2020  min"]..         
+00024ff0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00025000: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00025010: 7750 6f69 6e74 734f 7267 203d 206c 6f77  wPointsOrg = low
+00025020: 506f 696e 7473 0d0a 2020 2020 2020 2020  Points..        
+00025030: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
+00025040: 732e 736f 7274 2872 6576 6572 7365 3d54  s.sort(reverse=T
+00025050: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+00025060: 2020 2020 2020 6c6f 7750 6f69 6e74 7353        lowPointsS
+00025070: 6f72 7465 6420 3d20 6c6f 7750 6f69 6e74  orted = lowPoint
+00025080: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00025090: 2020 2069 6620 6461 7461 2e65 6d70 7479     if data.empty
+000250a0: 206f 7220 6c65 6e28 6c6f 7750 6f69 6e74   or len(lowPoint
+000250b0: 7329 203c 2031 3a0d 0a20 2020 2020 2020  s) < 1:..       
+000250c0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000250d0: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+000250e0: 2020 2020 2020 2020 2020 206c 7470 203d             ltp =
+000250f0: 2064 6174 612e 6865 6164 2831 295b 2243   data.head(1)["C
+00025100: 6c6f 7365 225d 2e69 6c6f 635b 305d 0d0a  lose"].iloc[0]..
+00025110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025120: 6966 2028 0d0a 2020 2020 2020 2020 2020  if (..          
+00025130: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
+00025140: 6e74 734f 7267 203d 3d20 6c6f 7750 6f69  ntsOrg == lowPoi
+00025150: 6e74 7353 6f72 7465 640d 0a20 2020 2020  ntsSorted..     
+00025160: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00025170: 6e64 206c 7470 203c 2068 6967 6865 7374  nd ltp < highest
+00025180: 546f 700d 0a20 2020 2020 2020 2020 2020  Top..           
+00025190: 2020 2020 2020 2020 2061 6e64 206c 7470           and ltp
+000251a0: 203e 206c 6f77 506f 696e 7473 5b30 5d0d   > lowPoints[0].
+000251b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000251c0: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+000251d0: 2020 2020 2020 2020 2073 6176 6564 203d           saved =
+000251e0: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
+000251f0: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
+00025200: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+00025210: 2c20 2250 6174 7465 726e 2229 0d0a 2020  , "Pattern")..  
+00025220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025230: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
+00025240: 7474 6572 6e22 5d20 3d20 280d 0a20 2020  ttern"] = (..   
+00025250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025260: 2020 2020 2073 6176 6564 5b30 5d20 0d0a       saved[0] ..
+00025270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025280: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00025290: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
+000252a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000252b0: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
+000252c0: 4545 4e0d 0a20 2020 2020 2020 2020 2020  EEN..           
+000252d0: 2020 2020 2020 2020 2020 2020 202b 2066               + f
+000252e0: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
+000252f0: 7374 546f 707d 2922 0d0a 2020 2020 2020  stTop})"..      
+00025300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025310: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+00025320: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+00025330: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00025340: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00025350: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
+00025360: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+00025370: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
+00025380: 7374 546f 707d 2922 0d0a 2020 2020 2020  stTop})"..      
+00025390: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000253a0: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
+000253b0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+000253c0: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
+000253d0: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
+000253e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000253f0: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
+00025400: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
+00025410: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00025420: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
+00025430: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
+00025440: 6620 766f 6c75 6d65 206f 6620 6c61 7374  f volume of last
+00025450: 2064 6179 2069 7320 6869 6768 6572 2074   day is higher t
+00025460: 6861 6e20 6176 670d 0a20 2020 2064 6566  han avg..    def
+00025470: 2076 616c 6964 6174 6556 6f6c 756d 6528   validateVolume(
+00025480: 0d0a 2020 2020 2020 2020 7365 6c66 2c20  ..        self, 
+00025490: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
+000254a0: 7361 7665 4469 6374 2c20 766f 6c75 6d65  saveDict, volume
+000254b0: 5261 7469 6f3d 322e 352c 206d 696e 566f  Ratio=2.5, minVo
+000254c0: 6c75 6d65 3d31 3030 0d0a 2020 2020 293a  lume=100..    ):
+000254d0: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+000254e0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+000254f0: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+00025500: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00025510: 7365 2c20 4661 6c73 650d 0a20 2020 2020  se, False..     
+00025520: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+00025530: 7928 290d 0a20 2020 2020 2020 2064 6174  y()..        dat
+00025540: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
+00025550: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
+00025560: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+00025570: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
+00025580: 5d2c 2030 290d 0a20 2020 2020 2020 2072  ], 0)..        r
+00025590: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
+000255a0: 6428 3129 0d0a 2020 2020 2020 2020 2320  d(1)..        # 
+000255b0: 4569 7468 6572 2074 6865 2072 6f6c 6c69  Either the rolli
+000255c0: 6e67 2076 6f6c 756d 6520 6f66 2070 6173  ng volume of pas
+000255d0: 7420 3230 2073 6573 7369 6f6e 7320 6f72  t 20 sessions or
+000255e0: 2074 6f64 6179 2773 2076 6f6c 756d 6520   today's volume 
+000255f0: 7368 6f75 6c64 2062 6520 3e20 6d69 6e20  should be > min 
+00025600: 766f 6c75 6d65 0d0a 2020 2020 2020 2020  volume..        
+00025610: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
+00025620: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00025630: 2020 7265 6365 6e74 5b22 566f 6c4d 4122    recent["VolMA"
+00025640: 5d2e 696c 6f63 5b30 5d20 3e3d 206d 696e  ].iloc[0] >= min
+00025650: 566f 6c75 6d65 0d0a 2020 2020 2020 2020  Volume..        
+00025660: 2020 2020 6f72 2072 6563 656e 745b 2256      or recent["V
+00025670: 6f6c 756d 6522 5d2e 696c 6f63 5b30 5d20  olume"].iloc[0] 
+00025680: 3e3d 206d 696e 566f 6c75 6d65 0d0a 2020  >= minVolume..  
+00025690: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000256a0: 2069 6620 7265 6365 6e74 5b22 566f 6c4d   if recent["VolM
+000256b0: 4122 5d2e 696c 6f63 5b30 5d20 3d3d 2030  A"].iloc[0] == 0
+000256c0: 3a20 2023 2048 616e 646c 6573 2044 6976  :  # Handles Div
+000256d0: 6964 6520 6279 2030 2077 6172 6e69 6e67  ide by 0 warning
+000256e0: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
+000256f0: 7665 4469 6374 5b22 566f 6c75 6d65 225d  veDict["Volume"]
+00025700: 203d 2030 2020 2320 2255 6e6b 6e6f 776e   = 0  # "Unknown
+00025710: 220d 0a20 2020 2020 2020 2020 2020 2073  "..            s
+00025720: 6372 6565 6e44 6963 745b 2256 6f6c 756d  creenDict["Volum
+00025730: 6522 5d20 3d20 300d 0a20 2020 2020 2020  e"] = 0..       
+00025740: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00025750: 652c 2068 6173 4d69 6e69 6d75 6d56 6f6c  e, hasMinimumVol
+00025760: 756d 650d 0a20 2020 2020 2020 2072 6174  ume..        rat
+00025770: 696f 203d 2072 6f75 6e64 2872 6563 656e  io = round(recen
+00025780: 745b 2256 6f6c 756d 6522 5d2e 696c 6f63  t["Volume"].iloc
+00025790: 5b30 5d20 2f20 7265 6365 6e74 5b22 566f  [0] / recent["Vo
+000257a0: 6c4d 4122 5d2e 696c 6f63 5b30 5d2c 2032  lMA"].iloc[0], 2
+000257b0: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
+000257c0: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
+000257d0: 7261 7469 6f0d 0a20 2020 2020 2020 2069  ratio..        i
+000257e0: 6620 7261 7469 6f20 3e3d 2076 6f6c 756d  f ratio >= volum
+000257f0: 6552 6174 696f 2061 6e64 2072 6174 696f  eRatio and ratio
+00025800: 2021 3d20 6e70 2e6e 616e 2061 6e64 2028   != np.nan and (
+00025810: 6e6f 7420 6d61 7468 2e69 7369 6e66 2872  not math.isinf(r
+00025820: 6174 696f 2929 3a0d 0a20 2020 2020 2020  atio)):..       
+00025830: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00025840: 2256 6f6c 756d 6522 5d20 3d20 7261 7469  "Volume"] = rati
+00025850: 6f0d 0a20 2020 2020 2020 2020 2020 2072  o..            r
+00025860: 6574 7572 6e20 5472 7565 2c20 6861 734d  eturn True, hasM
+00025870: 696e 696d 756d 566f 6c75 6d65 0d0a 2020  inimumVolume..  
+00025880: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00025890: 5b22 566f 6c75 6d65 225d 203d 2072 6174  ["Volume"] = rat
+000258a0: 696f 0d0a 2020 2020 2020 2020 7265 7475  io..        retu
+000258b0: 726e 2046 616c 7365 2c20 6861 734d 696e  rn False, hasMin
+000258c0: 696d 756d 566f 6c75 6d65 0d0a 0d0a 2020  imumVolume....  
+000258d0: 2020 2320 4669 6e64 2069 6620 7374 6f63    # Find if stoc
+000258e0: 6b20 6973 2076 616c 6964 6174 696e 6720  k is validating 
+000258f0: 766f 6c75 6d65 2073 7072 6561 6420 616e  volume spread an
+00025900: 616c 7973 6973 0d0a 2020 2020 6465 6620  alysis..    def 
+00025910: 7661 6c69 6461 7465 566f 6c75 6d65 5370  validateVolumeSp
+00025920: 7265 6164 416e 616c 7973 6973 2873 656c  readAnalysis(sel
+00025930: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+00025940: 742c 2073 6176 6544 6963 7429 3a0d 0a20  t, saveDict):.. 
+00025950: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00025960: 2020 2020 2020 2020 2069 6620 6466 2069           if df i
+00025970: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+00025980: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
+00025990: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000259a0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+000259b0: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+000259c0: 7928 290d 0a20 2020 2020 2020 2020 2020  y()..           
+000259d0: 2064 6174 6120 3d20 6461 7461 2e68 6561   data = data.hea
+000259e0: 6428 3229 0d0a 2020 2020 2020 2020 2020  d(2)..          
+000259f0: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
+00025a00: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
+00025a10: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00025a20: 650d 0a20 2020 2020 2020 2020 2020 2074  e..            t
+00025a30: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00025a40: 2020 2020 2023 2043 6865 636b 2066 6f72       # Check for
+00025a50: 2070 7265 7669 6f75 7320 5245 4420 6361   previous RED ca
+00025a60: 6e64 6c65 730d 0a20 2020 2020 2020 2020  ndles..         
+00025a70: 2020 2020 2020 2023 2043 7572 7265 6e74         # Current
+00025a80: 2063 616e 646c 6520 3d20 3074 682c 2050   candle = 0th, P
+00025a90: 7265 7669 6f75 7320 4361 6e64 6c65 203d  revious Candle =
+00025aa0: 2031 7374 2066 6f72 2066 6f6c 6c6f 7769   1st for followi
+00025ab0: 6e67 206c 6f67 6963 0d0a 2020 2020 2020  ng logic..      
+00025ac0: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
+00025ad0: 612e 696c 6f63 5b31 5d5b 224f 7065 6e22  a.iloc[1]["Open"
+00025ae0: 5d20 3e3d 2064 6174 612e 696c 6f63 5b31  ] >= data.iloc[1
+00025af0: 5d5b 2243 6c6f 7365 225d 3a0d 0a20 2020  ]["Close"]:..   
+00025b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b10: 2073 7072 6561 6431 203d 2061 6273 2864   spread1 = abs(d
+00025b20: 6174 612e 696c 6f63 5b31 5d5b 224f 7065  ata.iloc[1]["Ope
+00025b30: 6e22 5d20 2d20 6461 7461 2e69 6c6f 635b  n"] - data.iloc[
+00025b40: 315d 5b22 436c 6f73 6522 5d29 0d0a 2020  1]["Close"])..  
+00025b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b60: 2020 7370 7265 6164 3020 3d20 6162 7328    spread0 = abs(
+00025b70: 6461 7461 2e69 6c6f 635b 305d 5b22 4f70  data.iloc[0]["Op
+00025b80: 656e 225d 202d 2064 6174 612e 696c 6f63  en"] - data.iloc
+00025b90: 5b30 5d5b 2243 6c6f 7365 225d 290d 0a20  [0]["Close"]).. 
+00025ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025bb0: 2020 206c 6f77 6572 5f77 6963 6b5f 7370     lower_wick_sp
+00025bc0: 7265 6164 3020 3d20 280d 0a20 2020 2020  read0 = (..     
 00025bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025be0: 2020 2020 616e 6420 6461 7461 2e69 6c6f      and data.ilo
-00025bf0: 635b 305d 5b22 436c 6f73 6522 5d20 3c3d  c[0]["Close"] <=
-00025c00: 2064 6174 612e 696c 6f63 5b31 5d5b 224f   data.iloc[1]["O
-00025c10: 7065 6e22 5d0d 0a20 2020 2020 2020 2020  pen"]..         
-00025c20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00025c30: 6e64 2073 7072 6561 6430 203c 206c 6f77  nd spread0 < low
-00025c40: 6572 5f77 6963 6b5f 7370 7265 6164 300d  er_wick_spread0.
-00025c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025c60: 2020 2020 2020 2020 2061 6e64 2064 6174           and dat
-00025c70: 612e 696c 6f63 5b30 5d5b 2256 6f6c 756d  a.iloc[0]["Volum
-00025c80: 6522 5d20 3c3d 2069 6e74 2864 6174 612e  e"] <= int(data.
-00025c90: 696c 6f63 5b31 5d5b 2256 6f6c 756d 6522  iloc[1]["Volume"
-00025ca0: 5d20 2a20 302e 3735 290d 0a20 2020 2020  ] * 0.75)..     
-00025cb0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00025cc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00025cd0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00025ce0: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-00025cf0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00025d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d10: 2020 7361 7665 645b 305d 200d 0a20 2020    saved[0] ..   
-00025d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d30: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00025d40: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
-00025d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d60: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00025d70: 7874 2e47 5245 454e 0d0a 2020 2020 2020  xt.GREEN..      
-00025d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d90: 2020 2020 2020 2b20 2253 7570 706c 7920        + "Supply 
-00025da0: 4472 6f75 6768 7422 0d0a 2020 2020 2020  Drought"..      
-00025db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025dc0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-00025dd0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-00025de0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00025df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025e00: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00025e10: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
-00025e20: 7361 7665 645b 315d 202b 2022 5375 7070  saved[1] + "Supp
-00025e30: 6c79 2044 726f 7567 6874 220d 0a20 2020  ly Drought"..   
-00025e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e50: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00025e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025e70: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
-00025e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e90: 2020 2020 7370 7265 6164 3020 3c20 7370      spread0 < sp
-00025ea0: 7265 6164 310d 0a20 2020 2020 2020 2020  read1..         
-00025eb0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00025ec0: 6e64 2076 6f6c 3020 3e20 766f 6c31 0d0a  nd vol0 > vol1..
+00025be0: 2020 206d 6178 2864 6174 612e 696c 6f63     max(data.iloc
+00025bf0: 5b30 5d5b 224f 7065 6e22 5d2c 2064 6174  [0]["Open"], dat
+00025c00: 612e 696c 6f63 5b30 5d5b 2243 6c6f 7365  a.iloc[0]["Close
+00025c10: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
+00025c20: 2020 2020 2020 2020 2020 2020 202d 2064               - d
+00025c30: 6174 612e 696c 6f63 5b30 5d5b 224c 6f77  ata.iloc[0]["Low
+00025c40: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00025c50: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00025c60: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00025c70: 6f6c 3120 3d20 6461 7461 2e69 6c6f 635b  ol1 = data.iloc[
+00025c80: 315d 5b22 566f 6c75 6d65 225d 0d0a 2020  1]["Volume"]..  
+00025c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ca0: 2020 766f 6c30 203d 2064 6174 612e 696c    vol0 = data.il
+00025cb0: 6f63 5b30 5d5b 2256 6f6c 756d 6522 5d0d  oc[0]["Volume"].
+00025cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025cd0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+00025ce0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+00025cf0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+00025d00: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
+00025d10: 6174 7465 726e 2229 0d0a 2020 2020 2020  attern")..      
+00025d20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00025d30: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00025d40: 2020 2020 2020 2020 2020 2020 7370 7265              spre
+00025d50: 6164 3020 3e20 7370 7265 6164 310d 0a20  ad0 > spread1.. 
+00025d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d70: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
+00025d80: 3c20 766f 6c31 0d0a 2020 2020 2020 2020  < vol1..        
+00025d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025da0: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
+00025db0: 5b22 566f 6c75 6d65 225d 203c 2064 6174  ["Volume"] < dat
+00025dc0: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
+00025dd0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00025de0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00025df0: 6461 7461 2e69 6c6f 635b 305d 5b22 436c  data.iloc[0]["Cl
+00025e00: 6f73 6522 5d20 3c3d 2064 6174 612e 696c  ose"] <= data.il
+00025e10: 6f63 5b31 5d5b 224f 7065 6e22 5d0d 0a20  oc[1]["Open"].. 
+00025e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e30: 2020 2020 2020 2061 6e64 2073 7072 6561         and sprea
+00025e40: 6430 203c 206c 6f77 6572 5f77 6963 6b5f  d0 < lower_wick_
+00025e50: 7370 7265 6164 300d 0a20 2020 2020 2020  spread0..       
+00025e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e70: 2061 6e64 2064 6174 612e 696c 6f63 5b30   and data.iloc[0
+00025e80: 5d5b 2256 6f6c 756d 6522 5d20 3c3d 2069  ]["Volume"] <= i
+00025e90: 6e74 2864 6174 612e 696c 6f63 5b31 5d5b  nt(data.iloc[1][
+00025ea0: 2256 6f6c 756d 6522 5d20 2a20 302e 3735  "Volume"] * 0.75
+00025eb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00025ec0: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
 00025ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ee0: 2020 2020 2020 2020 616e 6420 6461 7461          and data
-00025ef0: 2e69 6c6f 635b 305d 5b22 566f 6c75 6d65  .iloc[0]["Volume
-00025f00: 225d 203e 2064 6174 612e 696c 6f63 5b30  "] > data.iloc[0
-00025f10: 5d5b 2256 6f6c 4d41 225d 0d0a 2020 2020  ]["VolMA"]..    
-00025f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f30: 2020 2020 616e 6420 6461 7461 2e69 6c6f      and data.ilo
-00025f40: 635b 305d 5b22 436c 6f73 6522 5d20 3c3d  c[0]["Close"] <=
-00025f50: 2064 6174 612e 696c 6f63 5b31 5d5b 224f   data.iloc[1]["O
-00025f60: 7065 6e22 5d0d 0a20 2020 2020 2020 2020  pen"]..         
-00025f70: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
-00025f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f90: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00025fa0: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+00025ee0: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+00025ef0: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
+00025f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f10: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+00025f20: 305d 200d 0a20 2020 2020 2020 2020 2020  0] ..           
+00025f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f40: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00025f50: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+00025f60: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00025f70: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+00025f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025f90: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00025fa0: 2253 7570 706c 7920 4472 6f75 6768 7422  "Supply Drought"
 00025fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025fc0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00025fd0: 7665 645b 305d 200d 0a20 2020 2020 2020  ved[0] ..       
+00025fc0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00025fd0: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
 00025fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ff0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-00026000: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
-00026010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026020: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
-00026030: 5245 454e 0d0a 2020 2020 2020 2020 2020  REEN..          
-00026040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026050: 2020 2b20 2244 656d 616e 6420 5269 7365    + "Demand Rise
-00026060: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00026070: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00026080: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
-00026090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000260a0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00025ff0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00026000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026010: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+00026020: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
+00026030: 202b 2022 5375 7070 6c79 2044 726f 7567   + "Supply Droug
+00026040: 6874 220d 0a20 2020 2020 2020 2020 2020  ht"..           
+00026050: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00026060: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
+00026070: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00026080: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00026090: 2020 2020 2020 2020 2020 2020 7370 7265              spre
+000260a0: 6164 3020 3c20 7370 7265 6164 310d 0a20  ad0 < spread1.. 
 000260b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000260c0: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
-000260d0: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
-000260e0: 5d20 2b20 2244 656d 616e 6420 5269 7365  ] + "Demand Rise
-000260f0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00026100: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00026110: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
-00026120: 2020 2020 6578 6365 7074 2049 6e64 6578      except Index
-00026130: 4572 726f 7220 6173 2065 3a20 2320 7072  Error as e: # pr
-00026140: 6167 6d61 3a20 6e6f 2063 6f76 6572 0d0a  agma: no cover..
-00026150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026160: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-00026170: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
-00026180: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
-00026190: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-000261a0: 730d 0a20 2020 2020 2020 2020 2020 2072  s..            r
-000261b0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-000261c0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-000261d0: 7074 696f 6e20 6173 2065 3a20 2023 2070  ption as e:  # p
-000261e0: 7261 676d 613a 206e 6f20 636f 7665 720d  ragma: no cover.
-000261f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00026200: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-00026210: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
-00026220: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
-00026230: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00026240: 7365 0d0a                                se..
+000260c0: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
+000260d0: 3e20 766f 6c31 0d0a 2020 2020 2020 2020  > vol1..        
+000260e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000260f0: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
+00026100: 5b22 566f 6c75 6d65 225d 203e 2064 6174  ["Volume"] > dat
+00026110: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
+00026120: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00026130: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00026140: 6461 7461 2e69 6c6f 635b 305d 5b22 436c  data.iloc[0]["Cl
+00026150: 6f73 6522 5d20 3c3d 2064 6174 612e 696c  ose"] <= data.il
+00026160: 6f63 5b31 5d5b 224f 7065 6e22 5d0d 0a20  oc[1]["Open"].. 
+00026170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026180: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
+00026190: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000261a0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+000261b0: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
+000261c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000261d0: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
+000261e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000261f0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+00026200: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
+00026210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026220: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00026230: 6f72 5465 7874 2e47 5245 454e 0d0a 2020  orText.GREEN..  
+00026240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026250: 2020 2020 2020 2020 2020 2b20 2244 656d            + "Dem
+00026260: 616e 6420 5269 7365 220d 0a20 2020 2020  and Rise"..     
+00026270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026280: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+00026290: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+000262a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000262b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000262c0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+000262d0: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+000262e0: 2073 6176 6564 5b31 5d20 2b20 2244 656d   saved[1] + "Dem
+000262f0: 616e 6420 5269 7365 220d 0a20 2020 2020  and Rise"..     
+00026300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026310: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00026320: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00026330: 7074 2049 6e64 6578 4572 726f 7220 6173  pt IndexError as
+00026340: 2065 3a20 2320 7072 6167 6d61 3a20 6e6f   e: # pragma: no
+00026350: 2063 6f76 6572 0d0a 2020 2020 2020 2020   cover..        
+00026360: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+00026370: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+00026380: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+00026390: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+000263a0: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
+000263b0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000263c0: 6c73 650d 0a20 2020 2020 2020 2065 7863  lse..        exc
+000263d0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+000263e0: 2065 3a20 2023 2070 7261 676d 613a 206e   e:  # pragma: n
+000263f0: 6f20 636f 7665 720d 0a20 2020 2020 2020  o cover..       
+00026400: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
+00026410: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
+00026420: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
+00026430: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00026440: 7475 726e 2046 616c 7365 0d0a            turn False..
```

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/classes/keys.py` & `pkscreener-0.45.20240521.393/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/courbd.ttf` & `pkscreener-0.45.20240521.393/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/globals.py` & `pkscreener-0.45.20240521.393/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240521.393/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240521.393/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240521.393/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240521.393/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.392
+Version: 0.45.20240521.393
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.392.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.393.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.391/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.392/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.392/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240521.393/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.392/setup.py` & `pkscreener-0.45.20240521.393/setup.py`

 * *Files identical despite different names*

