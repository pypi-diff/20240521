# Comparing `tmp/django_outlook_email_backend-1.1.6.tar.gz` & `tmp/django_outlook_email_backend-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-1.1.6.tar", last modified: Tue May 21 15:38:20 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-1.1.7.tar", last modified: Tue May 21 15:41:33 2024, max compression
```

## Comparing `django_outlook_email_backend-1.1.6.tar` & `django_outlook_email_backend-1.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.810405 django_outlook_email_backend-1.1.6/django_outlook_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/django_outlook_email_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.810405 django_outlook_email_backend-1.1.6/django_outlook_email/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/exceptions/microsoft_graph_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.810405 django_outlook_email_backend-1.1.6/django_outlook_email/senders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/django_outlook_email/senders/attachments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/attachments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/attachments/attachments_using_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/base_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/content_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/json_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/django_outlook_email/senders/microsoft_requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/microsoft_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/microsoft_requests/microsoft_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/mime_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:33.266749 django_outlook_email_backend-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-21 15:41:33.266749 django_outlook_email_backend-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:33.262749 django_outlook_email_backend-1.1.7/django_outlook_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/django_outlook_email_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:33.262749 django_outlook_email_backend-1.1.7/django_outlook_email/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/exceptions/microsoft_graph_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:33.266749 django_outlook_email_backend-1.1.7/django_outlook_email/senders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:33.266749 django_outlook_email_backend-1.1.7/django_outlook_email/senders/attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/attachments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/attachments/attachments_using_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/base_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/content_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/json_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:33.266749 django_outlook_email_backend-1.1.7/django_outlook_email/senders/microsoft_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/microsoft_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/microsoft_requests/microsoft_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/django_outlook_email/senders/mime_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:33.266749 django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-21 15:41:33.000000 django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 15:41:33.000000 django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:41:33.000000 django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 15:41:33.000000 django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 15:41:33.000000 django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:41:33.000000 django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:41:33.266749 django_outlook_email_backend-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 15:41:29.000000 django_outlook_email_backend-1.1.7/setup.py
```

### Comparing `django_outlook_email_backend-1.1.6/LICENSE` & `django_outlook_email_backend-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/PKG-INFO` & `django_outlook_email_backend-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.1.6
+Version: 1.1.7
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-1.1.6/README.md` & `django_outlook_email_backend-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/django_outlook_email/django_outlook_email_backend.py` & `django_outlook_email_backend-1.1.7/django_outlook_email/django_outlook_email_backend.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/django_outlook_email/senders/attachments/attachments_using_upload_session.py` & `django_outlook_email_backend-1.1.7/django_outlook_email/senders/attachments/attachments_using_upload_session.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/django_outlook_email/senders/content_types.py` & `django_outlook_email_backend-1.1.7/django_outlook_email/senders/content_types.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/django_outlook_email/senders/json_sender.py` & `django_outlook_email_backend-1.1.7/django_outlook_email/senders/json_sender.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/django_outlook_email/senders/microsoft_requests/microsoft_requests.py` & `django_outlook_email_backend-1.1.7/django_outlook_email/senders/microsoft_requests/microsoft_requests.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/django_outlook_email/senders/mime_sender.py` & `django_outlook_email_backend-1.1.7/django_outlook_email/senders/mime_sender.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/PKG-INFO` & `django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.1.6
+Version: 1.1.7
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/SOURCES.txt` & `django_outlook_email_backend-1.1.7/django_outlook_email_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.6/setup.py` & `django_outlook_email_backend-1.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='django_outlook_email-backend',
-    version='1.1.6',
+    version='1.1.7',
     description='Ouauth2 outlook email backend for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marc Claramunt',
     author_email='mclaramunt@enley.com',
     license='MIT',
     zip_safe=True,
```

