# Comparing `tmp/django_allauth_ui-0.3.2.tar.gz` & `tmp/django_allauth_ui-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allauth_ui-0.3.2.tar", max compression
+gzip compressed data, was "django_allauth_ui-0.3.3.tar", max compression
```

## Comparing `django_allauth_ui-0.3.2.tar` & `django_allauth_ui-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1069 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.2/LICENSE
--rw-r--r--   0        0        0       22 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.2/allauth_ui/__init__.py
--rw-r--r--   0        0        0       94 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.2/allauth_ui/apps.py
--rw-r--r--   0        0        0     8374 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.2/allauth_ui/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8352 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.2/allauth_ui/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      532 2022-12-20 01:16:52.519135 django_allauth_ui-0.3.2/allauth_ui/static/allauth_ui/input.css
--rw-r--r--   0        0        0    35561 2022-12-20 01:53:25.418792 django_allauth_ui-0.3.2/allauth_ui/static/allauth_ui/output.css
--rw-r--r--   0        0        0     1428 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/_button.html
--rw-r--r--   0        0        0      267 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/_links.html
--rw-r--r--   0        0        0      242 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/_non_field_errors.html
--rw-r--r--   0        0        0      925 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/_render_form.html
--rw-r--r--   0        0        0     1197 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/base.html
--rw-r--r--   0        0        0     1128 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/email_confirm.html
--rw-r--r--   0        0        0     2289 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/login.html
--rw-r--r--   0        0        0      445 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/logout.html
--rw-r--r--   0        0        0      752 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset.html
--rw-r--r--   0        0        0     1416 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     1329 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      554 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      912 2024-05-21 17:44:35.015917 django_allauth_ui-0.3.2/allauth_ui/templates/account/signup.html
--rw-r--r--   0        0        0      643 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/signup_closed.html
--rw-r--r--   0        0        0      830 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/account/verification_sent.html
--rw-r--r--   0        0        0      749 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0       34 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/base.html
--rw-r--r--   0        0        0     2140 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1396 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/login.html
--rw-r--r--   0        0        0      808 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/signup.html
--rw-r--r--   0        0        0      796 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      560 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/snippets/social_login.html
--rw-r--r--   0        0        0      786 2024-05-21 01:59:06.184416 django_allauth_ui-0.3.2/allauth_ui/templatetags/allauth_ui.py
--rw-r--r--   0        0        0     1147 2024-05-21 17:44:38.176280 django_allauth_ui-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3385 2023-12-18 19:19:03.900925 django_allauth_ui-0.3.3/README.md
+-rw-r--r--   0        0        0       22 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.3/allauth_ui/__init__.py
+-rw-r--r--   0        0        0       94 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.3/allauth_ui/apps.py
+-rw-r--r--   0        0        0     8374 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.3/allauth_ui/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8352 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.3/allauth_ui/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      532 2022-12-20 01:16:52.519135 django_allauth_ui-0.3.3/allauth_ui/static/allauth_ui/input.css
+-rw-r--r--   0        0        0    35561 2022-12-20 01:53:25.418792 django_allauth_ui-0.3.3/allauth_ui/static/allauth_ui/output.css
+-rw-r--r--   0        0        0     1428 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/_button.html
+-rw-r--r--   0        0        0      267 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/_links.html
+-rw-r--r--   0        0        0      242 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/_non_field_errors.html
+-rw-r--r--   0        0        0      925 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/_render_form.html
+-rw-r--r--   0        0        0     1197 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/base.html
+-rw-r--r--   0        0        0     1128 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     2289 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/login.html
+-rw-r--r--   0        0        0      445 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/logout.html
+-rw-r--r--   0        0        0      752 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/password_reset.html
+-rw-r--r--   0        0        0     1416 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     1329 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      554 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      912 2024-05-21 17:44:35.015917 django_allauth_ui-0.3.3/allauth_ui/templates/account/signup.html
+-rw-r--r--   0        0        0      643 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      830 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      749 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0       34 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/base.html
+-rw-r--r--   0        0        0     2140 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1396 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      808 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0      796 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      560 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/snippets/social_login.html
+-rw-r--r--   0        0        0      786 2024-05-21 01:59:06.184416 django_allauth_ui-0.3.3/allauth_ui/templatetags/allauth_ui.py
+-rw-r--r--   0        0        0     1168 2024-05-21 19:39:53.910911 django_allauth_ui-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.3/PKG-INFO
```

### Comparing `django_allauth_ui-0.3.2/LICENSE` & `django_allauth_ui-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/locale/es/LC_MESSAGES/django.po` & `django_allauth_ui-0.3.3/allauth_ui/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/locale/fr/LC_MESSAGES/django.po` & `django_allauth_ui-0.3.3/allauth_ui/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/static/allauth_ui/input.css` & `django_allauth_ui-0.3.3/allauth_ui/static/allauth_ui/input.css`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/static/allauth_ui/output.css` & `django_allauth_ui-0.3.3/allauth_ui/static/allauth_ui/output.css`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/_button.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/_button.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/_render_form.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/_render_form.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/base.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/base.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/email_confirm.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/login.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_done.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_from_key.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/password_reset_from_key_done.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/signup.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/signup_closed.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/account/verification_sent.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/authentication_error.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/connections.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/login.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/signup.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/snippets/provider_list.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templates/socialaccount/snippets/social_login.html` & `django_allauth_ui-0.3.3/allauth_ui/templates/socialaccount/snippets/social_login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/allauth_ui/templatetags/allauth_ui.py` & `django_allauth_ui-0.3.3/allauth_ui/templatetags/allauth_ui.py`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.2/pyproject.toml` & `django_allauth_ui-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-allauth-ui"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["Dani Hodovic <you@example.com>"]
 license = "MIT"
 packages = [
     { include = "allauth_ui" },
 ]
 include = ["allauth_ui/static/allauth_ui/output.css"]
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
 django-widget-tweaks = "^1.4.12"
 
 [tool.poetry.dev-dependencies]
```

