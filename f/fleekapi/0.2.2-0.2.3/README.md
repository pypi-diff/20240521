# Comparing `tmp/fleekapi-0.2.2.tar.gz` & `tmp/fleekapi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.2.2.tar", last modified: Mon May 20 21:14:01 2024, max compression
+gzip compressed data, was "fleekapi-0.2.3.tar", last modified: Mon May 20 21:50:04 2024, max compression
```

## Comparing `fleekapi-0.2.2.tar` & `fleekapi-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:14:01.308943 fleekapi-0.2.2/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 21:14:01.308943 fleekapi-0.2.2/PKG-INFO
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:14:01.304943 fleekapi-0.2.2/fleekapi/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       26 2024-05-19 13:15:32.000000 fleekapi-0.2.2/fleekapi/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3803 2024-05-20 20:51:08.000000 fleekapi-0.2.2/fleekapi/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      674 2024-05-19 13:15:32.000000 fleekapi-0.2.2/fleekapi/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      972 2024-05-19 13:15:32.000000 fleekapi-0.2.2/fleekapi/response.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:14:01.308943 fleekapi-0.2.2/fleekapi.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 21:14:01.000000 fleekapi-0.2.2/fleekapi.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      248 2024-05-20 21:14:01.000000 fleekapi-0.2.2/fleekapi.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-20 21:14:01.000000 fleekapi-0.2.2/fleekapi.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-20 21:14:01.000000 fleekapi-0.2.2/fleekapi.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-20 21:14:01.000000 fleekapi-0.2.2/fleekapi.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-20 21:14:01.308943 fleekapi-0.2.2/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     4013 2024-05-20 21:13:58.000000 fleekapi-0.2.2/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:50:04.102746 fleekapi-0.2.3/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 21:50:04.102746 fleekapi-0.2.3/PKG-INFO
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:50:04.098746 fleekapi-0.2.3/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:40:48.000000 fleekapi-0.2.3/fleekapi/__init__.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:50:04.102746 fleekapi-0.2.3/fleekapi.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      188 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-20 21:50:04.102746 fleekapi-0.2.3/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4013 2024-05-20 21:50:01.000000 fleekapi-0.2.3/setup.py
```

### Comparing `fleekapi-0.2.2/PKG-INFO` & `fleekapi-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleekapi
-Version: 0.2.2
+Version: 0.2.3
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.2.2/fleekapi.egg-info/PKG-INFO` & `fleekapi-0.2.3/fleekapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleekapi
-Version: 0.2.2
+Version: 0.2.3
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.2.2/setup.py` & `fleekapi-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'fleekapi'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/FleekAPI'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.2.02'
+VERSION = '0.2.03'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```

