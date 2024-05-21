# Comparing `tmp/loopies-scraper-0.0.2.tar.gz` & `tmp/loopies-scraper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopies-scraper-0.0.2.tar", last modified: Tue May 21 18:41:05 2024, max compression
+gzip compressed data, was "loopies-scraper-0.0.3.tar", last modified: Tue May 21 19:00:09 2024, max compression
```

## Comparing `loopies-scraper-0.0.2.tar` & `loopies-scraper-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 18:41:05.274978 loopies-scraper-0.0.2/
--rw-rw-rw-   0        0        0     1056 2024-05-11 13:52:55.000000 loopies-scraper-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      650 2024-05-21 18:41:05.274978 loopies-scraper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2024-05-11 13:52:56.000000 loopies-scraper-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 18:41:05.262474 loopies-scraper-0.0.2/loopies_scraper/
--rw-rw-rw-   0        0        0      498 2024-05-21 10:31:31.000000 loopies-scraper-0.0.2/loopies_scraper/__init__.py
--rw-rw-rw-   0        0        0     1974 2024-05-21 11:44:33.000000 loopies-scraper-0.0.2/loopies_scraper/chromedriver_options.py
--rw-rw-rw-   0        0        0     1659 2024-05-19 17:43:25.000000 loopies-scraper-0.0.2/loopies_scraper/data_manager.py
--rw-rw-rw-   0        0        0     1395 2024-05-21 11:26:01.000000 loopies-scraper-0.0.2/loopies_scraper/geckodriver_profile.py
--rw-rw-rw-   0        0        0      293 2024-05-21 11:34:49.000000 loopies-scraper-0.0.2/loopies_scraper/scraper.py
--rw-rw-rw-   0        0        0     4362 2024-05-21 11:07:24.000000 loopies-scraper-0.0.2/loopies_scraper/scraper_multiprocess.py
--rw-rw-rw-   0        0        0     1314 2024-05-11 14:01:56.000000 loopies-scraper-0.0.2/loopies_scraper/user_agent_generator.py
--rw-rw-rw-   0        0        0     2302 2024-05-21 15:44:45.000000 loopies-scraper-0.0.2/loopies_scraper/webdriver_controller.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:41:05.273475 loopies-scraper-0.0.2/loopies_scraper.egg-info/
--rw-rw-rw-   0        0        0      650 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 18:41:05.274978 loopies-scraper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-21 18:40:24.000000 loopies-scraper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:00:09.797750 loopies-scraper-0.0.3/
+-rw-rw-rw-   0        0        0     1056 2024-05-11 13:52:55.000000 loopies-scraper-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      650 2024-05-21 19:00:09.797750 loopies-scraper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2024-05-11 13:52:56.000000 loopies-scraper-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 19:00:09.789750 loopies-scraper-0.0.3/loopies_scraper/
+-rw-rw-rw-   0        0        0      498 2024-05-21 18:50:38.000000 loopies-scraper-0.0.3/loopies_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1975 2024-05-21 18:57:56.000000 loopies-scraper-0.0.3/loopies_scraper/chromedriver_options.py
+-rw-rw-rw-   0        0        0     1659 2024-05-19 17:43:25.000000 loopies-scraper-0.0.3/loopies_scraper/data_manager.py
+-rw-rw-rw-   0        0        0     1396 2024-05-21 18:58:04.000000 loopies-scraper-0.0.3/loopies_scraper/geckodriver_profile.py
+-rw-rw-rw-   0        0        0      294 2024-05-21 18:58:41.000000 loopies-scraper-0.0.3/loopies_scraper/scraper.py
+-rw-rw-rw-   0        0        0     4364 2024-05-21 18:58:36.000000 loopies-scraper-0.0.3/loopies_scraper/scraper_multiprocess.py
+-rw-rw-rw-   0        0        0     1314 2024-05-21 18:58:54.000000 loopies-scraper-0.0.3/loopies_scraper/user_agent_generator.py
+-rw-rw-rw-   0        0        0     2302 2024-05-21 18:59:00.000000 loopies-scraper-0.0.3/loopies_scraper/webdriver_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:00:09.796750 loopies-scraper-0.0.3/loopies_scraper.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 19:00:09.797750 loopies-scraper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-21 19:00:01.000000 loopies-scraper-0.0.3/setup.py
```

### Comparing `loopies-scraper-0.0.2/LICENSE` & `loopies-scraper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.2/PKG-INFO` & `loopies-scraper-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopies-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Web scraper for basic and/or list of pages scraping
 Author: tmspsk
 Keywords: python,scraper,multiprocess scraper,list,selenium webdriver
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `loopies-scraper-0.0.2/loopies_scraper/chromedriver_options.py` & `loopies-scraper-0.0.3/loopies_scraper/chromedriver_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 from selenium.webdriver.chrome.options import Options as ChromeOptions
-from user_agent_generator import UserAgentGenerator
+from .user_agent_generator import UserAgentGenerator
 
 class ChromedriverOptions:
 	chrome_options: ChromeOptions = None
 	
 	def __init__(self, proxy: str = None) -> None:
 		if proxy == None:
 			self.chrome_options = ChromeOptions()
```

### Comparing `loopies-scraper-0.0.2/loopies_scraper/data_manager.py` & `loopies-scraper-0.0.3/loopies_scraper/data_manager.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.2/loopies_scraper/geckodriver_profile.py` & `loopies-scraper-0.0.3/loopies_scraper/geckodriver_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 from selenium.webdriver.firefox.firefox_profile import FirefoxProfile
-from user_agent_generator import UserAgentGenerator
+from .user_agent_generator import UserAgentGenerator
 
 class GeckodriverProfile:
 	firefox_profile: FirefoxProfile = None
 	
 	def __init__(self, proxy: str = None) -> None:
 		if proxy == None:
 			self.firefox_profile = FirefoxProfile()
```

### Comparing `loopies-scraper-0.0.2/loopies_scraper/scraper_multiprocess.py` & `loopies-scraper-0.0.3/loopies_scraper/scraper_multiprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 import multiprocessing, json
 from functools import lru_cache 
-from data_manager import DataManager, QueueStatus
-from scraper import Scraper
+from .data_manager import DataManager, QueueStatus
+from .scraper import Scraper
 import os, json
 
 class MultiprocessScraper():
     def __init__(self, driver_name: str = None, proxy: str = None, processes_count: int = 1, file_path: str = './data.json') -> None:
         self.processes_count = processes_count
         self.driver_name = driver_name
         self.proxy = proxy
```

### Comparing `loopies-scraper-0.0.2/loopies_scraper/user_agent_generator.py` & `loopies-scraper-0.0.3/loopies_scraper/user_agent_generator.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.2/loopies_scraper/webdriver_controller.py` & `loopies-scraper-0.0.3/loopies_scraper/webdriver_controller.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.2/loopies_scraper.egg-info/PKG-INFO` & `loopies-scraper-0.0.3/loopies_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopies-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Web scraper for basic and/or list of pages scraping
 Author: tmspsk
 Keywords: python,scraper,multiprocess scraper,list,selenium webdriver
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `loopies-scraper-0.0.2/setup.py` & `loopies-scraper-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Web scraper for basic and/or list of pages scraping'
 LONG_DESCRIPTION = 'Wrapper for Selenium WebDriver and its configuration to turn it into web scraper to scrape list of pages or to use it as prebuilt scraper'
 
 # Setting up
 setup(
     name="loopies-scraper",
     version=VERSION,
```

