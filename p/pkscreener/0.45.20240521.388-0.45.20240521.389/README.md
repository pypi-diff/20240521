# Comparing `tmp/pkscreener-0.45.20240521.388.tar.gz` & `tmp/pkscreener-0.45.20240521.389.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240521.388.tar", last modified: Tue May 21 10:12:05 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240521.389.tar", last modified: Tue May 21 17:02:11 2024, max compression
```

## Comparing `pkscreener-0.45.20240521.388.tar` & `pkscreener-0.45.20240521.389.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 10:12:05.413684 pkscreener-0.45.20240521.388/
--rw-rw-rw-   0        0        0     1086 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-21 10:12:05.413684 pkscreener-0.45.20240521.388/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 10:12:05.398061 pkscreener-0.45.20240521.388/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:12:05.413684 pkscreener-0.45.20240521.388/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5641 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34249 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45624 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8313 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156140 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56423 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    85480 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-21 10:11:57.000000 pkscreener-0.45.20240521.388/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   145457 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1089 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53062 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34370 2024-05-21 10:07:47.000000 pkscreener-0.45.20240521.388/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:12:05.398061 pkscreener-0.45.20240521.388/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-21 10:12:05.000000 pkscreener-0.45.20240521.388/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-21 10:12:05.000000 pkscreener-0.45.20240521.388/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 10:12:05.000000 pkscreener-0.45.20240521.388/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-21 10:12:05.000000 pkscreener-0.45.20240521.388/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-21 10:12:05.000000 pkscreener-0.45.20240521.388/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-21 10:12:05.000000 pkscreener-0.45.20240521.388/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-21 10:12:05.413684 pkscreener-0.45.20240521.388/setup.cfg
--rw-rw-rw-   0        0        0     5728 2024-05-21 10:07:48.000000 pkscreener-0.45.20240521.388/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:02:11.350796 pkscreener-0.45.20240521.389/
+-rw-rw-rw-   0        0        0     1086 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/LICENSE-Others
+-rw-rw-rw-   0        0        0    27920 2024-05-21 17:02:11.350796 pkscreener-0.45.20240521.389/PKG-INFO
+-rw-rw-rw-   0        0        0    26981 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 17:02:11.335168 pkscreener-0.45.20240521.389/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:02:11.350796 pkscreener-0.45.20240521.389/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34249 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45624 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8313 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156228 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56423 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    85591 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-21 17:02:03.000000 pkscreener-0.45.20240521.389/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   146404 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1089 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53062 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34370 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:02:11.350796 pkscreener-0.45.20240521.389/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27920 2024-05-21 17:02:11.000000 pkscreener-0.45.20240521.389/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-21 17:02:11.000000 pkscreener-0.45.20240521.389/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 17:02:11.000000 pkscreener-0.45.20240521.389/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-21 17:02:11.000000 pkscreener-0.45.20240521.389/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 17:02:11.000000 pkscreener-0.45.20240521.389/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-21 17:02:11.000000 pkscreener-0.45.20240521.389/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-21 17:02:11.350796 pkscreener-0.45.20240521.389/setup.cfg
+-rw-rw-rw-   0        0        0     5728 2024-05-21 16:57:05.000000 pkscreener-0.45.20240521.389/setup.py
```

### Comparing `pkscreener-0.45.20240521.388/LICENSE` & `pkscreener-0.45.20240521.389/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/LICENSE-Others` & `pkscreener-0.45.20240521.389/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/PKG-INFO` & `pkscreener-0.45.20240521.389/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.388
+Version: 0.45.20240521.389
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.388.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.389.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -112,14 +112,19 @@
     15 > 52 week low breakout(today/1 wk)	16 > 10 days low breakout
     17 > 52 week high breakout(today/1 wk)	18 > Bullish Aroon(14) Crossover
     19 > MACD Histogram x below 0       	20 > Bullish for next day
     21 > Most Popular Stocks            	22 > View Stock Performance         
     23 > Breaking out now               	24 > Higher Highs,Lows & Close      
     25 > Lower Highs,Lows (Watch for Reversal)            	
 ```
+## Running Piped Scanners
+
+https://github.com/pkjmesra/PKScreener/assets/1358101/9e579371-1035-400a-9f65-139d8407f6c7
+
+
 ## How to use on your own local Windows/Linux/Macbook laptop?
 
 # Using docker, running within docker container
 * Download and install docker desktop: https://docs.docker.com/get-docker/
 * After installation, launch/run docker desktop and if it asks, login using your docker credentials.
 * Launch any command line (for example, cmd on windows or terminal on Mac) and type `docker pull pkjmesra/pkscreener:latest`. Then type `docker run -it pkjmesra/pkscreener:latest`.  
   The option `-i` will open the `pkscreener` in interactive mode within docker. `-t` will allocate a pseudo terminal for you so you can begin to use `pkscreener`
@@ -269,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.388/README.md` & `pkscreener-0.45.20240521.389/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,19 @@
     15 > 52 week low breakout(today/1 wk)	16 > 10 days low breakout
     17 > 52 week high breakout(today/1 wk)	18 > Bullish Aroon(14) Crossover
     19 > MACD Histogram x below 0       	20 > Bullish for next day
     21 > Most Popular Stocks            	22 > View Stock Performance         
     23 > Breaking out now               	24 > Higher Highs,Lows & Close      
     25 > Lower Highs,Lows (Watch for Reversal)            	
 ```
+## Running Piped Scanners
+
+https://github.com/pkjmesra/PKScreener/assets/1358101/9e579371-1035-400a-9f65-139d8407f6c7
+
+
 ## How to use on your own local Windows/Linux/Macbook laptop?
 
 # Using docker, running within docker container
 * Download and install docker desktop: https://docs.docker.com/get-docker/
 * After installation, launch/run docker desktop and if it asks, login using your docker credentials.
 * Launch any command line (for example, cmd on windows or terminal on Mac) and type `docker pull pkjmesra/pkscreener:latest`. Then type `docker run -it pkjmesra/pkscreener:latest`.  
   The option `-i` will open the `pkscreener` in interactive mode within docker. `-t` will allocate a pseudo terminal for you so you can begin to use `pkscreener`
@@ -247,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.388/pkscreener/__init__.py` & `pkscreener-0.45.20240521.389/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/ScreeningStatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -9442,318 +9442,324 @@
 00024e10: 7267 203d 206c 6f77 506f 696e 7473 0d0a  rg = lowPoints..
 00024e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00024e30: 6c6f 7750 6f69 6e74 732e 736f 7274 2872  lowPoints.sort(r
 00024e40: 6576 6572 7365 3d54 7275 6529 0d0a 2020  everse=True)..  
 00024e50: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
 00024e60: 7750 6f69 6e74 7353 6f72 7465 6420 3d20  wPointsSorted = 
 00024e70: 6c6f 7750 6f69 6e74 730d 0a20 2020 2020  lowPoints..     
-00024e80: 2020 2020 2020 2020 2020 206c 7470 203d             ltp =
-00024e90: 2064 6174 612e 6865 6164 2831 295b 2243   data.head(1)["C
-00024ea0: 6c6f 7365 225d 2e69 6c6f 635b 305d 0d0a  lose"].iloc[0]..
-00024eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ec0: 6966 2028 0d0a 2020 2020 2020 2020 2020  if (..          
-00024ed0: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
-00024ee0: 6e74 734f 7267 203d 3d20 6c6f 7750 6f69  ntsOrg == lowPoi
-00024ef0: 6e74 7353 6f72 7465 640d 0a20 2020 2020  ntsSorted..     
-00024f00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00024f10: 6e64 206c 7470 203c 2068 6967 6865 7374  nd ltp < highest
-00024f20: 546f 700d 0a20 2020 2020 2020 2020 2020  Top..           
-00024f30: 2020 2020 2020 2020 2061 6e64 206c 7470           and ltp
-00024f40: 203e 206c 6f77 506f 696e 7473 5b30 5d0d   > lowPoints[0].
-00024f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024f60: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-00024f70: 2020 2020 2020 2020 2073 6176 6564 203d           saved =
-00024f80: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-00024f90: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-00024fa0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00024fb0: 2c20 2250 6174 7465 726e 2229 0d0a 2020  , "Pattern")..  
+00024e80: 2020 2020 2020 2020 2020 2069 6620 6461             if da
+00024e90: 7461 2e65 6d70 7479 206f 7220 6c65 6e28  ta.empty or len(
+00024ea0: 6c6f 7750 6f69 6e74 7329 203c 2031 3a0d  lowPoints) < 1:.
+00024eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024ec0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00024ed0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00024ee0: 2020 206c 7470 203d 2064 6174 612e 6865     ltp = data.he
+00024ef0: 6164 2831 295b 2243 6c6f 7365 225d 2e69  ad(1)["Close"].i
+00024f00: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
+00024f10: 2020 2020 2020 2020 6966 2028 0d0a 2020          if (..  
+00024f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024f30: 2020 6c6f 7750 6f69 6e74 734f 7267 203d    lowPointsOrg =
+00024f40: 3d20 6c6f 7750 6f69 6e74 7353 6f72 7465  = lowPointsSorte
+00024f50: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+00024f60: 2020 2020 2020 2061 6e64 206c 7470 203c         and ltp <
+00024f70: 2068 6967 6865 7374 546f 700d 0a20 2020   highestTop..   
+00024f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024f90: 2061 6e64 206c 7470 203e 206c 6f77 506f   and ltp > lowPo
+00024fa0: 696e 7473 5b30 5d0d 0a20 2020 2020 2020  ints[0]..       
+00024fb0: 2020 2020 2020 2020 2029 3a0d 0a20 2020           ):..   
 00024fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fd0: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
-00024fe0: 7474 6572 6e22 5d20 3d20 280d 0a20 2020  ttern"] = (..   
-00024ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025000: 2020 2020 2073 6176 6564 5b30 5d20 0d0a       saved[0] ..
-00025010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025020: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00025030: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
-00025040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025050: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
-00025060: 4545 4e0d 0a20 2020 2020 2020 2020 2020  EEN..           
-00025070: 2020 2020 2020 2020 2020 2020 202b 2066               + f
-00025080: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
-00025090: 7374 546f 707d 2922 0d0a 2020 2020 2020  stTop})"..      
-000250a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000250b0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-000250c0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-000250d0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000250e0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-000250f0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-00025100: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
-00025110: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
-00025120: 7374 546f 707d 2922 0d0a 2020 2020 2020  stTop})"..      
-00025130: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00025140: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-00025150: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00025160: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-00025170: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
-00025180: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00025190: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-000251a0: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-000251b0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-000251c0: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-000251d0: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
-000251e0: 6620 766f 6c75 6d65 206f 6620 6c61 7374  f volume of last
-000251f0: 2064 6179 2069 7320 6869 6768 6572 2074   day is higher t
-00025200: 6861 6e20 6176 670d 0a20 2020 2064 6566  han avg..    def
-00025210: 2076 616c 6964 6174 6556 6f6c 756d 6528   validateVolume(
-00025220: 0d0a 2020 2020 2020 2020 7365 6c66 2c20  ..        self, 
-00025230: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
-00025240: 7361 7665 4469 6374 2c20 766f 6c75 6d65  saveDict, volume
-00025250: 5261 7469 6f3d 322e 352c 206d 696e 566f  Ratio=2.5, minVo
-00025260: 6c75 6d65 3d31 3030 0d0a 2020 2020 293a  lume=100..    ):
-00025270: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
-00025280: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-00025290: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
-000252a0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000252b0: 7365 2c20 4661 6c73 650d 0a20 2020 2020  se, False..     
-000252c0: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-000252d0: 7928 290d 0a20 2020 2020 2020 2064 6174  y()..        dat
-000252e0: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
-000252f0: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
-00025300: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-00025310: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
-00025320: 5d2c 2030 290d 0a20 2020 2020 2020 2072  ], 0)..        r
-00025330: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
-00025340: 6428 3129 0d0a 2020 2020 2020 2020 2320  d(1)..        # 
-00025350: 4569 7468 6572 2074 6865 2072 6f6c 6c69  Either the rolli
-00025360: 6e67 2076 6f6c 756d 6520 6f66 2070 6173  ng volume of pas
-00025370: 7420 3230 2073 6573 7369 6f6e 7320 6f72  t 20 sessions or
-00025380: 2074 6f64 6179 2773 2076 6f6c 756d 6520   today's volume 
-00025390: 7368 6f75 6c64 2062 6520 3e20 6d69 6e20  should be > min 
-000253a0: 766f 6c75 6d65 0d0a 2020 2020 2020 2020  volume..        
-000253b0: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
-000253c0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-000253d0: 2020 7265 6365 6e74 5b22 566f 6c4d 4122    recent["VolMA"
-000253e0: 5d2e 696c 6f63 5b30 5d20 3e3d 206d 696e  ].iloc[0] >= min
-000253f0: 566f 6c75 6d65 0d0a 2020 2020 2020 2020  Volume..        
-00025400: 2020 2020 6f72 2072 6563 656e 745b 2256      or recent["V
-00025410: 6f6c 756d 6522 5d2e 696c 6f63 5b30 5d20  olume"].iloc[0] 
-00025420: 3e3d 206d 696e 566f 6c75 6d65 0d0a 2020  >= minVolume..  
-00025430: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00025440: 2069 6620 7265 6365 6e74 5b22 566f 6c4d   if recent["VolM
-00025450: 4122 5d2e 696c 6f63 5b30 5d20 3d3d 2030  A"].iloc[0] == 0
-00025460: 3a20 2023 2048 616e 646c 6573 2044 6976  :  # Handles Div
-00025470: 6964 6520 6279 2030 2077 6172 6e69 6e67  ide by 0 warning
-00025480: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
-00025490: 7665 4469 6374 5b22 566f 6c75 6d65 225d  veDict["Volume"]
-000254a0: 203d 2030 2020 2320 2255 6e6b 6e6f 776e   = 0  # "Unknown
-000254b0: 220d 0a20 2020 2020 2020 2020 2020 2073  "..            s
-000254c0: 6372 6565 6e44 6963 745b 2256 6f6c 756d  creenDict["Volum
-000254d0: 6522 5d20 3d20 300d 0a20 2020 2020 2020  e"] = 0..       
-000254e0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000254f0: 652c 2068 6173 4d69 6e69 6d75 6d56 6f6c  e, hasMinimumVol
-00025500: 756d 650d 0a20 2020 2020 2020 2072 6174  ume..        rat
-00025510: 696f 203d 2072 6f75 6e64 2872 6563 656e  io = round(recen
-00025520: 745b 2256 6f6c 756d 6522 5d2e 696c 6f63  t["Volume"].iloc
-00025530: 5b30 5d20 2f20 7265 6365 6e74 5b22 566f  [0] / recent["Vo
-00025540: 6c4d 4122 5d2e 696c 6f63 5b30 5d2c 2032  lMA"].iloc[0], 2
-00025550: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
-00025560: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
-00025570: 7261 7469 6f0d 0a20 2020 2020 2020 2069  ratio..        i
-00025580: 6620 7261 7469 6f20 3e3d 2076 6f6c 756d  f ratio >= volum
-00025590: 6552 6174 696f 2061 6e64 2072 6174 696f  eRatio and ratio
-000255a0: 2021 3d20 6e70 2e6e 616e 2061 6e64 2028   != np.nan and (
-000255b0: 6e6f 7420 6d61 7468 2e69 7369 6e66 2872  not math.isinf(r
-000255c0: 6174 696f 2929 3a0d 0a20 2020 2020 2020  atio)):..       
-000255d0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-000255e0: 2256 6f6c 756d 6522 5d20 3d20 7261 7469  "Volume"] = rati
-000255f0: 6f0d 0a20 2020 2020 2020 2020 2020 2072  o..            r
-00025600: 6574 7572 6e20 5472 7565 2c20 6861 734d  eturn True, hasM
-00025610: 696e 696d 756d 566f 6c75 6d65 0d0a 2020  inimumVolume..  
-00025620: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00025630: 5b22 566f 6c75 6d65 225d 203d 2072 6174  ["Volume"] = rat
-00025640: 696f 0d0a 2020 2020 2020 2020 7265 7475  io..        retu
-00025650: 726e 2046 616c 7365 2c20 6861 734d 696e  rn False, hasMin
-00025660: 696d 756d 566f 6c75 6d65 0d0a 0d0a 2020  imumVolume....  
-00025670: 2020 2320 4669 6e64 2069 6620 7374 6f63    # Find if stoc
-00025680: 6b20 6973 2076 616c 6964 6174 696e 6720  k is validating 
-00025690: 766f 6c75 6d65 2073 7072 6561 6420 616e  volume spread an
-000256a0: 616c 7973 6973 0d0a 2020 2020 6465 6620  alysis..    def 
-000256b0: 7661 6c69 6461 7465 566f 6c75 6d65 5370  validateVolumeSp
-000256c0: 7265 6164 416e 616c 7973 6973 2873 656c  readAnalysis(sel
-000256d0: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-000256e0: 742c 2073 6176 6544 6963 7429 3a0d 0a20  t, saveDict):.. 
-000256f0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00025700: 2020 2020 2020 2020 2069 6620 6466 2069           if df i
-00025710: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-00025720: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
-00025730: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00025740: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00025750: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-00025760: 7928 290d 0a20 2020 2020 2020 2020 2020  y()..           
-00025770: 2064 6174 6120 3d20 6461 7461 2e68 6561   data = data.hea
-00025780: 6428 3229 0d0a 2020 2020 2020 2020 2020  d(2)..          
-00025790: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
-000257a0: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
-000257b0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000257c0: 650d 0a20 2020 2020 2020 2020 2020 2074  e..            t
-000257d0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-000257e0: 2020 2020 2023 2043 6865 636b 2066 6f72       # Check for
-000257f0: 2070 7265 7669 6f75 7320 5245 4420 6361   previous RED ca
-00025800: 6e64 6c65 730d 0a20 2020 2020 2020 2020  ndles..         
-00025810: 2020 2020 2020 2023 2043 7572 7265 6e74         # Current
-00025820: 2063 616e 646c 6520 3d20 3074 682c 2050   candle = 0th, P
-00025830: 7265 7669 6f75 7320 4361 6e64 6c65 203d  revious Candle =
-00025840: 2031 7374 2066 6f72 2066 6f6c 6c6f 7769   1st for followi
-00025850: 6e67 206c 6f67 6963 0d0a 2020 2020 2020  ng logic..      
-00025860: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
-00025870: 612e 696c 6f63 5b31 5d5b 224f 7065 6e22  a.iloc[1]["Open"
-00025880: 5d20 3e3d 2064 6174 612e 696c 6f63 5b31  ] >= data.iloc[1
-00025890: 5d5b 2243 6c6f 7365 225d 3a0d 0a20 2020  ]["Close"]:..   
-000258a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000258b0: 2073 7072 6561 6431 203d 2061 6273 2864   spread1 = abs(d
-000258c0: 6174 612e 696c 6f63 5b31 5d5b 224f 7065  ata.iloc[1]["Ope
-000258d0: 6e22 5d20 2d20 6461 7461 2e69 6c6f 635b  n"] - data.iloc[
-000258e0: 315d 5b22 436c 6f73 6522 5d29 0d0a 2020  1]["Close"])..  
-000258f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025900: 2020 7370 7265 6164 3020 3d20 6162 7328    spread0 = abs(
-00025910: 6461 7461 2e69 6c6f 635b 305d 5b22 4f70  data.iloc[0]["Op
-00025920: 656e 225d 202d 2064 6174 612e 696c 6f63  en"] - data.iloc
-00025930: 5b30 5d5b 2243 6c6f 7365 225d 290d 0a20  [0]["Close"]).. 
-00025940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025950: 2020 206c 6f77 6572 5f77 6963 6b5f 7370     lower_wick_sp
-00025960: 7265 6164 3020 3d20 280d 0a20 2020 2020  read0 = (..     
-00025970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025980: 2020 206d 6178 2864 6174 612e 696c 6f63     max(data.iloc
-00025990: 5b30 5d5b 224f 7065 6e22 5d2c 2064 6174  [0]["Open"], dat
-000259a0: 612e 696c 6f63 5b30 5d5b 2243 6c6f 7365  a.iloc[0]["Close
-000259b0: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
-000259c0: 2020 2020 2020 2020 2020 2020 202d 2064               - d
-000259d0: 6174 612e 696c 6f63 5b30 5d5b 224c 6f77  ata.iloc[0]["Low
-000259e0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-000259f0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00025a00: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00025a10: 6f6c 3120 3d20 6461 7461 2e69 6c6f 635b  ol1 = data.iloc[
-00025a20: 315d 5b22 566f 6c75 6d65 225d 0d0a 2020  1]["Volume"]..  
-00025a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a40: 2020 766f 6c30 203d 2064 6174 612e 696c    vol0 = data.il
-00025a50: 6f63 5b30 5d5b 2256 6f6c 756d 6522 5d0d  oc[0]["Volume"].
-00025a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025a70: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-00025a80: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-00025a90: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-00025aa0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
-00025ab0: 6174 7465 726e 2229 0d0a 2020 2020 2020  attern")..      
-00025ac0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00025ad0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00025ae0: 2020 2020 2020 2020 2020 2020 7370 7265              spre
-00025af0: 6164 3020 3e20 7370 7265 6164 310d 0a20  ad0 > spread1.. 
-00025b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b10: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
-00025b20: 3c20 766f 6c31 0d0a 2020 2020 2020 2020  < vol1..        
+00024fd0: 2073 6176 6564 203d 2073 656c 662e 6669   saved = self.fi
+00024fe0: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
+00024ff0: 6c75 6528 7363 7265 656e 4469 6374 2c20  lue(screenDict, 
+00025000: 7361 7665 4469 6374 2c20 2250 6174 7465  saveDict, "Patte
+00025010: 726e 2229 0d0a 2020 2020 2020 2020 2020  rn")..          
+00025020: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+00025030: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+00025040: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+00025050: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00025060: 6564 5b30 5d20 0d0a 2020 2020 2020 2020  ed[0] ..        
+00025070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025080: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+00025090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000250a0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+000250b0: 7254 6578 742e 4752 4545 4e0d 0a20 2020  rText.GREEN..   
+000250c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250d0: 2020 2020 202b 2066 2256 4350 2028 424f       + f"VCP (BO
+000250e0: 3a20 7b68 6967 6865 7374 546f 707d 2922  : {highestTop})"
+000250f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025100: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00025110: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+00025120: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00025130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025140: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00025150: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
+00025160: 645b 315d 202b 2066 2256 4350 2028 424f  d[1] + f"VCP (BO
+00025170: 3a20 7b68 6967 6865 7374 546f 707d 2922  : {highestTop})"
+00025180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025190: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+000251a0: 650d 0a20 2020 2020 2020 2065 7863 6570  e..        excep
+000251b0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+000251c0: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+000251d0: 636f 7665 720d 0a20 2020 2020 2020 2020  cover..         
+000251e0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+000251f0: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+00025200: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
+00025210: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00025220: 616c 7365 0d0a 0d0a 2020 2020 2320 5661  alse....    # Va
+00025230: 6c69 6461 7465 2069 6620 766f 6c75 6d65  lidate if volume
+00025240: 206f 6620 6c61 7374 2064 6179 2069 7320   of last day is 
+00025250: 6869 6768 6572 2074 6861 6e20 6176 670d  higher than avg.
+00025260: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00025270: 6556 6f6c 756d 6528 0d0a 2020 2020 2020  eVolume(..      
+00025280: 2020 7365 6c66 2c20 6466 2c20 7363 7265    self, df, scre
+00025290: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+000252a0: 2c20 766f 6c75 6d65 5261 7469 6f3d 322e  , volumeRatio=2.
+000252b0: 352c 206d 696e 566f 6c75 6d65 3d31 3030  5, minVolume=100
+000252c0: 0d0a 2020 2020 293a 0d0a 2020 2020 2020  ..    ):..      
+000252d0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+000252e0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+000252f0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00025300: 7475 726e 2046 616c 7365 2c20 4661 6c73  turn False, Fals
+00025310: 650d 0a20 2020 2020 2020 2064 6174 6120  e..        data 
+00025320: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
+00025330: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00025340: 2e66 696c 6c6e 6128 3029 0d0a 2020 2020  .fillna(0)..    
+00025350: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00025360: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+00025370: 202d 6e70 2e69 6e66 5d2c 2030 290d 0a20   -np.inf], 0).. 
+00025380: 2020 2020 2020 2072 6563 656e 7420 3d20         recent = 
+00025390: 6461 7461 2e68 6561 6428 3129 0d0a 2020  data.head(1)..  
+000253a0: 2020 2020 2020 2320 4569 7468 6572 2074        # Either t
+000253b0: 6865 2072 6f6c 6c69 6e67 2076 6f6c 756d  he rolling volum
+000253c0: 6520 6f66 2070 6173 7420 3230 2073 6573  e of past 20 ses
+000253d0: 7369 6f6e 7320 6f72 2074 6f64 6179 2773  sions or today's
+000253e0: 2076 6f6c 756d 6520 7368 6f75 6c64 2062   volume should b
+000253f0: 6520 3e20 6d69 6e20 766f 6c75 6d65 0d0a  e > min volume..
+00025400: 2020 2020 2020 2020 6861 734d 696e 696d          hasMinim
+00025410: 756d 566f 6c75 6d65 203d 2028 0d0a 2020  umVolume = (..  
+00025420: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+00025430: 5b22 566f 6c4d 4122 5d2e 696c 6f63 5b30  ["VolMA"].iloc[0
+00025440: 5d20 3e3d 206d 696e 566f 6c75 6d65 0d0a  ] >= minVolume..
+00025450: 2020 2020 2020 2020 2020 2020 6f72 2072              or r
+00025460: 6563 656e 745b 2256 6f6c 756d 6522 5d2e  ecent["Volume"].
+00025470: 696c 6f63 5b30 5d20 3e3d 206d 696e 566f  iloc[0] >= minVo
+00025480: 6c75 6d65 0d0a 2020 2020 2020 2020 290d  lume..        ).
+00025490: 0a20 2020 2020 2020 2069 6620 7265 6365  .        if rece
+000254a0: 6e74 5b22 566f 6c4d 4122 5d2e 696c 6f63  nt["VolMA"].iloc
+000254b0: 5b30 5d20 3d3d 2030 3a20 2023 2048 616e  [0] == 0:  # Han
+000254c0: 646c 6573 2044 6976 6964 6520 6279 2030  dles Divide by 0
+000254d0: 2077 6172 6e69 6e67 0d0a 2020 2020 2020   warning..      
+000254e0: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+000254f0: 566f 6c75 6d65 225d 203d 2030 2020 2320  Volume"] = 0  # 
+00025500: 2255 6e6b 6e6f 776e 220d 0a20 2020 2020  "Unknown"..     
+00025510: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00025520: 745b 2256 6f6c 756d 6522 5d20 3d20 300d  t["Volume"] = 0.
+00025530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00025540: 7572 6e20 4661 6c73 652c 2068 6173 4d69  urn False, hasMi
+00025550: 6e69 6d75 6d56 6f6c 756d 650d 0a20 2020  nimumVolume..   
+00025560: 2020 2020 2072 6174 696f 203d 2072 6f75       ratio = rou
+00025570: 6e64 2872 6563 656e 745b 2256 6f6c 756d  nd(recent["Volum
+00025580: 6522 5d2e 696c 6f63 5b30 5d20 2f20 7265  e"].iloc[0] / re
+00025590: 6365 6e74 5b22 566f 6c4d 4122 5d2e 696c  cent["VolMA"].il
+000255a0: 6f63 5b30 5d2c 2032 290d 0a20 2020 2020  oc[0], 2)..     
+000255b0: 2020 2073 6176 6544 6963 745b 2256 6f6c     saveDict["Vol
+000255c0: 756d 6522 5d20 3d20 7261 7469 6f0d 0a20  ume"] = ratio.. 
+000255d0: 2020 2020 2020 2069 6620 7261 7469 6f20         if ratio 
+000255e0: 3e3d 2076 6f6c 756d 6552 6174 696f 2061  >= volumeRatio a
+000255f0: 6e64 2072 6174 696f 2021 3d20 6e70 2e6e  nd ratio != np.n
+00025600: 616e 2061 6e64 2028 6e6f 7420 6d61 7468  an and (not math
+00025610: 2e69 7369 6e66 2872 6174 696f 2929 3a0d  .isinf(ratio)):.
+00025620: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+00025630: 6565 6e44 6963 745b 2256 6f6c 756d 6522  eenDict["Volume"
+00025640: 5d20 3d20 7261 7469 6f0d 0a20 2020 2020  ] = ratio..     
+00025650: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00025660: 7565 2c20 6861 734d 696e 696d 756d 566f  ue, hasMinimumVo
+00025670: 6c75 6d65 0d0a 2020 2020 2020 2020 7363  lume..        sc
+00025680: 7265 656e 4469 6374 5b22 566f 6c75 6d65  reenDict["Volume
+00025690: 225d 203d 2072 6174 696f 0d0a 2020 2020  "] = ratio..    
+000256a0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000256b0: 2c20 6861 734d 696e 696d 756d 566f 6c75  , hasMinimumVolu
+000256c0: 6d65 0d0a 0d0a 2020 2020 2320 4669 6e64  me....    # Find
+000256d0: 2069 6620 7374 6f63 6b20 6973 2076 616c   if stock is val
+000256e0: 6964 6174 696e 6720 766f 6c75 6d65 2073  idating volume s
+000256f0: 7072 6561 6420 616e 616c 7973 6973 0d0a  pread analysis..
+00025700: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00025710: 566f 6c75 6d65 5370 7265 6164 416e 616c  VolumeSpreadAnal
+00025720: 7973 6973 2873 656c 662c 2064 662c 2073  ysis(self, df, s
+00025730: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00025740: 6963 7429 3a0d 0a20 2020 2020 2020 2074  ict):..        t
+00025750: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00025760: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+00025770: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0d  r len(df) == 0:.
+00025780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025790: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+000257a0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+000257b0: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
+000257c0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+000257d0: 6461 7461 2e68 6561 6428 3229 0d0a 2020  data.head(2)..  
+000257e0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+000257f0: 2864 6174 6129 203c 2032 3a0d 0a20 2020  (data) < 2:..   
+00025800: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00025810: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+00025820: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00025830: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+00025840: 6865 636b 2066 6f72 2070 7265 7669 6f75  heck for previou
+00025850: 7320 5245 4420 6361 6e64 6c65 730d 0a20  s RED candles.. 
+00025860: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00025870: 2043 7572 7265 6e74 2063 616e 646c 6520   Current candle 
+00025880: 3d20 3074 682c 2050 7265 7669 6f75 7320  = 0th, Previous 
+00025890: 4361 6e64 6c65 203d 2031 7374 2066 6f72  Candle = 1st for
+000258a0: 2066 6f6c 6c6f 7769 6e67 206c 6f67 6963   following logic
+000258b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000258c0: 2020 6966 2064 6174 612e 696c 6f63 5b31    if data.iloc[1
+000258d0: 5d5b 224f 7065 6e22 5d20 3e3d 2064 6174  ]["Open"] >= dat
+000258e0: 612e 696c 6f63 5b31 5d5b 2243 6c6f 7365  a.iloc[1]["Close
+000258f0: 225d 3a0d 0a20 2020 2020 2020 2020 2020  "]:..           
+00025900: 2020 2020 2020 2020 2073 7072 6561 6431           spread1
+00025910: 203d 2061 6273 2864 6174 612e 696c 6f63   = abs(data.iloc
+00025920: 5b31 5d5b 224f 7065 6e22 5d20 2d20 6461  [1]["Open"] - da
+00025930: 7461 2e69 6c6f 635b 315d 5b22 436c 6f73  ta.iloc[1]["Clos
+00025940: 6522 5d29 0d0a 2020 2020 2020 2020 2020  e"])..          
+00025950: 2020 2020 2020 2020 2020 7370 7265 6164            spread
+00025960: 3020 3d20 6162 7328 6461 7461 2e69 6c6f  0 = abs(data.ilo
+00025970: 635b 305d 5b22 4f70 656e 225d 202d 2064  c[0]["Open"] - d
+00025980: 6174 612e 696c 6f63 5b30 5d5b 2243 6c6f  ata.iloc[0]["Clo
+00025990: 7365 225d 290d 0a20 2020 2020 2020 2020  se"])..         
+000259a0: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+000259b0: 5f77 6963 6b5f 7370 7265 6164 3020 3d20  _wick_spread0 = 
+000259c0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000259d0: 2020 2020 2020 2020 2020 206d 6178 2864             max(d
+000259e0: 6174 612e 696c 6f63 5b30 5d5b 224f 7065  ata.iloc[0]["Ope
+000259f0: 6e22 5d2c 2064 6174 612e 696c 6f63 5b30  n"], data.iloc[0
+00025a00: 5d5b 2243 6c6f 7365 225d 290d 0a20 2020  ]["Close"])..   
+00025a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a20: 2020 2020 202d 2064 6174 612e 696c 6f63       - data.iloc
+00025a30: 5b30 5d5b 224c 6f77 225d 0d0a 2020 2020  [0]["Low"]..    
+00025a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00025a60: 2020 2020 2020 2076 6f6c 3120 3d20 6461         vol1 = da
+00025a70: 7461 2e69 6c6f 635b 315d 5b22 566f 6c75  ta.iloc[1]["Volu
+00025a80: 6d65 225d 0d0a 2020 2020 2020 2020 2020  me"]..          
+00025a90: 2020 2020 2020 2020 2020 766f 6c30 203d            vol0 =
+00025aa0: 2064 6174 612e 696c 6f63 5b30 5d5b 2256   data.iloc[0]["V
+00025ab0: 6f6c 756d 6522 5d0d 0a20 2020 2020 2020  olume"]..       
+00025ac0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00025ad0: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+00025ae0: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+00025af0: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+00025b00: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
+00025b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025b20: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
 00025b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b40: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
-00025b50: 5b22 566f 6c75 6d65 225d 203c 2064 6174  ["Volume"] < dat
-00025b60: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
-00025b70: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00025b80: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00025b90: 6461 7461 2e69 6c6f 635b 305d 5b22 436c  data.iloc[0]["Cl
-00025ba0: 6f73 6522 5d20 3c3d 2064 6174 612e 696c  ose"] <= data.il
-00025bb0: 6f63 5b31 5d5b 224f 7065 6e22 5d0d 0a20  oc[1]["Open"].. 
-00025bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025bd0: 2020 2020 2020 2061 6e64 2073 7072 6561         and sprea
-00025be0: 6430 203c 206c 6f77 6572 5f77 6963 6b5f  d0 < lower_wick_
-00025bf0: 7370 7265 6164 300d 0a20 2020 2020 2020  spread0..       
-00025c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025c10: 2061 6e64 2064 6174 612e 696c 6f63 5b30   and data.iloc[0
-00025c20: 5d5b 2256 6f6c 756d 6522 5d20 3c3d 2069  ]["Volume"] <= i
-00025c30: 6e74 2864 6174 612e 696c 6f63 5b31 5d5b  nt(data.iloc[1][
-00025c40: 2256 6f6c 756d 6522 5d20 2a20 302e 3735  "Volume"] * 0.75
-00025c50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00025c60: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
-00025c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025c80: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-00025c90: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
-00025ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025cb0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-00025cc0: 305d 200d 0a20 2020 2020 2020 2020 2020  0] ..           
-00025cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ce0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00025cf0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-00025d00: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00025d10: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-00025d20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025d30: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00025d40: 2253 7570 706c 7920 4472 6f75 6768 7422  "Supply Drought"
-00025d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025d60: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00025d70: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00025b40: 2020 2020 7370 7265 6164 3020 3e20 7370      spread0 > sp
+00025b50: 7265 6164 310d 0a20 2020 2020 2020 2020  read1..         
+00025b60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00025b70: 6e64 2076 6f6c 3020 3c20 766f 6c31 0d0a  nd vol0 < vol1..
+00025b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b90: 2020 2020 2020 2020 616e 6420 6461 7461          and data
+00025ba0: 2e69 6c6f 635b 305d 5b22 566f 6c75 6d65  .iloc[0]["Volume
+00025bb0: 225d 203c 2064 6174 612e 696c 6f63 5b30  "] < data.iloc[0
+00025bc0: 5d5b 2256 6f6c 4d41 225d 0d0a 2020 2020  ]["VolMA"]..    
+00025bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025be0: 2020 2020 616e 6420 6461 7461 2e69 6c6f      and data.ilo
+00025bf0: 635b 305d 5b22 436c 6f73 6522 5d20 3c3d  c[0]["Close"] <=
+00025c00: 2064 6174 612e 696c 6f63 5b31 5d5b 224f   data.iloc[1]["O
+00025c10: 7065 6e22 5d0d 0a20 2020 2020 2020 2020  pen"]..         
+00025c20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00025c30: 6e64 2073 7072 6561 6430 203c 206c 6f77  nd spread0 < low
+00025c40: 6572 5f77 6963 6b5f 7370 7265 6164 300d  er_wick_spread0.
+00025c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025c60: 2020 2020 2020 2020 2061 6e64 2064 6174           and dat
+00025c70: 612e 696c 6f63 5b30 5d5b 2256 6f6c 756d  a.iloc[0]["Volum
+00025c80: 6522 5d20 3c3d 2069 6e74 2864 6174 612e  e"] <= int(data.
+00025c90: 696c 6f63 5b31 5d5b 2256 6f6c 756d 6522  iloc[1]["Volume"
+00025ca0: 5d20 2a20 302e 3735 290d 0a20 2020 2020  ] * 0.75)..     
+00025cb0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00025cc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00025cd0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+00025ce0: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+00025cf0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00025d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d10: 2020 7361 7665 645b 305d 200d 0a20 2020    saved[0] ..   
+00025d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d30: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00025d40: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
+00025d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d60: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+00025d70: 7874 2e47 5245 454e 0d0a 2020 2020 2020  xt.GREEN..      
 00025d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00025da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025db0: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
-00025dc0: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
-00025dd0: 202b 2022 5375 7070 6c79 2044 726f 7567   + "Supply Droug
-00025de0: 6874 220d 0a20 2020 2020 2020 2020 2020  ht"..           
-00025df0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00025e00: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
-00025e10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00025e20: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00025e30: 2020 2020 2020 2020 2020 2020 7370 7265              spre
-00025e40: 6164 3020 3c20 7370 7265 6164 310d 0a20  ad0 < spread1.. 
-00025e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e60: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
-00025e70: 3e20 766f 6c31 0d0a 2020 2020 2020 2020  > vol1..        
+00025d90: 2020 2020 2020 2b20 2253 7570 706c 7920        + "Supply 
+00025da0: 4472 6f75 6768 7422 0d0a 2020 2020 2020  Drought"..      
+00025db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025dc0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00025dd0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+00025de0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00025df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025e00: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00025e10: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+00025e20: 7361 7665 645b 315d 202b 2022 5375 7070  saved[1] + "Supp
+00025e30: 6c79 2044 726f 7567 6874 220d 0a20 2020  ly Drought"..   
+00025e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e50: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00025e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025e70: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
 00025e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e90: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
-00025ea0: 5b22 566f 6c75 6d65 225d 203e 2064 6174  ["Volume"] > dat
-00025eb0: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
-00025ec0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00025ed0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00025ee0: 6461 7461 2e69 6c6f 635b 305d 5b22 436c  data.iloc[0]["Cl
-00025ef0: 6f73 6522 5d20 3c3d 2064 6174 612e 696c  ose"] <= data.il
-00025f00: 6f63 5b31 5d5b 224f 7065 6e22 5d0d 0a20  oc[1]["Open"].. 
-00025f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f20: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-00025f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00025f40: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
-00025f50: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
-00025f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f70: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
-00025f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025f90: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-00025fa0: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
-00025fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025fc0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00025fd0: 6f72 5465 7874 2e47 5245 454e 0d0a 2020  orText.GREEN..  
+00025e90: 2020 2020 7370 7265 6164 3020 3c20 7370      spread0 < sp
+00025ea0: 7265 6164 310d 0a20 2020 2020 2020 2020  read1..         
+00025eb0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00025ec0: 6e64 2076 6f6c 3020 3e20 766f 6c31 0d0a  nd vol0 > vol1..
+00025ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ee0: 2020 2020 2020 2020 616e 6420 6461 7461          and data
+00025ef0: 2e69 6c6f 635b 305d 5b22 566f 6c75 6d65  .iloc[0]["Volume
+00025f00: 225d 203e 2064 6174 612e 696c 6f63 5b30  "] > data.iloc[0
+00025f10: 5d5b 2256 6f6c 4d41 225d 0d0a 2020 2020  ]["VolMA"]..    
+00025f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f30: 2020 2020 616e 6420 6461 7461 2e69 6c6f      and data.ilo
+00025f40: 635b 305d 5b22 436c 6f73 6522 5d20 3c3d  c[0]["Close"] <=
+00025f50: 2064 6174 612e 696c 6f63 5b31 5d5b 224f   data.iloc[1]["O
+00025f60: 7065 6e22 5d0d 0a20 2020 2020 2020 2020  pen"]..         
+00025f70: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
+00025f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f90: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00025fa0: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+00025fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025fc0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00025fd0: 7665 645b 305d 200d 0a20 2020 2020 2020  ved[0] ..       
 00025fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ff0: 2020 2020 2020 2020 2020 2b20 2244 656d            + "Dem
-00026000: 616e 6420 5269 7365 220d 0a20 2020 2020  and Rise"..     
+00025ff0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+00026000: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
 00026010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026020: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00026030: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+00026020: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
+00026030: 5245 454e 0d0a 2020 2020 2020 2020 2020  REEN..          
 00026040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026050: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00026060: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00026070: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-00026080: 2073 6176 6564 5b31 5d20 2b20 2244 656d   saved[1] + "Dem
-00026090: 616e 6420 5269 7365 220d 0a20 2020 2020  and Rise"..     
-000260a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000260b0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-000260c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000260d0: 7074 2049 6e64 6578 4572 726f 7220 6173  pt IndexError as
-000260e0: 2065 3a20 2320 7072 6167 6d61 3a20 6e6f   e: # pragma: no
-000260f0: 2063 6f76 6572 0d0a 2020 2020 2020 2020   cover..        
-00026100: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
-00026110: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
-00026120: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
-00026130: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00026140: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-00026150: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00026160: 6c73 650d 0a20 2020 2020 2020 2065 7863  lse..        exc
-00026170: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00026180: 2065 3a20 2023 2070 7261 676d 613a 206e   e:  # pragma: n
-00026190: 6f20 636f 7665 720d 0a20 2020 2020 2020  o cover..       
-000261a0: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-000261b0: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
-000261c0: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
-000261d0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000261e0: 7475 726e 2046 616c 7365 0d0a            turn False..
+00026050: 2020 2b20 2244 656d 616e 6420 5269 7365    + "Demand Rise
+00026060: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00026070: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00026080: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
+00026090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000260a0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+000260b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000260c0: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
+000260d0: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
+000260e0: 5d20 2b20 2244 656d 616e 6420 5269 7365  ] + "Demand Rise
+000260f0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00026100: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00026110: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
+00026120: 2020 2020 6578 6365 7074 2049 6e64 6578      except Index
+00026130: 4572 726f 7220 6173 2065 3a20 2320 7072  Error as e: # pr
+00026140: 6167 6d61 3a20 6e6f 2063 6f76 6572 0d0a  agma: no cover..
+00026150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026160: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+00026170: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
+00026180: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
+00026190: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000261a0: 730d 0a20 2020 2020 2020 2020 2020 2072  s..            r
+000261b0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+000261c0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000261d0: 7074 696f 6e20 6173 2065 3a20 2023 2070  ption as e:  # p
+000261e0: 7261 676d 613a 206e 6f20 636f 7665 720d  ragma: no cover.
+000261f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00026200: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+00026210: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
+00026220: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
+00026230: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00026240: 7365 0d0a                                se..
```

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,15 +812,16 @@
             except Exception as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
         else:
             OutputControls().printOutput(
                 colorText.BOLD + colorText.GREEN + "=> Already Cached." + colorText.END
             )
             if downloadOnly:
-                    OutputControls().printOutput(colorText.BOLD + colorText.GREEN + f"=> {cache_file}" + colorText.END)
+                OutputControls().printOutput(colorText.BOLD + colorText.GREEN + f"=> {cache_file}" + colorText.END)
+        return cache_file
 
     def downloadLatestData(stockDict,configManager,stockCodes=[],exchangeSuffix=".NS",downloadOnly=False):
         numStocksPerIteration = (int(len(stockCodes)/int(len(stockCodes)/10)) if len(stockCodes) >= 10 else len(stockCodes)) + 1
         queueCounter = 0
         iterations = int(len(stockCodes)/numStocksPerIteration) + 1
         tasksList = []
         while queueCounter < iterations:
@@ -1040,15 +1041,15 @@
         if resp is not None and resp.status_code == 200:
             contentLength = resp.headers.get("content-length")
             serverBytes = int(contentLength) if contentLength is not None else 0
             KB = 1024
             MB = KB * 1024
             chunksize = MB if serverBytes >= MB else (KB if serverBytes >= KB else 1)
             filesize = int( serverBytes / chunksize)
-            if filesize > 0 and chunksize == MB: # Saved data can't be in KBs. Something definitely went wrong.
+            if filesize > 40 and chunksize == MB: # Saved data can't be in KBs. Something definitely went wrong. It should be upward of 40MB
                 bar, spinner = tools.getProgressbarStyle()
                 try:
                     f = open(
                             os.path.join(Archiver.get_user_outputs_dir(), cache_file),
                             "w+b",
                         )  # .split(os.sep)[-1]
                     dl = 0
@@ -1116,15 +1117,15 @@
                         sys.stdout.write("\x1b[2K")  # delete the last line
                 except Exception as e:  # pragma: no cover
                     default_logger().debug(e, exc_info=True)
                     f.close()
                     OutputControls().printOutput("[!] Download Error - " + str(e))
             else:
                 default_logger().debug(
-                        f"Stock data cache file:{cache_file} on server has length ->{filesize}{chunksize}"
+                        f"Stock data cache file:{cache_file} on server has length ->{filesize} {'Mb' if chunksize >= MB else ('Kb' if chunksize >= KB else 'bytes')}"
                     )
             if not retrial and not stockDataLoaded:
                     # Don't try for more than once.
                 stockDict = tools.loadStockData(
                         stockDict,
                         configManager,
                         downloadOnly,
```

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/classes/keys.py` & `pkscreener-0.45.20240521.389/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/courbd.ttf` & `pkscreener-0.45.20240521.389/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/globals.py` & `pkscreener-0.45.20240521.389/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -2632,15 +2632,29 @@
             + colorText.GREEN
             + "[+] Caching Stock Data for future use, Please Wait... "
             + colorText.END,
             end="",
         )
         Utility.tools.saveStockData(stockDictPrimary, configManager, loadCount, intraday)
         if downloadOnly:
-            Utility.tools.saveStockData(stockDictPrimary, configManager, loadCount, intraday, downloadOnly=downloadOnly)
+            cache_file = Utility.tools.saveStockData(stockDictPrimary, configManager, loadCount, intraday, downloadOnly=downloadOnly)
+            cacheFileSize = os.stat(cache_file).st_size if os.path.exists(cache_file) else 0
+            if cacheFileSize < 1024*1024*50:
+                try:
+                    from PKDevTools.classes import Archiver
+                    log_file_path = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
+                    message=f"{cache_file} has size: {cacheFileSize}! Something is wrong!"
+                    if os.path.exists(log_file_path):
+                        sendMessageToTelegramChannel(caption=message,document_filePath=log_file_path, user="-1001785195297")
+                    else:
+                        sendMessageToTelegramChannel(message=message,user="-1001785195297")
+                except:
+                    pass
+                # Let's try again with logging
+                os.system(f"{sys.argv[0]} -a Y -e -l -d {'-i 1m' if configManager.isIntradayConfig() else ''}")
     else:
         OutputControls().printOutput(colorText.BOLD + colorText.GREEN + "[+] Skipped Saving!" + colorText.END)
 
 
 def saveNotifyResultsFile(
     screenResults, saveResults, defaultAnswer, menuChoiceHierarchy, user=None
 ):
```

### Comparing `pkscreener-0.45.20240521.388/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240521.389/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240521.389/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240521.389/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240521.389/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.388
+Version: 0.45.20240521.389
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.388.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.389.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -112,14 +112,19 @@
     15 > 52 week low breakout(today/1 wk)	16 > 10 days low breakout
     17 > 52 week high breakout(today/1 wk)	18 > Bullish Aroon(14) Crossover
     19 > MACD Histogram x below 0       	20 > Bullish for next day
     21 > Most Popular Stocks            	22 > View Stock Performance         
     23 > Breaking out now               	24 > Higher Highs,Lows & Close      
     25 > Lower Highs,Lows (Watch for Reversal)            	
 ```
+## Running Piped Scanners
+
+https://github.com/pkjmesra/PKScreener/assets/1358101/9e579371-1035-400a-9f65-139d8407f6c7
+
+
 ## How to use on your own local Windows/Linux/Macbook laptop?
 
 # Using docker, running within docker container
 * Download and install docker desktop: https://docs.docker.com/get-docker/
 * After installation, launch/run docker desktop and if it asks, login using your docker credentials.
 * Launch any command line (for example, cmd on windows or terminal on Mac) and type `docker pull pkjmesra/pkscreener:latest`. Then type `docker run -it pkjmesra/pkscreener:latest`.  
   The option `-i` will open the `pkscreener` in interactive mode within docker. `-t` will allocate a pseudo terminal for you so you can begin to use `pkscreener`
@@ -269,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.387/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.388/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240521.388/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240521.389/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.388/setup.py` & `pkscreener-0.45.20240521.389/setup.py`

 * *Files identical despite different names*

