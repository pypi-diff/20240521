# Comparing `tmp/pinscrape-3.1.0.tar.gz` & `tmp/pinscrape-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinscrape-3.1.0.tar", last modified: Sat May 18 11:39:10 2024, max compression
+gzip compressed data, was "pinscrape-3.2.0.tar", last modified: Tue May 21 08:47:23 2024, max compression
```

## Comparing `pinscrape-3.1.0.tar` & `pinscrape-3.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:39:10.468636 pinscrape-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-18 11:38:50.000000 pinscrape-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-18 11:39:10.468636 pinscrape-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-18 11:38:50.000000 pinscrape-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:39:10.464636 pinscrape-3.1.0/pinscrape/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-18 11:38:50.000000 pinscrape-3.1.0/pinscrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 11:38:50.000000 pinscrape-3.1.0/pinscrape/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-18 11:38:50.000000 pinscrape-3.1.0/pinscrape/pinscrape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:39:10.468636 pinscrape-3.1.0/pinscrape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 11:39:10.468636 pinscrape-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-18 11:38:50.000000 pinscrape-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:47:23.188009 pinscrape-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 08:47:09.000000 pinscrape-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 08:47:23.184009 pinscrape-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 08:47:09.000000 pinscrape-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:47:23.184009 pinscrape-3.2.0/pinscrape/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-21 08:47:09.000000 pinscrape-3.2.0/pinscrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 08:47:09.000000 pinscrape-3.2.0/pinscrape/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-21 08:47:09.000000 pinscrape-3.2.0/pinscrape/pinscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:47:23.184009 pinscrape-3.2.0/pinscrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:47:23.188009 pinscrape-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-21 08:47:09.000000 pinscrape-3.2.0/setup.py
```

### Comparing `pinscrape-3.1.0/LICENSE` & `pinscrape-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinscrape-3.1.0/PKG-INFO` & `pinscrape-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.1.0
+Version: 3.2.0
 Summary: Pinterest | a simple data scraper for pinterest
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.28.1
+Requires-Dist: requests==2.32.0
 Requires-Dist: beautifulsoup4==4.11.1
 Requires-Dist: tqdm==4.66.3
 Requires-Dist: pydotmap
 Requires-Dist: opencv-python
 Requires-Dist: pytest==7.2.0
 
 # pinscrape
```

### Comparing `pinscrape-3.1.0/README.md` & `pinscrape-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pinscrape-3.1.0/pinscrape/pinscrape.py` & `pinscrape-3.2.0/pinscrape/pinscrape.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,29 +35,35 @@
     def get_source(self, url: str, proxies: dict) -> None:
         try:
             res = get(url, proxies=proxies)
         except Exception:
             return
         html = soup(res.text, 'html.parser')
         json_data = html.find_all("script", attrs={"id": "__PWS_INITIAL_PROPS__"})
-        self.json_data_list.append(json.loads(json_data[0].string))
+        if not len(json_data):
+            json_data = html.find_all("script", attrs={"id": "__PWS_DATA__"})
+
+        self.json_data_list.append(json.loads(json_data[0].string)) if len(json_data) else self.json_data_list.append({})
 
     # --------------------------- READ JSON OF PINTEREST WEBSITE ----------------------
     def save_image_url(self, max_images: int) -> list:
         url_list = []
         for js in self.json_data_list:
             try:
                 data = DotMap(js)
                 urls = []
-                for pin in data.initialReduxState.pins:
-                    if isinstance(data.initialReduxState.pins[pin].images.get("orig"), list):
-                        for i in data.initialReduxState.pins[pin].images.get("orig"):
+                if not data.initialReduxState and not data.props:
+                    return []
+                pins = data.initialReduxState.pins if data.initialReduxState else data.props.initialReduxState.pins
+                for pin in pins:
+                    if isinstance(pins[pin].images.get("orig"), list):
+                        for i in pins[pin].images.get("orig"):
                             urls.append(i.get("url"))
                     else:
-                        urls.append(data.initialReduxState.pins[pin].images.get("orig").get("url"))
+                        urls.append(pins[pin].images.get("orig").get("url"))
 
                 for url in urls:
                     url_list.append(url)
                     if max_images is not None and max_images == len(url_list):
                         return list(set(url_list))
             except Exception:
                 continue
@@ -92,37 +98,38 @@
         for i in range(num_of_workers):
             param.append((url_list[((i*idx)):(idx*(i+1))], output_folder))
         with ThreadPoolExecutor(max_workers=num_of_workers) as executor:
             executor.map(self.saving_op, param)
 
     # -------------------------- get user keyword and google search for that keywords ---------------------
     @staticmethod
-    def start_scraping(max_images, key=None, proxies={}):
+    def start_scraping(max_images, key=None, proxies: dict = {}):
         assert key is not None, "Please provide keyword for searching images"
         keyword = key + " pinterest"
         keyword = keyword.replace("+", "%20")
-        url = f'https://www.bing.com/search?q={keyword}&pq=messi+pinterest&first=1&FORM=PERE'
+        url = f'https://www.bing.com/search?q={keyword}&first=1&FORM=PERE'
         res = get(url, proxies=proxies)
         searched_urls = PinterestImageScraper.get_pinterest_links(res.content, max_images)
 
-        return searched_urls, key.replace(" ", "_")
+        return searched_urls, key.replace(" ", "_"), res.status_code
 
     def scrape(self, key: str = None, output_folder: str = "", proxies: dict = {}, threads: int = 10, max_images: int = None) -> dict:
-        extracted_urls, keyword = PinterestImageScraper.start_scraping(max_images, key, proxies)
+        extracted_urls, keyword, search_engine_status_code = PinterestImageScraper.start_scraping(max_images, key, proxies)
         self.unique_img = []
         self.json_data_list = []
 
         for i in extracted_urls:
             self.get_source(i, proxies)
 
         # get all urls of images and save in a list
         url_list = self.save_image_url(max_images)
 
         return_data = {
             "isDownloaded": False,
+            "search_engine_status_code": search_engine_status_code,
             "url_list": url_list,
             "extracted_urls": extracted_urls,
             "keyword": key
         }
 
         # download images from saved images url
         if len(url_list):
```

### Comparing `pinscrape-3.1.0/pinscrape.egg-info/PKG-INFO` & `pinscrape-3.2.0/pinscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.1.0
+Version: 3.2.0
 Summary: Pinterest | a simple data scraper for pinterest
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.28.1
+Requires-Dist: requests==2.32.0
 Requires-Dist: beautifulsoup4==4.11.1
 Requires-Dist: tqdm==4.66.3
 Requires-Dist: pydotmap
 Requires-Dist: opencv-python
 Requires-Dist: pytest==7.2.0
 
 # pinscrape
```

### Comparing `pinscrape-3.1.0/setup.py` & `pinscrape-3.2.0/setup.py`

 * *Files identical despite different names*

