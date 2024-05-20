# Comparing `tmp/fleekapi-0.2.3.tar.gz` & `tmp/fleekapi-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.2.3.tar", last modified: Mon May 20 21:50:04 2024, max compression
+gzip compressed data, was "fleekapi-0.2.4.tar", last modified: Mon May 20 22:00:03 2024, max compression
```

## Comparing `fleekapi-0.2.3.tar` & `fleekapi-0.2.4.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:50:04.102746 fleekapi-0.2.3/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 21:50:04.102746 fleekapi-0.2.3/PKG-INFO
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:50:04.098746 fleekapi-0.2.3/fleekapi/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:40:48.000000 fleekapi-0.2.3/fleekapi/__init__.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:50:04.102746 fleekapi-0.2.3/fleekapi.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      188 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-20 21:50:04.000000 fleekapi-0.2.3/fleekapi.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-20 21:50:04.102746 fleekapi-0.2.3/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     4013 2024-05-20 21:50:01.000000 fleekapi-0.2.3/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 22:00:03.698767 fleekapi-0.2.4/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 22:00:03.698767 fleekapi-0.2.4/PKG-INFO
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 22:00:03.698767 fleekapi-0.2.4/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       17 2024-05-20 21:58:20.000000 fleekapi-0.2.4/fleekapi/__init__.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 22:00:03.698767 fleekapi-0.2.4/fleekapi/src/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       68 2024-05-20 21:58:20.000000 fleekapi-0.2.4/fleekapi/src/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3803 2024-05-20 20:51:08.000000 fleekapi-0.2.4/fleekapi/src/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      674 2024-05-19 13:15:32.000000 fleekapi-0.2.4/fleekapi/src/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      972 2024-05-19 13:15:32.000000 fleekapi-0.2.4/fleekapi/src/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 22:00:03.698767 fleekapi-0.2.4/fleekapi.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 22:00:03.000000 fleekapi-0.2.4/fleekapi.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      285 2024-05-20 22:00:03.000000 fleekapi-0.2.4/fleekapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-20 22:00:03.000000 fleekapi-0.2.4/fleekapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-20 22:00:03.000000 fleekapi-0.2.4/fleekapi.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-20 22:00:03.000000 fleekapi-0.2.4/fleekapi.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-20 22:00:03.698767 fleekapi-0.2.4/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4013 2024-05-20 21:59:50.000000 fleekapi-0.2.4/setup.py
```

### Comparing `fleekapi-0.2.3/PKG-INFO` & `fleekapi-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleekapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.2.3/fleekapi.egg-info/PKG-INFO` & `fleekapi-0.2.4/fleekapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleekapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.2.3/setup.py` & `fleekapi-0.2.4/setup.py`

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
-VERSION = '0.2.03'
+VERSION = '0.2.04'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```

