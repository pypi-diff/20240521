# Comparing `tmp/ellis_django_views-0.1888.tar.gz` & `tmp/ellis_django_views-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellis_django_views-0.1888.tar", last modified: Tue May 21 12:05:29 2024, max compression
+gzip compressed data, was "ellis_django_views-0.2.tar", last modified: Tue May 21 12:18:59 2024, max compression
```

## Comparing `ellis_django_views-0.1888.tar` & `ellis_django_views-0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:05:29.014016 ellis_django_views-0.1888/
--rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.1888/LICENSE
--rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.1888/MANIFEST.in
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4562 2024-05-21 12:05:29.013622 ellis_django_views-0.1888/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)     3622 2024-05-21 12:05:12.000000 ellis_django_views-0.1888/README.md
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:05:28.978185 ellis_django_views-0.1888/ellis_django_views/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.1888/ellis_django_views/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.1888/ellis_django_views/apps.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:05:28.985398 ellis_django_views-0.1888/ellis_django_views/migrations/
--rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.1888/ellis_django_views/migrations/0001_initial.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.1888/ellis_django_views/migrations/__init__.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:05:29.009767 ellis_django_views-0.1888/ellis_django_views/tests/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.1888/ellis_django_views/tests/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.1888/ellis_django_views/tests/models.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.1888/ellis_django_views/tests/serializers.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.1888/ellis_django_views/tests/test_views.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.1888/ellis_django_views/tests/urls.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.1888/ellis_django_views/tests/views.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:05:29.012839 ellis_django_views-0.1888/ellis_django_views/utils/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.1888/ellis_django_views/utils/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.1888/ellis_django_views/utils/error_messages.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.1888/ellis_django_views/utils/request_params.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.1888/ellis_django_views/utils/url_names.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.1888/ellis_django_views/utils/url_paths.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.1888/ellis_django_views/views_abstract.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.1888/ellis_django_views/views_implementation.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:05:28.983109 ellis_django_views-0.1888/ellis_django_views.egg-info/
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4562 2024-05-21 12:05:28.000000 ellis_django_views-0.1888/ellis_django_views.egg-info/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 12:05:28.000000 ellis_django_views-0.1888/ellis_django_views.egg-info/SOURCES.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 12:05:28.000000 ellis_django_views-0.1888/ellis_django_views.egg-info/dependency_links.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 12:05:28.000000 ellis_django_views-0.1888/ellis_django_views.egg-info/requires.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 12:05:28.000000 ellis_django_views-0.1888/ellis_django_views.egg-info/top_level.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 12:05:29.014150 ellis_django_views-0.1888/setup.cfg
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1408 2024-05-21 12:05:24.000000 ellis_django_views-0.1888/setup.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:18:59.095550 ellis_django_views-0.2/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.2/LICENSE
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.2/MANIFEST.in
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4675 2024-05-21 12:18:59.095246 ellis_django_views-0.2/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     3738 2024-05-21 12:18:38.000000 ellis_django_views-0.2/README.md
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:18:59.075544 ellis_django_views-0.2/ellis_django_views/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.2/ellis_django_views/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.2/ellis_django_views/apps.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:18:59.086756 ellis_django_views-0.2/ellis_django_views/migrations/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.2/ellis_django_views/migrations/0001_initial.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.2/ellis_django_views/migrations/__init__.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:18:59.091481 ellis_django_views-0.2/ellis_django_views/tests/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.2/ellis_django_views/tests/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.2/ellis_django_views/tests/models.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.2/ellis_django_views/tests/serializers.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.2/ellis_django_views/tests/test_views.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.2/ellis_django_views/tests/urls.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.2/ellis_django_views/tests/views.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:18:59.094671 ellis_django_views-0.2/ellis_django_views/utils/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.2/ellis_django_views/utils/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.2/ellis_django_views/utils/error_messages.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.2/ellis_django_views/utils/request_params.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.2/ellis_django_views/utils/url_names.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.2/ellis_django_views/utils/url_paths.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.2/ellis_django_views/views_abstract.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.2/ellis_django_views/views_implementation.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:18:59.084554 ellis_django_views-0.2/ellis_django_views.egg-info/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4675 2024-05-21 12:18:59.000000 ellis_django_views-0.2/ellis_django_views.egg-info/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 12:18:59.000000 ellis_django_views-0.2/ellis_django_views.egg-info/SOURCES.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 12:18:59.000000 ellis_django_views-0.2/ellis_django_views.egg-info/dependency_links.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 12:18:59.000000 ellis_django_views-0.2/ellis_django_views.egg-info/requires.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 12:18:59.000000 ellis_django_views-0.2/ellis_django_views.egg-info/top_level.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 12:18:59.095624 ellis_django_views-0.2/setup.cfg
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1405 2024-05-21 12:18:55.000000 ellis_django_views-0.2/setup.py
```

### Comparing `ellis_django_views-0.1888/LICENSE` & `ellis_django_views-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/PKG-INFO` & `ellis_django_views-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis_django_views
-Version: 0.1888
+Version: 0.2
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -29,15 +29,15 @@
 ## Table of Contents
 - [Quick Start](#quick-start)
 - [Usage Example](#usage-example)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## Quick Start
+## Quick Start<a name="quick-start" />
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -68,15 +68,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## Usage Example
+## Usage Example<a name="usage-example" />
 
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
 
-## Features
+## Features<a name="features" />
 
 - **Simplified CRUD Operations**: Easily create, retrieve, update, and delete views with minimal setup.
 - **Authorization Support**: Implement custom authorization logic.
 - **Serializer Integration**: Define serializers for your models to handle validation and representation.
 - **Test URLs**: Built-in support for testing your views.
 
-## Contributing
+## Contributing<a name="contributing" />
 
 If you have any suggestions or would like to contribute, please get in contact with [Carl Ellis](mailto:carl.ellis@hotmail.com.au).
 
-## License
+## License<a name="license" />
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ellis_django_views-0.1888/README.md` & `ellis_django_views-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## Table of Contents
 - [Quick Start](#quick-start)
 - [Usage Example](#usage-example)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## Quick Start
+## Quick Start<a name="quick-start" />
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -44,15 +44,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## Usage Example
+## Usage Example<a name="usage-example" />
 
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
 
-## Features
+## Features<a name="features" />
 
 - **Simplified CRUD Operations**: Easily create, retrieve, update, and delete views with minimal setup.
 - **Authorization Support**: Implement custom authorization logic.
 - **Serializer Integration**: Define serializers for your models to handle validation and representation.
 - **Test URLs**: Built-in support for testing your views.
 
-## Contributing
+## Contributing<a name="contributing" />
 
 If you have any suggestions or would like to contribute, please get in contact with [Carl Ellis](mailto:carl.ellis@hotmail.com.au).
 
-## License
+## License<a name="license" />
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ellis_django_views-0.1888/ellis_django_views/migrations/0001_initial.py` & `ellis_django_views-0.2/ellis_django_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/ellis_django_views/tests/models.py` & `ellis_django_views-0.2/ellis_django_views/tests/models.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/ellis_django_views/tests/test_views.py` & `ellis_django_views-0.2/ellis_django_views/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/ellis_django_views/tests/urls.py` & `ellis_django_views-0.2/ellis_django_views/tests/urls.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/ellis_django_views/tests/views.py` & `ellis_django_views-0.2/ellis_django_views/tests/views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/ellis_django_views/utils/request_params.py` & `ellis_django_views-0.2/ellis_django_views/utils/request_params.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/ellis_django_views/views_abstract.py` & `ellis_django_views-0.2/ellis_django_views/views_abstract.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/ellis_django_views/views_implementation.py` & `ellis_django_views-0.2/ellis_django_views/views_implementation.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/ellis_django_views.egg-info/PKG-INFO` & `ellis_django_views-0.2/ellis_django_views.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis-django-views
-Version: 0.1888
+Version: 0.2
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -29,15 +29,15 @@
 ## Table of Contents
 - [Quick Start](#quick-start)
 - [Usage Example](#usage-example)
 - [Features](#features)
 - [Contributing](#contributing)
 - [License](#license)
 
-## Quick Start
+## Quick Start<a name="quick-start" />
 
 1. Add `'ellis_django_views'` to your `INSTALLED_APPS` in `settings.py`:
 
     ```python
     # django-project/settings.py
 
     INSTALLED_APPS = [
@@ -68,15 +68,15 @@
 
 4. Run tests:
 
     ```bash
     python manage.py test ellis_django_views
     ```
 
-## Usage Example
+## Usage Example<a name="usage-example" />
 
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
 
-## Features
+## Features<a name="features" />
 
 - **Simplified CRUD Operations**: Easily create, retrieve, update, and delete views with minimal setup.
 - **Authorization Support**: Implement custom authorization logic.
 - **Serializer Integration**: Define serializers for your models to handle validation and representation.
 - **Test URLs**: Built-in support for testing your views.
 
-## Contributing
+## Contributing<a name="contributing" />
 
 If you have any suggestions or would like to contribute, please get in contact with [Carl Ellis](mailto:carl.ellis@hotmail.com.au).
 
-## License
+## License<a name="license" />
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ellis_django_views-0.1888/ellis_django_views.egg-info/SOURCES.txt` & `ellis_django_views-0.2/ellis_django_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.1888/setup.py` & `ellis_django_views-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     include_package_data=True,
     name='ellis_django_views',
-    version='0.1888',
+    version='0.2',
     packages=find_packages(),
     description='Generic views for Model View Serializer (MVS) pattern',
     author='Carl Victor Ellis',
     author_email='carl.ellis@hotmail.com.au',
     license='GNU',
     url='https://carlellis.io',
     long_description=open('README.md').read(),
```

