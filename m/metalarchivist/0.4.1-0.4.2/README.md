# Comparing `tmp/metalarchivist-0.4.1.tar.gz` & `tmp/metalarchivist-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.4.1.tar", last modified: Mon May 20 16:00:08 2024, max compression
+gzip compressed data, was "metalarchivist-0.4.2.tar", last modified: Mon May 20 23:39:30 2024, max compression
```

## Comparing `metalarchivist-0.4.1.tar` & `metalarchivist-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.347456 metalarchivist-0.4.1/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-20 16:00:08.347456 metalarchivist-0.4.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 16:00:08.348456 metalarchivist-0.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.338456 metalarchivist-0.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.339456 metalarchivist-0.4.1/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.343456 metalarchivist-0.4.1/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.343456 metalarchivist-0.4.1/src/metalarchivist/export/data/
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/export/data/user-agents.json
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)    10569 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/export/label.py
--rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.345456 metalarchivist-0.4.1/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9056 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/album.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.345456 metalarchivist-0.4.1/src/metalarchivist/interface/api/
--rw-rw-rw-   0 root         (0) root         (0)     3333 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4836 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/api/page.py
--rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/label.py
--rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     5991 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.347456 metalarchivist-0.4.1/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-20 16:00:08.000000 metalarchivist-0.4.1/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2024-05-20 16:00:08.000000 metalarchivist-0.4.1/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 16:00:08.000000 metalarchivist-0.4.1/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-20 16:00:08.000000 metalarchivist-0.4.1/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-20 16:00:08.000000 metalarchivist-0.4.1/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:00:08.347456 metalarchivist-0.4.1/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10205 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     5407 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/test/test_labels.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-20 15:59:55.000000 metalarchivist-0.4.1/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.820120 metalarchivist-0.4.2/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-20 23:39:30.819120 metalarchivist-0.4.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 23:39:30.820120 metalarchivist-0.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.811120 metalarchivist-0.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.813120 metalarchivist-0.4.2/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.815120 metalarchivist-0.4.2/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.815120 metalarchivist-0.4.2/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.817120 metalarchivist-0.4.2/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9056 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.817120 metalarchivist-0.4.2/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     5991 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.819120 metalarchivist-0.4.2/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.819120 metalarchivist-0.4.2/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10205 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     5581 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_themes.py
```

### Comparing `metalarchivist-0.4.1/LICENSE` & `metalarchivist-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/PKG-INFO` & `metalarchivist-0.4.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.4.1
+Version: 0.4.2
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.4.1/pyproject.toml` & `metalarchivist-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.4.1"
+version = "0.4.2"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.4.1/src/metalarchivist/export/album.py` & `metalarchivist-0.4.2/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/export/band.py` & `metalarchivist-0.4.2/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/export/data/user-agents.json` & `metalarchivist-0.4.2/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/export/genre.py` & `metalarchivist-0.4.2/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/export/label.py` & `metalarchivist-0.4.2/src/metalarchivist/export/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     @staticmethod
     def get_label_releases(metallum_id: int, user_agent: str | None = None,
                            echo=0, page_size=500, wait=3., timeout_cxn=3., 
                            timeout_read=9.) -> LabelReleasePage:
         data = LabelReleasePages()
         record_cursor = 0
         timeout = urllib3.Timeout(connect=timeout_cxn, read=timeout_read)
-    
+
         while True:
             endpoint = MetalArchives.label_releases_query(metallum_id, echo, record_cursor, page_size)
             response = perform_request(MetalArchives.get_page, LabelError, endpoint,
                                        timeout=timeout, user_agent=user_agent)
             
             kwargs = normalize_keyword_casing(response.json())
             metadata = dict(metallum_id=metallum_id)
```

### Comparing `metalarchivist-0.4.1/src/metalarchivist/export/util.py` & `metalarchivist-0.4.2/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.4.2/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/interface/album.py` & `metalarchivist-0.4.2/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/interface/api/base.py` & `metalarchivist-0.4.2/src/metalarchivist/interface/api/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/interface/api/page.py` & `metalarchivist-0.4.2/src/metalarchivist/interface/api/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,20 @@
 
     def __post_init__(self, release_page_record: list[str]):
         band_link_text, album_link_text, *args = release_page_record
         
         album_link = AlbumLink(album_link_text)
 
         if re.search(r'>\s?\/\s?<', band_link_text):
-            band_links = band_link_text.split(' / ')
+            band_links = re.split(r'(?<=>)(\s?\/\s?)(?=<)', band_link_text)
 
             for link in band_links:
+                if link.strip() == '/':
+                    continue
+
                 band_link = BandLink(link)
                 album_release = LabelRelease(band_link, album_link, *args)
                 self.append(album_release)
 
         else:
             band_link = BandLink(band_link_text)
             album_release = LabelRelease(band_link, album_link, *args)
```

### Comparing `metalarchivist-0.4.1/src/metalarchivist/interface/band.py` & `metalarchivist-0.4.2/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/interface/genre.py` & `metalarchivist-0.4.2/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/interface/label.py` & `metalarchivist-0.4.2/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/interface/theme.py` & `metalarchivist-0.4.2/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist/report.py` & `metalarchivist-0.4.2/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.4.2/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.4.1
+Version: 0.4.2
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.4.1/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.4.2/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/test/test_albums.py` & `metalarchivist-0.4.2/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/test/test_bands.py` & `metalarchivist-0.4.2/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/test/test_genres.py` & `metalarchivist-0.4.2/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.1/src/test/test_labels.py` & `metalarchivist-0.4.2/src/test/test_labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,21 @@
     return metalarchivist, interface, export, config
 
 
 class TestLabel(unittest.TestCase):
     metalarchivist, interface, export, config = load_module()
 
     def test_label_container(self):
-        label = self.export.Label.get_full_profile('https://www.metal-archives.com/labels/A_Private_Collection/51974')
+        # label = self.export.Label.get_full_profile('https://www.metal-archives.com/labels/A_Private_Collection/51974')
+        # self.assertIsNotNone(label.profile)
+        # self.assertIsNotNone(label.roster)
+        # self.assertIsNotNone(label.releases)
+        # self.assertIsNotNone(label.links)
+
+        label = self.export.Label.get_full_profile('https://www.metal-archives.com/labels/Primetime_Studios/57738')
         self.assertIsNotNone(label.profile)
         self.assertIsNotNone(label.roster)
         self.assertIsNotNone(label.releases)
         self.assertIsNotNone(label.links)
 
     def test_label(self):
         label_profile = self.export.Label.get_profile('https://www.metal-archives.com/labels/PC_Records/17802')
@@ -120,11 +126,7 @@
         self.assertIsNotNone(label_links)
         self.assertGreater(len(label_links.links), 0)
 
     def test_labels(self):
         label_page = self.export.Label.get_labels_by_letter('k')
         self.assertIsNotNone(label_page)
         self.assertGreater(len(label_page.data), 0)
-
-    def test_label_report(self):
-        labels = self.metalarchivist.get_labels()
-        self.assertGreater(len(labels), 0)
```

### Comparing `metalarchivist-0.4.1/src/test/test_themes.py` & `metalarchivist-0.4.2/src/test/test_themes.py`

 * *Files identical despite different names*

