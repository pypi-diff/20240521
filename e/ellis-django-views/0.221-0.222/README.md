# Comparing `tmp/ellis_django_views-0.221.tar.gz` & `tmp/ellis_django_views-0.222.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellis_django_views-0.221.tar", last modified: Tue May 21 12:26:34 2024, max compression
+gzip compressed data, was "ellis_django_views-0.222.tar", last modified: Tue May 21 12:27:46 2024, max compression
```

## Comparing `ellis_django_views-0.221.tar` & `ellis_django_views-0.222.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:26:34.904855 ellis_django_views-0.221/
--rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.221/LICENSE
--rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.221/MANIFEST.in
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4654 2024-05-21 12:26:34.904549 ellis_django_views-0.221/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)     3715 2024-05-21 12:26:13.000000 ellis_django_views-0.221/README.md
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:26:34.868871 ellis_django_views-0.221/ellis_django_views/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.221/ellis_django_views/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.221/ellis_django_views/apps.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:26:34.878731 ellis_django_views-0.221/ellis_django_views/migrations/
--rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.221/ellis_django_views/migrations/0001_initial.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.221/ellis_django_views/migrations/__init__.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:26:34.894044 ellis_django_views-0.221/ellis_django_views/tests/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.221/ellis_django_views/tests/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.221/ellis_django_views/tests/models.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.221/ellis_django_views/tests/serializers.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.221/ellis_django_views/tests/test_views.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.221/ellis_django_views/tests/urls.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.221/ellis_django_views/tests/views.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:26:34.903945 ellis_django_views-0.221/ellis_django_views/utils/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.221/ellis_django_views/utils/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.221/ellis_django_views/utils/error_messages.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.221/ellis_django_views/utils/request_params.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.221/ellis_django_views/utils/url_names.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.221/ellis_django_views/utils/url_paths.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.221/ellis_django_views/views_abstract.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.221/ellis_django_views/views_implementation.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:26:34.875086 ellis_django_views-0.221/ellis_django_views.egg-info/
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4654 2024-05-21 12:26:34.000000 ellis_django_views-0.221/ellis_django_views.egg-info/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 12:26:34.000000 ellis_django_views-0.221/ellis_django_views.egg-info/SOURCES.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 12:26:34.000000 ellis_django_views-0.221/ellis_django_views.egg-info/dependency_links.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 12:26:34.000000 ellis_django_views-0.221/ellis_django_views.egg-info/requires.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 12:26:34.000000 ellis_django_views-0.221/ellis_django_views.egg-info/top_level.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 12:26:34.904984 ellis_django_views-0.221/setup.cfg
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1407 2024-05-21 12:26:28.000000 ellis_django_views-0.221/setup.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:27:46.958989 ellis_django_views-0.222/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.222/LICENSE
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.222/MANIFEST.in
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4669 2024-05-21 12:27:46.958692 ellis_django_views-0.222/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     3730 2024-05-21 12:27:36.000000 ellis_django_views-0.222/README.md
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:27:46.945194 ellis_django_views-0.222/ellis_django_views/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.222/ellis_django_views/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.222/ellis_django_views/apps.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:27:46.951467 ellis_django_views-0.222/ellis_django_views/migrations/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.222/ellis_django_views/migrations/0001_initial.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.222/ellis_django_views/migrations/__init__.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:27:46.954906 ellis_django_views-0.222/ellis_django_views/tests/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.222/ellis_django_views/tests/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.222/ellis_django_views/tests/models.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.222/ellis_django_views/tests/serializers.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.222/ellis_django_views/tests/test_views.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.222/ellis_django_views/tests/urls.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.222/ellis_django_views/tests/views.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:27:46.958106 ellis_django_views-0.222/ellis_django_views/utils/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.222/ellis_django_views/utils/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.222/ellis_django_views/utils/error_messages.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.222/ellis_django_views/utils/request_params.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.222/ellis_django_views/utils/url_names.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.222/ellis_django_views/utils/url_paths.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.222/ellis_django_views/views_abstract.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.222/ellis_django_views/views_implementation.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:27:46.950224 ellis_django_views-0.222/ellis_django_views.egg-info/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4669 2024-05-21 12:27:46.000000 ellis_django_views-0.222/ellis_django_views.egg-info/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 12:27:46.000000 ellis_django_views-0.222/ellis_django_views.egg-info/SOURCES.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 12:27:46.000000 ellis_django_views-0.222/ellis_django_views.egg-info/dependency_links.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 12:27:46.000000 ellis_django_views-0.222/ellis_django_views.egg-info/requires.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 12:27:46.000000 ellis_django_views-0.222/ellis_django_views.egg-info/top_level.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 12:27:46.959065 ellis_django_views-0.222/setup.cfg
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1407 2024-05-21 12:27:44.000000 ellis_django_views-0.222/setup.py
```

### Comparing `ellis_django_views-0.221/LICENSE` & `ellis_django_views-0.222/LICENSE`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/PKG-INFO` & `ellis_django_views-0.222/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis_django_views
-Version: 0.221
+Version: 0.222
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -29,15 +29,15 @@
 ## Table of Contents
 - [Quick Start](#quick)
 - [Usage Example](#usage)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## <a name="quick" /> Quick Start
+## <a name="quick" ><a/> Quick Start
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -68,15 +68,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## <a name="usage" /> Usage Example
+## <a name="usage" ><a/> Usage Example
 
 1. Import CRUD views from `'ellis_django_views.views_implementation'` and your own models and serializers:
 
     ```python
     # django-project/django-app/views.py
     from DjangoApp.models import YourModel
     from DjangoApp.serializers import YourSerializer
@@ -130,22 +130,22 @@
         path('post/', CreateView.as_view(), name='create'),
         path('get/', RequestView.as_view(), name='get'),
         path('put/', UpdateView.as_view(), name='put'),
         path('delete/', DeleteView.as_view(), name='delete'),
     ]
     ```
 
-## <a name="features" /> Features
+## <a name="features" ><a/> Features
 
 - **Simplified CRUD Operations**: Easily create, retrieve, update, and delete views with minimal setup.
 - **Authorization Support**: Implement custom authorization logic.
 - **Serializer Integration**: Define serializers for your models to handle validation and representation.
 - **Test URLs**: Built-in support for testing your views.
 
-## <a name="contributing" /> Contributing
+## <a name="contributing" ><a/> Contributing
 
 If you have any suggestions or would like to contribute, please get in contact with [Carl Ellis](mailto:carl.ellis@hotmail.com.au).
 
-## <a name="license" /> License
+## <a name="license" ><a/> License
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ellis_django_views-0.221/README.md` & `ellis_django_views-0.222/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## Table of Contents
 - [Quick Start](#quick)
 - [Usage Example](#usage)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## <a name="quick" /> Quick Start
+## <a name="quick" ><a/> Quick Start
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -44,15 +44,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## <a name="usage" /> Usage Example
+## <a name="usage" ><a/> Usage Example
 
 1. Import CRUD views from `'ellis_django_views.views_implementation'` and your own models and serializers:
 
     ```python
     # django-project/django-app/views.py
     from DjangoApp.models import YourModel
     from DjangoApp.serializers import YourSerializer
@@ -106,21 +106,21 @@
         path('post/', CreateView.as_view(), name='create'),
         path('get/', RequestView.as_view(), name='get'),
         path('put/', UpdateView.as_view(), name='put'),
         path('delete/', DeleteView.as_view(), name='delete'),
     ]
     ```
 
-## <a name="features" /> Features
+## <a name="features" ><a/> Features
 
 - **Simplified CRUD Operations**: Easily create, retrieve, update, and delete views with minimal setup.
 - **Authorization Support**: Implement custom authorization logic.
 - **Serializer Integration**: Define serializers for your models to handle validation and representation.
 - **Test URLs**: Built-in support for testing your views.
 
-## <a name="contributing" /> Contributing
+## <a name="contributing" ><a/> Contributing
 
 If you have any suggestions or would like to contribute, please get in contact with [Carl Ellis](mailto:carl.ellis@hotmail.com.au).
 
-## <a name="license" /> License
+## <a name="license" ><a/> License
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ellis_django_views-0.221/ellis_django_views/migrations/0001_initial.py` & `ellis_django_views-0.222/ellis_django_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/ellis_django_views/tests/models.py` & `ellis_django_views-0.222/ellis_django_views/tests/models.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/ellis_django_views/tests/test_views.py` & `ellis_django_views-0.222/ellis_django_views/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/ellis_django_views/tests/urls.py` & `ellis_django_views-0.222/ellis_django_views/tests/urls.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/ellis_django_views/tests/views.py` & `ellis_django_views-0.222/ellis_django_views/tests/views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/ellis_django_views/utils/request_params.py` & `ellis_django_views-0.222/ellis_django_views/utils/request_params.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/ellis_django_views/views_abstract.py` & `ellis_django_views-0.222/ellis_django_views/views_abstract.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/ellis_django_views/views_implementation.py` & `ellis_django_views-0.222/ellis_django_views/views_implementation.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/ellis_django_views.egg-info/PKG-INFO` & `ellis_django_views-0.222/ellis_django_views.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis-django-views
-Version: 0.221
+Version: 0.222
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -29,15 +29,15 @@
 ## Table of Contents
 - [Quick Start](#quick)
 - [Usage Example](#usage)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## <a name="quick" /> Quick Start
+## <a name="quick" ><a/> Quick Start
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -68,15 +68,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## <a name="usage" /> Usage Example
+## <a name="usage" ><a/> Usage Example
 
 1. Import CRUD views from `'ellis_django_views.views_implementation'` and your own models and serializers:
 
     ```python
     # django-project/django-app/views.py
     from DjangoApp.models import YourModel
     from DjangoApp.serializers import YourSerializer
@@ -130,22 +130,22 @@
         path('post/', CreateView.as_view(), name='create'),
         path('get/', RequestView.as_view(), name='get'),
         path('put/', UpdateView.as_view(), name='put'),
         path('delete/', DeleteView.as_view(), name='delete'),
     ]
     ```
 
-## <a name="features" /> Features
+## <a name="features" ><a/> Features
 
 - **Simplified CRUD Operations**: Easily create, retrieve, update, and delete views with minimal setup.
 - **Authorization Support**: Implement custom authorization logic.
 - **Serializer Integration**: Define serializers for your models to handle validation and representation.
 - **Test URLs**: Built-in support for testing your views.
 
-## <a name="contributing" /> Contributing
+## <a name="contributing" ><a/> Contributing
 
 If you have any suggestions or would like to contribute, please get in contact with [Carl Ellis](mailto:carl.ellis@hotmail.com.au).
 
-## <a name="license" /> License
+## <a name="license" ><a/> License
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ellis_django_views-0.221/ellis_django_views.egg-info/SOURCES.txt` & `ellis_django_views-0.222/ellis_django_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.221/setup.py` & `ellis_django_views-0.222/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     include_package_data=True,
     name='ellis_django_views',
-    version='0.221',
+    version='0.222',
     packages=find_packages(),
     description='Generic views for Model View Serializer (MVS) pattern',
     author='Carl Victor Ellis',
     author_email='carl.ellis@hotmail.com.au',
     license='GNU',
     url='https://carlellis.io',
     long_description=open('README.md').read(),
```

