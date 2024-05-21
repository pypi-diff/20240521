# Comparing `tmp/loopies-scraper-0.0.3.tar.gz` & `tmp/loopies-scraper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopies-scraper-0.0.3.tar", last modified: Tue May 21 19:00:09 2024, max compression
+gzip compressed data, was "loopies-scraper-0.0.4.tar", last modified: Tue May 21 19:07:47 2024, max compression
```

## Comparing `loopies-scraper-0.0.3.tar` & `loopies-scraper-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 19:00:09.797750 loopies-scraper-0.0.3/
--rw-rw-rw-   0        0        0     1056 2024-05-11 13:52:55.000000 loopies-scraper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      650 2024-05-21 19:00:09.797750 loopies-scraper-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        9 2024-05-11 13:52:56.000000 loopies-scraper-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 19:00:09.789750 loopies-scraper-0.0.3/loopies_scraper/
--rw-rw-rw-   0        0        0      498 2024-05-21 18:50:38.000000 loopies-scraper-0.0.3/loopies_scraper/__init__.py
--rw-rw-rw-   0        0        0     1975 2024-05-21 18:57:56.000000 loopies-scraper-0.0.3/loopies_scraper/chromedriver_options.py
--rw-rw-rw-   0        0        0     1659 2024-05-19 17:43:25.000000 loopies-scraper-0.0.3/loopies_scraper/data_manager.py
--rw-rw-rw-   0        0        0     1396 2024-05-21 18:58:04.000000 loopies-scraper-0.0.3/loopies_scraper/geckodriver_profile.py
--rw-rw-rw-   0        0        0      294 2024-05-21 18:58:41.000000 loopies-scraper-0.0.3/loopies_scraper/scraper.py
--rw-rw-rw-   0        0        0     4364 2024-05-21 18:58:36.000000 loopies-scraper-0.0.3/loopies_scraper/scraper_multiprocess.py
--rw-rw-rw-   0        0        0     1314 2024-05-21 18:58:54.000000 loopies-scraper-0.0.3/loopies_scraper/user_agent_generator.py
--rw-rw-rw-   0        0        0     2302 2024-05-21 18:59:00.000000 loopies-scraper-0.0.3/loopies_scraper/webdriver_controller.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:00:09.796750 loopies-scraper-0.0.3/loopies_scraper.egg-info/
--rw-rw-rw-   0        0        0      650 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-21 19:00:09.000000 loopies-scraper-0.0.3/loopies_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 19:00:09.797750 loopies-scraper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-21 19:00:01.000000 loopies-scraper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:07:47.731373 loopies-scraper-0.0.4/
+-rw-rw-rw-   0        0        0     1056 2024-05-11 13:52:55.000000 loopies-scraper-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      650 2024-05-21 19:07:47.731373 loopies-scraper-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2024-05-11 13:52:56.000000 loopies-scraper-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 19:07:47.724373 loopies-scraper-0.0.4/loopies_scraper/
+-rw-rw-rw-   0        0        0      498 2024-05-21 18:50:38.000000 loopies-scraper-0.0.4/loopies_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1975 2024-05-21 18:57:56.000000 loopies-scraper-0.0.4/loopies_scraper/chromedriver_options.py
+-rw-rw-rw-   0        0        0     1659 2024-05-19 17:43:25.000000 loopies-scraper-0.0.4/loopies_scraper/data_manager.py
+-rw-rw-rw-   0        0        0     1396 2024-05-21 18:58:04.000000 loopies-scraper-0.0.4/loopies_scraper/geckodriver_profile.py
+-rw-rw-rw-   0        0        0      294 2024-05-21 18:58:41.000000 loopies-scraper-0.0.4/loopies_scraper/scraper.py
+-rw-rw-rw-   0        0        0     4364 2024-05-21 18:58:36.000000 loopies-scraper-0.0.4/loopies_scraper/scraper_multiprocess.py
+-rw-rw-rw-   0        0        0     1314 2024-05-21 18:58:54.000000 loopies-scraper-0.0.4/loopies_scraper/user_agent_generator.py
+-rw-rw-rw-   0        0        0     2304 2024-05-21 19:06:53.000000 loopies-scraper-0.0.4/loopies_scraper/webdriver_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:07:47.730373 loopies-scraper-0.0.4/loopies_scraper.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-05-21 19:07:47.000000 loopies-scraper-0.0.4/loopies_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2024-05-21 19:07:47.000000 loopies-scraper-0.0.4/loopies_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:07:47.000000 loopies-scraper-0.0.4/loopies_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-21 19:07:47.000000 loopies-scraper-0.0.4/loopies_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-21 19:07:47.000000 loopies-scraper-0.0.4/loopies_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 19:07:47.731373 loopies-scraper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-21 19:07:18.000000 loopies-scraper-0.0.4/setup.py
```

### Comparing `loopies-scraper-0.0.3/LICENSE` & `loopies-scraper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.3/PKG-INFO` & `loopies-scraper-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopies-scraper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Web scraper for basic and/or list of pages scraping
 Author: tmspsk
 Keywords: python,scraper,multiprocess scraper,list,selenium webdriver
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `loopies-scraper-0.0.3/loopies_scraper/chromedriver_options.py` & `loopies-scraper-0.0.4/loopies_scraper/chromedriver_options.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.3/loopies_scraper/data_manager.py` & `loopies-scraper-0.0.4/loopies_scraper/data_manager.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.3/loopies_scraper/geckodriver_profile.py` & `loopies-scraper-0.0.4/loopies_scraper/geckodriver_profile.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.3/loopies_scraper/scraper_multiprocess.py` & `loopies-scraper-0.0.4/loopies_scraper/scraper_multiprocess.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.3/loopies_scraper/user_agent_generator.py` & `loopies-scraper-0.0.4/loopies_scraper/user_agent_generator.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.3/loopies_scraper/webdriver_controller.py` & `loopies-scraper-0.0.4/loopies_scraper/webdriver_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python
 import time, os
 from sys import platform
 from selenium import webdriver
-from geckodriver_profile import GeckodriverProfile
-from chromedriver_options import ChromedriverOptions
+from .geckodriver_profile import GeckodriverProfile
+from .chromedriver_options import ChromedriverOptions
 
 class WebDriverController:
 	driver: object = None
 
 	def __init__(self, driver_name: str, proxy: str = None) -> None:
 		if driver_name == "firefox":
 			path = None
```

### Comparing `loopies-scraper-0.0.3/loopies_scraper.egg-info/PKG-INFO` & `loopies-scraper-0.0.4/loopies_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopies-scraper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Web scraper for basic and/or list of pages scraping
 Author: tmspsk
 Keywords: python,scraper,multiprocess scraper,list,selenium webdriver
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `loopies-scraper-0.0.3/setup.py` & `loopies-scraper-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Web scraper for basic and/or list of pages scraping'
 LONG_DESCRIPTION = 'Wrapper for Selenium WebDriver and its configuration to turn it into web scraper to scrape list of pages or to use it as prebuilt scraper'
 
 # Setting up
 setup(
     name="loopies-scraper",
     version=VERSION,
```

