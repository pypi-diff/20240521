# Comparing `tmp/django_mailing-0.2.3.tar.gz` & `tmp/django_mailing-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mailing-0.2.3.tar", last modified: Thu May 16 19:23:05 2024, max compression
+gzip compressed data, was "django_mailing-0.2.4.tar", last modified: Tue May 21 18:31:45 2024, max compression
```

## Comparing `django_mailing-0.2.3.tar` & `django_mailing-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.072550 django_mailing-0.2.3/
--rwxr-xr-x   0 jparadis   (501) staff       (20)      178 2023-05-05 14:19:38.000000 django_mailing-0.2.3/AUTHORS.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)       41 2023-05-05 14:19:38.000000 django_mailing-0.2.3/CHANGES.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1113 2023-05-05 14:19:38.000000 django_mailing-0.2.3/LICENSE.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)      134 2023-05-05 14:19:38.000000 django_mailing-0.2.3/MANIFEST.in
--rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-16 19:23:05.072117 django_mailing-0.2.3/PKG-INFO
--rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.3/README.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.071553 django_mailing-0.2.3/django_mailing.egg-info/
--rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/PKG-INFO
--rw-r--r--   0 jparadis   (501) staff       (20)      687 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/SOURCES.txt
--rw-r--r--   0 jparadis   (501) staff       (20)        1 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/dependency_links.txt
--rw-r--r--   0 jparadis   (501) staff       (20)       49 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/requires.txt
--rw-r--r--   0 jparadis   (501) staff       (20)        8 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/top_level.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.065151 django_mailing-0.2.3/docs/
--rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.3/docs/usage.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.068071 django_mailing-0.2.3/mailing/
--rwxr-xr-x   0 jparadis   (501) staff       (20)      525 2024-05-16 19:18:24.000000 django_mailing-0.2.3/mailing/__init__.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     5372 2024-05-16 19:14:13.000000 django_mailing-0.2.3/mailing/mail.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)        0 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/models.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     2307 2024-05-03 13:13:32.000000 django_mailing-0.2.3/mailing/shortcuts.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1938 2024-05-03 13:13:16.000000 django_mailing-0.2.3/mailing/tasks.py
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.059106 django_mailing-0.2.3/mailing/templates/
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.069004 django_mailing-0.2.3/mailing/templates/mailing/
--rwxr-xr-x   0 jparadis   (501) staff       (20)     3245 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/base.html
--rwxr-xr-x   0 jparadis   (501) staff       (20)      150 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/base.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.070993 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/
--rw-r--r--   0 jparadis   (501) staff       (20)     2555 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/README.markdown
--rw-r--r--   0 jparadis   (501) staff       (20)      352 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/contributors.txt
--rw-r--r--   0 jparadis   (501) staff       (20)    12246 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/email.html
--rw-r--r--   0 jparadis   (501) staff       (20)     6542 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/email_lite.html
--rwxr-xr-x   0 jparadis   (501) staff       (20)       26 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/views.py
--rw-r--r--   0 jparadis   (501) staff       (20)       38 2024-05-16 19:23:05.072638 django_mailing-0.2.3/setup.cfg
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1099 2023-05-05 14:19:38.000000 django_mailing-0.2.3/setup.py
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-21 18:31:45.647029 django_mailing-0.2.4/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      178 2023-05-05 14:19:38.000000 django_mailing-0.2.4/AUTHORS.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)       41 2023-05-05 14:19:38.000000 django_mailing-0.2.4/CHANGES.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     1113 2023-05-05 14:19:38.000000 django_mailing-0.2.4/LICENSE.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      134 2023-05-05 14:19:38.000000 django_mailing-0.2.4/MANIFEST.in
+-rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-21 18:31:45.646144 django_mailing-0.2.4/PKG-INFO
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.4/README.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-21 18:31:45.645597 django_mailing-0.2.4/django_mailing.egg-info/
+-rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-21 18:31:45.000000 django_mailing-0.2.4/django_mailing.egg-info/PKG-INFO
+-rw-r--r--   0 jparadis   (501) staff       (20)      687 2024-05-21 18:31:45.000000 django_mailing-0.2.4/django_mailing.egg-info/SOURCES.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)        1 2024-05-21 18:31:45.000000 django_mailing-0.2.4/django_mailing.egg-info/dependency_links.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)       49 2024-05-21 18:31:45.000000 django_mailing-0.2.4/django_mailing.egg-info/requires.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)        8 2024-05-21 18:31:45.000000 django_mailing-0.2.4/django_mailing.egg-info/top_level.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-21 18:31:45.637695 django_mailing-0.2.4/docs/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.4/docs/usage.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-21 18:31:45.641133 django_mailing-0.2.4/mailing/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      525 2024-05-21 16:17:12.000000 django_mailing-0.2.4/mailing/__init__.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     6922 2024-05-21 18:29:58.000000 django_mailing-0.2.4/mailing/mail.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)        0 2023-05-05 14:19:38.000000 django_mailing-0.2.4/mailing/models.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     2347 2024-05-21 15:14:58.000000 django_mailing-0.2.4/mailing/shortcuts.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     2000 2024-05-21 15:14:19.000000 django_mailing-0.2.4/mailing/tasks.py
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-21 18:31:45.631264 django_mailing-0.2.4/mailing/templates/
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-21 18:31:45.642355 django_mailing-0.2.4/mailing/templates/mailing/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     3245 2023-05-05 14:19:38.000000 django_mailing-0.2.4/mailing/templates/mailing/base.html
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      150 2023-05-05 14:19:38.000000 django_mailing-0.2.4/mailing/templates/mailing/base.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-21 18:31:45.644602 django_mailing-0.2.4/mailing/templates/mailing/email_boiletplate/
+-rw-r--r--   0 jparadis   (501) staff       (20)     2555 2023-05-05 14:19:38.000000 django_mailing-0.2.4/mailing/templates/mailing/email_boiletplate/README.markdown
+-rw-r--r--   0 jparadis   (501) staff       (20)      352 2023-05-05 14:19:38.000000 django_mailing-0.2.4/mailing/templates/mailing/email_boiletplate/contributors.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)    12246 2023-05-05 14:19:38.000000 django_mailing-0.2.4/mailing/templates/mailing/email_boiletplate/email.html
+-rw-r--r--   0 jparadis   (501) staff       (20)     6542 2023-05-05 14:19:38.000000 django_mailing-0.2.4/mailing/templates/mailing/email_boiletplate/email_lite.html
+-rwxr-xr-x   0 jparadis   (501) staff       (20)       26 2023-05-05 14:19:38.000000 django_mailing-0.2.4/mailing/views.py
+-rw-r--r--   0 jparadis   (501) staff       (20)       38 2024-05-21 18:31:45.647131 django_mailing-0.2.4/setup.cfg
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     1099 2023-05-05 14:19:38.000000 django_mailing-0.2.4/setup.py
```

### Comparing `django_mailing-0.2.3/LICENSE.txt` & `django_mailing-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.3/PKG-INFO` & `django_mailing-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailing
-Version: 0.2.3
+Version: 0.2.4
 Summary: A flexible Django app for templated mailings with support for celery queuing, SendGrid and more.
 Home-page: http://github.com/JeromeParadis/django-mailing
 Author: Jerome Paradis
 Author-email: jparadis@paradivision.com
 License: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django_mailing-0.2.3/README.txt` & `django_mailing-0.2.4/README.txt`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.3/django_mailing.egg-info/PKG-INFO` & `django_mailing-0.2.4/django_mailing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailing
-Version: 0.2.3
+Version: 0.2.4
 Summary: A flexible Django app for templated mailings with support for celery queuing, SendGrid and more.
 Home-page: http://github.com/JeromeParadis/django-mailing
 Author: Jerome Paradis
 Author-email: jparadis@paradivision.com
 License: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django_mailing-0.2.3/django_mailing.egg-info/SOURCES.txt` & `django_mailing-0.2.4/django_mailing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.3/docs/usage.txt` & `django_mailing-0.2.4/docs/usage.txt`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.3/mailing/__init__.py` & `django_mailing-0.2.4/mailing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Versioning
 # --------------------------------
 #VERSION = (0, 1, 0, "beta", 11) # following PEP 386
-VERSION = (0, 2, 3, "f") # following PEP 386
+VERSION = (0, 2, 4, "f") # following PEP 386
 DEV_N = None
 
 def get_version():
     version = "%s.%s" % (VERSION[0], VERSION[1])
     if VERSION[2]:
         version = "%s.%s" % (version, VERSION[2])
     if VERSION[3] != "f":
```

### Comparing `django_mailing-0.2.3/mailing/mail.py` & `django_mailing-0.2.4/mailing/mail.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from __future__ import absolute_import
 from django.conf import settings
 from django.core.mail import EmailMultiAlternatives, EmailMessage
+from django.core import mail
+from django.core.mail.backends.smtp import EmailBackend
 from django.template.loader import render_to_string
 from django.utils import translation
 import six
 import json 
 
 # Define exception classes
 # --------------------------------
+class MailerException(Exception):
+    pass
+
+class MailerConfigurationException(Exception):
+    pass
+
 class MailerInvalidBodyError(Exception):
-    def __init__(self, value):
-        self.value = value
-    def __str__(self):
-        return repr(self.value)
+    pass
 
 class MailerMissingSubjectError(Exception):
-    def __init__(self, value=None):
-        self.value = value
-    def __str__(self):
-        return repr(self.value if value else '')
+    pass
 
 def send_email_default(*args, **kwargs):
     send_email(args[3],args[0],args[1], from_email=args[2], category='django core email')
 
-def send_email(recipients, subject, text_content=None, html_content=None, from_email=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None, reply_to=None):
+def send_email(recipients, subject, text_content=None, html_content=None, from_email=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None, reply_to=None, options=None):
     """
     Will send a multi-format email to recipients. Email may be queued through celery
     """
     from django.conf import settings
     if not bypass_queue and hasattr(settings, 'MAILING_USE_CELERY') and settings.MAILING_USE_CELERY:
         from celery.execute import send_task
-        return send_task('mailing.queue_send_email',[recipients, subject, text_content, html_content, from_email, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files, reply_to])
+        return send_task('mailing.queue_send_email',[recipients, subject, text_content, html_content, from_email, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files, reply_to, options])
     else:
 
         header_category_value = '%s%s' % (settings.MAILING_HEADER_CATEGORY_PREFIX if hasattr(settings, 'MAILING_HEADER_CATEGORY_PREFIX') else '', category)
         # Check for sendgrid support and add category header
         # --------------------------------
         if hasattr(settings, 'MAILING_USE_SENDGRID'):
             send_grid_support = settings.MAILING_USE_SENDGRID
@@ -79,34 +81,61 @@
             recipients_list = [settings.MAILING_MAILTO_HIJACK]
 
         if not subject:
             raise MailerMissingSubjectError('Subject not supplied')
 
         # Send ascii, html or multi-part email
         # --------------------------------
-        if text_content or html_content:
-            if use_base_template:
-                prev_language = translation.get_language()
-                language and translation.activate(language)
-                text_content = render_to_string('mailing/base.txt', {'mailing_text_body': text_content, 'mailing_subject': subject, 'settings': settings}) if text_content else None
-                html_content = render_to_string('mailing/base.html', {'mailing_html_body': html_content, 'mailing_subject': subject, 'settings': settings}) if html_content else None
-                translation.activate(prev_language)
-            msg = EmailMultiAlternatives(subject, text_content if text_content else html_content, from_email if from_email else settings.DEFAULT_FROM_EMAIL, recipients_list, cc=cc, bcc=bcc, attachments=attachments, headers = headers, reply_to=reply_to)
-            if html_content and text_content:
-                msg.attach_alternative(html_content, "text/html")
-            elif html_content: # Only HTML
-                msg.content_subtype = "html"
-
-            # Attach files through attach_files helper
-            # --------------------------------
-            if attach_files:
-                for att in attach_files:  # attachments are tuples of (filepath, mimetype, filename)
-                    with open(att[0], 'rb') as f:
-                        content = f.read()
-                    msg.attach(att[2], content, att[1])
+        def get_connection():
+            if options and options.get('connection_name', None):
+                if options['connection_name'] in settings.EMAIL_CONNECTIONS:
+                    params = settings.EMAIL_CONNECTIONS[options['connection_name']]
+                    connection = mail.get_connection(
+                        host=params.get('HOST', None),
+                        port=params.get('PORT', None),
+                        username=params.get('HOST_USER', None),
+                        password=params.get('HOST_PASSWORD', None),
+                        use_tls=params.get('USE_TLS', None),
+                        use_ssl=params.get('USE_SSL', None),
+                        timeout=params.get('TIMEOUT', None),
+                        ssl_keyfile=params.get('SSL_KEYFILE', None),
+                        ssl_certfile=params.get('SSL_CERTFILE', None)
+                    )
+                    if headers and 'X-SMTPAPI' in headers:
+                        del headers['X-SMTPAPI']
+                else:
+                    raise MailerConfigurationException('Invalid connection name for email backend.')
+            elif options and options.get('connection', None):
+                connection = options['connection']
+            else:
+                connection = mail.get_connection()
+            return connection
 
-            # Send email
-            # --------------------------------
+        # raise Exception(options, connection, settings.EMAIL_CONNECTIONS)
 
-            msg.send(fail_silently=fail_silently)
+        if text_content or html_content:
+            with get_connection() as connection:
+                if use_base_template:
+                    prev_language = translation.get_language()
+                    language and translation.activate(language)
+                    text_content = render_to_string('mailing/base.txt', {'mailing_text_body': text_content, 'mailing_subject': subject, 'settings': settings}) if text_content else None
+                    html_content = render_to_string('mailing/base.html', {'mailing_html_body': html_content, 'mailing_subject': subject, 'settings': settings}) if html_content else None
+                    translation.activate(prev_language)
+                msg = EmailMultiAlternatives(subject, text_content if text_content else html_content, from_email if from_email else settings.DEFAULT_FROM_EMAIL, recipients_list, cc=cc, bcc=bcc, attachments=attachments, headers = headers, reply_to=reply_to, connection=connection)
+                if html_content and text_content:
+                    msg.attach_alternative(html_content, "text/html")
+                elif html_content: # Only HTML
+                    msg.content_subtype = "html"
+
+                # Attach files through attach_files helper
+                # --------------------------------
+                if attach_files:
+                    for att in attach_files:  # attachments are tuples of (filepath, mimetype, filename)
+                        with open(att[0], 'rb') as f:
+                            content = f.read()
+                        msg.attach(att[2], content, att[1])
+
+                # Send email
+                # --------------------------------
+                msg.send(fail_silently=fail_silently)
         else:
             raise MailerInvalidBodyError('No text or html body supplied.')
```

### Comparing `django_mailing-0.2.3/mailing/shortcuts.py` & `django_mailing-0.2.4/mailing/shortcuts.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from django.conf import settings
 from django.template.loader import render_to_string
 from django.template import TemplateDoesNotExist
 from django.utils import translation
 
 from mailing.mail import send_email
 
-def render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None, reply_to=None):
+def render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None, reply_to=None, options=None):
     if not bypass_queue and hasattr(settings, 'MAILING_USE_CELERY') and settings.MAILING_USE_CELERY:
         from celery.execute import send_task
-        return send_task('mailing.queue_render_send_email',[recipients, template, data, from_email, subject, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files, reply_to])
+        return send_task('mailing.queue_render_send_email',[recipients, template, data, from_email, subject, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files, reply_to, options])
     else:
         # Set language
         # --------------------------------
         prev_language = translation.get_language()
         language and translation.activate(language)
         if subject:
             my_subject = subject
@@ -35,9 +35,9 @@
 
         try:
             html_content = render_to_string('%s.html' % template, data)
         except TemplateDoesNotExist:
             html_content = None
 
         translation.activate(prev_language)
-        send_email(recipients, my_subject, text_content, html_content, from_email, use_base_template, category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to)
+        send_email(recipients, my_subject, text_content, html_content, from_email, use_base_template, category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to, options=options)
```

### Comparing `django_mailing-0.2.3/mailing/tasks.py` & `django_mailing-0.2.4/mailing/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 
 from celery.utils.log import get_task_logger
 
 logger = get_task_logger(__name__)
 
 @shared_task(name="mailing.queue_send_email")
-def queue_send_email(recipients, subject, text_content=None, html_content=None, from_email=settings.DEFAULT_FROM_EMAIL, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None, reply_to=None): 
+def queue_send_email(recipients, subject, text_content=None, html_content=None, from_email=settings.DEFAULT_FROM_EMAIL, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None, reply_to=None, options=None): 
     
     logger.debug('Sending %s to %s' % (subject, ','.join(recipients), ))
 
-    send_email(recipients=recipients, subject=subject, text_content=text_content, html_content=html_content, from_email=from_email, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to)
+    send_email(recipients=recipients, subject=subject, text_content=text_content, html_content=html_content, from_email=from_email, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to, options=options)
 
     return True
 
 @shared_task(name="mailing.queue_render_send_email")
-def queue_render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None, reply_to=None):
+def queue_render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None, reply_to=None, options=None):
     
     logger.debug('Rendering and sending %s to %s' % (template, ','.join(recipients), ))
 
-    render_send_email(recipients=recipients, template=template, data=data, from_email=from_email, subject=subject, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to)
+    render_send_email(recipients=recipients, template=template, data=data, from_email=from_email, subject=subject, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to, options=options)
 
     return True
```

### Comparing `django_mailing-0.2.3/mailing/templates/mailing/base.html` & `django_mailing-0.2.4/mailing/templates/mailing/base.html`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/README.markdown` & `django_mailing-0.2.4/mailing/templates/mailing/email_boiletplate/README.markdown`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/email.html` & `django_mailing-0.2.4/mailing/templates/mailing/email_boiletplate/email.html`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/email_lite.html` & `django_mailing-0.2.4/mailing/templates/mailing/email_boiletplate/email_lite.html`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.3/setup.py` & `django_mailing-0.2.4/setup.py`

 * *Files identical despite different names*

