# Comparing `tmp/wawona-1.2.0.tar.gz` & `tmp/wawona-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wawona-1.2.0.tar", last modified: Mon May 20 12:45:40 2024, max compression
+gzip compressed data, was "wawona-1.2.1.tar", last modified: Tue May 21 00:55:44 2024, max compression
```

## Comparing `wawona-1.2.0.tar` & `wawona-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-20 12:45:40.863347 wawona-1.2.0/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.2.0/LICENSE
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     5440 2024-05-20 12:45:40.862640 wawona-1.2.0/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     4327 2024-05-20 12:43:00.000000 wawona-1.2.0/README.md
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1132 2024-05-20 12:44:31.000000 wawona-1.2.0/pyproject.toml
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-05-20 12:45:40.863508 wawona-1.2.0/setup.cfg
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-20 12:45:40.852120 wawona-1.2.0/src/
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-20 12:45:40.856878 wawona-1.2.0/src/wawona/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.2.0/src/wawona/__init__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.2.0/src/wawona/__main__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)    22382 2024-05-20 12:43:00.000000 wawona-1.2.0/src/wawona/wawona.py
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-20 12:45:40.861935 wawona-1.2.0/src/wawona.egg-info/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     5440 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/SOURCES.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/dependency_links.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/entry_points.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       96 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/requires.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/top_level.txt
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-21 00:55:44.404984 wawona-1.2.1/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.2.1/LICENSE
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5440 2024-05-21 00:55:44.399581 wawona-1.2.1/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     4327 2024-05-20 12:43:00.000000 wawona-1.2.1/README.md
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1132 2024-05-21 00:55:21.000000 wawona-1.2.1/pyproject.toml
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-05-21 00:55:44.405232 wawona-1.2.1/setup.cfg
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-21 00:55:44.367219 wawona-1.2.1/src/
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-21 00:55:44.371763 wawona-1.2.1/src/wawona/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.2.1/src/wawona/__init__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.2.1/src/wawona/__main__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)    22566 2024-05-21 00:53:05.000000 wawona-1.2.1/src/wawona/wawona.py
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-21 00:55:44.393879 wawona-1.2.1/src/wawona.egg-info/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5440 2024-05-21 00:55:44.000000 wawona-1.2.1/src/wawona.egg-info/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-05-21 00:55:44.000000 wawona-1.2.1/src/wawona.egg-info/SOURCES.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-05-21 00:55:44.000000 wawona-1.2.1/src/wawona.egg-info/dependency_links.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-05-21 00:55:44.000000 wawona-1.2.1/src/wawona.egg-info/entry_points.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       96 2024-05-21 00:55:44.000000 wawona-1.2.1/src/wawona.egg-info/requires.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-05-21 00:55:44.000000 wawona-1.2.1/src/wawona.egg-info/top_level.txt
```

### Comparing `wawona-1.2.0/LICENSE` & `wawona-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wawona-1.2.0/PKG-INFO` & `wawona-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.2.0
+Version: 1.2.1
 Summary: Easily make office reservations in sequoia from the command line.
 Author-email: yuzawa-san <jtyuzawa+wawona@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
```

### Comparing `wawona-1.2.0/README.md` & `wawona-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wawona-1.2.0/pyproject.toml` & `wawona-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wawona"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="yuzawa-san", email="jtyuzawa+wawona@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Easily make office reservations in sequoia from the command line."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `wawona-1.2.0/src/wawona/wawona.py` & `wawona-1.2.1/src/wawona/wawona.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 
 import inquirer
 import keyring
 import pytz
 import requests
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 from texttable import Texttable
+from webdriver_manager.chrome import ChromeDriverManager
 
 config_path = "%s/.config/wawona" % os.environ["HOME"]
 config_file = "%s/config.json" % config_path
 
 TERMINAL_CHAR_ASPECT_RATIO = 8 / 10
 FLOOR_PLAN_BUFFER = 4
 FLOOR_PLAN_COLS = 120
@@ -87,15 +89,15 @@
         return token
     print("Loading auth flow in standalone Chrome...")
     print("NOTE: If you get the alert with 'chromedriver cannot be opened because the developer cannot be verified.',"
           "select 'Cancel' to proceed.")
     print("PROTIP: Enable 'Remember Me' and 'Keep me signed in' and 'Trusted Device' to speed up subsequent logins.")
     chrome_options = Options()
     chrome_options.add_argument("user-data-dir=%s/selenium" % config_path)
-    driver = webdriver.Chrome(options=chrome_options)
+    driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install()), options=chrome_options)
     driver.get("https://login.sequoia.com/?redirect=https://px.sequoia.com/workplace/")
     try:
         WebDriverWait(driver, 300).until(EC.url_to_be("https://px.sequoia.com/workplace/"))
         cookies = driver.get_cookies()
         if VERBOSE:
             print("COOKIES", cookies)
         for cookie in cookies:
```

### Comparing `wawona-1.2.0/src/wawona.egg-info/PKG-INFO` & `wawona-1.2.1/src/wawona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.2.0
+Version: 1.2.1
 Summary: Easily make office reservations in sequoia from the command line.
 Author-email: yuzawa-san <jtyuzawa+wawona@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
```

