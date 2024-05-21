# Comparing `tmp/baseapp-message-templates-1.7.tar.gz` & `tmp/baseapp-message-templates-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp-message-templates-1.7.tar", last modified: Thu Feb  1 17:59:52 2024, max compression
+gzip compressed data, was "baseapp-message-templates-1.8.tar", last modified: Tue May 21 13:17:19 2024, max compression
```

## Comparing `baseapp-message-templates-1.7.tar` & `baseapp-message-templates-1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:52.268276 baseapp-message-templates-1.7/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-02-01 17:59:52.268276 baseapp-message-templates-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:52.264276 baseapp-message-templates-1.7/baseapp_message_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/custom_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:52.264276 baseapp-message-templates-1.7/baseapp_message_templates/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/migrations/0002_auto_20240108_1503.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/migrations/0003_alter_emailtemplate_name_alter_smstemplate_name.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/sms_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:52.264276 baseapp-message-templates-1.7/baseapp_message_templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/tests/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:52.264276 baseapp-message-templates-1.7/baseapp_message_templates/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/tests/unit/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/baseapp_message_templates/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:52.264276 baseapp-message-templates-1.7/baseapp_message_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-02-01 17:59:51.000000 baseapp-message-templates-1.7/baseapp_message_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-02-01 17:59:52.000000 baseapp-message-templates-1.7/baseapp_message_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 17:59:51.000000 baseapp-message-templates-1.7/baseapp_message_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-01 17:59:51.000000 baseapp-message-templates-1.7/baseapp_message_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 17:59:51.000000 baseapp-message-templates-1.7/baseapp_message_templates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-01 17:59:52.268276 baseapp-message-templates-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:52.264276 baseapp-message-templates-1.7/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-01 17:59:49.000000 baseapp-message-templates-1.7/testproject/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:19.741272 baseapp-message-templates-1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-05-21 13:17:19.741272 baseapp-message-templates-1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:19.737272 baseapp-message-templates-1.8/baseapp_message_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/custom_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:19.741272 baseapp-message-templates-1.8/baseapp_message_templates/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/migrations/0002_auto_20240108_1503.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/migrations/0003_alter_emailtemplate_name_alter_smstemplate_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/sms_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:19.741272 baseapp-message-templates-1.8/baseapp_message_templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/tests/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:19.741272 baseapp-message-templates-1.8/baseapp_message_templates/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/tests/unit/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/baseapp_message_templates/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:19.737272 baseapp-message-templates-1.8/baseapp_message_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-05-21 13:17:19.000000 baseapp-message-templates-1.8/baseapp_message_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 13:17:19.000000 baseapp-message-templates-1.8/baseapp_message_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:17:19.000000 baseapp-message-templates-1.8/baseapp_message_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-21 13:17:19.000000 baseapp-message-templates-1.8/baseapp_message_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:17:19.000000 baseapp-message-templates-1.8/baseapp_message_templates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 13:17:19.741272 baseapp-message-templates-1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:19.741272 baseapp-message-templates-1.8/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-21 13:17:18.000000 baseapp-message-templates-1.8/testproject/settings.py
```

### Comparing `baseapp-message-templates-1.7/PKG-INFO` & `baseapp-message-templates-1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-message-templates
-Version: 1.7
+Version: 1.8
 Summary: A BaseApp app that allows the use of customizable e-mail and sms templates.
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause
 Description: 
         # BaseApp Message Templates - Django
@@ -181,27 +181,35 @@
         
         Once you've added `html_content` to your template, either programatically or through the Django Admin, a message can now be sent through the `send` method of `EmailTemplate`. 
         
         The only required parameter for `send` is `recipients`, which is a list of one or more strings containing the e-mail addresses of the recipients. A `context` dict can be passed in optionally if the HTML content is expected one or more key/value pairs to be provided.
         
         The `use_base_template` flag will determine whether this message should extend from a base HTML template. If set to `True`, the message will extend from the base template that is located at a certain path. This path will either be the value of `extended_with` if provided, or the value of `DEFAULT_EMAIL_TEMPLATE`. 
         
-        Finally, the `attachments` parameter is a list of one or more files that will be send along with this particular message. These attachments will be sent along with any static attachments that have been attached to the template itself through `Attachment`.
+        The `attachments` parameter is a list of one or more files that will be send along with this particular message. These attachments will be sent along with any static attachments that have been attached to the template itself through `Attachment`.
+        
+        Finally, the `subject` parameter is a string, which will override the copy template subject if passed.
         
         ```py
         from baseapp_message_templates.models import EmailTemplate
         
         
         template = EmailTemplate.objects.get("Test Template")
         
         recipients = ["john@test.com"]
         context = {"content": "Hello."}
         extended_with = "apps/base/templates/test-template.html"
         
         template.send(recipients, context, True, extended_with)
+        
+        # example with attachments and custom subject
+        attachments = [attch_1, ...]
+        subject = f'Custom subject {var}'
+        template.send(recipients, context, True, extended_with, 
+                      attachments=attachments, subject=subject)
         ```
         
         ### SmsTemplate Model
         
         The `SmsTemplate` model has two fields:
         * `name`: this name must be unique.
         * `message`: this is a textfield and does not accept HTML
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: baseapp-message-templates Version: 1.7 Summary: A
+Metadata-Version: 2.1 Name: baseapp-message-templates Version: 1.8 Summary: A
 BaseApp app that allows the use of customizable e-mail and sms templates. Home-
 page: https://github.com/silverlogic/baseapp-backend Author: The SilverLogic
 Author-email: dev@tsl.io License: BSD-3-Clause Description: # BaseApp Message
 Templates - Django This app provides the integration of custom e-mail and sms
 template configuration with The SilverLogic's [BaseApp](https://bitbucket.org/
 silverlogic/baseapp-django-v2). ## Install the package Add to `requirements/
 base.txt`: ```bash git+https://bitbucket.org/silverlogic/baseapp-message-
@@ -97,33 +97,37 @@
 `send` is `recipients`, which is a list of one or more strings containing the
 e-mail addresses of the recipients. A `context` dict can be passed in
 optionally if the HTML content is expected one or more key/value pairs to be
 provided. The `use_base_template` flag will determine whether this message
 should extend from a base HTML template. If set to `True`, the message will
 extend from the base template that is located at a certain path. This path will
 either be the value of `extended_with` if provided, or the value of
-`DEFAULT_EMAIL_TEMPLATE`. Finally, the `attachments` parameter is a list of one
-or more files that will be send along with this particular message. These
-attachments will be sent along with any static attachments that have been
-attached to the template itself through `Attachment`. ```py from
+`DEFAULT_EMAIL_TEMPLATE`. The `attachments` parameter is a list of one or more
+files that will be send along with this particular message. These attachments
+will be sent along with any static attachments that have been attached to the
+template itself through `Attachment`. Finally, the `subject` parameter is a
+string, which will override the copy template subject if passed. ```py from
 baseapp_message_templates.models import EmailTemplate template =
 EmailTemplate.objects.get("Test Template") recipients = ["john@test.com"]
 context = {"content": "Hello."} extended_with = "apps/base/templates/test-
-template.html" template.send(recipients, context, True, extended_with) ``` ###
-SmsTemplate Model The `SmsTemplate` model has two fields: * `name`: this name
-must be unique. * `message`: this is a textfield and does not accept HTML ###
-Creating migrations for your template Once you have installed the package you
-can simply create a migration to input your templates like so: ```py from
-__future__ import unicode_literals from django.db import migrations def
-create_object(sms_template, name, message): sms_template.objects.create
-( name=name, message=message, ) def create_sms_templates(apps,
-schema_migration): sms_template = apps.get_model("baseapp_message_templates",
-"SmsTemplate") create_object( sms_template, "First Template", """ Hello, {
-{ some_variable }}. """, ) create_object( sms_template, "Second template", """
-Hello, {{ some_other_variable }}. """, ) class Migration(migrations.Migration):
+template.html" template.send(recipients, context, True, extended_with) #
+example with attachments and custom subject attachments = [attch_1, ...]
+subject = f'Custom subject {var}' template.send(recipients, context, True,
+extended_with, attachments=attachments, subject=subject) ``` ### SmsTemplate
+Model The `SmsTemplate` model has two fields: * `name`: this name must be
+unique. * `message`: this is a textfield and does not accept HTML ### Creating
+migrations for your template Once you have installed the package you can simply
+create a migration to input your templates like so: ```py from __future__
+import unicode_literals from django.db import migrations def create_object
+(sms_template, name, message): sms_template.objects.create( name=name,
+message=message, ) def create_sms_templates(apps, schema_migration):
+sms_template = apps.get_model("baseapp_message_templates", "SmsTemplate")
+create_object( sms_template, "First Template", """ Hello, {{ some_variable }}.
+""", ) create_object( sms_template, "Second template", """ Hello, {
+{ some_other_variable }}. """, ) class Migration(migrations.Migration):
 dependencies = [("some_app", "0002_some_previus_migration")] operations =
 [migrations.RunPython(create_sms_templates, migrations.RunPython.noop)] ```
 OBS: make sure that the variables are the right ones that you will pass as
 context when getting the message. ### Get the template message To get the
 template message you can simply use the util functions `get_sms_message` from
 `sms_utils` passing as first parameter the name of the template and the second
 parameter the context with your variables if needed. ```py from
```

### Comparing `baseapp-message-templates-1.7/README.md` & `baseapp-message-templates-1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -173,27 +173,35 @@
 
 Once you've added `html_content` to your template, either programatically or through the Django Admin, a message can now be sent through the `send` method of `EmailTemplate`. 
 
 The only required parameter for `send` is `recipients`, which is a list of one or more strings containing the e-mail addresses of the recipients. A `context` dict can be passed in optionally if the HTML content is expected one or more key/value pairs to be provided.
 
 The `use_base_template` flag will determine whether this message should extend from a base HTML template. If set to `True`, the message will extend from the base template that is located at a certain path. This path will either be the value of `extended_with` if provided, or the value of `DEFAULT_EMAIL_TEMPLATE`. 
 
-Finally, the `attachments` parameter is a list of one or more files that will be send along with this particular message. These attachments will be sent along with any static attachments that have been attached to the template itself through `Attachment`.
+The `attachments` parameter is a list of one or more files that will be send along with this particular message. These attachments will be sent along with any static attachments that have been attached to the template itself through `Attachment`.
+
+Finally, the `subject` parameter is a string, which will override the copy template subject if passed.
 
 ```py
 from baseapp_message_templates.models import EmailTemplate
 
 
 template = EmailTemplate.objects.get("Test Template")
 
 recipients = ["john@test.com"]
 context = {"content": "Hello."}
 extended_with = "apps/base/templates/test-template.html"
 
 template.send(recipients, context, True, extended_with)
+
+# example with attachments and custom subject
+attachments = [attch_1, ...]
+subject = f'Custom subject {var}'
+template.send(recipients, context, True, extended_with, 
+              attachments=attachments, subject=subject)
 ```
 
 ### SmsTemplate Model
 
 The `SmsTemplate` model has two fields:
 * `name`: this name must be unique.
 * `message`: this is a textfield and does not accept HTML
```

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/admin.py` & `baseapp-message-templates-1.8/baseapp_message_templates/admin.py`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/custom_templates.py` & `baseapp-message-templates-1.8/baseapp_message_templates/custom_templates.py`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/filters.py` & `baseapp-message-templates-1.8/baseapp_message_templates/filters.py`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/migrations/0001_initial.py` & `baseapp-message-templates-1.8/baseapp_message_templates/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/migrations/0002_auto_20240108_1503.py` & `baseapp-message-templates-1.8/baseapp_message_templates/migrations/0002_auto_20240108_1503.py`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/migrations/0003_alter_emailtemplate_name_alter_smstemplate_name.py` & `baseapp-message-templates-1.8/baseapp_message_templates/migrations/0003_alter_emailtemplate_name_alter_smstemplate_name.py`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/models.py` & `baseapp-message-templates-1.8/baseapp_message_templates/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,27 +62,28 @@
     def send(
         self,
         recipients: List[str],
         context={},
         use_base_template=False,
         extended_with="",
         attachments=[],
+        custom_subject="",
     ):
         if not self.html_content:
             raise Exception("HTML content required to send e-mail")
 
         if not use_base_template:
             base_template_route = ""
         else:
             base_template_route = extended_with or settings.DEFAULT_EMAIL_TEMPLATE
 
-        html_content, text_content, subject = get_full_copy_template(
+        html_content, text_content, copy_template_subject = get_full_copy_template(
             self, context, use_base_template, base_template_route
         )
-
+        subject = custom_subject if custom_subject else copy_template_subject
         mail = EmailMultiAlternatives(
             subject, text_content, from_email=settings.DEFAULT_FROM_EMAIL, to=recipients
         )
 
         # combine static attachments from template with dynamic attachments
         mail.attach_alternative(html_content, "text/html")
         all_attachments = list(self.static_attachments.all()) + attachments
```

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/sendgrid.py` & `baseapp-message-templates-1.8/baseapp_message_templates/sendgrid.py`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/tests/unit/test_templates.py` & `baseapp-message-templates-1.8/baseapp_message_templates/tests/unit/test_templates.py`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates/utils.py` & `baseapp-message-templates-1.8/baseapp_message_templates/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import uuid
 from itertools import islice
 from typing import Iterator
 
+from django.core.files.uploadedfile import InMemoryUploadedFile, TemporaryUploadedFile
 from django.core.mail import EmailMessage
 from django.utils.deconstruct import deconstructible
 
 
 @deconstructible
 class random_name_in(object):
     def __init__(self, dir):
@@ -17,14 +18,20 @@
         filename = "{}.{}".format(uuid.uuid4(), ext)
         return os.path.join(self.dir, filename)
 
 
 def attach_files(mail: EmailMessage, attachments):
     for attachment in attachments:
         attachment_file = attachment.file if hasattr(attachment, "file") else attachment
-        name = attachment.filename if hasattr(attachment, "filename") else attachment_file.name
+        if isinstance(attachment, TemporaryUploadedFile) or isinstance(
+            attachment, InMemoryUploadedFile
+        ):
+            name = attachment.name
+        else:
+            name = attachment.filename if hasattr(attachment, "filename") else attachment_file.name
+
         mail.attach(name, attachment_file.read())
 
 
 def chunk(it: Iterator, size: int):
     it = iter(it)
     return iter(lambda: tuple(islice(it, size)), ())
```

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates.egg-info/PKG-INFO` & `baseapp-message-templates-1.8/baseapp_message_templates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-message-templates
-Version: 1.7
+Version: 1.8
 Summary: A BaseApp app that allows the use of customizable e-mail and sms templates.
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause
 Description: 
         # BaseApp Message Templates - Django
@@ -181,27 +181,35 @@
         
         Once you've added `html_content` to your template, either programatically or through the Django Admin, a message can now be sent through the `send` method of `EmailTemplate`. 
         
         The only required parameter for `send` is `recipients`, which is a list of one or more strings containing the e-mail addresses of the recipients. A `context` dict can be passed in optionally if the HTML content is expected one or more key/value pairs to be provided.
         
         The `use_base_template` flag will determine whether this message should extend from a base HTML template. If set to `True`, the message will extend from the base template that is located at a certain path. This path will either be the value of `extended_with` if provided, or the value of `DEFAULT_EMAIL_TEMPLATE`. 
         
-        Finally, the `attachments` parameter is a list of one or more files that will be send along with this particular message. These attachments will be sent along with any static attachments that have been attached to the template itself through `Attachment`.
+        The `attachments` parameter is a list of one or more files that will be send along with this particular message. These attachments will be sent along with any static attachments that have been attached to the template itself through `Attachment`.
+        
+        Finally, the `subject` parameter is a string, which will override the copy template subject if passed.
         
         ```py
         from baseapp_message_templates.models import EmailTemplate
         
         
         template = EmailTemplate.objects.get("Test Template")
         
         recipients = ["john@test.com"]
         context = {"content": "Hello."}
         extended_with = "apps/base/templates/test-template.html"
         
         template.send(recipients, context, True, extended_with)
+        
+        # example with attachments and custom subject
+        attachments = [attch_1, ...]
+        subject = f'Custom subject {var}'
+        template.send(recipients, context, True, extended_with, 
+                      attachments=attachments, subject=subject)
         ```
         
         ### SmsTemplate Model
         
         The `SmsTemplate` model has two fields:
         * `name`: this name must be unique.
         * `message`: this is a textfield and does not accept HTML
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: baseapp-message-templates Version: 1.7 Summary: A
+Metadata-Version: 2.1 Name: baseapp-message-templates Version: 1.8 Summary: A
 BaseApp app that allows the use of customizable e-mail and sms templates. Home-
 page: https://github.com/silverlogic/baseapp-backend Author: The SilverLogic
 Author-email: dev@tsl.io License: BSD-3-Clause Description: # BaseApp Message
 Templates - Django This app provides the integration of custom e-mail and sms
 template configuration with The SilverLogic's [BaseApp](https://bitbucket.org/
 silverlogic/baseapp-django-v2). ## Install the package Add to `requirements/
 base.txt`: ```bash git+https://bitbucket.org/silverlogic/baseapp-message-
@@ -97,33 +97,37 @@
 `send` is `recipients`, which is a list of one or more strings containing the
 e-mail addresses of the recipients. A `context` dict can be passed in
 optionally if the HTML content is expected one or more key/value pairs to be
 provided. The `use_base_template` flag will determine whether this message
 should extend from a base HTML template. If set to `True`, the message will
 extend from the base template that is located at a certain path. This path will
 either be the value of `extended_with` if provided, or the value of
-`DEFAULT_EMAIL_TEMPLATE`. Finally, the `attachments` parameter is a list of one
-or more files that will be send along with this particular message. These
-attachments will be sent along with any static attachments that have been
-attached to the template itself through `Attachment`. ```py from
+`DEFAULT_EMAIL_TEMPLATE`. The `attachments` parameter is a list of one or more
+files that will be send along with this particular message. These attachments
+will be sent along with any static attachments that have been attached to the
+template itself through `Attachment`. Finally, the `subject` parameter is a
+string, which will override the copy template subject if passed. ```py from
 baseapp_message_templates.models import EmailTemplate template =
 EmailTemplate.objects.get("Test Template") recipients = ["john@test.com"]
 context = {"content": "Hello."} extended_with = "apps/base/templates/test-
-template.html" template.send(recipients, context, True, extended_with) ``` ###
-SmsTemplate Model The `SmsTemplate` model has two fields: * `name`: this name
-must be unique. * `message`: this is a textfield and does not accept HTML ###
-Creating migrations for your template Once you have installed the package you
-can simply create a migration to input your templates like so: ```py from
-__future__ import unicode_literals from django.db import migrations def
-create_object(sms_template, name, message): sms_template.objects.create
-( name=name, message=message, ) def create_sms_templates(apps,
-schema_migration): sms_template = apps.get_model("baseapp_message_templates",
-"SmsTemplate") create_object( sms_template, "First Template", """ Hello, {
-{ some_variable }}. """, ) create_object( sms_template, "Second template", """
-Hello, {{ some_other_variable }}. """, ) class Migration(migrations.Migration):
+template.html" template.send(recipients, context, True, extended_with) #
+example with attachments and custom subject attachments = [attch_1, ...]
+subject = f'Custom subject {var}' template.send(recipients, context, True,
+extended_with, attachments=attachments, subject=subject) ``` ### SmsTemplate
+Model The `SmsTemplate` model has two fields: * `name`: this name must be
+unique. * `message`: this is a textfield and does not accept HTML ### Creating
+migrations for your template Once you have installed the package you can simply
+create a migration to input your templates like so: ```py from __future__
+import unicode_literals from django.db import migrations def create_object
+(sms_template, name, message): sms_template.objects.create( name=name,
+message=message, ) def create_sms_templates(apps, schema_migration):
+sms_template = apps.get_model("baseapp_message_templates", "SmsTemplate")
+create_object( sms_template, "First Template", """ Hello, {{ some_variable }}.
+""", ) create_object( sms_template, "Second template", """ Hello, {
+{ some_other_variable }}. """, ) class Migration(migrations.Migration):
 dependencies = [("some_app", "0002_some_previus_migration")] operations =
 [migrations.RunPython(create_sms_templates, migrations.RunPython.noop)] ```
 OBS: make sure that the variables are the right ones that you will pass as
 context when getting the message. ### Get the template message To get the
 template message you can simply use the util functions `get_sms_message` from
 `sms_utils` passing as first parameter the name of the template and the second
 parameter the context with your variables if needed. ```py from
```

### Comparing `baseapp-message-templates-1.7/baseapp_message_templates.egg-info/SOURCES.txt` & `baseapp-message-templates-1.8/baseapp_message_templates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseapp-message-templates-1.7/setup.cfg` & `baseapp-message-templates-1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = baseapp_message_templates
-version = 1.7
+version = 1.8
 description = A BaseApp app that allows the use of customizable e-mail and sms templates.
 long_description = file: README.md
 url = https://github.com/silverlogic/baseapp-backend
 author = The SilverLogic
 author_email = dev@tsl.io
 license = BSD-3-Clause
 classifiers =
```

