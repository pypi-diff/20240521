# Comparing `tmp/pinterest-crawler-0.1.3.tar.gz` & `tmp/pinterest_crawler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinterest-crawler-0.1.3.tar", last modified: Thu Jul 13 07:19:02 2023, max compression
+gzip compressed data, was "pinterest_crawler-0.2.0.tar", last modified: Tue May 21 09:24:50 2024, max compression
```

## Comparing `pinterest-crawler-0.1.3.tar` & `pinterest_crawler-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:19:02.111185 pinterest-crawler-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-13 07:19:02.111185 pinterest-crawler-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:19:02.107185 pinterest-crawler-0.1.3/pinterest_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/pinterest_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/pinterest_crawler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/pinterest_crawler/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/pinterest_crawler/pinterest_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/pinterest_crawler/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:19:02.111185 pinterest-crawler-0.1.3/pinterest_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-13 07:19:02.000000 pinterest-crawler-0.1.3/pinterest_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-13 07:19:02.000000 pinterest-crawler-0.1.3/pinterest_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:19:02.000000 pinterest-crawler-0.1.3/pinterest_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 07:19:02.000000 pinterest-crawler-0.1.3/pinterest_crawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:19:02.000000 pinterest-crawler-0.1.3/pinterest_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 07:19:02.000000 pinterest-crawler-0.1.3/pinterest_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:19:02.111185 pinterest-crawler-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-13 07:18:50.000000 pinterest-crawler-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:24:50.350388 pinterest_crawler-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-21 09:24:50.350388 pinterest_crawler-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:24:50.346387 pinterest_crawler-0.2.0/pinterest_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/pinterest_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/pinterest_crawler/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/pinterest_crawler/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/pinterest_crawler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/pinterest_crawler/pinterest_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/pinterest_crawler/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:24:50.346387 pinterest_crawler-0.2.0/pinterest_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-21 09:24:50.000000 pinterest_crawler-0.2.0/pinterest_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-21 09:24:50.000000 pinterest_crawler-0.2.0/pinterest_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:24:50.000000 pinterest_crawler-0.2.0/pinterest_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 09:24:50.000000 pinterest_crawler-0.2.0/pinterest_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:24:50.000000 pinterest_crawler-0.2.0/pinterest_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 09:24:50.000000 pinterest_crawler-0.2.0/pinterest_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:24:50.350388 pinterest_crawler-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:24:50.346387 pinterest_crawler-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-21 09:24:46.000000 pinterest_crawler-0.2.0/tests/test_pinterest_crawler.py
```

### Comparing `pinterest-crawler-0.1.3/LICENSE.md` & `pinterest_crawler-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pinterest-crawler-0.1.3/PKG-INFO` & `pinterest_crawler-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,65 @@
 Metadata-Version: 2.1
 Name: pinterest-crawler
-Version: 0.1.3
+Version: 0.2.0
 Summary: Pinterest Crawler: Download as many images as you want about the searched words
 Home-page: https://github.com/SajjadAemmi/Pinterest-Crawler
 Author: Sajjad Aemmi
 Author-email: sajjadaemmi@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: requests
 
 # Pinterest Crawler
 
 [![Upload Python Package](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-publish.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-publish.yml)
 [![Python package](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-package.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-package.yml)
 [![Python application](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-app.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-app.yml)
+[![Downloads](https://static.pepy.tech/badge/pinterest-crawler)](https://pepy.tech/project/pinterest-crawler)
 
 <img src="https://raw.githubusercontent.com/SajjadAemmi/Pinterest-Crawler/main/Pinterest-Logo.png" width="400px">
 
 Downloads HD images from pinterest by your favorite keywords. A useful tool to create a dataset for machine learning projects.
 
 ## Install
+
 Install the package with pip in a Python>=3.8 environment:
-```
+
+```bash
 pip install pinterest-crawler
 ```
 
 ## Usage
 
 ### CLI
+
 Pinterest Crawler may be used directly in the Command Line Interface (CLI):
 
 ```bash
 pinterest-crawler --keywords lion tiger bear
 ```
 
 Also you can write your favorite keywords in a file for example `my_keywords.txt` and set path of file in `--keywords` argument:
+
 ```bash
 pinterest-crawler --keywords my_keywords.txt
 ```
 
-### Python 
-Coming soon...
+### Python
+
+Pinterest Crawler may also be used directly in a Python environment, and accepts the same arguments as in the CLI example above:
+
+```python
+from pinterest_crawler import PinterestCrawler
+
+
+pinterest_crawler = PinterestCrawler()
+pinterest_crawler(keywords=['lion', 'programmer'])
+```
+
 <!-- Due to some limitations of Pinterest, you can download 100 images per keyword. If you want to download more images, you can run following command for infinite execution:
 
 ```
 python loop.py
 ``` -->
 
 ## TODO
```

### Comparing `pinterest-crawler-0.1.3/README.md` & `pinterest_crawler-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 # Pinterest Crawler
 
 [![Upload Python Package](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-publish.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-publish.yml)
 [![Python package](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-package.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-package.yml)
 [![Python application](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-app.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-app.yml)
+[![Downloads](https://static.pepy.tech/badge/pinterest-crawler)](https://pepy.tech/project/pinterest-crawler)
 
 <img src="https://raw.githubusercontent.com/SajjadAemmi/Pinterest-Crawler/main/Pinterest-Logo.png" width="400px">
 
 Downloads HD images from pinterest by your favorite keywords. A useful tool to create a dataset for machine learning projects.
 
 ## Install
+
 Install the package with pip in a Python>=3.8 environment:
-```
+
+```bash
 pip install pinterest-crawler
 ```
 
 ## Usage
 
 ### CLI
+
 Pinterest Crawler may be used directly in the Command Line Interface (CLI):
 
 ```bash
 pinterest-crawler --keywords lion tiger bear
 ```
 
 Also you can write your favorite keywords in a file for example `my_keywords.txt` and set path of file in `--keywords` argument:
+
 ```bash
 pinterest-crawler --keywords my_keywords.txt
 ```
 
-### Python 
-Coming soon...
+### Python
+
+Pinterest Crawler may also be used directly in a Python environment, and accepts the same arguments as in the CLI example above:
+
+```python
+from pinterest_crawler import PinterestCrawler
+
+
+pinterest_crawler = PinterestCrawler()
+pinterest_crawler(keywords=['lion', 'programmer'])
+```
+
 <!-- Due to some limitations of Pinterest, you can download 100 images per keyword. If you want to download more images, you can run following command for infinite execution:
 
 ```
 python loop.py
 ``` -->
 
 ## TODO
```

### Comparing `pinterest-crawler-0.1.3/pinterest_crawler/config.py` & `pinterest_crawler-0.2.0/pinterest_crawler/config.py`

 * *Files identical despite different names*

### Comparing `pinterest-crawler-0.1.3/pinterest_crawler/scraper.py` & `pinterest_crawler-0.2.0/pinterest_crawler/scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,59 +14,62 @@
         self.config = config
 
     def download_images(self, output_path) -> int:
         # prev get links
         results = self.get_urls()
         try:
             os.makedirs(output_path)
-            print("Directory ", output_path, " Created ")
+            print(f"Directory {output_path} Created")
         except FileExistsError:
             pass
-        
+
         number = 0
         listdir = os.listdir(output_path)
         if results != None:
             for i in results:
                 file_name = i.split("/")[-1]
                 if file_name not in listdir:
                     try:
                         number += 1
-                        print("Download ::: ", i)
-                        urllib.request.urlretrieve(i, os.path.join(output_path, file_name))
+                        print("Downloading", i)
+                        urllib.request.urlretrieve(
+                            i, os.path.join(output_path, file_name))
                     except Exception as e:
                         print("Error:", e)
 
         return number
 
     def get_urls(self) -> list:
         SOURCE_URL = self.config.source_url,
         DATA = self.config.image_data,
         URL_CONSTANT = self.config.search_url
 
-        r = requests.get(URL_CONSTANT, params={"source_url": SOURCE_URL, "data": DATA})
+        r = requests.get(URL_CONSTANT, params={
+                         "source_url": SOURCE_URL, "data": DATA})
         jsonData = json.loads(r.content)
         resource_response = jsonData["resource_response"]
         data = resource_response["data"]
         results = data["results"]
-        
+
         for i in results:
             try:
-                self.image_urls.append(i["objects"][0]["cover_images"][0]["originals"]["url"])
+                self.image_urls.append(
+                    i["objects"][0]["cover_images"][0]["originals"]["url"])
             except:
                 self.URL = None
                 self.search(i)
                 if self.URL != None:
                     self.image_urls.append(self.URL)
 
         if len(self.image_urls) < int(self.config.file_length):
             try:
-                print("Creating links", len(self.image_urls))
+                print(f"{len(self.image_urls)} images Founded")
                 return self.image_urls[0:self.config.file_length]
-            except:
-                pass
+            except Exception as e:
+                print("Error:", e)
 
     def search(self, d):
         if isinstance(d, dict):
             for k, v in d.items():
                 if isinstance(v, dict):
                     if k == "orig":
                         self.URL = v["url"]
```

### Comparing `pinterest-crawler-0.1.3/pinterest_crawler.egg-info/PKG-INFO` & `pinterest_crawler-0.2.0/pinterest_crawler.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,65 @@
 Metadata-Version: 2.1
 Name: pinterest-crawler
-Version: 0.1.3
+Version: 0.2.0
 Summary: Pinterest Crawler: Download as many images as you want about the searched words
 Home-page: https://github.com/SajjadAemmi/Pinterest-Crawler
 Author: Sajjad Aemmi
 Author-email: sajjadaemmi@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: requests
 
 # Pinterest Crawler
 
 [![Upload Python Package](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-publish.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-publish.yml)
 [![Python package](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-package.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-package.yml)
 [![Python application](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-app.yml/badge.svg)](https://github.com/SajjadAemmi/Pinterest-Crawler/actions/workflows/python-app.yml)
+[![Downloads](https://static.pepy.tech/badge/pinterest-crawler)](https://pepy.tech/project/pinterest-crawler)
 
 <img src="https://raw.githubusercontent.com/SajjadAemmi/Pinterest-Crawler/main/Pinterest-Logo.png" width="400px">
 
 Downloads HD images from pinterest by your favorite keywords. A useful tool to create a dataset for machine learning projects.
 
 ## Install
+
 Install the package with pip in a Python>=3.8 environment:
-```
+
+```bash
 pip install pinterest-crawler
 ```
 
 ## Usage
 
 ### CLI
+
 Pinterest Crawler may be used directly in the Command Line Interface (CLI):
 
 ```bash
 pinterest-crawler --keywords lion tiger bear
 ```
 
 Also you can write your favorite keywords in a file for example `my_keywords.txt` and set path of file in `--keywords` argument:
+
 ```bash
 pinterest-crawler --keywords my_keywords.txt
 ```
 
-### Python 
-Coming soon...
+### Python
+
+Pinterest Crawler may also be used directly in a Python environment, and accepts the same arguments as in the CLI example above:
+
+```python
+from pinterest_crawler import PinterestCrawler
+
+
+pinterest_crawler = PinterestCrawler()
+pinterest_crawler(keywords=['lion', 'programmer'])
+```
+
 <!-- Due to some limitations of Pinterest, you can download 100 images per keyword. If you want to download more images, you can run following command for infinite execution:
 
 ```
 python loop.py
 ``` -->
 
 ## TODO
```

### Comparing `pinterest-crawler-0.1.3/setup.py` & `pinterest_crawler-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from setuptools import setup, find_packages
+from setuptools import setup
 
 
 def post_install():
     """ Implement post installation routine """
     with open('./requirements.txt') as f:
         install_requires = f.read().splitlines()
 
@@ -19,23 +19,23 @@
 
 
 pre_install()
 
 
 setup(
     name='pinterest-crawler',
-    version='0.1.3',
+    version='0.2.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=["pinterest_crawler"],
     setup_requires=[],
     url='https://github.com/SajjadAemmi/Pinterest-Crawler',
     license='',
     author='Sajjad Aemmi',
     author_email='sajjadaemmi@gmail.com',
     description='Pinterest Crawler: Download as many images as you want about the searched words',
     include_package_data=True,
     install_requires=post_install(),
     entry_points={
-        "console_scripts": ["pinterest-crawler=pinterest_crawler.pinterest_crawler:main"],
+        "console_scripts": ["pinterest-crawler=pinterest_crawler.main:main"],
     },
 )
```

