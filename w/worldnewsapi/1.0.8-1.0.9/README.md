# Comparing `tmp/worldnewsapi-1.0.8.tar.gz` & `tmp/worldnewsapi-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worldnewsapi-1.0.8.tar", last modified: Thu Mar  7 15:37:23 2024, max compression
+gzip compressed data, was "worldnewsapi-1.0.9.tar", last modified: Thu Mar  7 22:53:40 2024, max compression
```

## Comparing `worldnewsapi-1.0.8.tar` & `worldnewsapi-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 15:37:23.161006 worldnewsapi-1.0.8/
--rw-rw-rw-   0        0        0     2054 2024-03-07 15:37:23.160478 worldnewsapi-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4404 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/README.md
--rw-rw-rw-   0        0        0     1113 2024-03-07 13:36:21.000000 worldnewsapi-1.0.8/README_pypi.md
--rw-rw-rw-   0        0        0     2671 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       76 2024-03-07 15:37:23.162011 worldnewsapi-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1234 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-07 15:37:23.140955 worldnewsapi-1.0.8/test/
--rw-rw-rw-   0        0        0     1477 2024-03-07 15:36:55.000000 worldnewsapi-1.0.8/test/test_extract_links_response.py
--rw-rw-rw-   0        0        0     1629 2024-03-07 15:36:56.000000 worldnewsapi-1.0.8/test/test_extract_news_response.py
--rw-rw-rw-   0        0        0     1589 2024-03-07 15:36:56.000000 worldnewsapi-1.0.8/test/test_geo_coordinates_response.py
--rw-rw-rw-   0        0        0     1537 2024-03-07 15:36:56.000000 worldnewsapi-1.0.8/test/test_news.py
--rw-rw-rw-   0        0        0     1283 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/test/test_news_api.py
--rw-rw-rw-   0        0        0     1622 2024-03-07 15:36:56.000000 worldnewsapi-1.0.8/test/test_news_article.py
--rw-rw-rw-   0        0        0     2646 2024-03-07 15:36:57.000000 worldnewsapi-1.0.8/test/test_search_news_response.py
-drwxrwxrwx   0        0        0        0 2024-03-07 15:37:23.145510 worldnewsapi-1.0.8/worldnewsapi/
--rw-rw-rw-   0        0        0     1317 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/worldnewsapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-07 15:37:23.154464 worldnewsapi-1.0.8/worldnewsapi/api/
--rw-rw-rw-   0        0        0       93 2024-03-07 15:37:00.000000 worldnewsapi-1.0.8/worldnewsapi/api/__init__.py
--rw-rw-rw-   0        0        0    79356 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/worldnewsapi/api/news_api.py
--rw-rw-rw-   0        0        0    26009 2024-03-07 15:37:00.000000 worldnewsapi-1.0.8/worldnewsapi/api_client.py
--rw-rw-rw-   0        0        0      688 2024-03-07 15:37:00.000000 worldnewsapi-1.0.8/worldnewsapi/api_response.py
--rw-rw-rw-   0        0        0    15674 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/worldnewsapi/configuration.py
--rw-rw-rw-   0        0        0     6213 2024-03-07 15:37:00.000000 worldnewsapi-1.0.8/worldnewsapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-07 15:37:23.158973 worldnewsapi-1.0.8/worldnewsapi/models/
--rw-rw-rw-   0        0        0      745 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/worldnewsapi/models/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-03-07 15:36:55.000000 worldnewsapi-1.0.8/worldnewsapi/models/extract_links_response.py
--rw-rw-rw-   0        0        0     3412 2024-03-07 15:36:55.000000 worldnewsapi-1.0.8/worldnewsapi/models/extract_news_response.py
--rw-rw-rw-   0        0        0     2723 2024-03-07 15:36:56.000000 worldnewsapi-1.0.8/worldnewsapi/models/geo_coordinates_response.py
--rw-rw-rw-   0        0        0     3643 2024-03-07 15:36:56.000000 worldnewsapi-1.0.8/worldnewsapi/models/news.py
--rw-rw-rw-   0        0        0     3662 2024-03-07 15:36:56.000000 worldnewsapi-1.0.8/worldnewsapi/models/news_article.py
--rw-rw-rw-   0        0        0     3188 2024-03-07 15:36:56.000000 worldnewsapi-1.0.8/worldnewsapi/models/search_news_response.py
--rw-rw-rw-   0        0        0        0 2024-03-07 15:36:59.000000 worldnewsapi-1.0.8/worldnewsapi/py.typed
--rw-rw-rw-   0        0        0     9642 2024-03-07 15:37:00.000000 worldnewsapi-1.0.8/worldnewsapi/rest.py
-drwxrwxrwx   0        0        0        0 2024-03-07 15:37:23.158973 worldnewsapi-1.0.8/worldnewsapi.egg-info/
--rw-rw-rw-   0        0        0     2054 2024-03-07 15:37:23.000000 worldnewsapi-1.0.8/worldnewsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      964 2024-03-07 15:37:23.000000 worldnewsapi-1.0.8/worldnewsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 15:37:23.000000 worldnewsapi-1.0.8/worldnewsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-03-07 15:37:23.000000 worldnewsapi-1.0.8/worldnewsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-07 15:37:23.000000 worldnewsapi-1.0.8/worldnewsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.406098 worldnewsapi-1.0.9/
+-rw-rw-rw-   0        0        0     2054 2024-03-07 22:53:40.406098 worldnewsapi-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4404 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1113 2024-03-07 13:36:21.000000 worldnewsapi-1.0.9/README_pypi.md
+-rw-rw-rw-   0        0        0     2671 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       76 2024-03-07 22:53:40.407096 worldnewsapi-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.375962 worldnewsapi-1.0.9/test/
+-rw-rw-rw-   0        0        0     1477 2024-03-07 22:53:11.000000 worldnewsapi-1.0.9/test/test_extract_links_response.py
+-rw-rw-rw-   0        0        0     1629 2024-03-07 22:53:11.000000 worldnewsapi-1.0.9/test/test_extract_news_response.py
+-rw-rw-rw-   0        0        0     1589 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/test/test_geo_coordinates_response.py
+-rw-rw-rw-   0        0        0     1537 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/test/test_news.py
+-rw-rw-rw-   0        0        0     1283 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/test/test_news_api.py
+-rw-rw-rw-   0        0        0     1622 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/test/test_news_article.py
+-rw-rw-rw-   0        0        0     2646 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/test/test_search_news_response.py
+drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.380962 worldnewsapi-1.0.9/worldnewsapi/
+-rw-rw-rw-   0        0        0     1317 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.399414 worldnewsapi-1.0.9/worldnewsapi/api/
+-rw-rw-rw-   0        0        0       93 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/api/__init__.py
+-rw-rw-rw-   0        0        0    79356 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/api/news_api.py
+-rw-rw-rw-   0        0        0    26009 2024-03-07 22:53:16.000000 worldnewsapi-1.0.9/worldnewsapi/api_client.py
+-rw-rw-rw-   0        0        0      688 2024-03-07 22:53:16.000000 worldnewsapi-1.0.9/worldnewsapi/api_response.py
+-rw-rw-rw-   0        0        0    15674 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/configuration.py
+-rw-rw-rw-   0        0        0     6213 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.403924 worldnewsapi-1.0.9/worldnewsapi/models/
+-rw-rw-rw-   0        0        0      745 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/models/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-03-07 22:53:11.000000 worldnewsapi-1.0.9/worldnewsapi/models/extract_links_response.py
+-rw-rw-rw-   0        0        0     3412 2024-03-07 22:53:11.000000 worldnewsapi-1.0.9/worldnewsapi/models/extract_news_response.py
+-rw-rw-rw-   0        0        0     2723 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/worldnewsapi/models/geo_coordinates_response.py
+-rw-rw-rw-   0        0        0     3643 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/worldnewsapi/models/news.py
+-rw-rw-rw-   0        0        0     3662 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/worldnewsapi/models/news_article.py
+-rw-rw-rw-   0        0        0     3188 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/worldnewsapi/models/search_news_response.py
+-rw-rw-rw-   0        0        0        0 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/py.typed
+-rw-rw-rw-   0        0        0     9642 2024-03-07 22:53:16.000000 worldnewsapi-1.0.9/worldnewsapi/rest.py
+drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.405097 worldnewsapi-1.0.9/worldnewsapi.egg-info/
+-rw-rw-rw-   0        0        0     2054 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/top_level.txt
```

### Comparing `worldnewsapi-1.0.8/PKG-INFO` & `worldnewsapi-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worldnewsapi
-Version: 1.0.8
+Version: 1.0.9
 Summary: The world's news wrapped into a single API.
 Home-page: 
 Author: David Urbansky
 Author-email: David Urbansky <mail@worldnewsapi.com>
 Project-URL: Homepage, https://worldnewsapi.com
 Project-URL: Documentation, https://worldnewsapi.com/docs
 Project-URL: Repository, https://github.com/ddsky/world-news-api-clients/tree/main/python
```

### Comparing `worldnewsapi-1.0.8/README.md` & `worldnewsapi-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # worldnewsapi
 
 The World News API gives you access to thousands of news sources in over 50 languages from over 150 countries. News are semantically tagged allowing for semantic news search like never before.
 
 This is the python-package for easy acccess to the api.
 
 - API version: 1.1
-- Package version: 1.0.8
+- Package version: 1.0.9
 
 ## Resources
 
 - [Homepage](https://worldnewsapi.com/)
 - [Tutorial](https://worldnewsapi.com/docs/#Tutorial-Getting-Started) 
 
 ## Requirements
```

### Comparing `worldnewsapi-1.0.8/README_pypi.md` & `worldnewsapi-1.0.9/README_pypi.md`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/pyproject.toml` & `worldnewsapi-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "worldnewsapi"
-version = "1.0.8"
+version = "1.0.9"
 description = "World News API"
 authors = ["David Urbansky <mail@worldnewsapi.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/ddsky/world-news-api-clients/tree/main/python/"
 keywords = ["OpenAPI", "OpenAPI-Generator", "World News API"]
 include = ["worldnewsapi/py.typed"]
@@ -69,15 +69,15 @@
 #
 ### This one can be tricky to get passing if you use a lot of untyped libraries
 #warn_return_any = true
 
 # The following section is used by PiPy
 [project]
 name = "worldnewsapi"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="David Urbansky", email="mail@worldnewsapi.com" },
 ]
 description = "The world's news wrapped into a single API."
 readme = "README_pypi.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `worldnewsapi-1.0.8/setup.py` & `worldnewsapi-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "worldnewsapi"
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `worldnewsapi-1.0.8/test/test_extract_links_response.py` & `worldnewsapi-1.0.9/test/test_extract_links_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/test/test_extract_news_response.py` & `worldnewsapi-1.0.9/test/test_extract_news_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/test/test_geo_coordinates_response.py` & `worldnewsapi-1.0.9/test/test_geo_coordinates_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/test/test_news.py` & `worldnewsapi-1.0.9/test/test_news.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/test/test_news_api.py` & `worldnewsapi-1.0.9/test/test_news_api.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/test/test_news_article.py` & `worldnewsapi-1.0.9/test/test_news_article.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/test/test_search_news_response.py` & `worldnewsapi-1.0.9/test/test_search_news_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/__init__.py` & `worldnewsapi-1.0.9/worldnewsapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 # import apis into sdk package
 from worldnewsapi.api.news_api import NewsApi
 
 # import ApiClient
 from worldnewsapi.api_response import ApiResponse
 from worldnewsapi.api_client import ApiClient
```

### Comparing `worldnewsapi-1.0.8/worldnewsapi/api/news_api.py` & `worldnewsapi-1.0.9/worldnewsapi/api/news_api.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/api_client.py` & `worldnewsapi-1.0.9/worldnewsapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.8/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `worldnewsapi-1.0.8/worldnewsapi/api_response.py` & `worldnewsapi-1.0.9/worldnewsapi/api_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/configuration.py` & `worldnewsapi-1.0.9/worldnewsapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.1\n"\
-               "SDK Package Version: 1.0.8".\
+               "SDK Package Version: 1.0.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `worldnewsapi-1.0.8/worldnewsapi/exceptions.py` & `worldnewsapi-1.0.9/worldnewsapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/models/__init__.py` & `worldnewsapi-1.0.9/worldnewsapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/models/extract_links_response.py` & `worldnewsapi-1.0.9/worldnewsapi/models/extract_links_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/models/extract_news_response.py` & `worldnewsapi-1.0.9/worldnewsapi/models/extract_news_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/models/geo_coordinates_response.py` & `worldnewsapi-1.0.9/worldnewsapi/models/geo_coordinates_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/models/news.py` & `worldnewsapi-1.0.9/worldnewsapi/models/news.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/models/news_article.py` & `worldnewsapi-1.0.9/worldnewsapi/models/news_article.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/models/search_news_response.py` & `worldnewsapi-1.0.9/worldnewsapi/models/search_news_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi/rest.py` & `worldnewsapi-1.0.9/worldnewsapi/rest.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.8/worldnewsapi.egg-info/PKG-INFO` & `worldnewsapi-1.0.9/worldnewsapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worldnewsapi
-Version: 1.0.8
+Version: 1.0.9
 Summary: The world's news wrapped into a single API.
 Home-page: 
 Author: David Urbansky
 Author-email: David Urbansky <mail@worldnewsapi.com>
 Project-URL: Homepage, https://worldnewsapi.com
 Project-URL: Documentation, https://worldnewsapi.com/docs
 Project-URL: Repository, https://github.com/ddsky/world-news-api-clients/tree/main/python
```

### Comparing `worldnewsapi-1.0.8/worldnewsapi.egg-info/SOURCES.txt` & `worldnewsapi-1.0.9/worldnewsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

