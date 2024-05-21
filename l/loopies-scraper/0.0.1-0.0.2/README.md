# Comparing `tmp/loopies-scraper-0.0.1.tar.gz` & `tmp/loopies-scraper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopies-scraper-0.0.1.tar", last modified: Sat May 11 14:11:36 2024, max compression
+gzip compressed data, was "loopies-scraper-0.0.2.tar", last modified: Tue May 21 18:41:05 2024, max compression
```

## Comparing `loopies-scraper-0.0.1.tar` & `loopies-scraper-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 14:11:36.303799 loopies-scraper-0.0.1/
--rw-rw-rw-   0        0        0     1056 2024-05-11 13:52:55.000000 loopies-scraper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      650 2024-05-11 14:11:36.303799 loopies-scraper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        9 2024-05-11 13:52:56.000000 loopies-scraper-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 14:11:36.294290 loopies-scraper-0.0.1/loopies_scraper/
--rw-rw-rw-   0        0        0      428 2024-05-11 13:53:01.000000 loopies-scraper-0.0.1/loopies_scraper/__init__.py
--rw-rw-rw-   0        0        0     2094 2024-05-11 13:53:17.000000 loopies-scraper-0.0.1/loopies_scraper/chromedriver_options.py
--rw-rw-rw-   0        0        0     1664 2024-05-11 12:03:02.000000 loopies-scraper-0.0.1/loopies_scraper/data_manager.py
--rw-rw-rw-   0        0        0     1395 2024-05-11 14:02:00.000000 loopies-scraper-0.0.1/loopies_scraper/geckodriver_profile.py
--rw-rw-rw-   0        0        0      568 2024-05-11 14:01:58.000000 loopies-scraper-0.0.1/loopies_scraper/scraper.py
--rw-rw-rw-   0        0        0      767 2024-05-11 14:02:20.000000 loopies-scraper-0.0.1/loopies_scraper/test.py
--rw-rw-rw-   0        0        0     1314 2024-05-11 14:01:56.000000 loopies-scraper-0.0.1/loopies_scraper/user_agent_generator.py
--rw-rw-rw-   0        0        0     2436 2024-05-11 11:54:55.000000 loopies-scraper-0.0.1/loopies_scraper/webdriver_controller.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:11:36.302799 loopies-scraper-0.0.1/loopies_scraper.egg-info/
--rw-rw-rw-   0        0        0      650 2024-05-11 14:11:36.000000 loopies-scraper-0.0.1/loopies_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2024-05-11 14:11:36.000000 loopies-scraper-0.0.1/loopies_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 14:11:36.000000 loopies-scraper-0.0.1/loopies_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-11 14:11:36.000000 loopies-scraper-0.0.1/loopies_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-11 14:11:36.000000 loopies-scraper-0.0.1/loopies_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 14:11:36.303799 loopies-scraper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1036 2024-05-11 14:11:33.000000 loopies-scraper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:41:05.274978 loopies-scraper-0.0.2/
+-rw-rw-rw-   0        0        0     1056 2024-05-11 13:52:55.000000 loopies-scraper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      650 2024-05-21 18:41:05.274978 loopies-scraper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2024-05-11 13:52:56.000000 loopies-scraper-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 18:41:05.262474 loopies-scraper-0.0.2/loopies_scraper/
+-rw-rw-rw-   0        0        0      498 2024-05-21 10:31:31.000000 loopies-scraper-0.0.2/loopies_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1974 2024-05-21 11:44:33.000000 loopies-scraper-0.0.2/loopies_scraper/chromedriver_options.py
+-rw-rw-rw-   0        0        0     1659 2024-05-19 17:43:25.000000 loopies-scraper-0.0.2/loopies_scraper/data_manager.py
+-rw-rw-rw-   0        0        0     1395 2024-05-21 11:26:01.000000 loopies-scraper-0.0.2/loopies_scraper/geckodriver_profile.py
+-rw-rw-rw-   0        0        0      293 2024-05-21 11:34:49.000000 loopies-scraper-0.0.2/loopies_scraper/scraper.py
+-rw-rw-rw-   0        0        0     4362 2024-05-21 11:07:24.000000 loopies-scraper-0.0.2/loopies_scraper/scraper_multiprocess.py
+-rw-rw-rw-   0        0        0     1314 2024-05-11 14:01:56.000000 loopies-scraper-0.0.2/loopies_scraper/user_agent_generator.py
+-rw-rw-rw-   0        0        0     2302 2024-05-21 15:44:45.000000 loopies-scraper-0.0.2/loopies_scraper/webdriver_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:41:05.273475 loopies-scraper-0.0.2/loopies_scraper.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-21 18:41:05.000000 loopies-scraper-0.0.2/loopies_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 18:41:05.274978 loopies-scraper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-21 18:40:24.000000 loopies-scraper-0.0.2/setup.py
```

### Comparing `loopies-scraper-0.0.1/LICENSE` & `loopies-scraper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.1/PKG-INFO` & `loopies-scraper-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopies-scraper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Web scraper for basic and/or list of pages scraping
 Author: tmspsk
 Keywords: python,scraper,multiprocess scraper,list,selenium webdriver
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `loopies-scraper-0.0.1/loopies_scraper/chromedriver_options.py` & `loopies-scraper-0.0.2/loopies_scraper/chromedriver_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 			self.chrome_options = ChromeOptions()
 			self.chrome_options.add_argument('--no-sandbox')
 			self.chrome_options.add_argument('--disable-dev-shm-usage')
 			self.chrome_options.add_argument('--disable-notifications')
 			self.chrome_options.add_argument('--ignore-certificate-errors')
 			self.chrome_options.add_argument('--disable-infobars')
 			self.chrome_options.add_argument('--webhooks-notification-dismissed=true')
-			self.chrome_options.add_argument('--user-data=C:\\Users\\user\\AppData\\Local\\Google\\Chrome\\User Data\\Default')
 			self.chrome_options.add_argument("--disable-popup-blocking")
 			user_agent = UserAgentGenerator().user_agent
 			self.chrome_options.add_argument(f'--user-agent={user_agent}')
 		elif proxy == 'tor':
 			self.chrome_options = ChromeOptions()
 			self.chrome_options.add_argument('--no-sandbox')
 			self.chrome_options.add_argument('--disable-dev-shm-usage')
```

### Comparing `loopies-scraper-0.0.1/loopies_scraper/data_manager.py` & `loopies-scraper-0.0.2/loopies_scraper/data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def ready_to_get_url(self):
         while self.queue_status.value is QueueStatus.NOT_STARTED.value:
             print(f"urls queue status: {self.queue_status.value}, sleeping for 5s...")
             time.sleep(5)
 
         while self.queue_status.value is QueueStatus.STARTED.value:
-            if not self.urls_queue.empty():
+            if not self.queue.empty():
                 return True
             else:
                 print(f"urls queue status: {self.queue_status.value}, urls queue is empty, sleeping for 5s...")
                 time.sleep(5)
         
         if self.queue_status.value is QueueStatus.DONE.value:
             if not self.queue.empty():
```

### Comparing `loopies-scraper-0.0.1/loopies_scraper/geckodriver_profile.py` & `loopies-scraper-0.0.2/loopies_scraper/geckodriver_profile.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.1/loopies_scraper/user_agent_generator.py` & `loopies-scraper-0.0.2/loopies_scraper/user_agent_generator.py`

 * *Files identical despite different names*

### Comparing `loopies-scraper-0.0.1/loopies_scraper/webdriver_controller.py` & `loopies-scraper-0.0.2/loopies_scraper/webdriver_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,32 +13,27 @@
 			path = None
 			if platform == "linux":
 				path = os.path.normpath(f'{os.getcwd()}/webdrivers/geckodriver')
 			if platform == "win32":
 				path = os.path.normpath(f'{os.getcwd()}/webdrivers/geckodriver.exe')
 			if path is not None:
 				geckodriver_profile = GeckodriverProfile(proxy=proxy)
-				self.driver = webdriver.Firefox(firefox_profile=geckodriver_profile.firefox_profile)
+				self.driver = webdriver.Firefox(executable_path=path, firefox_profile=geckodriver_profile.firefox_profile)
 				self.driver.set_window_position(0, 0)
 				self.driver.set_window_size(1920, 1080)
 
-		# google-chrome 
-		# --remote-debugging-port=9222 
-		# --user-data-dir=remote-profile 
-		# --proxy-server="socks5://127.0.0.1:9050"
 		if driver_name == "chrome":
 			path = None
 			if platform == "linux":
 				path = os.path.normpath(f'{os.getcwd()}/webdrivers/chromedriver')
 			if platform == "win32":
 				path = os.path.normpath(f'{os.getcwd()}/webdrivers/chromedriver.exe')
 			if path is not None:
 				chromedriver_options = ChromedriverOptions(proxy=proxy)
-				self.driver = webdriver.Chrome(options=chromedriver_options.chrome_options)
-				# self.driver = webdriver.Chrome()
+				self.driver = webdriver.Chrome(executable_path=path, options=chromedriver_options.chrome_options)
 				self.driver.set_window_position(0, 0)
 				self.driver.set_window_size(1920, 1080)
 		
 	def scroll_to_element(self, element):
 		location = element.location
 		window_size = self.driver.get_window_size()
 		options = {
```

### Comparing `loopies-scraper-0.0.1/loopies_scraper.egg-info/PKG-INFO` & `loopies-scraper-0.0.2/loopies_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopies-scraper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Web scraper for basic and/or list of pages scraping
 Author: tmspsk
 Keywords: python,scraper,multiprocess scraper,list,selenium webdriver
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `loopies-scraper-0.0.1/setup.py` & `loopies-scraper-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Web scraper for basic and/or list of pages scraping'
 LONG_DESCRIPTION = 'Wrapper for Selenium WebDriver and its configuration to turn it into web scraper to scrape list of pages or to use it as prebuilt scraper'
 
 # Setting up
 setup(
     name="loopies-scraper",
     version=VERSION,
     author="tmspsk",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests*"]),
     install_requires=['selenium', 'fake_useragent'],
     keywords=['python', 'scraper', 'multiprocess scraper', 'list', 'selenium webdriver'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

