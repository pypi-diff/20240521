# Comparing `tmp/django-ckeditor-link-0.5.1.tar.gz` & `tmp/django_ckeditor_link-0.5.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ckeditor-link-0.5.1.tar", last modified: Wed Jun 28 11:18:52 2023, max compression
+gzip compressed data, was "django_ckeditor_link-0.5.3.dev0.tar", last modified: Tue May 21 13:20:42 2024, max compression
```

## Comparing `django-ckeditor-link-0.5.1.tar` & `django_ckeditor_link-0.5.3.dev0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.142580 django-ckeditor-link-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-28 11:18:52.142580 django-ckeditor-link-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/link_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/link_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/link_model/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/link_model/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/admin/ckeditor_link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/static/admin/ckeditor_link/css/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/admin/ckeditor_link/css/link_admin.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
--rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.134580 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
--rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/templatetags/ckeditor_link_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.138580 django-ckeditor-link-0.5.1/ckeditor_link/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/settings_no_headless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.142580 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.142580 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_link_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/test_templatetag.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.142580 django-ckeditor-link-0.5.1/ckeditor_link/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/utils/django_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/ckeditor_link/tests/utils/selenium_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:18:52.142580 django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-28 11:18:52.000000 django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-28 11:18:52.000000 django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:18:52.000000 django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:18:52.000000 django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-28 11:18:52.000000 django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 11:18:52.000000 django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-28 11:18:52.142580 django-ckeditor-link-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-06-28 11:18:43.000000 django-ckeditor-link-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.703189 django_ckeditor_link-0.5.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-21 13:20:42.703189 django_ckeditor_link-0.5.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/link_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/link_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/link_model/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/link_model/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/admin/ckeditor_link/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/admin/ckeditor_link/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/admin/ckeditor_link/css/link_admin.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/
+-rw-r--r--   0 runner    (1001) docker     (127)    53964 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35607 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18527 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15579 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.695188 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/
+-rw-r--r--   0 runner    (1001) docker     (127)    53964 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35607 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18527 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15579 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.699189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/templatetags/ckeditor_link_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.703189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/settings_no_headless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.703189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.703189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_link_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_templatetag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.703189 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/utils/django_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/utils/selenium_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:20:42.703189 django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-21 13:20:42.000000 django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-21 13:20:42.000000 django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:20:42.000000 django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:20:42.000000 django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 13:20:42.000000 django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 13:20:42.000000 django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:20:42.703189 django_ckeditor_link-0.5.3.dev0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1266 2024-05-21 13:20:35.000000 django_ckeditor_link-0.5.3.dev0/setup.py
```

### Comparing `django-ckeditor-link-0.5.1/CHANGELOG.txt` & `django_ckeditor_link-0.5.3.dev0/CHANGELOG.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ==== 0.4.5 (under development) ===
 
 - ?
 
+==== 0.5.2 (2024-05-21) ===
+
+- no functional changes
+- REMOVE print statement
+- introduce pre-commit / ruff / black and other goodies
+- remove python 3.7 from test matrix
+
+
 ==== 0.5.1 (2023-06-28) ===
 
 - introduce CKEDITOR_LINK_MODEL_USE_FILER_ADDONS, to enable usage of
   django-filer-addons.filer_gui.fields.FilerFileField in ckeditor_link.link_model
   (instead of the default filer field).
```

### Comparing `django-ckeditor-link-0.5.1/LICENSE` & `django_ckeditor_link-0.5.3.dev0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -332,8 +332,8 @@
   <signature of Ty Coon>, 1 April 1989
   Ty Coon, President of Vice
 
 This General Public License does not permit incorporating your program into
 proprietary programs.  If your program is a subroutine library, you may
 consider it more useful to permit linking proprietary applications with the
 library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.
+Public License instead of this License.
```

### Comparing `django-ckeditor-link-0.5.1/PKG-INFO` & `django_ckeditor_link-0.5.3.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditor-link
-Version: 0.5.1
+Version: 0.5.3.dev0
 Summary: Alternative link dialog for ckeditor 4, using django modeladmin forms.
 Home-page: http://github.com/bnzk/django-ckeditor-link
 Author: Ben Stähli
 Author-email: bnzk@bnzk.ch
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=1.11
 
 # django-ckeditor-link
 
 Build status fails sometimes - selenium and iframes and ... sleep. Passes with local tox, believe me.
 
 [![CI](https://img.shields.io/github/actions/workflow/status/bnzk/django-ckeditor-link/ci.yml?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-ckeditor-link/actions/workflows/ci.yml)
 [![Version](https://img.shields.io/pypi/v/django-ckeditor-link.svg?style=flat-square "Version")](https://pypi.python.org/pypi/django-ckeditor-link/)
```

### Comparing `django-ckeditor-link-0.5.1/README.md` & `django_ckeditor_link-0.5.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/admin.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 from django.conf import settings
-from django.urls import path
 from django.contrib import admin
 from django.db import models
 from django.forms import widgets
 from django.http import JsonResponse
+from django.urls import path
 
 
 class DjangoLinkAdmin(admin.ModelAdmin):
-
     def get_model_perms(self, request):
         """
         http://stackoverflow.com/questions/2431727/django-admin-hide-a-model
         Return empty perms dict thus hiding the model from admin index.
         """
         return {}
 
     @property
     def media(self):
         original_media = super(DjangoLinkAdmin, self).media
-        css = {
-            'all': (
-                settings.STATIC_URL + 'admin/ckeditor_link/css/link_admin.css',
-            )
-        }
+        css = {"all": (settings.STATIC_URL + "admin/ckeditor_link/css/link_admin.css",)}
         new_media = widgets.Media(css=css)
         return original_media + new_media
 
     def get_urls(self):
         """
         add verify url.
         """
         my_urls = [
             path(
-                'verify/',
+                "verify/",
                 self.admin_site.admin_view(self.verify),
-                name=self._get_verify_url_name()
+                name=self._get_verify_url_name(),
             ),
         ]
         return my_urls + super(DjangoLinkAdmin, self).get_urls()
 
     def _get_verify_url_name(self):
-        return '{0}_{1}_verify'.format(self.model._meta.app_label,
-                                       self.model._meta.model_name)
+        return "{0}_{1}_verify".format(
+            self.model._meta.app_label, self.model._meta.model_name
+        )
 
     def verify(self, request):
         """
         verify data with modelform, send through data.
         :param request:
         :return:
         """
-        form = self.get_form(request, )(request.POST)
+        form = self.get_form(
+            request,
+        )(request.POST)
         if form.is_valid():
             verified_data = form.cleaned_data
             obj = self.model(**verified_data)
-            link_value = ''
+            link_value = ""
             # prepopulate href
-            if (getattr(obj, 'get_link', None)):
+            if getattr(obj, "get_link", None):
                 link_value = obj.get_link()
             # basic serialize only
             for key, value in verified_data.items():
                 if isinstance(value, models.Model):
                     verified_data[key] = value.id
-            return_data = {"valid": 'true', 'data': verified_data, 'link_value': link_value}
+            return_data = {
+                "valid": "true",
+                "data": verified_data,
+                "link_value": link_value,
+            }
         else:
             errors = form.errors
-            return_data = {"valid": 'false', 'errors': errors}
+            return_data = {"valid": "false", "errors": errors}
         return JsonResponse(return_data)
 
     def save_model(self, request, obj, form, change):
         """
         no save!
         """
         return False
 
     def get_changeform_initial_data(self, request):
         initial = super(DjangoLinkAdmin, self).get_changeform_initial_data(request)
-        if request.GET.get('page', None):
-            initial['cms_page'] = request.GET.get('page')
+        if request.GET.get("page", None):
+            initial["cms_page"] = request.GET.get("page")
         return initial
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/link_model/models.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/link_model/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     from __builtin__ import str
 
 from django.conf import settings
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from .conf import (
+    CKEDITOR_LINK_MODEL_USE_FILER_ADDONS,
     CKEDITOR_LINK_TYPE_CHOICES,
     CKEDITOR_LINK_USE_CMS_FILER,
-    CKEDITOR_LINK_MODEL_USE_FILER_ADDONS,
 )
 
 # dropped in favour of builtins/str, see above
 # try:
 #     unicode('')
 # except NameError:
 #     unicode = str
@@ -28,95 +28,95 @@
     #     max_length=255,
     #     blank=True,
     #     default='',
     # )
     link_type = models.CharField(
         max_length=20,
         blank=True,
-        default='',
-        verbose_name=_('Link type'),
+        default="",
+        verbose_name=_("Link type"),
     )
     link_style = models.CharField(
         max_length=64,
         blank=True,
-        default='',
-        verbose_name=_('Link Style'),
+        default="",
+        verbose_name=_("Link Style"),
     )
     free = models.CharField(
         max_length=512,
-        default='',
+        default="",
         blank=True,
         verbose_name=_("Internal / Other"),
     )
     external = models.URLField(
         blank=True,
-        default='',
+        default="",
         verbose_name=_("External Address"),
     )
     mailto = models.EmailField(
-        default='',
+        default="",
         blank=True,
         verbose_name=_("E-Mail"),
     )
     phone = models.CharField(
         max_length=64,
-        default='',
+        default="",
         blank=True,
         verbose_name=_("Phone"),
     )
 
     class Meta:
         abstract = True
 
     def get_link(self):
         # if link type set, give priority!
         # this will alter your object!
         if self.link_type:
             for key, display in CKEDITOR_LINK_TYPE_CHOICES:
-                if not key == self.link_type:
+                if key != self.link_type:
                     setattr(self, key, None)
         # generic foreign key link check
         fk_link = self._check_link_for_foreign_key()
         if fk_link:
             return fk_link
         # other custom link types
         if self.free:
             return self.free
         elif self.external:
             link = self.external
-            if not link.startswith('http'):
-                link = 'http://%s' % link
+            if not link.startswith("http"):
+                link = "http://%s" % link
             return link
         elif self.mailto:
             return "mailto:%s" % self.mailto
         elif self.phone:
             return "tel:%s" % self.phone
-        return ''
+        return ""
 
     def get_link_text(self):
         obj = None
-        if getattr(self, 'link_text', None):
+        if getattr(self, "link_text", None):
             return self.link_text
-        if getattr(self, 'name', None):
+        if getattr(self, "name", None):
             return self.name
         if self.link_type:
             obj = self._check_foreign_key_value()
         if object is not None:
             return str(obj)
-        return ''
+        return ""
 
     def get_link_type(self):
         return self.link_type
 
     def get_link_style(self):
         return self.link_style
 
     def get_link_target(self):
         type = self.get_link_type()
-        if type in ['file', 'external']:
+        if type in ["file", "external"]:
             return "_blank"
         return ""
 
     def _check_foreign_key_value(self):
         """
         check if link type and it's value are a foreign key
         Returns: foreign key value, if available
@@ -127,96 +127,96 @@
         except ObjectDoesNotExist:
             pass
         return None
 
     def _check_link_for_foreign_key(self):
         value = self._check_foreign_key_value()
         # print(isinstance(value, models.Model))
-        if value and getattr(value, 'get_absolute_url', None):
+        if value and getattr(value, "get_absolute_url", None):
             link = value.get_absolute_url()
             return link
         return None
 
 
 class Link(LinkBase):
     """
     if in installed apps, this will be created and available out of the box
     beware: no migrations yet!
     """
+
     pass
 
 
 if CKEDITOR_LINK_USE_CMS_FILER:
-
     from cms.models.fields import PageField
-    print(CKEDITOR_LINK_MODEL_USE_FILER_ADDONS)
+
     if CKEDITOR_LINK_MODEL_USE_FILER_ADDONS:
         from filer_addons.filer_gui.fields import FilerFileField
     else:
         from filer.fields.file import FilerFileField
 
-    class CMSFilerLinkBase(LinkBase):  # noqa
+    class CMSFilerLinkBase(LinkBase):
         cms_page = PageField(
             null=True,
             on_delete=models.SET_NULL,
             related_name="%(app_label)s_%(class)s_set",
             blank=True,
         )
         html_anchor = models.SlugField(
-            default='',
+            default="",
             blank=True,
-            verbose_name='Anker',
+            verbose_name="Anker",
         )
         file = FilerFileField(
             null=True,
             on_delete=models.SET_NULL,
             related_name="%(app_label)s_%(class)s_set",
             blank=True,
         )
 
         def __init__(self, *args, **kwargs):
-            if kwargs.get('page', None):
-                self.cms_page = kwargs.get('page')
+            if kwargs.get("page", None):
+                self.cms_page = kwargs.get("page")
             super(CMSFilerLinkBase, self).__init__(*args, **kwargs)
 
         class Meta:
             abstract = True
 
         def get_link(self):
             # best practice is to call super first, so not relevant attrs are nulled
             super_link = super(CMSFilerLinkBase, self).get_link()
             fk_obj = self._check_foreign_key_value()
-            if self.get_link_type() == 'cms_page' and super_link:
+            if self.get_link_type() == "cms_page" and super_link:
                 if self.html_anchor:
-                    super_link += '#%s' % self.html_anchor
-                if getattr(self.cms_page, 'node', None):
+                    super_link += "#%s" % self.html_anchor
+                if getattr(self.cms_page, "node", None):
                     # cms>=3.5
-                    site = getattr(self.cms_page.node, 'site', None)
+                    site = getattr(self.cms_page.node, "site", None)
                 else:
                     # cms<3.5
-                    site = getattr(self.cms_page, 'site', None)
+                    site = getattr(self.cms_page, "site", None)
                 if site.id == settings.SITE_ID:
                     return super_link
                 else:
-                    return '//' + site.domain + super_link
-            elif self.get_link_type() == 'file' and fk_obj:
+                    return "//" + site.domain + super_link
+            elif self.get_link_type() == "file" and fk_obj:
                 return fk_obj.url
             return super_link
 
         def get_link_target(self):
             fk_obj = self._check_foreign_key_value()
-            if self.get_link_type() == 'cms_page' and fk_obj:
+            if self.get_link_type() == "cms_page" and fk_obj:
                 site = self._get_cms_page_site()
-                if not site.id == settings.SITE_ID:
+                if site.id != settings.SITE_ID:
                     return "_blank"
             else:
                 return super(CMSFilerLinkBase, self).get_link_target()
             return ""
 
         def _get_cms_page_site(self):
             fk_obj = self._check_foreign_key_value()
-            if self.get_link_type() == 'cms_page' and fk_obj:
-                if getattr(self.cms_page, 'node', None):
+            if self.get_link_type() == "cms_page" and fk_obj:
+                if getattr(self.cms_page, "node", None):
                     site = self.cms_page.node.site
                 else:
                     site = self.cms_page.site
             return site
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,72 @@
-# coding: utf-8
-from __future__ import unicode_literals
 import re
 
 from cms.models import CMSPlugin
 from django.core.management.base import BaseCommand
 
 
 class Command(BaseCommand):
     """
     dont use this yet, it assumes too many things of your existing installation.
     rather use it as starting point, and copy and paste it.
     """
-    help = 'Check for djangocms-text-ckeditor subplugins, convert to django-ckeditor-link style'  # noqa
+
+    help = (
+        "Check for djangocms-text-ckeditor subplugins, convert to "
+        "django-ckeditor-link style"
+    )
 
     def add_arguments(self, parser):
         parser.add_argument(
-            'plugins',
-            nargs='+',
-            help='Plugins to check',
+            "plugins",
+            nargs="+",
+            help="Plugins to check",
         )
         parser.add_argument(
-            '--field',
+            "--field",
             required=True,
-            help='Field to check',
+            help="Field to check",
         )
 
     def handle(self, *args, **options):
-
-        text_plugins = CMSPlugin.objects.filter(
-            plugin_type__in=options['plugins']
-        )
+        text_plugins = CMSPlugin.objects.filter(plugin_type__in=options["plugins"])
         for plugin in text_plugins:
             instance, plugin_class = plugin.get_plugin_instance()
-            img_pattern = re.compile(r'<img.*?>')
-            obj_pattern = re.compile(r'plugin_obj_[0-9]*')
+            img_pattern = re.compile(r"<img.*?>")
+            obj_pattern = re.compile(r"plugin_obj_[0-9]*")
             image_tags = re.findall(img_pattern, instance.body)
             if len(image_tags):
                 for tag in image_tags:
                     obj_match = re.findall(obj_pattern, tag)
                     if len(obj_match):
-                        plugin_id = obj_match[0].replace('plugin_obj_', '')
+                        plugin_id = obj_match[0].replace("plugin_obj_", "")
                         # print plugin_id
                         link_plugin = CMSPlugin.objects.get(pk=plugin_id)
                         # print link_plugin
                         link_instance, link_class = link_plugin.get_plugin_instance()
                         link_data = {
-                            'link_text': link_instance.get_link_text(),
-                            'link': link_instance.get_link(),
-                            'link_type': link_instance.get_link_type(),
-                            'page': link_instance.page_id,
-                            'file': link_instance.file_id,
-                            'external': link_instance.external_url,
-                            'mailto': link_instance.mailto,
-                            'phone': link_instance.phone,
+                            "link_text": link_instance.get_link_text(),
+                            "link": link_instance.get_link(),
+                            "link_type": link_instance.get_link_type(),
+                            "page": link_instance.page_id,
+                            "file": link_instance.file_id,
+                            "external": link_instance.external_url,
+                            "mailto": link_instance.mailto,
+                            "phone": link_instance.phone,
                         }
                         for key, value in link_data.iteritems():
                             if not value:
-                                link_data[key] = ''
-                        new_link = '<a href="{link}"' \
-                                   ' data-ckeditor-link="true"' \
-                                   ' data-link_type="{link_type}"' \
-                                   ' data-page="{page}"' \
-                                   ' data-file="{file}"' \
-                                   ' data-external="{external_url}"' \
-                                   ' data-mailto="{mailto}"' \
-                                   ' data-phone="{mailto}"' \
-                                   '>' \
-                                   '{link_text}</a>'.format(**link_data)
+                                link_data[key] = ""
+                        new_link = (
+                            '<a href="{link}"'
+                            ' data-ckeditor-link="true"'
+                            ' data-link_type="{link_type}"'
+                            ' data-page="{page}"'
+                            ' data-file="{file}"'
+                            ' data-external="{external_url}"'
+                            ' data-mailto="{mailto}"'
+                            ' data-phone="{mailto}"'
+                            ">"
+                            "{link_text}</a>".format(**link_data)
+                        )
                         instance.body = instance.body.replace(tag, new_link)
                 instance.save()
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,13 @@
 (function($) {
     // CMS.$ will be passed for $
     $(document).ready(function() {
-
-        CKEDITOR.plugins.add('cmsplugins', {
-
+        CKEDITOR.plugins.add("cmsplugins", {
             // Register the icons. They must match command names.
-            icons: 'cmsplugins',
+            icons: "cmsplugins",
 
             // The plugin initialization logic goes inside this method.
             init: function(editor) {
                 var that = this;
 
                 this.options = CMS.CKEditor.options.settings;
                 this.editor = editor;
@@ -17,246 +15,290 @@
                 /**
                  * populated with _fresh_ child plugins
                  */
                 this.child_plugins = [];
                 this.setupCancelCleanupCallback(this.options);
 
                 // don't do anything if there are no plugins defined
-                if (this.options === undefined || this.options.plugins === undefined) return false;
+                if (this.options === undefined || this.options.plugins === undefined)
+                    return false;
 
                 this.setupDialog();
 
                 // add the button
-                this.editor.ui.add('cmsplugins', CKEDITOR.UI_PANELBUTTON, {
-                    'toolbar': 'cms,0',
-                    'label': this.options.lang.toolbar,
-                    'title': this.options.lang.toolbar,
-                    'className': 'cke_panelbutton__cmsplugins',
-                    'modes': {
+                this.editor.ui.add("cmsplugins", CKEDITOR.UI_PANELBUTTON, {
+                    toolbar: "cms,0",
+                    label: this.options.lang.toolbar,
+                    title: this.options.lang.toolbar,
+                    className: "cke_panelbutton__cmsplugins",
+                    modes: {
                         wysiwyg: 1
                     },
-                    'editorFocus': 0,
+                    editorFocus: 0,
 
-                    'panel': {
-                        'css': [CKEDITOR.skin.getPath('editor')].concat(that.editor.config.contentsCss),
-                        'attributes': {
-                            role: 'cmsplugins',
-                            'aria-label': this.options.lang.aria
-                        }
+                    panel: {
+                        css: [CKEDITOR.skin.getPath("editor")].concat(
+                            that.editor.config.contentsCss,
+                        ),
+                        attributes: {
+                            role: "cmsplugins",
+                            "aria-label": this.options.lang.aria,
+                        },
                     },
 
                     // this is called when creating the dropdown list
-                    'onBlock': function(panel, block) {
-                        block.element.setHtml(that.editor.plugins.cmsplugins.setupDropdown());
+                    onBlock: function(panel, block) {
+                        block.element.setHtml(
+                            that.editor.plugins.cmsplugins.setupDropdown(),
+                        );
 
-                        var anchors = $(block.element.$).find('.cke_panel_listItem a');
-                        anchors.bind('click', function(e) {
+                        var anchors = $(block.element.$).find(".cke_panel_listItem a");
+                        anchors.bind("click", function(e) {
                             e.preventDefault();
 
                             that.addPlugin($(this), panel);
                         });
-                    }
+                    },
                 });
 
                 // handle edit event via context menu
                 if (this.editor.contextMenu) {
                     this.setupContextMenu();
-                    this.editor.addCommand('cmspluginsEdit', {
+                    this.editor.addCommand("cmspluginsEdit", {
                         exec: function() {
                             var selection = that.editor.getSelection();
-                            var element = selection.getSelectedElement() || selection.getCommonAncestor().getAscendant('a', true);
+                            var element =
+                                selection.getSelectedElement() ||
+                                selection.getCommonAncestor().getAscendant("a", true);
                             that.editPlugin(element);
-                        }
+                        },
                     });
                 }
 
                 // handle edit event on double click
                 // if event is a jQuery event (touchend), than we mutate
                 // event a bit so we make the payload similar to what ckeditor.event produces
                 var handleEdit = function(event) {
-                    if (event.type === 'touchend' || event.type === 'click') {
+                    if (event.type === "touchend" || event.type === "click") {
                         var element = event.currentTarget;
                         event.data = event.data || {};
-                        that.editor.getSelection().fake(new CKEDITOR.dom.element(element));
+                        that.editor
+                            .getSelection()
+                            .fake(new CKEDITOR.dom.element(element));
                     } else {
                         // heavily relies on the fact that double click
                         // also selects an element
                         var selection = that.editor.getSelection();
-                        var element = selection.getSelectedElement() || selection.getCommonAncestor().getAscendant('a', true);
+                        var element =
+                            selection.getSelectedElement() ||
+                            selection.getCommonAncestor().getAscendant("a", true);
                     }
-                    if (element && element.getAttribute('id').indexOf('plugin_obj_') === 0) {
-                        event.data.dialog = '';
+                    if (
+                        element &&
+                        element.getAttribute("id").indexOf("plugin_obj_") === 0
+                    ) {
+                        event.data.dialog = "";
                         that.editPlugin(element);
                     }
-                }
-                this.editor.on('doubleclick', handleEdit);
-                this.editor.on('instanceReady', function() {
-                    CMS.$('[id*="plugin_obj_"]', CMS.$('iframe.cke_wysiwyg_frame')[0]
-                        .contentWindow.document.documentElement).on('click touchend', handleEdit);
+                };
+                this.editor.on("doubleclick", handleEdit);
+                this.editor.on("instanceReady", function() {
+                    CMS.$(
+                        '[id*="plugin_obj_"]',
+                        CMS.$("iframe.cke_wysiwyg_frame")[0].contentWindow.document
+                        .documentElement,
+                    ).on("click touchend", handleEdit);
                 });
 
                 // setup CKEDITOR.htmlDataProcessor
                 this.setupDataProcessor();
             },
 
             setupDialog: function() {
                 var that = this;
                 var definition = function() {
                     return {
-                        'title': '',
-                        'minWidth': 600,
-                        'minHeight': 200,
-                        'contents': [{
-                            'elements': [{
-                                type: 'html',
-                                html: '<iframe style="position:static; width:100%; height:100%; border:none;" />'
-                            }]
-                        }],
-                        'onOk': function() {
-                            var iframe = $(CKEDITOR.dialog.getCurrent().parts.contents.$).find('iframe').contents();
-                            iframe.find('form').submit();
+                        title: "",
+                        minWidth: 600,
+                        minHeight: 200,
+                        contents: [{
+                            elements: [{
+                                type: "html",
+                                html: '<iframe style="position:static; width:100%; height:100%; border:none;" />',
+                            }, ],
+                        }, ],
+                        onOk: function() {
+                            var iframe = $(
+                                    CKEDITOR.dialog.getCurrent().parts.contents.$,
+                                )
+                                .find("iframe")
+                                .contents();
+                            iframe.find("form").submit();
 
                             // catch the reload event and reattach
                             var reload = CMS.API.Helpers.reloadBrowser;
 
                             CMS.API.Helpers.reloadBrowser = function() {
                                 CKEDITOR.dialog.getCurrent().hide();
 
                                 that.insertPlugin(CMS.API.Helpers.dataBridge);
 
                                 CMS.API.Helpers.reloadBrowser = reload;
                                 return false;
                             };
                             return false;
-                        }
-                    }
+                        },
+                    };
                 };
 
                 // set default definition and open dialog
-                CKEDITOR.dialog.add('cmspluginsDialog', definition);
+                CKEDITOR.dialog.add("cmspluginsDialog", definition);
             },
 
             setupDropdown: function() {
                 var tpl = '<div class="cke_panel_block">';
 
                 // loop through the groups
                 $.each(this.options.plugins, function(i, group) {
                     // add template
-                    tpl += '<h1 class="cke_panel_grouptitle">' + group.group + '</h1>';
+                    tpl += '<h1 class="cke_panel_grouptitle">' + group.group + "</h1>";
                     tpl += '<ul role="presentation" class="cke_panel_list">';
                     // loop through the plugins
                     $.each(group.items, function(ii, item) {
-                        tpl += '<li class="cke_panel_listItem"><a href="#" rel="' + item.type + '">' + item.title + '</a></li>';
+                        tpl +=
+                            '<li class="cke_panel_listItem"><a href="#" rel="' +
+                            item.type +
+                            '">' +
+                            item.title +
+                            "</a></li>";
                     });
-                    tpl += '</ul>';
+                    tpl += "</ul>";
                 });
 
-                tpl += '</div>';
+                tpl += "</div>";
 
                 return tpl;
             },
 
             setupContextMenu: function() {
-                this.editor.addMenuGroup('cmspluginsGroup');
-                this.editor.addMenuItem('cmspluginsItem', {
+                this.editor.addMenuGroup("cmspluginsGroup");
+                this.editor.addMenuItem("cmspluginsItem", {
                     label: this.options.lang.edit,
-                    icon: this.path + 'icons/cmsplugins.png',
-                    command: 'cmspluginsEdit',
-                    group: 'cmspluginsGroup'
+                    icon: this.path + "icons/cmsplugins.png",
+                    command: "cmspluginsEdit",
+                    group: "cmspluginsGroup",
                 });
 
-                this.editor.removeMenuItem('image');
+                this.editor.removeMenuItem("image");
 
                 this.editor.contextMenu.addListener(function(element) {
-                    if (element.$.id.indexOf('plugin_obj_') === 0) {
+                    if (element.$.id.indexOf("plugin_obj_") === 0) {
                         return {
                             cmspluginsItem: CKEDITOR.TRISTATE_OFF
                         };
                     }
                 });
             },
 
             editPlugin: function(element) {
-                var id = element.getAttribute('id').replace('plugin_obj_', '');
-                this.editor.openDialog('cmspluginsDialog');
+                var id = element.getAttribute("id").replace("plugin_obj_", "");
+                this.editor.openDialog("cmspluginsDialog");
                 var body = CMS.$(document);
 
                 // now tweak in dynamic stuff
                 var dialog = CKEDITOR.dialog.getCurrent();
                 dialog.resize(body.width() * 0.8, body.height() * 0.7);
-                $(dialog.getElement().$).addClass('cms-ckeditor-dialog');
+                $(dialog.getElement().$).addClass("cms-ckeditor-dialog");
                 $(dialog.parts.title.$).text(this.options.lang.edit);
-                $(dialog.parts.contents.$).find('iframe').attr('src', '../' + id + '/?_popup=1&no_preview')
-                    .bind('load', function() {
-                        $(this).contents().find('.submit-row').hide().end()
-                            .find('#container').css('min-width', 0).css('padding', 0);
+                $(dialog.parts.contents.$)
+                    .find("iframe")
+                    .attr("src", "../" + id + "/?_popup=1&no_preview")
+                    .bind("load", function() {
+                        $(this)
+                            .contents()
+                            .find(".submit-row")
+                            .hide()
+                            .end()
+                            .find("#container")
+                            .css("min-width", 0)
+                            .css("padding", 0);
                     });
             },
 
             addPlugin: function(item, panel) {
                 var that = this;
 
                 // hide the panel
                 panel.hide();
 
                 // lets figure out how to write something to the editor
                 this.editor.focus();
-                this.editor.fire('saveSnapshot');
+                this.editor.fire("saveSnapshot");
 
                 // gather data
                 var data = {
-                    'placeholder_id': this.options.placeholder_id,
-                    'plugin_type': item.attr('rel'),
-                    'plugin_parent': this.options.plugin_id,
-                    'plugin_language': this.options.plugin_language
+                    placeholder_id: this.options.placeholder_id,
+                    plugin_type: item.attr("rel"),
+                    plugin_parent: this.options.plugin_id,
+                    plugin_language: this.options.plugin_language,
                 };
 
                 that.addPluginDialog(item, data);
             },
 
             addPluginDialog: function(item, data) {
                 var body = CMS.$(document);
                 // open the dialog
                 var selected_text = this.editor.getSelection().getSelectedText();
-                this.editor.openDialog('cmspluginsDialog');
+                this.editor.openDialog("cmspluginsDialog");
 
                 // now tweak in dynamic stuff
                 var dialog = CKEDITOR.dialog.getCurrent();
                 dialog.resize(body.width() * 0.8, body.height() * 0.7);
-                $(dialog.getElement().$).addClass('cms-ckeditor-dialog');
+                $(dialog.getElement().$).addClass("cms-ckeditor-dialog");
                 $(dialog.parts.title.$).text(this.options.lang.add);
-                $(dialog.parts.contents.$).find('iframe').attr('src', this.options.add_plugin_url + '?' + $.param(data))
-                    .bind('load', function() {
-                        $(this).contents().find('.submit-row').hide().end()
-                            .find('#container').css('min-width', 0).css('padding', 0)
-                            .find('#id_name').val(selected_text);
+                $(dialog.parts.contents.$)
+                    .find("iframe")
+                    .attr("src", this.options.add_plugin_url + "?" + $.param(data))
+                    .bind("load", function() {
+                        $(this)
+                            .contents()
+                            .find(".submit-row")
+                            .hide()
+                            .end()
+                            .find("#container")
+                            .css("min-width", 0)
+                            .css("padding", 0)
+                            .find("#id_name")
+                            .val(selected_text);
                     });
             },
 
             // on ajax receivement from server, build <a> or <img> tag dependig in the plugin type
             insertPlugin: function(data) {
                 var that = this;
-                var element, attrs = {
-                    id: 'plugin_obj_' + data.plugin_id
-                };
+                var element,
+                    attrs = {
+                        id: "plugin_obj_" + data.plugin_id
+                    };
                 if (data.plugin_type === this.options.lang.link) {
-                    element = new CKEDITOR.dom.element('a', this.editor.document);
+                    element = new CKEDITOR.dom.element("a", this.editor.document);
                     $.extend(attrs, {
-                        'href': '#',
-                        'data-cmsplugin_title': data.plugin_desc,
-                        'data-cmsplugin_alt': data.plugin_type,
-                        'data-cmsplugin_src': data.plugin_icon
+                        href: "#",
+                        "data-cmsplugin_title": data.plugin_desc,
+                        "data-cmsplugin_alt": data.plugin_type,
+                        "data-cmsplugin_src": data.plugin_icon,
                     });
                     element.setText(data.plugin_name);
                 } else {
-                    element = new CKEDITOR.dom.element('img', this.editor.document);
+                    element = new CKEDITOR.dom.element("img", this.editor.document);
                     $.extend(attrs, {
-                        'title': data.plugin_desc,
-                        'alt': data.plugin_type,
-                        'src': data.plugin_icon
+                        title: data.plugin_desc,
+                        alt: data.plugin_type,
+                        src: data.plugin_icon,
                     });
                 }
                 element.setAttributes(attrs);
 
                 // in case it's a fresh text plugin children don't have to be
                 // deleted separately
                 if (!this.options.delete_on_cancel) {
@@ -270,96 +312,118 @@
              * creation was cancelled - we need to clean up created plugins.
              *
              * @method setupCancelCleanupCallback
              * @public
              * @param {Object} data plugin data
              */
             setupCancelCleanupCallback: function setupCancelCleanupCallback(data) {
-                if (!window.parent || !window.parent.CMS || !window.parent.CMS.API || !window.parent.CMS.API.Helpers) {
+                if (
+                    !window.parent ||
+                    !window.parent.CMS ||
+                    !window.parent.CMS.API ||
+                    !window.parent.CMS.API.Helpers
+                ) {
                     return;
                 }
                 var that = this;
                 var CMS = window.parent.CMS;
                 var cancelModalCallback = function cancelModalCallback(e, opts) {
                     if (!that.options.delete_on_cancel && !that.child_plugins.length) {
                         return;
                     }
                     e.preventDefault();
                     CMS.API.Toolbar.showLoader();
                     var data = {
-                        token: that.options.cancel_plugin_token
+                        token: that.options.cancel_plugin_token,
                     };
                     if (!that.options.delete_on_cancel) {
                         data.child_plugins = that.child_plugins;
                     }
                     $.ajax({
-                        method: 'POST',
-                        url: that.options.cancel_plugin_url,
-                        data: data,
-                        // use 'child_plugins' instead of default 'child_plugins[]'
-                        traditional: true
-                    }).done(function(res) {
-                        CMS.API.Helpers.removeEventListener('modal-close.text-plugin-' + that.options.plugin_id);
-                        opts.instance.close();
-                    }).fail(function(res) {
-                        CMS.API.Messages.open({
-                            message: res.responseText + ' | ' + res.status + ' ' + res.statusText,
-                            delay: 0,
-                            error: true
+                            method: "POST",
+                            url: that.options.cancel_plugin_url,
+                            data: data,
+                            // use 'child_plugins' instead of default 'child_plugins[]'
+                            traditional: true,
+                        })
+                        .done(function(res) {
+                            CMS.API.Helpers.removeEventListener(
+                                "modal-close.text-plugin-" + that.options.plugin_id,
+                            );
+                            opts.instance.close();
+                        })
+                        .fail(function(res) {
+                            CMS.API.Messages.open({
+                                message: res.responseText +
+                                    " | " +
+                                    res.status +
+                                    " " +
+                                    res.statusText,
+                                delay: 0,
+                                error: true,
+                            });
                         });
-                    });
                 };
-                CMS.API.Helpers.addEventListener('modal-close.text-plugin-' + that.options.plugin_id, cancelModalCallback);
+                CMS.API.Helpers.addEventListener(
+                    "modal-close.text-plugin-" + that.options.plugin_id,
+                    cancelModalCallback,
+                );
             },
 
             setupDataProcessor: function() {
                 var link_name = this.options.lang.link;
                 var link_pattern = new RegExp("^" + link_name + "\\s-\\s(.+)$");
 
                 this.editor.dataProcessor.dataFilter.addRules({
                     elements: {
                         // on load from server replace <img> tag by <a> in order to display a real link
                         img: function(element) {
                             var new_element, matches;
-                            if (element.attributes.id && element.attributes.alt &&
+                            if (
+                                element.attributes.id &&
+                                element.attributes.alt &&
                                 element.attributes.alt === link_name &&
-                                element.attributes.id.indexOf('plugin_obj_') === 0) {
+                                element.attributes.id.indexOf("plugin_obj_") === 0
+                            ) {
                                 matches = link_pattern.exec(element.attributes.title);
-                                new_element = new CKEDITOR.htmlParser.element('a', {
-                                    'href': '#',
-                                    'id': element.attributes.id,
-                                    'data-cmsplugin_title': element.attributes.title,
-                                    'data-cmsplugin_src': element.attributes.src,
-                                    'data-cmsplugin_alt': element.attributes.alt
+                                new_element = new CKEDITOR.htmlParser.element("a", {
+                                    href: "#",
+                                    id: element.attributes.id,
+                                    "data-cmsplugin_title": element.attributes.title,
+                                    "data-cmsplugin_src": element.attributes.src,
+                                    "data-cmsplugin_alt": element.attributes.alt,
                                 });
                                 if (matches) {
-                                    new_element.add(new CKEDITOR.htmlParser.text(matches[1]));
+                                    new_element.add(
+                                        new CKEDITOR.htmlParser.text(matches[1]),
+                                    );
                                 }
                                 return new_element;
                             }
-                        }
-                    }
+                        },
+                    },
                 });
 
                 this.editor.dataProcessor.htmlFilter.addRules({
                     elements: {
                         // on post to server replace <a> tag by <img> in order keep plugin format consistent
                         a: function(element) {
                             var new_element;
-                            if (element.attributes.id && element.attributes.id.indexOf('plugin_obj_') === 0) {
-                                new_element = new CKEDITOR.htmlParser.element('img', {
+                            if (
+                                element.attributes.id &&
+                                element.attributes.id.indexOf("plugin_obj_") === 0
+                            ) {
+                                new_element = new CKEDITOR.htmlParser.element("img", {
                                     id: element.attributes.id,
-                                    src: element.attributes['data-cmsplugin_src'],
-                                    title: element.attributes['data-cmsplugin_title'],
-                                    alt: element.attributes['data-cmsplugin_alt']
+                                    src: element.attributes["data-cmsplugin_src"],
+                                    title: element.attributes["data-cmsplugin_title"],
+                                    alt: element.attributes["data-cmsplugin_alt"],
                                 });
                                 return new_element;
                             }
-                        }
-                    }
+                        },
+                    },
                 });
-            }
-
+            },
         });
-
     });
 })(CMS.$);
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,13 @@
 (function($) {
     // CMS.$ will be passed for $
     $(document).ready(function() {
-
-        CKEDITOR.plugins.add('cmsplugins', {
-
+        CKEDITOR.plugins.add("cmsplugins", {
             // Register the icons. They must match command names.
-            icons: 'cmsplugins',
+            icons: "cmsplugins",
 
             // The plugin initialization logic goes inside this method.
             init: function(editor) {
                 var that = this;
 
                 this.options = CMS.CKEditor.options.settings;
                 this.editor = editor;
@@ -17,246 +15,290 @@
                 /**
                  * populated with _fresh_ child plugins
                  */
                 this.child_plugins = [];
                 this.setupCancelCleanupCallback(this.options);
 
                 // don't do anything if there are no plugins defined
-                if (this.options === undefined || this.options.plugins === undefined) return false;
+                if (this.options === undefined || this.options.plugins === undefined)
+                    return false;
 
                 this.setupDialog();
 
                 // add the button
-                this.editor.ui.add('cmsplugins', CKEDITOR.UI_PANELBUTTON, {
-                    'toolbar': 'cms,0',
-                    'label': this.options.lang.toolbar,
-                    'title': this.options.lang.toolbar,
-                    'className': 'cke_panelbutton__cmsplugins',
-                    'modes': {
+                this.editor.ui.add("cmsplugins", CKEDITOR.UI_PANELBUTTON, {
+                    toolbar: "cms,0",
+                    label: this.options.lang.toolbar,
+                    title: this.options.lang.toolbar,
+                    className: "cke_panelbutton__cmsplugins",
+                    modes: {
                         wysiwyg: 1
                     },
-                    'editorFocus': 0,
+                    editorFocus: 0,
 
-                    'panel': {
-                        'css': [CKEDITOR.skin.getPath('editor')].concat(that.editor.config.contentsCss),
-                        'attributes': {
-                            role: 'cmsplugins',
-                            'aria-label': this.options.lang.aria
-                        }
+                    panel: {
+                        css: [CKEDITOR.skin.getPath("editor")].concat(
+                            that.editor.config.contentsCss,
+                        ),
+                        attributes: {
+                            role: "cmsplugins",
+                            "aria-label": this.options.lang.aria,
+                        },
                     },
 
                     // this is called when creating the dropdown list
-                    'onBlock': function(panel, block) {
-                        block.element.setHtml(that.editor.plugins.cmsplugins.setupDropdown());
+                    onBlock: function(panel, block) {
+                        block.element.setHtml(
+                            that.editor.plugins.cmsplugins.setupDropdown(),
+                        );
 
-                        var anchors = $(block.element.$).find('.cke_panel_listItem a');
-                        anchors.bind('click', function(e) {
+                        var anchors = $(block.element.$).find(".cke_panel_listItem a");
+                        anchors.bind("click", function(e) {
                             e.preventDefault();
 
                             that.addPlugin($(this), panel);
                         });
-                    }
+                    },
                 });
 
                 // handle edit event via context menu
                 if (this.editor.contextMenu) {
                     this.setupContextMenu();
-                    this.editor.addCommand('cmspluginsEdit', {
+                    this.editor.addCommand("cmspluginsEdit", {
                         exec: function() {
                             var selection = that.editor.getSelection();
-                            var element = selection.getSelectedElement() || selection.getCommonAncestor().getAscendant('a', true);
+                            var element =
+                                selection.getSelectedElement() ||
+                                selection.getCommonAncestor().getAscendant("a", true);
                             that.editPlugin(element);
-                        }
+                        },
                     });
                 }
 
                 // handle edit event on double click
                 // if event is a jQuery event (touchend), than we mutate
                 // event a bit so we make the payload similar to what ckeditor.event produces
                 var handleEdit = function(event) {
-                    if (event.type === 'touchend' || event.type === 'click') {
+                    if (event.type === "touchend" || event.type === "click") {
                         var element = event.currentTarget;
                         event.data = event.data || {};
-                        that.editor.getSelection().fake(new CKEDITOR.dom.element(element));
+                        that.editor
+                            .getSelection()
+                            .fake(new CKEDITOR.dom.element(element));
                     } else {
                         // heavily relies on the fact that double click
                         // also selects an element
                         var selection = that.editor.getSelection();
-                        var element = selection.getSelectedElement() || selection.getCommonAncestor().getAscendant('a', true);
+                        var element =
+                            selection.getSelectedElement() ||
+                            selection.getCommonAncestor().getAscendant("a", true);
                     }
-                    if (element && element.getAttribute('id').indexOf('plugin_obj_') === 0) {
-                        event.data.dialog = '';
+                    if (
+                        element &&
+                        element.getAttribute("id").indexOf("plugin_obj_") === 0
+                    ) {
+                        event.data.dialog = "";
                         that.editPlugin(element);
                     }
-                }
-                this.editor.on('doubleclick', handleEdit);
-                this.editor.on('instanceReady', function() {
-                    CMS.$('[id*="plugin_obj_"]', CMS.$('iframe.cke_wysiwyg_frame')[0]
-                        .contentWindow.document.documentElement).on('click touchend', handleEdit);
+                };
+                this.editor.on("doubleclick", handleEdit);
+                this.editor.on("instanceReady", function() {
+                    CMS.$(
+                        '[id*="plugin_obj_"]',
+                        CMS.$("iframe.cke_wysiwyg_frame")[0].contentWindow.document
+                        .documentElement,
+                    ).on("click touchend", handleEdit);
                 });
 
                 // setup CKEDITOR.htmlDataProcessor
                 this.setupDataProcessor();
             },
 
             setupDialog: function() {
                 var that = this;
                 var definition = function() {
                     return {
-                        'title': '',
-                        'minWidth': 600,
-                        'minHeight': 200,
-                        'contents': [{
-                            'elements': [{
-                                type: 'html',
-                                html: '<iframe style="position:static; width:100%; height:100%; border:none;" />'
-                            }]
-                        }],
-                        'onOk': function() {
-                            var iframe = $(CKEDITOR.dialog.getCurrent().parts.contents.$).find('iframe').contents();
-                            iframe.find('form').submit();
+                        title: "",
+                        minWidth: 600,
+                        minHeight: 200,
+                        contents: [{
+                            elements: [{
+                                type: "html",
+                                html: '<iframe style="position:static; width:100%; height:100%; border:none;" />',
+                            }, ],
+                        }, ],
+                        onOk: function() {
+                            var iframe = $(
+                                    CKEDITOR.dialog.getCurrent().parts.contents.$,
+                                )
+                                .find("iframe")
+                                .contents();
+                            iframe.find("form").submit();
 
                             // catch the reload event and reattach
                             var reload = CMS.API.Helpers.reloadBrowser;
 
                             CMS.API.Helpers.reloadBrowser = function() {
                                 CKEDITOR.dialog.getCurrent().hide();
 
                                 that.insertPlugin(CMS.API.Helpers.dataBridge);
 
                                 CMS.API.Helpers.reloadBrowser = reload;
                                 return false;
                             };
                             return false;
-                        }
-                    }
+                        },
+                    };
                 };
 
                 // set default definition and open dialog
-                CKEDITOR.dialog.add('cmspluginsDialog', definition);
+                CKEDITOR.dialog.add("cmspluginsDialog", definition);
             },
 
             setupDropdown: function() {
                 var tpl = '<div class="cke_panel_block">';
 
                 // loop through the groups
                 $.each(this.options.plugins, function(i, group) {
                     // add template
-                    tpl += '<h1 class="cke_panel_grouptitle">' + group.group + '</h1>';
+                    tpl += '<h1 class="cke_panel_grouptitle">' + group.group + "</h1>";
                     tpl += '<ul role="presentation" class="cke_panel_list">';
                     // loop through the plugins
                     $.each(group.items, function(ii, item) {
-                        tpl += '<li class="cke_panel_listItem"><a href="#" rel="' + item.type + '">' + item.title + '</a></li>';
+                        tpl +=
+                            '<li class="cke_panel_listItem"><a href="#" rel="' +
+                            item.type +
+                            '">' +
+                            item.title +
+                            "</a></li>";
                     });
-                    tpl += '</ul>';
+                    tpl += "</ul>";
                 });
 
-                tpl += '</div>';
+                tpl += "</div>";
 
                 return tpl;
             },
 
             setupContextMenu: function() {
-                this.editor.addMenuGroup('cmspluginsGroup');
-                this.editor.addMenuItem('cmspluginsItem', {
+                this.editor.addMenuGroup("cmspluginsGroup");
+                this.editor.addMenuItem("cmspluginsItem", {
                     label: this.options.lang.edit,
-                    icon: this.path + 'icons/cmsplugins.png',
-                    command: 'cmspluginsEdit',
-                    group: 'cmspluginsGroup'
+                    icon: this.path + "icons/cmsplugins.png",
+                    command: "cmspluginsEdit",
+                    group: "cmspluginsGroup",
                 });
 
-                this.editor.removeMenuItem('image');
+                this.editor.removeMenuItem("image");
 
                 this.editor.contextMenu.addListener(function(element) {
-                    if (element.$.id.indexOf('plugin_obj_') === 0) {
+                    if (element.$.id.indexOf("plugin_obj_") === 0) {
                         return {
                             cmspluginsItem: CKEDITOR.TRISTATE_OFF
                         };
                     }
                 });
             },
 
             editPlugin: function(element) {
-                var id = element.getAttribute('id').replace('plugin_obj_', '');
-                this.editor.openDialog('cmspluginsDialog');
+                var id = element.getAttribute("id").replace("plugin_obj_", "");
+                this.editor.openDialog("cmspluginsDialog");
                 var body = CMS.$(document);
 
                 // now tweak in dynamic stuff
                 var dialog = CKEDITOR.dialog.getCurrent();
                 dialog.resize(body.width() * 0.8, body.height() * 0.7);
-                $(dialog.getElement().$).addClass('cms-ckeditor-dialog');
+                $(dialog.getElement().$).addClass("cms-ckeditor-dialog");
                 $(dialog.parts.title.$).text(this.options.lang.edit);
-                $(dialog.parts.contents.$).find('iframe').attr('src', '../' + id + '/?_popup=1&no_preview')
-                    .bind('load', function() {
-                        $(this).contents().find('.submit-row').hide().end()
-                            .find('#container').css('min-width', 0).css('padding', 0);
+                $(dialog.parts.contents.$)
+                    .find("iframe")
+                    .attr("src", "../" + id + "/?_popup=1&no_preview")
+                    .bind("load", function() {
+                        $(this)
+                            .contents()
+                            .find(".submit-row")
+                            .hide()
+                            .end()
+                            .find("#container")
+                            .css("min-width", 0)
+                            .css("padding", 0);
                     });
             },
 
             addPlugin: function(item, panel) {
                 var that = this;
 
                 // hide the panel
                 panel.hide();
 
                 // lets figure out how to write something to the editor
                 this.editor.focus();
-                this.editor.fire('saveSnapshot');
+                this.editor.fire("saveSnapshot");
 
                 // gather data
                 var data = {
-                    'placeholder_id': this.options.placeholder_id,
-                    'plugin_type': item.attr('rel'),
-                    'plugin_parent': this.options.plugin_id,
-                    'plugin_language': this.options.plugin_language
+                    placeholder_id: this.options.placeholder_id,
+                    plugin_type: item.attr("rel"),
+                    plugin_parent: this.options.plugin_id,
+                    plugin_language: this.options.plugin_language,
                 };
 
                 that.addPluginDialog(item, data);
             },
 
             addPluginDialog: function(item, data) {
                 var body = CMS.$(document);
                 // open the dialog
                 var selected_text = this.editor.getSelection().getSelectedText();
-                this.editor.openDialog('cmspluginsDialog');
+                this.editor.openDialog("cmspluginsDialog");
 
                 // now tweak in dynamic stuff
                 var dialog = CKEDITOR.dialog.getCurrent();
                 dialog.resize(body.width() * 0.8, body.height() * 0.7);
-                $(dialog.getElement().$).addClass('cms-ckeditor-dialog');
+                $(dialog.getElement().$).addClass("cms-ckeditor-dialog");
                 $(dialog.parts.title.$).text(this.options.lang.add);
-                $(dialog.parts.contents.$).find('iframe').attr('src', this.options.add_plugin_url + '?' + $.param(data))
-                    .bind('load', function() {
-                        $(this).contents().find('.submit-row').hide().end()
-                            .find('#container').css('min-width', 0).css('padding', 0)
-                            .find('#id_name').val(selected_text);
+                $(dialog.parts.contents.$)
+                    .find("iframe")
+                    .attr("src", this.options.add_plugin_url + "?" + $.param(data))
+                    .bind("load", function() {
+                        $(this)
+                            .contents()
+                            .find(".submit-row")
+                            .hide()
+                            .end()
+                            .find("#container")
+                            .css("min-width", 0)
+                            .css("padding", 0)
+                            .find("#id_name")
+                            .val(selected_text);
                     });
             },
 
             // on ajax receivement from server, build <a> or <img> tag dependig in the plugin type
             insertPlugin: function(data) {
                 var that = this;
-                var element, attrs = {
-                    id: 'plugin_obj_' + data.plugin_id
-                };
+                var element,
+                    attrs = {
+                        id: "plugin_obj_" + data.plugin_id
+                    };
                 if (data.plugin_type === this.options.lang.link) {
-                    element = new CKEDITOR.dom.element('a', this.editor.document);
+                    element = new CKEDITOR.dom.element("a", this.editor.document);
                     $.extend(attrs, {
-                        'href': '#',
-                        'data-cmsplugin_title': data.plugin_desc,
-                        'data-cmsplugin_alt': data.plugin_type,
-                        'data-cmsplugin_src': data.plugin_icon
+                        href: "#",
+                        "data-cmsplugin_title": data.plugin_desc,
+                        "data-cmsplugin_alt": data.plugin_type,
+                        "data-cmsplugin_src": data.plugin_icon,
                     });
                     element.setText(data.plugin_name);
                 } else {
-                    element = new CKEDITOR.dom.element('img', this.editor.document);
+                    element = new CKEDITOR.dom.element("img", this.editor.document);
                     $.extend(attrs, {
-                        'title': data.plugin_desc,
-                        'alt': data.plugin_type,
-                        'src': data.plugin_icon
+                        title: data.plugin_desc,
+                        alt: data.plugin_type,
+                        src: data.plugin_icon,
                     });
                 }
                 element.setAttributes(attrs);
 
                 // in case it's a fresh text plugin children don't have to be
                 // deleted separately
                 if (!this.options.delete_on_cancel) {
@@ -270,96 +312,118 @@
              * creation was cancelled - we need to clean up created plugins.
              *
              * @method setupCancelCleanupCallback
              * @public
              * @param {Object} data plugin data
              */
             setupCancelCleanupCallback: function setupCancelCleanupCallback(data) {
-                if (!window.parent || !window.parent.CMS || !window.parent.CMS.API || !window.parent.CMS.API.Helpers) {
+                if (
+                    !window.parent ||
+                    !window.parent.CMS ||
+                    !window.parent.CMS.API ||
+                    !window.parent.CMS.API.Helpers
+                ) {
                     return;
                 }
                 var that = this;
                 var CMS = window.parent.CMS;
                 var cancelModalCallback = function cancelModalCallback(e, opts) {
                     if (!that.options.delete_on_cancel && !that.child_plugins.length) {
                         return;
                     }
                     e.preventDefault();
                     CMS.API.Toolbar.showLoader();
                     var data = {
-                        token: that.options.cancel_plugin_token
+                        token: that.options.cancel_plugin_token,
                     };
                     if (!that.options.delete_on_cancel) {
                         data.child_plugins = that.child_plugins;
                     }
                     $.ajax({
-                        method: 'POST',
-                        url: that.options.cancel_plugin_url,
-                        data: data,
-                        // use 'child_plugins' instead of default 'child_plugins[]'
-                        traditional: true
-                    }).done(function(res) {
-                        CMS.API.Helpers.removeEventListener('modal-close.text-plugin-' + that.options.plugin_id);
-                        opts.instance.close();
-                    }).fail(function(res) {
-                        CMS.API.Messages.open({
-                            message: res.responseText + ' | ' + res.status + ' ' + res.statusText,
-                            delay: 0,
-                            error: true
+                            method: "POST",
+                            url: that.options.cancel_plugin_url,
+                            data: data,
+                            // use 'child_plugins' instead of default 'child_plugins[]'
+                            traditional: true,
+                        })
+                        .done(function(res) {
+                            CMS.API.Helpers.removeEventListener(
+                                "modal-close.text-plugin-" + that.options.plugin_id,
+                            );
+                            opts.instance.close();
+                        })
+                        .fail(function(res) {
+                            CMS.API.Messages.open({
+                                message: res.responseText +
+                                    " | " +
+                                    res.status +
+                                    " " +
+                                    res.statusText,
+                                delay: 0,
+                                error: true,
+                            });
                         });
-                    });
                 };
-                CMS.API.Helpers.addEventListener('modal-close.text-plugin-' + that.options.plugin_id, cancelModalCallback);
+                CMS.API.Helpers.addEventListener(
+                    "modal-close.text-plugin-" + that.options.plugin_id,
+                    cancelModalCallback,
+                );
             },
 
             setupDataProcessor: function() {
                 var link_name = this.options.lang.link;
                 var link_pattern = new RegExp("^" + link_name + "\\s-\\s(.+)$");
 
                 this.editor.dataProcessor.dataFilter.addRules({
                     elements: {
                         // on load from server replace <img> tag by <a> in order to display a real link
                         img: function(element) {
                             var new_element, matches;
-                            if (element.attributes.id && element.attributes.alt &&
+                            if (
+                                element.attributes.id &&
+                                element.attributes.alt &&
                                 element.attributes.alt === link_name &&
-                                element.attributes.id.indexOf('plugin_obj_') === 0) {
+                                element.attributes.id.indexOf("plugin_obj_") === 0
+                            ) {
                                 matches = link_pattern.exec(element.attributes.title);
-                                new_element = new CKEDITOR.htmlParser.element('a', {
-                                    'href': '#',
-                                    'id': element.attributes.id,
-                                    'data-cmsplugin_title': element.attributes.title,
-                                    'data-cmsplugin_src': element.attributes.src,
-                                    'data-cmsplugin_alt': element.attributes.alt
+                                new_element = new CKEDITOR.htmlParser.element("a", {
+                                    href: "#",
+                                    id: element.attributes.id,
+                                    "data-cmsplugin_title": element.attributes.title,
+                                    "data-cmsplugin_src": element.attributes.src,
+                                    "data-cmsplugin_alt": element.attributes.alt,
                                 });
                                 if (matches) {
-                                    new_element.add(new CKEDITOR.htmlParser.text(matches[1]));
+                                    new_element.add(
+                                        new CKEDITOR.htmlParser.text(matches[1]),
+                                    );
                                 }
                                 return new_element;
                             }
-                        }
-                    }
+                        },
+                    },
                 });
 
                 this.editor.dataProcessor.htmlFilter.addRules({
                     elements: {
                         // on post to server replace <a> tag by <img> in order keep plugin format consistent
                         a: function(element) {
                             var new_element;
-                            if (element.attributes.id && element.attributes.id.indexOf('plugin_obj_') === 0) {
-                                new_element = new CKEDITOR.htmlParser.element('img', {
+                            if (
+                                element.attributes.id &&
+                                element.attributes.id.indexOf("plugin_obj_") === 0
+                            ) {
+                                new_element = new CKEDITOR.htmlParser.element("img", {
                                     id: element.attributes.id,
-                                    src: element.attributes['data-cmsplugin_src'],
-                                    title: element.attributes['data-cmsplugin_title'],
-                                    alt: element.attributes['data-cmsplugin_alt']
+                                    src: element.attributes["data-cmsplugin_src"],
+                                    title: element.attributes["data-cmsplugin_title"],
+                                    alt: element.attributes["data-cmsplugin_alt"],
                                 });
                                 return new_element;
                             }
-                        }
-                    }
+                        },
+                    },
                 });
-            }
-
+            },
         });
-
     });
 })(CMS.$);
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/templatetags/ckeditor_link_tags.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/templatetags/ckeditor_link_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,80 @@
+import contextlib
 import importlib
 
+from django import template
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured, ObjectDoesNotExist
-
-from ckeditor_link import conf
-from django import template
 from django.template.defaultfilters import stringfilter
 
+from ckeditor_link import conf
 
 try:
     module_name, class_name = conf.CKEDITOR_LINK_MODEL.rsplit(".", 1)
     my_module = importlib.import_module(module_name)
     ckeditor_link_class = getattr(my_module, class_name, None)
 except ImportError:
     ckeditor_link_class = None
 
 
 register = template.Library()
 
 
 @register.filter
 @stringfilter
-def ckeditor_link_add_links(html):
+def ckeditor_link_add_links(html):  # noqa: C901
     # lxml is not a dependency, but needed for this tag.
     from lxml.html import fragment_fromstring, tostring
+
     if not ckeditor_link_class:
         # TODO: use some log thing, or rais ImproperlyConfigured!
         if settings.DEBUG:
-            msg = "Warning: CKEDITOR_LINK_MODEL (%s) could not be imported!?" % (conf.CKEDITOR_LINK_MODEL, )
+            msg = "Warning: CKEDITOR_LINK_MODEL (%s) could not be imported!?" % (
+                conf.CKEDITOR_LINK_MODEL,
+            )
             raise ImproperlyConfigured(msg)
         return html
     fragment = fragment_fromstring("<div>" + html + "</div>")
-    links = fragment.cssselect('a')
+    links = fragment.cssselect("a")
     for link in links:
-        if link.get('data-ckeditor-link', None):
-            link.attrib.pop('data-ckeditor-link')
+        if link.get("data-ckeditor-link", None):
+            link.attrib.pop("data-ckeditor-link")
             kwargs = {}
             dummy_link = ckeditor_link_class()
             for key, value in link.items():
-                if key.startswith('data-'):
-                    new_key = key.replace('data-', '', 1)
+                if key.startswith("data-"):
+                    new_key = key.replace("data-", "", 1)
                     # DEPRECATED: use CKEDITOR_LINK_ATTR_MODIFIERS setting!
-                    if new_key == 'page_2':
-                        new_key = 'cms_page'  # backward compat, for 0.2.0
-                    if new_key == 'cms_page_2':
-                        new_key = 'cms_page'
+                    if new_key == "page_2":
+                        new_key = "cms_page"  # backward compat, for 0.2.0
+                    if new_key == "cms_page_2":
+                        new_key = "cms_page"
                     # until here
                     if hasattr(dummy_link, new_key):
                         if hasattr(dummy_link, new_key + "_id"):
                             # set fk directly
                             new_key = new_key + "_id"
                             if not value:
                                 value = None
                         kwargs[new_key] = value
                         link.attrib.pop(key)
             for key, formatted_string in conf.CKEDITOR_LINK_ATTR_MODIFIERS.items():
-                try:
+                with contextlib.suppress(KeyError):
+                    # this error is an option, we dont know at all how our link is/was
+                    # built, maybe ages ago
                     kwargs[key] = formatted_string.format(**kwargs)
-                except KeyError:
-                    # this is an option, we dont know at all how our link is/was built (ages ago)
-                    pass
             try:
                 # this can go wrong with fk and the like
                 real_link = ckeditor_link_class(**kwargs)
-                link.set('href', real_link.get_link())
-                if getattr(real_link, 'get_link_target', None):
-                    link.set('target', real_link.get_link_target())
-                if getattr(real_link, 'get_link_style', None):
-                    link.set('class', real_link.get_link_style())
-                if getattr(real_link, 'get_link_attrs', None):
+                link.set("href", real_link.get_link())
+                if getattr(real_link, "get_link_target", None):
+                    link.set("target", real_link.get_link_target())
+                if getattr(real_link, "get_link_style", None):
+                    link.set("class", real_link.get_link_style())
+                if getattr(real_link, "get_link_attrs", None):
                     for attr, value in real_link.get_link_attrs().items():
                         link.set(attr, value)
             except (ValueError, ObjectDoesNotExist):
                 continue
     # arf: http://makble.com/python-why-lxml-etree-tostring-method-returns-bytes
     # beautifulsoup to the rescue!
-    return tostring(fragment, encoding='unicode')
+    return tostring(fragment, encoding="unicode")
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/settings.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Settings that need to be set in order to run the tests."""
+import logging
 import os
+
 # import sys
 import tempfile
-import logging
 
 # compat
 import django
+
 if django.VERSION[:2] < (1, 10):
     from django.core.urlresolvers import reverse_lazy
 else:
     from django.urls import reverse_lazy
 
 
 DEBUG = True
@@ -19,154 +21,158 @@
 HEADLESS_TESTING = True
 
 
 CKEDITOR_LINK_USE_CMS_FILER = True
 
 # not a good example, but working for our tests
 CKEDITOR_LINK_ATTR_MODIFIERS = {
-    'target': '{target}--xy',
+    "target": "{target}--xy",
 }
-CKEDITOR_LINK_MODEL = 'ckeditor_link.tests.test_app.models.LinkModel'
-CKEDITOR_LINK_IFRAME_URL = reverse_lazy('admin:test_app_linkmodel_add')
-CKEDITOR_LINK_VERIFY_URL = reverse_lazy('admin:test_app_linkmodel_verify')
+CKEDITOR_LINK_MODEL = "ckeditor_link.tests.test_app.models.LinkModel"
+CKEDITOR_LINK_IFRAME_URL = reverse_lazy("admin:test_app_linkmodel_add")
+CKEDITOR_LINK_VERIFY_URL = reverse_lazy("admin:test_app_linkmodel_verify")
 
 CKEDITOR_CONFIGS = {
-    'default': {
-        'djangolinkIframeURL': CKEDITOR_LINK_IFRAME_URL,
-        'djangolinkVerifyURL': CKEDITOR_LINK_VERIFY_URL,
-        'djangolinkFallbackField': 'external_url',
-        'linkShowAdvancedTab': False,
-        'extraPlugins': ','.join(
+    "default": {
+        "djangolinkIframeURL": CKEDITOR_LINK_IFRAME_URL,
+        "djangolinkVerifyURL": CKEDITOR_LINK_VERIFY_URL,
+        "djangolinkFallbackField": "external_url",
+        "linkShowAdvancedTab": False,
+        "extraPlugins": ",".join(
             [
                 # your extra plugins here
-                'djangolink',
-                'autolink',
-                'autoembed',
-                'embedsemantic',
-                'autogrow',
-                'devtools',
-                'widget',
-                'lineutils',
-                'clipboard',
-                'dialog',
-                'dialogui',
-                'elementspath'
-            ]),
-        'toolbar': 'Custom',
-        'toolbar_Custom': [
-            ['Bold', 'Underline'],
-            ['DjangoLink', 'Unlink'],
-            ['Link', 'Unlink'],
-            ['RemoveFormat', 'Source']
-        ]
+                "djangolink",
+                "autolink",
+                "autoembed",
+                "embedsemantic",
+                "autogrow",
+                "devtools",
+                "widget",
+                "lineutils",
+                "clipboard",
+                "dialog",
+                "dialogui",
+                "elementspath",
+            ]
+        ),
+        "toolbar": "Custom",
+        "toolbar_Custom": [
+            ["Bold", "Underline"],
+            ["DjangoLink", "Unlink"],
+            ["Link", "Unlink"],
+            ["RemoveFormat", "Source"],
+        ],
     }
 }
 
-CMS_TEMPLATES = (
-    ('cms_dummy.html', 'Dummy'),
-)
+CMS_TEMPLATES = (("cms_dummy.html", "Dummy"),)
 
 SITE_ID = 1
 
-APP_ROOT = os.path.abspath(
-    os.path.join(os.path.dirname(__file__), ".."))
+APP_ROOT = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 
 DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': 'db.sqlite',
+    "default": {
+        "ENGINE": "django.db.backends.sqlite3",
+        "NAME": "db.sqlite",
     }
 }
 
-LANGUAGE_CODE = 'en'
+LANGUAGE_CODE = "en"
 LANGUAGES = (
-    ('en', 'ENGLISHS', ),
+    (
+        "en",
+        "ENGLISHS",
+    ),
 )
 
-X_FRAME_OPTIONS = 'SAMEORIGIN'
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
-ROOT_URLCONF = 'ckeditor_link.tests.urls'
+X_FRAME_OPTIONS = "SAMEORIGIN"
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
+ROOT_URLCONF = "ckeditor_link.tests.urls"
 
 # media root is overridden when needed in tests
-MEDIA_ROOT = tempfile.mkdtemp(suffix='ckeditor_media_root')
+MEDIA_ROOT = tempfile.mkdtemp(suffix="ckeditor_media_root")
 MEDIA_URL = "/media/"
-STATIC_URL = '/static/'
-STATIC_ROOT = os.path.join(APP_ROOT, '../test_app_static')
-STATICFILES_DIRS = (
-    os.path.join(APP_ROOT, 'static'),
-)
+STATIC_URL = "/static/"
+STATIC_ROOT = os.path.join(APP_ROOT, "../test_app_static")
+STATICFILES_DIRS = (os.path.join(APP_ROOT, "static"),)
 
 # TEMPLATE_DIRS = (
 #     os.path.join(APP_ROOT, 'tests/test_app/templates'),
 # )
 
-COVERAGE_REPORT_HTML_OUTPUT_DIR = os.path.join(
-    os.path.join(APP_ROOT, 'tests/coverage'))
+COVERAGE_REPORT_HTML_OUTPUT_DIR = os.path.join(os.path.join(APP_ROOT, "tests/coverage"))
 COVERAGE_MODULE_EXCLUDES = [
-    'tests$', 'settings$', 'urls$', 'locale$',
-    'migrations', 'fixtures', 'admin$', 'django_extensions',
+    "tests$",
+    "settings$",
+    "urls$",
+    "locale$",
+    "migrations",
+    "fixtures",
+    "admin$",
+    "django_extensions",
 ]
 
 EXTERNAL_APPS = (
-    'django.contrib.admin',
+    "django.contrib.admin",
     # 'django.contrib.admindocs',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.messages',
-    'django.contrib.sessions',
-    'django.contrib.staticfiles',
-    'django.contrib.sitemaps',
-    'django.contrib.sites',
-    'ckeditor',
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.messages",
+    "django.contrib.sessions",
+    "django.contrib.staticfiles",
+    "django.contrib.sitemaps",
+    "django.contrib.sites",
+    "ckeditor",
     # 'djangocms_text_ckeditor',
-    'cms',
-    'treebeard',
-    'menus',
-    'filer',
-    'sekizai',
-    'easy_thumbnails',
+    "cms",
+    "treebeard",
+    "menus",
+    "filer",
+    "sekizai",
+    "easy_thumbnails",
 )
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'OPTIONS': {
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
-                'django.template.context_processors.i18n',
-                'django.template.context_processors.request',
-                'django.template.context_processors.media',
-                'django.template.context_processors.static',
-                'sekizai.context_processors.sekizai',
-                'cms.context_processors.cms_settings',
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
+                "django.template.context_processors.i18n",
+                "django.template.context_processors.request",
+                "django.template.context_processors.media",
+                "django.template.context_processors.static",
+                "sekizai.context_processors.sekizai",
+                "cms.context_processors.cms_settings",
             ],
-            'loaders': [
-                'django.template.loaders.filesystem.Loader',
-                'django.template.loaders.app_directories.Loader',
+            "loaders": [
+                "django.template.loaders.filesystem.Loader",
+                "django.template.loaders.app_directories.Loader",
                 # 'django.template.loaders.eggs.Loader',
             ],
-        }
+        },
     },
 ]
 
 
 INTERNAL_APPS = (
-    'ckeditor_link',
+    "ckeditor_link",
     # 'ckeditor_link',
-    'ckeditor_link.tests.test_app',
+    "ckeditor_link.tests.test_app",
 )
 
 MIDDLEWARE = (
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
     # Uncomment the next line for simple clickjacking protection:
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
-    'django.middleware.locale.LocaleMiddleware',
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
+    "django.middleware.locale.LocaleMiddleware",
 )
 
 INSTALLED_APPS = EXTERNAL_APPS + INTERNAL_APPS
 COVERAGE_MODULE_EXCLUDES += EXTERNAL_APPS
 
-SECRET_KEY = 'foobarXXXxxsvXY'
+SECRET_KEY = "foobarXXXxxsvXY"
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/admin.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/admin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+# compat
+import django
 from django import forms
 from django.contrib import admin
 
 from ckeditor_link.admin import DjangoLinkAdmin
-from .models import TestModel, LinkModel, ContribLinkModel, CMSFilerLinkModel
 
-# compat
-import django
+from .models import CMSFilerLinkModel, ContribLinkModel, LinkModel, TestModel
+
 if django.VERSION[:2] < (1, 10):
     from django.forms.extras.widgets import SelectDateWidget
 else:
     from django.forms.widgets import SelectDateWidget
 
 
 class LinkModelForm(forms.ModelForm):
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/0001_initial.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_app/models.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,66 @@
-from django.db import models
+# compat
+import django
 from ckeditor.fields import RichTextField
-from ckeditor_link.link_model.models import CMSFilerLinkBase, LinkBase
+from django.db import models
 
+from ckeditor_link.link_model.models import CMSFilerLinkBase, LinkBase
 
-# compat
-import django
 if django.VERSION[:2] < (1, 10):
     from django.core.urlresolvers import reverse
 else:
     from django.urls import reverse
 
 
 class TestModel(models.Model):
-    title = models.CharField(max_length=255, )
-    richtext = RichTextField(default='')
-    richtext_second = RichTextField(default='')
+    title = models.CharField(
+        max_length=255,
+    )
+    richtext = RichTextField(default="")
+    richtext_second = RichTextField(default="")
 
     def __str__(self):
         return "%s" % self.title
 
     def get_absolute_url(self):
-        return reverse('testmodel_detail', args=(self.id, ))
+        return reverse("testmodel_detail", args=(self.id,))
 
 
 # @python_2_unicode_compatible
 # class CMSTestModel(models.Model):
 #     title = models.CharField(max_length=255, )
 #     richtext = HTMLField()
 #
 #     def __str__(self):
 #         return "%s" % self.title
 
 
 class LinkModelBase(models.Model):
-    external_url = models.CharField(max_length=255, blank=True, default='',)
-    email = models.EmailField(blank=True, default='',)
+    external_url = models.CharField(
+        max_length=255,
+        blank=True,
+        default="",
+    )
+    email = models.EmailField(
+        blank=True,
+        default="",
+    )
     # http://stackoverflow.com/questions/12644142/prefill-a-datetimefield-from-url-in-django-admin
     when = models.DateField(blank=True, null=True)
     testmodel = models.ForeignKey(
         TestModel,
         null=True,
         on_delete=models.CASCADE,
         default=None,
         blank=True,
     )
     target = models.CharField(
         max_length=255,
         blank=True,
-        default='',
+        default="",
     )
 
     class Meta:
         abstract = True
 
     def __str__(self):
         return "LINK object: %s" % self.get_link()
@@ -72,15 +81,15 @@
     def get_link_target(self):
         return "_blank"
 
     def get_link_style(self):
         return "no-css-class"
 
     def get_link_attrs(self):
-        return {'data-test': 'abc'}
+        return {"data-test": "abc"}
 
 
 class LinkModel(LinkModelBase):
     pass
 
 
 class ContribLinkModel(LinkBase):
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_editor.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_editor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,122 @@
 # -*- coding: utf-8 -*-
 from time import sleep
 
+# compat
+import django
 from selenium.common.exceptions import NoSuchElementException
 
-from ckeditor_link.tests.utils.selenium_utils import SeleniumTestCase
 from ckeditor_link.tests.test_app.models import TestModel
+from ckeditor_link.tests.utils.selenium_utils import SeleniumTestCase
 
-
-# compat
-import django
 if django.VERSION[:2] < (1, 10):
     from django.core.urlresolvers import reverse
 else:
     from django.urls import reverse
 
 
 class ckeditor_linkEditorTests(SeleniumTestCase):
-    fixtures = ['test_app.json', ]
+    fixtures = [
+        "test_app.json",
+    ]
 
     def setUp(self):
         self.existing = TestModel.objects.get(pk=1)
         super(ckeditor_linkEditorTests, self).setUp()
 
     def tearDown(self):
         self.webdriver.quit()
 
     def test_app_index_get(self):
         # if this fails, everything is probably broken.
         self.login()
-        self.open(reverse('admin:index'))
+        self.open(reverse("admin:index"))
         self.webdriver.find_css(".app-test_app")
 
     def test_editor_has_button_dialog_opens_has_form(self):
         self.login()
-        self.open(reverse('admin:test_app_testmodel_change', args=[self.existing.id]))
+        self.open(
+            reverse(
+                "admin:test_app_testmodel_change",
+                args=[self.existing.id],
+            ),
+        )
         # wait = WebDriverWait(self.webdriver, 5)
-        # element = wait.until(EC.frame_to_be_available_and_switch_to_it((By.CSS_SELECTOR, '.cke_dialog_ui_html')))
-        # WebDriverWait(self.webdriver, 4).until(EC.presence_of_element_located(By.CSS_SELECTOR, '.cke_dialog_ui_html'))
+        # element = wait.until(
+        #     EC.frame_to_be_available_and_switch_to_it(
+        #         (By.CSS_SELECTOR, ".cke_dialog_ui_html")
+        #     )
+        # )
+        # WebDriverWait(self.webdriver, 4).until(
+        #     EC.presence_of_element_located(By.CSS_SELECTOR, ".cke_dialog_ui_html")
+        # )
         sleep(1)  # #1 may ckeditor be very slow, so the click event is not handled?!
         button = self.webdriver.wait_for_css(".cke_button__djangolink")
         button[0].click()
         self.webdriver.wait_for_css(".cke_dialog_title")
         # sleep(2)  # argh
         iframe = self.webdriver.find_css(".cke_dialog_ui_html")
         self.webdriver.switch_to.frame(iframe)
         self.webdriver.wait_for_css("#id_target")
 
     def test_dialog_form_validation(self):
         self.login()
-        self.open(reverse('admin:test_app_testmodel_change', args=[self.existing.id]))
+        self.open(reverse("admin:test_app_testmodel_change", args=[self.existing.id]))
         sleep(1)  # #1
         button = self.webdriver.wait_for_css(".cke_button__djangolink")
         button[0].click()
         self.webdriver.wait_for_css(".cke_dialog_title")
         # sleep(2)  # argh
         iframe = self.webdriver.find_css(".cke_dialog_ui_html")
         self.webdriver.switch_to.frame(iframe)
         email = self.webdriver.wait_for_css("#id_email")
-        email.send_keys('what-foo')
+        email.send_keys("what-foo")
         self.webdriver.switch_to.default_content()
         ok = self.webdriver.wait_for_css(".cke_dialog_ui_button_ok")
         ok.click()
         self.webdriver.switch_to.frame(iframe)
         self.webdriver.wait_for_css(".field-email .errorlist")
-        email.send_keys('root@example.com')
+        email.send_keys("root@example.com")
         self.webdriver.switch_to.default_content()
         ok = self.webdriver.wait_for_css(".cke_dialog_ui_button_ok")
         ok.click()
         sleep(1)  # argh
         try:
             # check that dialog is gone or invisible
             title = self.webdriver.find_css(".cke_dialog_title")
             self.assertFalse(title.is_displayed())
         except NoSuchElementException:
             # ok if removed from the DOM!!
             pass
 
     def test_no_fake_null_as_string_values(self):
         self.login()
-        self.open(reverse('admin:test_app_testmodel_change', args=[self.existing.id]))
+        self.open(reverse("admin:test_app_testmodel_change", args=[self.existing.id]))
         sleep(1)  # argh
         button = self.webdriver.wait_for_css(".cke_button__djangolink")
         button[0].click()
         self.webdriver.wait_for_css(".cke_dialog_title")
         sleep(1)  # argh
         iframe = self.webdriver.find_css(".cke_dialog_ui_html")
         self.webdriver.switch_to.frame(iframe)
-        self.webdriver.wait_for_css("#id_testmodel")  # just wait for it, then send with "null"
+        self.webdriver.wait_for_css(
+            "#id_testmodel"
+        )  # just wait for it, then send with "null"
         self.webdriver.switch_to.default_content()
         ok = self.webdriver.wait_for_css(".cke_dialog_ui_button_ok")
         ok.click()
         sleep(1)  # argh
         # inserted at first position in html, so this should work.
         ckcontent_iframe = self.webdriver.find_css("#cke_id_richtext iframe")
         self.webdriver.switch_to.frame(ckcontent_iframe)
         link = self.webdriver.wait_for_css("body a[data-ckeditor-link=true]")
-        self.assertEqual('', link.get_attribute('data-testmodel'))
+        self.assertEqual("", link.get_attribute("data-testmodel"))
 
     def test_two_editors_in_same_form(self):
         # TODO
         self.login()
-        self.open(reverse('admin:test_app_testmodel_change', args=[self.existing.id]))
+        self.open(reverse("admin:test_app_testmodel_change", args=[self.existing.id]))
 
     def test_dialog_submit_and_link_attrs(self):
         # TODO
         self.login()
-        self.open(reverse('admin:test_app_testmodel_change', args=[self.existing.id]))
+        self.open(reverse("admin:test_app_testmodel_change", args=[self.existing.id]))
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_link_model.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_link_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,104 +2,115 @@
 from ckeditor_link.templatetags import ckeditor_link_tags
 
 try:
     reload
 except NameError:
     from importlib import reload
 
-from ckeditor_link.tests.utils.selenium_utils import SeleniumTestCase
+# compat
+import django
 from cms import api
 from cms.constants import TEMPLATE_INHERITANCE_MAGIC
 from django.test import Client, override_settings
 
-from ckeditor_link.tests.test_app.models import TestModel
 from ckeditor_link import conf
+from ckeditor_link.tests.test_app.models import TestModel
+from ckeditor_link.tests.utils.selenium_utils import SeleniumTestCase
 
-# compat
-import django
 if django.VERSION[:2] < (1, 10):
     from django.core.urlresolvers import reverse
 else:
     from django.urls import reverse
 
 
 class ContribLinkModelTests(SeleniumTestCase):
-    fixtures = ['test_app_link_model.json', ]
+    fixtures = [
+        "test_app_link_model.json",
+    ]
 
     def setUp(self):
         self.test_object = TestModel.objects.get(pk=101)
         self.test_object_cms_page = TestModel.objects.get(pk=102)
         self.page1 = api.create_page(
-            slug='page1',
+            slug="page1",
             title="Page1",
-            language='en',
+            language="en",
             template=TEMPLATE_INHERITANCE_MAGIC,
-            parent=None
+            parent=None,
         )
-        self.page1.publish('en')
+        self.page1.publish("en")
         self.page2 = api.create_page(
             title="Page2",
-            language='en',
+            language="en",
             template=TEMPLATE_INHERITANCE_MAGIC,
             parent=None,
-            position='first-child',
+            position="first-child",
         )
-        self.page2.publish('en')
+        self.page2.publish("en")
         # page2 has id=3!
         super(ContribLinkModelTests, self).setUp()
 
     def tearDown(self):
         self.webdriver.quit()
 
     def test_admin_loads(self):
         """
         loading link forms
         """
         self.login()
-        self.open(reverse('admin:test_app_contriblinkmodel_add'))
-        self.webdriver.wait_for_css("#id_external", )
-        self.open(reverse('admin:test_app_cmsfilerlinkmodel_add'))
-        self.webdriver.wait_for_css("#id_cms_page_0", )
+        self.open(reverse("admin:test_app_contriblinkmodel_add"))
+        self.webdriver.wait_for_css(
+            "#id_external",
+        )
+        self.open(reverse("admin:test_app_cmsfilerlinkmodel_add"))
+        self.webdriver.wait_for_css(
+            "#id_cms_page_0",
+        )
 
     def test_admin_page_fallback(self):
         """
         older versions have "page" instead of cms_page as data- attributes
         """
         self.login()
-        self.open('{}?page={}'.format(
-            reverse('admin:test_app_cmsfilerlinkmodel_add'),
-            self.page2.id
-        ))
-        self.webdriver.wait_for_css("#id_cms_page_1 option", )
-        option = self.webdriver.wait_for_css("#id_cms_page_1 option[selected]", )
-        self.assertEqual(option.get_attribute('value'), str(self.page2.id))
+        self.open(
+            "{}?page={}".format(
+                reverse("admin:test_app_cmsfilerlinkmodel_add"), self.page2.id
+            )
+        )
+        self.webdriver.wait_for_css(
+            "#id_cms_page_1 option",
+        )
+        option = self.webdriver.wait_for_css(
+            "#id_cms_page_1 option[selected]",
+        )
+        self.assertEqual(option.get_attribute("value"), str(self.page2.id))
 
     @override_settings(
-        CKEDITOR_LINK_MODEL='ckeditor_link.tests.test_app.models.CMSFilerLinkModel'
+        CKEDITOR_LINK_MODEL="ckeditor_link.tests.test_app.models.CMSFilerLinkModel"
     )
     def test_cms_page_link_fallback(self):
         reload(conf)
         reload(ckeditor_link_tags)
         client = Client()
-        url = reverse('testmodel_detail', args=[self.test_object_cms_page.id])
+        url = reverse("testmodel_detail", args=[self.test_object_cms_page.id])
         self.test_object_cms_page.richtext = self.test_object_cms_page.richtext.replace(
-            '<cms_page_id_page2>', str(self.page2.id)
+            "<cms_page_id_page2>", str(self.page2.id)
         )
         self.test_object_cms_page.save()
         response = client.get(url)
         self.assertContains(response, 'href="/page2/"')
 
     @override_settings(
-        CKEDITOR_LINK_MODEL='ckeditor_link.tests.test_app.models.CMSFilerLinkModel',
+        CKEDITOR_LINK_MODEL="ckeditor_link.tests.test_app.models.CMSFilerLinkModel",
         SITE_ID=2,
     )
     def test_cms_page_link_to_other_site(self):
         reload(conf)
         reload(ckeditor_link_tags)
         client = Client()
-        url = reverse('testmodel_detail', args=[self.test_object_cms_page.id])
+        url = reverse("testmodel_detail", args=[self.test_object_cms_page.id])
         self.test_object_cms_page.richtext = self.test_object_cms_page.richtext.replace(
-            '<cms_page_id_page2>', str(self.page2.id)
+            "<cms_page_id_page2>", str(self.page2.id)
         )
         self.test_object_cms_page.save()
         response = client.get(url)
         self.assertContains(response, 'href="//example.com/page2/"')
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/test_templatetag.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_templatetag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # -*- coding: utf-8 -*-
-from django.test import Client
-from django.test import TestCase
+# compat
+import django
+from django.test import Client, TestCase
 
 from ckeditor_link.tests.test_app.models import TestModel
 
-# compat
-import django
 if django.VERSION[:2] < (1, 10):
     from django.core.urlresolvers import reverse
 else:
     from django.urls import reverse
 
 
 class CKeditorLinkTemplateTagTests(TestCase):
-    fixtures = ['test_app.json', ]
+    fixtures = [
+        "test_app.json",
+    ]
 
     def setUp(self):
         self.test_object = TestModel.objects.get(pk=2)
         self.test_object_not_existing_fk = TestModel.objects.get(pk=1)
 
     def tearDown(self):
         pass
 
     def test_tag_link_target_class_value(self):
         """
         does it transform everything as it should?
         """
         client = Client()
-        url = reverse('testmodel_detail', args=[self.test_object.id])
+        url = reverse("testmodel_detail", args=[self.test_object.id])
         response = client.get(url)
         # check it!
         self.assertEqual(response.status_code, 200)
 
     def test_tag_no_destruction_of_existing_links(self):
         """
         normal existing <a href="xx" should not be tinkered with
@@ -39,42 +40,42 @@
         pass
 
     def test_tag_robustness(self):
         """
         can it handle LinkModel with for example no get_css_class method?
         """
         client = Client()
-        url = reverse('testmodel_detail', args=[self.test_object.id])
+        url = reverse("testmodel_detail", args=[self.test_object.id])
         response = client.get(url)
         # check it!
         self.assertEqual(response.status_code, 200)
 
     def test_not_existing_foreign_key_value(self):
         """
         can it handle no more existing foreign key values set in links?
         """
         client = Client()
-        url = reverse('testmodel_detail', args=[self.test_object_not_existing_fk.id])
+        url = reverse("testmodel_detail", args=[self.test_object_not_existing_fk.id])
         response = client.get(url)
         # no exception, there we go!
         self.assertEqual(response.status_code, 200)
 
     def test_get_link_attrs(self):
         """
         can it output correct link attrs
         """
         client = Client()
-        url = reverse('testmodel_detail', args=[self.test_object.id])
+        url = reverse("testmodel_detail", args=[self.test_object.id])
         response = client.get(url)
         # no exception, there we go!
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, 'data-test="abc"')
 
     def test_tag_attr_modifiers(self):
         """
         do attr modifiers work?
         has data-target="targetvalue", needs <a href="targetvalue--xy"
         """
         client = Client()
-        url = reverse('testmodel_detail', args=[self.test_object.id])
+        url = reverse("testmodel_detail", args=[self.test_object.id])
         response = client.get(url)
         self.assertContains(response, 'href="targetvalue--xy"')
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/urls.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/urls.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """URLs to run the tests."""
-from django.conf.urls import include
-from django.urls import path, re_path
+
 from django.contrib import admin
+from django.urls import include, path
 
 from ckeditor_link.tests.test_app.views import TestModelDetailView
 
-
 urlpatterns = [
-    path('admin/', admin.site.urls),
-    re_path(r'^testmodel/(?P<pk>\d+)/$', TestModelDetailView.as_view(), name='testmodel_detail'),
-    path('', include('cms.urls')),
+    path("admin/", admin.site.urls),
+    path("testmodel/<int:pk>/", TestModelDetailView.as_view(), name="testmodel_detail"),
+    path("", include("cms.urls")),
 ]
 
 # if settings.DEBUG:
 #     urlpatterns += [
-#         url(r'^media/(?P<path>.*)$', 'django.views.static.serve', {'document_root': settings.MEDIA_ROOT}),
+#         url(
+#             r"^media/(?P<path>.*)$",
+#             "django.views.static.serve",
+#             {"document_root": settings.MEDIA_ROOT},
+#         ),
 #     ]
```

### Comparing `django-ckeditor-link-0.5.1/ckeditor_link/tests/utils/selenium_utils.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/utils/selenium_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,54 @@
+# compat
+import django
 from django.conf import settings
 from django.contrib.auth.models import User
 from django.contrib.staticfiles.testing import StaticLiveServerTestCase
+from selenium import webdriver
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.common.by import By
-from selenium.webdriver.support.wait import WebDriverWait
-from selenium import webdriver
 from selenium.webdriver.firefox.options import Options
+from selenium.webdriver.support.wait import WebDriverWait
 
-
-# compat
-import django
 if django.VERSION[:2] < (1, 10):
     from django.core.urlresolvers import reverse
 else:
     from django.urls import reverse
 
 
 class SeleniumTestCase(StaticLiveServerTestCase):
     """
     A base test case for Selenium, providing hepler methods for generating
     clients and logging in profiles.
     """
 
-    username = 'admin'
-    password = 'admin'
+    username = "admin"
+    password = "admin"
 
     def setUp(self):
-        User.objects.create_superuser(self.username, 'admin@free.fr', self.password)
+        User.objects.create_superuser(self.username, "admin@free.fr", self.password)
         # Instantiating the WebDriver will load your browser
         options = Options()
         if settings.HEADLESS_TESTING:
             options.add_argument("--headless")
-        self.webdriver = CustomWebDriver(options=options, )
+        self.webdriver = CustomWebDriver(
+            options=options,
+        )
 
     def open(self, url):
         self.webdriver.get("%s%s" % (self.live_server_url, url))
 
     def login(self):
-        self.open(reverse('admin:index'))
-        # SeleniFIXTURESum knows it has to wait for page loads (except for AJAX requests)
+        self.open(reverse("admin:index"))
+        # Selenium knows it has to wait for page loads (except for AJAX requests)
         # so we don't need to do anything about that, and can just
         # call find_css. Since we can chain methods, we can
         # call the built-in send_keys method right away to change the
         # value of the field
-        self.webdriver.find_css('#id_username').send_keys(self.username)
+        self.webdriver.find_css("#id_username").send_keys(self.username)
         # for the password, we can now just call find_css since we know the page
         # has been rendered
         self.webdriver.find_css("#id_password").send_keys(self.password)
         # You're not limited to CSS selectors only, check
         # http://seleniumhq.org/docs/03_webdriver.html for
         # a more compreehensive documentation.
         self.webdriver.find_element_by_xpath('//input[@type="submit"]').click()
@@ -65,13 +66,17 @@
         if found == 1:
             return elems[0]
         elif not elems:
             raise NoSuchElementException(css_selector)
         return elems
 
     def wait_for_css(self, css_selector, timeout=4):
-        """ Shortcut for WebDriverWait"""
-        return WebDriverWait(self, timeout).until(lambda driver: driver.find_css(css_selector))
+        """Shortcut for WebDriverWait"""
+        return WebDriverWait(self, timeout).until(
+            lambda driver: driver.find_css(css_selector)
+        )
 
     def wait_for_iframe(self, iframe_selector, timeout=4):
-        """ Shortcut for WebDriverWait"""
-        return WebDriverWait(self, timeout).until(lambda driver: driver.frame_to_be_available_and_switch_to_it())
+        """Shortcut for WebDriverWait"""
+        return WebDriverWait(self, timeout).until(
+            lambda driver: driver.frame_to_be_available_and_switch_to_it()
+        )
```

### Comparing `django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/PKG-INFO` & `django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditor-link
-Version: 0.5.1
+Version: 0.5.3.dev0
 Summary: Alternative link dialog for ckeditor 4, using django modeladmin forms.
 Home-page: http://github.com/bnzk/django-ckeditor-link
 Author: Ben Stähli
 Author-email: bnzk@bnzk.ch
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=1.11
 
 # django-ckeditor-link
 
 Build status fails sometimes - selenium and iframes and ... sleep. Passes with local tox, believe me.
 
 [![CI](https://img.shields.io/github/actions/workflow/status/bnzk/django-ckeditor-link/ci.yml?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-ckeditor-link/actions/workflows/ci.yml)
 [![Version](https://img.shields.io/pypi/v/django-ckeditor-link.svg?style=flat-square "Version")](https://pypi.python.org/pypi/django-ckeditor-link/)
```

### Comparing `django-ckeditor-link-0.5.1/django_ckeditor_link.egg-info/SOURCES.txt` & `django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 CHANGELOG.txt
 DESCRIPTION
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 ckeditor_link/__init__.py
 ckeditor_link/admin.py
 ckeditor_link/conf.py
 ckeditor_link/link_model/__init__.py
 ckeditor_link/link_model/conf.py
 ckeditor_link/link_model/models.py
```

### Comparing `django-ckeditor-link-0.5.1/setup.py` & `django_ckeditor_link-0.5.3.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # coding: utf-8
-from setuptools import setup, find_packages
 import os
 
+from setuptools import find_packages, setup
 
 # not so bad: http://joebergantine.com/blog/2015/jul/17/releasing-package-pypi/
-version = __import__('ckeditor_link').__version__
+version = __import__("ckeditor_link").__version__
 
 
 def read(fname):
     # read the contents of a text file
-    return open(os.path.join(os.path.dirname(__file__), fname)).read()
+    with open(os.path.join(os.path.dirname(__file__), fname)) as file:
+        content = file.read()
+    return content
 
 
 setup(
     name="django-ckeditor-link",
     version=version,
-    url='http://github.com/bnzk/django-ckeditor-link',
-    license='MIT',
-    platforms=['OS Independent'],
-    description=read('DESCRIPTION'),
-    long_description=read('README.md'),
+    url="http://github.com/bnzk/django-ckeditor-link",
+    license="MIT",
+    platforms=["OS Independent"],
+    description=read("DESCRIPTION"),
+    long_description=read("README.md"),
     long_description_content_type="text/markdown",
-    author=u'Ben Stähli',
-    author_email='bnzk@bnzk.ch',
+    author="Ben Stähli",
+    author_email="bnzk@bnzk.ch",
     packages=find_packages(),
     install_requires=(
         # 'Django>=1.3,<1.5',  # no need to limit while in development
-        'Django>=1.11',
+        "Django>=1.11",
     ),
     include_package_data=True,
     zip_safe=False,
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Framework :: Django',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Topic :: Internet :: WWW/HTTP',
+        "Development Status :: 4 - Beta",
+        "Framework :: Django",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Topic :: Internet :: WWW/HTTP",
     ],
 )
```

