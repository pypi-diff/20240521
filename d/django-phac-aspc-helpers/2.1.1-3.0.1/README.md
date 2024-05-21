# Comparing `tmp/django-phac_aspc-helpers-2.1.1.tar.gz` & `tmp/django_phac_aspc_helpers-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-phac_aspc-helpers-2.1.1.tar", last modified: Sat Mar  9 17:08:51 2024, max compression
+gzip compressed data, was "django_phac_aspc_helpers-3.0.1.tar", last modified: Tue May 21 18:51:15 2024, max compression
```

## Comparing `django-phac_aspc-helpers-2.1.1.tar` & `django_phac_aspc_helpers-3.0.1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.988638 django-phac_aspc-helpers-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-03-09 17:08:51.988638 django-phac_aspc-helpers-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.988638 django-phac_aspc-helpers-2.1.1/django_phac_aspc_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-03-09 17:08:51.000000 django-phac_aspc-helpers-2.1.1/django_phac_aspc_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-03-09 17:08:51.000000 django-phac_aspc-helpers-2.1.1/django_phac_aspc_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 17:08:51.000000 django-phac_aspc-helpers-2.1.1/django_phac_aspc_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-09 17:08:51.000000 django-phac_aspc-helpers-2.1.1/django_phac_aspc_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-09 17:08:51.000000 django-phac_aspc-helpers-2.1.1/django_phac_aspc_helpers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.972638 django-phac_aspc-helpers-2.1.1/phac_aspc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.972638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.972638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/admin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.972638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/admin/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/admin/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/admin/decorators/admin_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/comma_separated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.972638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.972638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/auth/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/auth/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/jinja_dtl_interop_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.972638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/jinja_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/jinja_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/jinja_utils/include_from_dtl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.972638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.964638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/en_CA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.964638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/language.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/logging/configure_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/logging/json_post_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/logging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/ready/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/ready/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/ready/ready.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.964638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.968638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/ms-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr__dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en__dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en__dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr__dark.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.968638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.968638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.968638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.976638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.980638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_page_description.html
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_retry.html
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_title.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_general.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/microsoft_logo.html
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/signin_with_microsoft.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.980638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.980638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_include_from_jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_inline_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.980638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/urls/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/urls/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/urls/wet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.980638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/views/wet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.980638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/localization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/localization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.980638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/localization/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/localization/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/localization/decorators/localization_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/localization/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.984638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/localization.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/localization_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/logging_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/security_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.984638 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/configuration_verification_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/configure_settings_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/env_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/is_running_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/wet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/phac_aspc/vanilla.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-09 17:08:51.988638 django-phac_aspc-helpers-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.984638 django-phac_aspc-helpers-2.1.1/testapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/jinja2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.984638 django-phac_aspc-helpers-2.1.1/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/model_factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.984638 django-phac_aspc-helpers-2.1.1/testapp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:51.988638 django-phac_aspc-helpers-2.1.1/testapp/tests/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/django/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_admin_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_comma_separated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_excel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_phac_aspc_wet.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_vanilla_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/pytest_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-09 17:08:40.000000 django-phac_aspc-helpers-2.1.1/testapp/tests/test_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.120214 django_phac_aspc_helpers-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26234 2024-05-21 18:51:15.120214 django_phac_aspc_helpers-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24964 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.120214 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26234 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/decorators/admin_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/comma_separated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_dtl_interop_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_utils/include_from_dtl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.100214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/configure_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/json_post_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/ready/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/ready/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/ready/ready.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/ms-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr__dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en__dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en__dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr__dark.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_page_description.html
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_retry.html
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_title.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_general.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/microsoft_logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/signin_with_microsoft.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_include_from_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_inline_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/wet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/views/wet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/decorators/localization_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/localization_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/logging_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/security_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/configuration_verification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/configure_settings_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/is_running_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/wet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-21 18:51:15.120214 django_phac_aspc_helpers-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/jinja2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/model_factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/testapp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/testapp/tests/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_admin_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_comma_separated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12721 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_excel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_phac_aspc_wet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_vanilla_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/pytest_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/test_rules.py
```

### Comparing `django-phac_aspc-helpers-2.1.1/LICENSE` & `django_phac_aspc_helpers-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/PKG-INFO` & `django_phac_aspc_helpers-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-phac_aspc-helpers
-Version: 2.1.1
+Version: 3.0.1
 Summary: Set of helpers for Django used at PHAC-ASPC
 Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
 Author: Luc Belliveau
 Author-email: luc.belliveau@phac-aspc.gc.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -113,21 +113,21 @@
 environment variables. By default, these environment variables are read from the
 `.env` file in your project's root. This is done via the [django-environ](https://django-environ.readthedocs.io/en/latest/)
 library; refer to their documentation on how to format special data types like lists.
 
 Alternatively, these environment variables can be declared in your `settings.py`
 itself. There are two important caveats when doing so:
 
-  1) `settings.py` declarations take precedence over any instances of the same
-  env var in your `.env` file
-  2) any env vars declared in `settings.py` for this library **must** be declared
-  **before** any imports from `phac_aspc` occur!
-     - similarly, you should not consume`phac_aspc` modules anywhere that executes
+1. `settings.py` declarations take precedence over any instances of the same
+   env var in your `.env` file
+2. any env vars declared in `settings.py` for this library **must** be declared
+   **before** any imports from `phac_aspc` occur!
+   - similarly, you should not consume`phac_aspc` modules anywhere that executes
      prior to Django's consumption of your app's settings module (e.g. in `manage.py`)
-     - `phac_aspc` modules that don't, directly or indirectly, depend on these
+   - `phac_aspc` modules that don't, directly or indirectly, depend on these
      env vars are theoretically safe anywhere, **but** we don't currently identify
      these modules, or make promises that any given module won't start depending
      on env vars in the future
 
 All env vars for this library are prefixed with `PHAC_ASPC_`. Available `PHAC_ASPC_`
 env vars are listed under their coresponding "feature" sections below.
 
@@ -232,19 +232,19 @@
 The login flow is triggered by redirecting the browser to the named route
 `phac_aspc_helper_login`. The browser will automatically redirect the user to
 Microsoft's Sign in page and after successful authentication, return the user to
 the redirect route named `phac_aspc_authorize` along with a token containing
 information about the user.
 
 By default, the authentication backend will look for a user who's username is
-the user's uuid from Microsoft - if not found a new user is created.  To
+the user's uuid from Microsoft - if not found a new user is created. To
 customize this behaviour, a custom authentication backend class can be specified
 via `PHAC_ASPC_OAUTH_USE_BACKEND` in `settings.py`.
 
-After successful authentication, the user is redirected to `/`.  To customize
+After successful authentication, the user is redirected to `/`. To customize
 this behaviour, set `PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN` in `settings.py` to the
 name of the desired route.
 
 Redirecting to a specific page is also supported through the `?next=<url>` query parameter. See "Template Tag" examples below.
 
 ```python
 
@@ -340,23 +340,23 @@
 {{ phac_aspc.phac_aspc_auth_signin_microsoft_button(request.GET.urlencode()) }}
 ```
 
 #### Handling Errors
 
 If there are any errors during the authentication flow, they are displayed to
 the user via the [error.html](phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html)
-template.  The template can be extended using standard django templating by
+template. The template can be extended using standard django templating by
 creating a `templates/phac_aspc/helpers/auth/error.html` file in the host
 project.
 
 #### Strings and locales
 
 Strings displayed to the user during the authentication flow are available in
-Canada's both official languages.  These strings can be customized by creating
-templates in the host project.  Here is a list of strings and templates used by
+Canada's both official languages. These strings can be customized by creating
+templates in the host project. Here is a list of strings and templates used by
 the authentication flow:
 
 | Template                    | Context                                              |
 | --------------------------- | ---------------------------------------------------- |
 | error_title.html            | Error page title tag value                           |
 | error_page_description.html | Description of error page (meta tag)                 |
 | error_type_general.html     | Error header displayed for general exceptions        |
@@ -484,17 +484,17 @@
 can be changed in your projects settings using `LANGUAGES` and `LANGUAGE_CODE`.
 
 > For more information on Django's localization, see their
 > [documentation](https://docs.djangoproject.com/en/4.1/topics/i18n/).
 
 #### Localization Environment variables
 
-| Variable                        | Type | Purpose                         |
-| ------------------------------- | ---- | ------------------------------- |
-| PHAC_ASPC_LANGUAGE_CODE         | str  | Default language                |
+| Variable                | Type | Purpose          |
+| ----------------------- | ---- | ---------------- |
+| PHAC_ASPC_LANGUAGE_CODE | str  | Default language |
 
 #### lang template tag
 
 In your templates, retrieve the current language code using the `lang` tag.
 
 ```django
 {% load localization %}
@@ -566,15 +566,15 @@
 ```python
 import phac_aspc.django.helpers.jinja_utils as include_from_dtl
 
 
 def environment(**options):
     env = Environment(**options)
     env.globals.update({
-       ..., # other utils and constants 
+       ..., # other utils and constants
        "include_from_dtl": include_from_dtl,
     })
     return env
 ```
 
 And then use it from a Jinja2 template:
 
@@ -707,7 +707,14 @@
 ### Local development
 
 You can consume the helpers project locally by installing it in editable mode. This is useful for extracting project features into this library. In your requirements.txt, comment out the line with django-phac_aspc-helpers, and add the following line with the file path to this repo, then re-install. Make sure to first uninstall the package if it was already installed, e.g. `pip uninstall -y django-phac_aspc-helpers`
 
 ```ini
 -e file:///absolute_path/to/django-phac_aspc-helpers
 ```
+
+### Generating test coverage
+
+1. `coverage run --source=. ./manage.py test`
+2. `coverage html`
+3. `python -m http.server 1337`
+4. visit `http://localhost:1337/htmlcov/` and dig into modules to see which individual line coverage
```

### Comparing `django-phac_aspc-helpers-2.1.1/README.md` & `django_phac_aspc_helpers-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,21 +80,21 @@
 environment variables. By default, these environment variables are read from the
 `.env` file in your project's root. This is done via the [django-environ](https://django-environ.readthedocs.io/en/latest/)
 library; refer to their documentation on how to format special data types like lists.
 
 Alternatively, these environment variables can be declared in your `settings.py`
 itself. There are two important caveats when doing so:
 
-  1) `settings.py` declarations take precedence over any instances of the same
-  env var in your `.env` file
-  2) any env vars declared in `settings.py` for this library **must** be declared
-  **before** any imports from `phac_aspc` occur!
-     - similarly, you should not consume`phac_aspc` modules anywhere that executes
+1. `settings.py` declarations take precedence over any instances of the same
+   env var in your `.env` file
+2. any env vars declared in `settings.py` for this library **must** be declared
+   **before** any imports from `phac_aspc` occur!
+   - similarly, you should not consume`phac_aspc` modules anywhere that executes
      prior to Django's consumption of your app's settings module (e.g. in `manage.py`)
-     - `phac_aspc` modules that don't, directly or indirectly, depend on these
+   - `phac_aspc` modules that don't, directly or indirectly, depend on these
      env vars are theoretically safe anywhere, **but** we don't currently identify
      these modules, or make promises that any given module won't start depending
      on env vars in the future
 
 All env vars for this library are prefixed with `PHAC_ASPC_`. Available `PHAC_ASPC_`
 env vars are listed under their coresponding "feature" sections below.
 
@@ -199,19 +199,19 @@
 The login flow is triggered by redirecting the browser to the named route
 `phac_aspc_helper_login`. The browser will automatically redirect the user to
 Microsoft's Sign in page and after successful authentication, return the user to
 the redirect route named `phac_aspc_authorize` along with a token containing
 information about the user.
 
 By default, the authentication backend will look for a user who's username is
-the user's uuid from Microsoft - if not found a new user is created.  To
+the user's uuid from Microsoft - if not found a new user is created. To
 customize this behaviour, a custom authentication backend class can be specified
 via `PHAC_ASPC_OAUTH_USE_BACKEND` in `settings.py`.
 
-After successful authentication, the user is redirected to `/`.  To customize
+After successful authentication, the user is redirected to `/`. To customize
 this behaviour, set `PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN` in `settings.py` to the
 name of the desired route.
 
 Redirecting to a specific page is also supported through the `?next=<url>` query parameter. See "Template Tag" examples below.
 
 ```python
 
@@ -307,23 +307,23 @@
 {{ phac_aspc.phac_aspc_auth_signin_microsoft_button(request.GET.urlencode()) }}
 ```
 
 #### Handling Errors
 
 If there are any errors during the authentication flow, they are displayed to
 the user via the [error.html](phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html)
-template.  The template can be extended using standard django templating by
+template. The template can be extended using standard django templating by
 creating a `templates/phac_aspc/helpers/auth/error.html` file in the host
 project.
 
 #### Strings and locales
 
 Strings displayed to the user during the authentication flow are available in
-Canada's both official languages.  These strings can be customized by creating
-templates in the host project.  Here is a list of strings and templates used by
+Canada's both official languages. These strings can be customized by creating
+templates in the host project. Here is a list of strings and templates used by
 the authentication flow:
 
 | Template                    | Context                                              |
 | --------------------------- | ---------------------------------------------------- |
 | error_title.html            | Error page title tag value                           |
 | error_page_description.html | Description of error page (meta tag)                 |
 | error_type_general.html     | Error header displayed for general exceptions        |
@@ -451,17 +451,17 @@
 can be changed in your projects settings using `LANGUAGES` and `LANGUAGE_CODE`.
 
 > For more information on Django's localization, see their
 > [documentation](https://docs.djangoproject.com/en/4.1/topics/i18n/).
 
 #### Localization Environment variables
 
-| Variable                        | Type | Purpose                         |
-| ------------------------------- | ---- | ------------------------------- |
-| PHAC_ASPC_LANGUAGE_CODE         | str  | Default language                |
+| Variable                | Type | Purpose          |
+| ----------------------- | ---- | ---------------- |
+| PHAC_ASPC_LANGUAGE_CODE | str  | Default language |
 
 #### lang template tag
 
 In your templates, retrieve the current language code using the `lang` tag.
 
 ```django
 {% load localization %}
@@ -533,15 +533,15 @@
 ```python
 import phac_aspc.django.helpers.jinja_utils as include_from_dtl
 
 
 def environment(**options):
     env = Environment(**options)
     env.globals.update({
-       ..., # other utils and constants 
+       ..., # other utils and constants
        "include_from_dtl": include_from_dtl,
     })
     return env
 ```
 
 And then use it from a Jinja2 template:
 
@@ -674,7 +674,14 @@
 ### Local development
 
 You can consume the helpers project locally by installing it in editable mode. This is useful for extracting project features into this library. In your requirements.txt, comment out the line with django-phac_aspc-helpers, and add the following line with the file path to this repo, then re-install. Make sure to first uninstall the package if it was already installed, e.g. `pip uninstall -y django-phac_aspc-helpers`
 
 ```ini
 -e file:///absolute_path/to/django-phac_aspc-helpers
 ```
+
+### Generating test coverage
+
+1. `coverage run --source=. ./manage.py test`
+2. `coverage html`
+3. `python -m http.server 1337`
+4. visit `http://localhost:1337/htmlcov/` and dig into modules to see which individual line coverage
```

### Comparing `django-phac_aspc-helpers-2.1.1/django_phac_aspc_helpers.egg-info/PKG-INFO` & `django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-phac_aspc-helpers
-Version: 2.1.1
+Version: 3.0.1
 Summary: Set of helpers for Django used at PHAC-ASPC
 Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
 Author: Luc Belliveau
 Author-email: luc.belliveau@phac-aspc.gc.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -113,21 +113,21 @@
 environment variables. By default, these environment variables are read from the
 `.env` file in your project's root. This is done via the [django-environ](https://django-environ.readthedocs.io/en/latest/)
 library; refer to their documentation on how to format special data types like lists.
 
 Alternatively, these environment variables can be declared in your `settings.py`
 itself. There are two important caveats when doing so:
 
-  1) `settings.py` declarations take precedence over any instances of the same
-  env var in your `.env` file
-  2) any env vars declared in `settings.py` for this library **must** be declared
-  **before** any imports from `phac_aspc` occur!
-     - similarly, you should not consume`phac_aspc` modules anywhere that executes
+1. `settings.py` declarations take precedence over any instances of the same
+   env var in your `.env` file
+2. any env vars declared in `settings.py` for this library **must** be declared
+   **before** any imports from `phac_aspc` occur!
+   - similarly, you should not consume`phac_aspc` modules anywhere that executes
      prior to Django's consumption of your app's settings module (e.g. in `manage.py`)
-     - `phac_aspc` modules that don't, directly or indirectly, depend on these
+   - `phac_aspc` modules that don't, directly or indirectly, depend on these
      env vars are theoretically safe anywhere, **but** we don't currently identify
      these modules, or make promises that any given module won't start depending
      on env vars in the future
 
 All env vars for this library are prefixed with `PHAC_ASPC_`. Available `PHAC_ASPC_`
 env vars are listed under their coresponding "feature" sections below.
 
@@ -232,19 +232,19 @@
 The login flow is triggered by redirecting the browser to the named route
 `phac_aspc_helper_login`. The browser will automatically redirect the user to
 Microsoft's Sign in page and after successful authentication, return the user to
 the redirect route named `phac_aspc_authorize` along with a token containing
 information about the user.
 
 By default, the authentication backend will look for a user who's username is
-the user's uuid from Microsoft - if not found a new user is created.  To
+the user's uuid from Microsoft - if not found a new user is created. To
 customize this behaviour, a custom authentication backend class can be specified
 via `PHAC_ASPC_OAUTH_USE_BACKEND` in `settings.py`.
 
-After successful authentication, the user is redirected to `/`.  To customize
+After successful authentication, the user is redirected to `/`. To customize
 this behaviour, set `PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN` in `settings.py` to the
 name of the desired route.
 
 Redirecting to a specific page is also supported through the `?next=<url>` query parameter. See "Template Tag" examples below.
 
 ```python
 
@@ -340,23 +340,23 @@
 {{ phac_aspc.phac_aspc_auth_signin_microsoft_button(request.GET.urlencode()) }}
 ```
 
 #### Handling Errors
 
 If there are any errors during the authentication flow, they are displayed to
 the user via the [error.html](phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html)
-template.  The template can be extended using standard django templating by
+template. The template can be extended using standard django templating by
 creating a `templates/phac_aspc/helpers/auth/error.html` file in the host
 project.
 
 #### Strings and locales
 
 Strings displayed to the user during the authentication flow are available in
-Canada's both official languages.  These strings can be customized by creating
-templates in the host project.  Here is a list of strings and templates used by
+Canada's both official languages. These strings can be customized by creating
+templates in the host project. Here is a list of strings and templates used by
 the authentication flow:
 
 | Template                    | Context                                              |
 | --------------------------- | ---------------------------------------------------- |
 | error_title.html            | Error page title tag value                           |
 | error_page_description.html | Description of error page (meta tag)                 |
 | error_type_general.html     | Error header displayed for general exceptions        |
@@ -484,17 +484,17 @@
 can be changed in your projects settings using `LANGUAGES` and `LANGUAGE_CODE`.
 
 > For more information on Django's localization, see their
 > [documentation](https://docs.djangoproject.com/en/4.1/topics/i18n/).
 
 #### Localization Environment variables
 
-| Variable                        | Type | Purpose                         |
-| ------------------------------- | ---- | ------------------------------- |
-| PHAC_ASPC_LANGUAGE_CODE         | str  | Default language                |
+| Variable                | Type | Purpose          |
+| ----------------------- | ---- | ---------------- |
+| PHAC_ASPC_LANGUAGE_CODE | str  | Default language |
 
 #### lang template tag
 
 In your templates, retrieve the current language code using the `lang` tag.
 
 ```django
 {% load localization %}
@@ -566,15 +566,15 @@
 ```python
 import phac_aspc.django.helpers.jinja_utils as include_from_dtl
 
 
 def environment(**options):
     env = Environment(**options)
     env.globals.update({
-       ..., # other utils and constants 
+       ..., # other utils and constants
        "include_from_dtl": include_from_dtl,
     })
     return env
 ```
 
 And then use it from a Jinja2 template:
 
@@ -707,7 +707,14 @@
 ### Local development
 
 You can consume the helpers project locally by installing it in editable mode. This is useful for extracting project features into this library. In your requirements.txt, comment out the line with django-phac_aspc-helpers, and add the following line with the file path to this repo, then re-install. Make sure to first uninstall the package if it was already installed, e.g. `pip uninstall -y django-phac_aspc-helpers`
 
 ```ini
 -e file:///absolute_path/to/django-phac_aspc-helpers
 ```
+
+### Generating test coverage
+
+1. `coverage run --source=. ./manage.py test`
+2. `coverage html`
+3. `python -m http.server 1337`
+4. visit `http://localhost:1337/htmlcov/` and dig into modules to see which individual line coverage
```

### Comparing `django-phac_aspc-helpers-2.1.1/django_phac_aspc_helpers.egg-info/SOURCES.txt` & `django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/admin/decorators/admin_decorators.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/decorators/admin_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/comma_separated_field.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/comma_separated_field.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/fields.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/fields.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/apps.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/apps.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/auth/backend.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/backend.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/auth/views.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/views.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/jinja_dtl_interop_utils.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_dtl_interop_utils.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/locale/language.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/language.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/logging/configure_logging.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/configure_logging.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/logging/json_post_handlers.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/json_post_handlers.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/logging/utils.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/utils.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/ready/__init__.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/ready/__init__.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr.svg` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr.svg`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr__dark.svg` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr__dark.svg`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en.svg` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en.svg`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en__dark.svg` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en__dark.svg`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en.svg` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en.svg`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en__dark.svg` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en__dark.svg`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr.svg` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr.svg`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr__dark.svg` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr__dark.svg`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/__init__.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_include_from_jinja.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_include_from_jinja.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_inline_svg.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_inline_svg.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/urls/auth.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/auth.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/helpers/views/wet.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/views/wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/localization/decorators/localization_decorators.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/decorators/localization_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/logging.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/logging.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/logging_env.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/logging_env.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/security.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/security.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/security_env.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/security_env.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/configuration_verification_utils.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/configuration_verification_utils.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/configure_settings_for_tests.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/configure_settings_for_tests.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/django/settings/utils/env_utils.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/rules.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/rules.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/phac_aspc/vanilla.py` & `django_phac_aspc_helpers-3.0.1/phac_aspc/vanilla.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/setup.cfg` & `django_phac_aspc_helpers-3.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-phac_aspc-helpers
-version = 2.1.1
+version = 3.0.1
 description = Set of helpers for Django used at PHAC-ASPC
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PHACDataHub/django-phac_aspc-helpers
 author = Luc Belliveau
 author_email = luc.belliveau@phac-aspc.gc.ca
 license = MIT
```

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/migrations/0001_initial.py` & `django_phac_aspc_helpers-3.0.1/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/model_factories.py` & `django_phac_aspc_helpers-3.0.1/testapp/model_factories.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/models.py` & `django_phac_aspc_helpers-3.0.1/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/settings.py` & `django_phac_aspc_helpers-3.0.1/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/tests/django/conftest.py` & `django_phac_aspc_helpers-3.0.1/testapp/tests/django/conftest.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_admin_decorators.py` & `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_admin_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_comma_separated_field.py` & `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_comma_separated_field.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_phac_aspc_wet.py` & `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_phac_aspc_wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_ready.py` & `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_ready.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/tests/django/test_vanilla_utils.py` & `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_vanilla_utils.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/tests/pytest_runner.py` & `django_phac_aspc_helpers-3.0.1/testapp/tests/pytest_runner.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-2.1.1/testapp/tests/test_rules.py` & `django_phac_aspc_helpers-3.0.1/testapp/tests/test_rules.py`

 * *Files identical despite different names*

