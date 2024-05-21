# Comparing `tmp/django_allauth_ui-0.3.1.tar.gz` & `tmp/django_allauth_ui-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allauth_ui-0.3.1.tar", max compression
+gzip compressed data, was "django_allauth_ui-0.3.2.tar", max compression
```

## Comparing `django_allauth_ui-0.3.1.tar` & `django_allauth_ui-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1069 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.1/LICENSE
--rw-r--r--   0        0        0       22 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.1/allauth_ui/__init__.py
--rw-r--r--   0        0        0       94 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.1/allauth_ui/apps.py
--rw-r--r--   0        0        0     8374 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.1/allauth_ui/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8352 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.1/allauth_ui/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      532 2022-12-20 01:16:52.519135 django_allauth_ui-0.3.1/allauth_ui/static/allauth_ui/input.css
--rw-r--r--   0        0        0    35561 2022-12-20 01:53:25.418792 django_allauth_ui-0.3.1/allauth_ui/static/allauth_ui/output.css
--rw-r--r--   0        0        0     1428 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/_button.html
--rw-r--r--   0        0        0      267 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/_links.html
--rw-r--r--   0        0        0      242 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/_non_field_errors.html
--rw-r--r--   0        0        0      925 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/_render_form.html
--rw-r--r--   0        0        0     1197 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/base.html
--rw-r--r--   0        0        0     1128 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/email_confirm.html
--rw-r--r--   0        0        0     2289 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/login.html
--rw-r--r--   0        0        0      445 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/logout.html
--rw-r--r--   0        0        0      752 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset.html
--rw-r--r--   0        0        0     1416 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     1329 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      554 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      686 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/signup.html
--rw-r--r--   0        0        0      643 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/signup_closed.html
--rw-r--r--   0        0        0      830 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/verification_sent.html
--rw-r--r--   0        0        0      749 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0       34 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/base.html
--rw-r--r--   0        0        0     2140 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1396 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/login.html
--rw-r--r--   0        0        0      808 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/signup.html
--rw-r--r--   0        0        0      796 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      560 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/snippets/social_login.html
--rw-r--r--   0        0        0      786 2024-05-21 01:59:06.184416 django_allauth_ui-0.3.1/allauth_ui/templatetags/allauth_ui.py
--rw-r--r--   0        0        0     1147 2024-05-21 02:37:11.874358 django_allauth_ui-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.2/LICENSE
+-rw-r--r--   0        0        0       22 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.2/allauth_ui/__init__.py
+-rw-r--r--   0        0        0       94 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.2/allauth_ui/apps.py
+-rw-r--r--   0        0        0     8374 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.2/allauth_ui/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8352 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.2/allauth_ui/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      532 2022-12-20 01:16:52.519135 django_allauth_ui-0.3.2/allauth_ui/static/allauth_ui/input.css
+-rw-r--r--   0        0        0    35561 2022-12-20 01:53:25.418792 django_allauth_ui-0.3.2/allauth_ui/static/allauth_ui/output.css
+-rw-r--r--   0        0        0     1428 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/_button.html
+-rw-r--r--   0        0        0      267 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/_links.html
+-rw-r--r--   0        0        0      242 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/_non_field_errors.html
+-rw-r--r--   0        0        0      925 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/_render_form.html
+-rw-r--r--   0        0        0     1197 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/base.html
+-rw-r--r--   0        0        0     1128 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     2289 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/login.html
+-rw-r--r--   0        0        0      445 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/logout.html
+-rw-r--r--   0        0        0      752 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset.html
+-rw-r--r--   0        0        0     1416 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     1329 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      554 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      912 2024-05-21 17:44:35.015917 django_allauth_ui-0.3.2/allauth_ui/templates/account/signup.html
+-rw-r--r--   0        0        0      643 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      830 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      749 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0       34 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/base.html
+-rw-r--r--   0        0        0     2140 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1396 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      808 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0      796 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      560 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/snippets/social_login.html
+-rw-r--r--   0        0        0      786 2024-05-21 01:59:06.184416 django_allauth_ui-0.3.2/allauth_ui/templatetags/allauth_ui.py
+-rw-r--r--   0        0        0     1147 2024-05-21 17:44:38.176280 django_allauth_ui-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.2/PKG-INFO
```

### Comparing `django_allauth_ui-0.3.1/LICENSE` & `django_allauth_ui-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/locale/es/LC_MESSAGES/django.po` & `django_allauth_ui-0.3.2/allauth_ui/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/locale/fr/LC_MESSAGES/django.po` & `django_allauth_ui-0.3.2/allauth_ui/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/static/allauth_ui/input.css` & `django_allauth_ui-0.3.2/allauth_ui/static/allauth_ui/input.css`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/static/allauth_ui/output.css` & `django_allauth_ui-0.3.2/allauth_ui/static/allauth_ui/output.css`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/_button.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/_button.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/_render_form.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/_render_form.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/base.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/base.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/email_confirm.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/login.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_done.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_from_key.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_from_key_done.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/signup.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/signup.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-{% extends "account/base.html" %}
+{% extends "socialaccount/base.html" %}
 {% load i18n %}
 {% block head_title %}
-    {% translate "Sign up" %}
+    {% trans "Sign Up" %}
 {% endblock %}
 {% block whitebox %}
-    <h1 class="mb-5 text-3xl text-center">Sign up</h1>
-    <form id="signup_form"
+    <h1 class="mb-5 text-3xl text-center">{% trans "Sign Up" %}</h1>
+    <p class="my-5">
+        {% blocktrans with provider_name=account.get_provider.name site_name=site.name %}
+  You are about to use your {{provider_name}} account to login to
+  {{site_name}}. As a final step, please complete the following form:
+{% endblocktrans %}
+    </p>
+    <form class="signup"
+          id="signup_form"
           method="post"
-          action="{% url 'account_signup' %}"
-          novalidate>
+          action="{% url 'socialaccount_signup' %}">
         {% include "account/_render_form.html" %}
         {% translate "Sign up" as signup_text %}
         {% include "account/_button.html" with text=signup_text %}
     </form>
-    <a class="self-center pt-8 text-xs text-blue-400 justify-self-center hover:text-blue-500"
-       href="{{ login_url }}">{% translate "Already have an account? Sign in." %}</a>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/signup_closed.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/account/verification_sent.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/authentication_error.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/connections.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/login.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/signup.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/account/signup.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-{% extends "socialaccount/base.html" %}
-{% load i18n %}
+{% extends "account/base.html" %}
+{% load i18n allauth_ui %}
 {% block head_title %}
-    {% trans "Sign Up" %}
+    {% translate "Sign up" %}
 {% endblock %}
 {% block whitebox %}
-    <h1 class="mb-5 text-3xl text-center">{% trans "Sign Up" %}</h1>
-    <p class="my-5">
-        {% blocktrans with provider_name=account.get_provider.name site_name=site.name %}
-  You are about to use your {{provider_name}} account to login to
-  {{site_name}}. As a final step, please complete the following form:
-{% endblocktrans %}
-    </p>
-    <form class="signup"
-          id="signup_form"
+    <h1 class="mb-5 text-3xl text-center">Sign up</h1>
+    <form id="signup_form"
           method="post"
-          action="{% url 'socialaccount_signup' %}">
+          action="{% url 'account_signup' %}"
+          novalidate>
         {% include "account/_render_form.html" %}
         {% translate "Sign up" as signup_text %}
         {% include "account/_button.html" with text=signup_text %}
     </form>
+    <a class="self-center pt-8 text-xs text-blue-400 justify-self-center hover:text-blue-500"
+       href="{{ login_url }}">{% translate "Already have an account? Sign in." %}</a>
+    {% check_allauth_socialaccount_installed as is_allauth_socialaccount_installed %}
+    {% if is_allauth_socialaccount_installed %}
+        {% include "socialaccount/snippets/social_login.html" %}
+    {% endif %}
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/snippets/provider_list.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/snippets/social_login.html` & `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/snippets/social_login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/allauth_ui/templatetags/allauth_ui.py` & `django_allauth_ui-0.3.2/allauth_ui/templatetags/allauth_ui.py`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.1/pyproject.toml` & `django_allauth_ui-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-allauth-ui"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Dani Hodovic <you@example.com>"]
 license = "MIT"
 packages = [
     { include = "allauth_ui" },
 ]
 include = ["allauth_ui/static/allauth_ui/output.css"]
```

### Comparing `django_allauth_ui-0.3.1/PKG-INFO` & `django_allauth_ui-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-ui
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 License: MIT
 Author: Dani Hodovic
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

