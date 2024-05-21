# Comparing `tmp/ellis_django_views-0.15.tar.gz` & `tmp/ellis_django_views-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellis_django_views-0.15.tar", last modified: Tue May 21 10:58:10 2024, max compression
+gzip compressed data, was "ellis_django_views-0.18.tar", last modified: Tue May 21 11:26:04 2024, max compression
```

## Comparing `ellis_django_views-0.15.tar` & `ellis_django_views-0.18.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.643673 ellis_django_views-0.15/
--rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.15/LICENSE
--rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 06:59:28.000000 ellis_django_views-0.15/MANIFEST.in
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1075 2024-05-21 10:58:10.643351 ellis_django_views-0.15/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      610 2024-05-21 06:55:57.000000 ellis_django_views-0.15/README.md
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.574254 ellis_django_views-0.15/ellis_django_views/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.15/ellis_django_views/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.15/ellis_django_views/apps.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.593935 ellis_django_views-0.15/ellis_django_views/migrations/
--rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.15/ellis_django_views/migrations/0001_initial.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.15/ellis_django_views/migrations/__init__.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.625062 ellis_django_views-0.15/ellis_django_views/tests/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.15/ellis_django_views/tests/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.15/ellis_django_views/tests/models.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.15/ellis_django_views/tests/serializers.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.15/ellis_django_views/tests/test_views.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.15/ellis_django_views/tests/urls.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.15/ellis_django_views/tests/views.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.642796 ellis_django_views-0.15/ellis_django_views/utils/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.15/ellis_django_views/utils/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.15/ellis_django_views/utils/error_messages.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.15/ellis_django_views/utils/request_params.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.15/ellis_django_views/utils/url_names.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.15/ellis_django_views/utils/url_paths.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.15/ellis_django_views/views_abstract.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.15/ellis_django_views/views_implementation.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 10:58:10.588642 ellis_django_views-0.15/ellis_django_views.egg-info/
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1075 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/SOURCES.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/dependency_links.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/requires.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 10:58:10.000000 ellis_django_views-0.15/ellis_django_views.egg-info/top_level.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 10:58:10.643771 ellis_django_views-0.15/setup.cfg
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1521 2024-05-21 10:57:51.000000 ellis_django_views-0.15/setup.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 11:26:04.112304 ellis_django_views-0.18/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.18/LICENSE
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.18/MANIFEST.in
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1075 2024-05-21 11:26:04.111901 ellis_django_views-0.18/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     2064 2024-05-21 11:25:38.000000 ellis_django_views-0.18/README.md
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 11:26:04.100166 ellis_django_views-0.18/ellis_django_views/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.18/ellis_django_views/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.18/ellis_django_views/apps.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 11:26:04.104218 ellis_django_views-0.18/ellis_django_views/migrations/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.18/ellis_django_views/migrations/0001_initial.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.18/ellis_django_views/migrations/__init__.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 11:26:04.108250 ellis_django_views-0.18/ellis_django_views/tests/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.18/ellis_django_views/tests/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.18/ellis_django_views/tests/models.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.18/ellis_django_views/tests/serializers.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.18/ellis_django_views/tests/test_views.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.18/ellis_django_views/tests/urls.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.18/ellis_django_views/tests/views.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 11:26:04.111218 ellis_django_views-0.18/ellis_django_views/utils/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.18/ellis_django_views/utils/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.18/ellis_django_views/utils/error_messages.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.18/ellis_django_views/utils/request_params.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.18/ellis_django_views/utils/url_names.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.18/ellis_django_views/utils/url_paths.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.18/ellis_django_views/views_abstract.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.18/ellis_django_views/views_implementation.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 11:26:04.103104 ellis_django_views-0.18/ellis_django_views.egg-info/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1075 2024-05-21 11:26:04.000000 ellis_django_views-0.18/ellis_django_views.egg-info/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 11:26:04.000000 ellis_django_views-0.18/ellis_django_views.egg-info/SOURCES.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 11:26:04.000000 ellis_django_views-0.18/ellis_django_views.egg-info/dependency_links.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 11:26:04.000000 ellis_django_views-0.18/ellis_django_views.egg-info/requires.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 11:26:04.000000 ellis_django_views-0.18/ellis_django_views.egg-info/top_level.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 11:26:04.112395 ellis_django_views-0.18/setup.cfg
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1521 2024-05-21 11:25:45.000000 ellis_django_views-0.18/setup.py
```

### Comparing `ellis_django_views-0.15/LICENSE` & `ellis_django_views-0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/PKG-INFO` & `ellis_django_views-0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis_django_views
-Version: 0.15
+Version: 0.18
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `ellis_django_views-0.15/ellis_django_views/migrations/0001_initial.py` & `ellis_django_views-0.18/ellis_django_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/ellis_django_views/tests/models.py` & `ellis_django_views-0.18/ellis_django_views/tests/models.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/ellis_django_views/tests/test_views.py` & `ellis_django_views-0.18/ellis_django_views/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/ellis_django_views/tests/urls.py` & `ellis_django_views-0.18/ellis_django_views/tests/urls.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/ellis_django_views/tests/views.py` & `ellis_django_views-0.18/ellis_django_views/tests/views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/ellis_django_views/utils/request_params.py` & `ellis_django_views-0.18/ellis_django_views/utils/request_params.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/ellis_django_views/views_abstract.py` & `ellis_django_views-0.18/ellis_django_views/views_abstract.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/ellis_django_views/views_implementation.py` & `ellis_django_views-0.18/ellis_django_views/views_implementation.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/ellis_django_views.egg-info/PKG-INFO` & `ellis_django_views-0.18/ellis_django_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis-django-views
-Version: 0.15
+Version: 0.18
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `ellis_django_views-0.15/ellis_django_views.egg-info/SOURCES.txt` & `ellis_django_views-0.18/ellis_django_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.15/setup.py` & `ellis_django_views-0.18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     include_package_data=True,
     name='ellis_django_views',
-    version='0.15',
+    version='0.18',
     packages=find_packages(),
     description='Generic views for Model View Serializer (MVS) pattern',
     author='Carl Victor Ellis',
     author_email='carl.ellis@hotmail.com.au',
     license='GNU',
     url='https://carlellis.io',
     long_description='Ellis views are generic views for Create, Request, Update and Delete views, simply define serializer_model, model and is_authorised methods.',
```

