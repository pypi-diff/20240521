# Comparing `tmp/django_outlook_email_backend-1.1.5.tar.gz` & `tmp/django_outlook_email_backend-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-1.1.5.tar", last modified: Mon May 13 14:49:45 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-1.1.6.tar", last modified: Tue May 21 15:38:20 2024, max compression
```

## Comparing `django_outlook_email_backend-1.1.5.tar` & `django_outlook_email_backend-1.1.6.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:49:45.241500 django_outlook_email_backend-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 14:49:45.241500 django_outlook_email_backend-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:49:45.241500 django_outlook_email_backend-1.1.5/django_outlook_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/django_outlook_email_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:49:45.241500 django_outlook_email_backend-1.1.5/django_outlook_email/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/exceptions/microsoft_graph_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:49:45.241500 django_outlook_email_backend-1.1.5/django_outlook_email/senders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/senders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/senders/base_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/senders/content_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/senders/json_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/django_outlook_email/senders/mime_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:49:45.241500 django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 14:49:45.000000 django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 14:49:45.000000 django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:49:45.000000 django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 14:49:45.000000 django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 14:49:45.000000 django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:49:45.000000 django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:49:45.241500 django_outlook_email_backend-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 14:49:39.000000 django_outlook_email_backend-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.810405 django_outlook_email_backend-1.1.6/django_outlook_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/django_outlook_email_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.810405 django_outlook_email_backend-1.1.6/django_outlook_email/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/exceptions/microsoft_graph_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.810405 django_outlook_email_backend-1.1.6/django_outlook_email/senders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/django_outlook_email/senders/attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/attachments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/attachments/attachments_using_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/base_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/content_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/json_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/django_outlook_email/senders/microsoft_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/microsoft_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/microsoft_requests/microsoft_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/django_outlook_email/senders/mime_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:38:20.000000 django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:38:20.814405 django_outlook_email_backend-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 15:38:14.000000 django_outlook_email_backend-1.1.6/setup.py
```

### Comparing `django_outlook_email_backend-1.1.5/LICENSE` & `django_outlook_email_backend-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.5/PKG-INFO` & `django_outlook_email_backend-1.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.1.5
+Version: 1.1.6
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -17,14 +17,18 @@
 License-File: LICENSE
 Requires-Dist: requests~=2.25
 Requires-Dist: msal==1.*
 
 # Django outlook email backend
 ### Outlook api email backend for Django
 
+## First steps
+Retrieve the client id, client secret and tenant id from the Azure portal. Follow this steps:https://learn.microsoft.com/en-us/industry/retail/intelligent-recommendations/quickstart-endpoint
+Add the Mail.send permision to the app in the Azure portal.
+
 ## Requirements
 - Python 3.8+
 - Django 5.0, 4.2
 
 ## Installation
 Install using pip...
 ```commandline
```

### Comparing `django_outlook_email_backend-1.1.5/django_outlook_email/django_outlook_email_backend.py` & `django_outlook_email_backend-1.1.6/django_outlook_email/django_outlook_email_backend.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.5/django_outlook_email/senders/content_types.py` & `django_outlook_email_backend-1.1.6/django_outlook_email/senders/content_types.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.5/django_outlook_email/senders/mime_sender.py` & `django_outlook_email_backend-1.1.6/django_outlook_email/senders/mime_sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         encoding = email_message.encoding or settings.DEFAULT_CHARSET
         from_email = sanitize_address(email_message.from_email, encoding)
 
         message = email_message.message()
 
         try:
             response = requests.post(
-                "https://graph.microsoft.com/v1.0/users/" + from_email + "/sendMail",
+                "https://outlook.office365.com/v1.0/users/" + from_email + "/sendMail",
                 data=base64.b64encode(message.as_bytes(linesep="\r\n")),
 
                 headers={"Authorization": "Bearer " + self.access_token, "Content-type": "text/plain"}
             )
         except requests.exceptions.RequestException:
             if not self.fail_silently:
                 raise
```

### Comparing `django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/PKG-INFO` & `django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.1.5
+Version: 1.1.6
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -17,14 +17,18 @@
 License-File: LICENSE
 Requires-Dist: requests~=2.25
 Requires-Dist: msal==1.*
 
 # Django outlook email backend
 ### Outlook api email backend for Django
 
+## First steps
+Retrieve the client id, client secret and tenant id from the Azure portal. Follow this steps:https://learn.microsoft.com/en-us/industry/retail/intelligent-recommendations/quickstart-endpoint
+Add the Mail.send permision to the app in the Azure portal.
+
 ## Requirements
 - Python 3.8+
 - Django 5.0, 4.2
 
 ## Installation
 Install using pip...
 ```commandline
```

### Comparing `django_outlook_email_backend-1.1.5/django_outlook_email_backend.egg-info/SOURCES.txt` & `django_outlook_email_backend-1.1.6/django_outlook_email_backend.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,13 +6,17 @@
 django_outlook_email/exceptions/__init__.py
 django_outlook_email/exceptions/microsoft_graph_exceptions.py
 django_outlook_email/senders/__init__.py
 django_outlook_email/senders/base_sender.py
 django_outlook_email/senders/content_types.py
 django_outlook_email/senders/json_sender.py
 django_outlook_email/senders/mime_sender.py
+django_outlook_email/senders/attachments/__init__.py
+django_outlook_email/senders/attachments/attachments_using_upload_session.py
+django_outlook_email/senders/microsoft_requests/__init__.py
+django_outlook_email/senders/microsoft_requests/microsoft_requests.py
 django_outlook_email_backend.egg-info/PKG-INFO
 django_outlook_email_backend.egg-info/SOURCES.txt
 django_outlook_email_backend.egg-info/dependency_links.txt
 django_outlook_email_backend.egg-info/requires.txt
 django_outlook_email_backend.egg-info/top_level.txt
 django_outlook_email_backend.egg-info/zip-safe
```

