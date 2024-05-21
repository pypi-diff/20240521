# Comparing `tmp/ellis_django_views-0.21.tar.gz` & `tmp/ellis_django_views-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellis_django_views-0.21.tar", last modified: Tue May 21 12:21:33 2024, max compression
+gzip compressed data, was "ellis_django_views-0.22.tar", last modified: Tue May 21 12:23:02 2024, max compression
```

## Comparing `ellis_django_views-0.21.tar` & `ellis_django_views-0.22.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:21:33.847112 ellis_django_views-0.21/
--rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.21/LICENSE
--rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.21/MANIFEST.in
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4676 2024-05-21 12:21:33.846611 ellis_django_views-0.21/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)     3738 2024-05-21 12:21:29.000000 ellis_django_views-0.21/README.md
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:21:33.827816 ellis_django_views-0.21/ellis_django_views/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.21/ellis_django_views/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.21/ellis_django_views/apps.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:21:33.838144 ellis_django_views-0.21/ellis_django_views/migrations/
--rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.21/ellis_django_views/migrations/0001_initial.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.21/ellis_django_views/migrations/__init__.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:21:33.842383 ellis_django_views-0.21/ellis_django_views/tests/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.21/ellis_django_views/tests/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.21/ellis_django_views/tests/models.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.21/ellis_django_views/tests/serializers.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.21/ellis_django_views/tests/test_views.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.21/ellis_django_views/tests/urls.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.21/ellis_django_views/tests/views.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:21:33.845851 ellis_django_views-0.21/ellis_django_views/utils/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.21/ellis_django_views/utils/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.21/ellis_django_views/utils/error_messages.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.21/ellis_django_views/utils/request_params.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.21/ellis_django_views/utils/url_names.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.21/ellis_django_views/utils/url_paths.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.21/ellis_django_views/views_abstract.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.21/ellis_django_views/views_implementation.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:21:33.836698 ellis_django_views-0.21/ellis_django_views.egg-info/
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4676 2024-05-21 12:21:33.000000 ellis_django_views-0.21/ellis_django_views.egg-info/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 12:21:33.000000 ellis_django_views-0.21/ellis_django_views.egg-info/SOURCES.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 12:21:33.000000 ellis_django_views-0.21/ellis_django_views.egg-info/dependency_links.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 12:21:33.000000 ellis_django_views-0.21/ellis_django_views.egg-info/requires.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 12:21:33.000000 ellis_django_views-0.21/ellis_django_views.egg-info/top_level.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 12:21:33.847206 ellis_django_views-0.21/setup.cfg
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1406 2024-05-21 12:21:24.000000 ellis_django_views-0.21/setup.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:23:02.150818 ellis_django_views-0.22/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.22/LICENSE
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.22/MANIFEST.in
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4648 2024-05-21 12:23:02.150474 ellis_django_views-0.22/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     3710 2024-05-21 12:22:49.000000 ellis_django_views-0.22/README.md
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:23:02.135053 ellis_django_views-0.22/ellis_django_views/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.22/ellis_django_views/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.22/ellis_django_views/apps.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:23:02.141846 ellis_django_views-0.22/ellis_django_views/migrations/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.22/ellis_django_views/migrations/0001_initial.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.22/ellis_django_views/migrations/__init__.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:23:02.147307 ellis_django_views-0.22/ellis_django_views/tests/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.22/ellis_django_views/tests/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.22/ellis_django_views/tests/models.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.22/ellis_django_views/tests/serializers.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.22/ellis_django_views/tests/test_views.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.22/ellis_django_views/tests/urls.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.22/ellis_django_views/tests/views.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:23:02.149949 ellis_django_views-0.22/ellis_django_views/utils/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.22/ellis_django_views/utils/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.22/ellis_django_views/utils/error_messages.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.22/ellis_django_views/utils/request_params.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.22/ellis_django_views/utils/url_names.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.22/ellis_django_views/utils/url_paths.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.22/ellis_django_views/views_abstract.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.22/ellis_django_views/views_implementation.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:23:02.140120 ellis_django_views-0.22/ellis_django_views.egg-info/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4648 2024-05-21 12:23:02.000000 ellis_django_views-0.22/ellis_django_views.egg-info/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 12:23:02.000000 ellis_django_views-0.22/ellis_django_views.egg-info/SOURCES.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 12:23:02.000000 ellis_django_views-0.22/ellis_django_views.egg-info/dependency_links.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 12:23:02.000000 ellis_django_views-0.22/ellis_django_views.egg-info/requires.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 12:23:02.000000 ellis_django_views-0.22/ellis_django_views.egg-info/top_level.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 12:23:02.150889 ellis_django_views-0.22/setup.cfg
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1406 2024-05-21 12:22:56.000000 ellis_django_views-0.22/setup.py
```

### Comparing `ellis_django_views-0.21/LICENSE` & `ellis_django_views-0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/PKG-INFO` & `ellis_django_views-0.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis_django_views
-Version: 0.21
+Version: 0.22
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -23,21 +23,21 @@
 License-File: LICENSE
 
 # Django Generic Ellis Views
 
 Django Generic Ellis Views provides generic views for Create, Retrieve, Update, and Delete operations, requiring only the definition of serializer, model, and authorization methods.
 
 ## Table of Contents
-- [Quick Start](#quick-start)
-- [Usage Example](#usage-example)
+- [Quick Start](#quick)
+- [Usage Example](#usage)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## Quick Start<a name="quick-start" />
+## Quick Start<a name="quick" />
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -68,15 +68,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## Usage Example<a name="usage-example" />
+## Usage Example<a name="usage" />
 
 1. Import CRUD views from `'ellis_django_views.views_implementation'` and your own models and serializers:
 
     ```python
     # django-project/django-app/views.py
     from DjangoApp.models import YourModel
     from DjangoApp.serializers import YourSerializer
```

### Comparing `ellis_django_views-0.21/README.md` & `ellis_django_views-0.22/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Django Generic Ellis Views
 
 Django Generic Ellis Views provides generic views for Create, Retrieve, Update, and Delete operations, requiring only the definition of serializer, model, and authorization methods.
 
 ## Table of Contents
-- [Quick Start](#quick-start)
-- [Usage Example](#usage-example)
+- [Quick Start](#quick)
+- [Usage Example](#usage)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## Quick Start<a name="quick-start" />
+## Quick Start<a name="quick" />
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -44,15 +44,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## Usage Example<a name="usage-example" />
+## Usage Example<a name="usage" />
 
 1. Import CRUD views from `'ellis_django_views.views_implementation'` and your own models and serializers:
 
     ```python
     # django-project/django-app/views.py
     from DjangoApp.models import YourModel
     from DjangoApp.serializers import YourSerializer
```

### Comparing `ellis_django_views-0.21/ellis_django_views/migrations/0001_initial.py` & `ellis_django_views-0.22/ellis_django_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/ellis_django_views/tests/models.py` & `ellis_django_views-0.22/ellis_django_views/tests/models.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/ellis_django_views/tests/test_views.py` & `ellis_django_views-0.22/ellis_django_views/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/ellis_django_views/tests/urls.py` & `ellis_django_views-0.22/ellis_django_views/tests/urls.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/ellis_django_views/tests/views.py` & `ellis_django_views-0.22/ellis_django_views/tests/views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/ellis_django_views/utils/request_params.py` & `ellis_django_views-0.22/ellis_django_views/utils/request_params.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/ellis_django_views/views_abstract.py` & `ellis_django_views-0.22/ellis_django_views/views_abstract.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/ellis_django_views/views_implementation.py` & `ellis_django_views-0.22/ellis_django_views/views_implementation.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/ellis_django_views.egg-info/PKG-INFO` & `ellis_django_views-0.22/ellis_django_views.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis-django-views
-Version: 0.21
+Version: 0.22
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -23,21 +23,21 @@
 License-File: LICENSE
 
 # Django Generic Ellis Views
 
 Django Generic Ellis Views provides generic views for Create, Retrieve, Update, and Delete operations, requiring only the definition of serializer, model, and authorization methods.
 
 ## Table of Contents
-- [Quick Start](#quick-start)
-- [Usage Example](#usage-example)
+- [Quick Start](#quick)
+- [Usage Example](#usage)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## Quick Start<a name="quick-start" />
+## Quick Start<a name="quick" />
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -68,15 +68,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## Usage Example<a name="usage-example" />
+## Usage Example<a name="usage" />
 
 1. Import CRUD views from `'ellis_django_views.views_implementation'` and your own models and serializers:
 
     ```python
     # django-project/django-app/views.py
     from DjangoApp.models import YourModel
     from DjangoApp.serializers import YourSerializer
```

### Comparing `ellis_django_views-0.21/ellis_django_views.egg-info/SOURCES.txt` & `ellis_django_views-0.22/ellis_django_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.21/setup.py` & `ellis_django_views-0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     include_package_data=True,
     name='ellis_django_views',
-    version='0.21',
+    version='0.22',
     packages=find_packages(),
     description='Generic views for Model View Serializer (MVS) pattern',
     author='Carl Victor Ellis',
     author_email='carl.ellis@hotmail.com.au',
     license='GNU',
     url='https://carlellis.io',
     long_description=open('README.md').read(),
```

