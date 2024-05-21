# Comparing `tmp/django_ckeditor_link-0.5.3.tar.gz` & `tmp/django_ckeditor_link-0.5.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ckeditor_link-0.5.3.tar", last modified: Tue May 21 13:57:19 2024, max compression
+gzip compressed data, was "django_ckeditor_link-0.5.3.dev0.tar", last modified: Tue May 21 13:20:42 2024, max compression
```

## Comparing `django_ckeditor_link-0.5.3.tar` & `django_ckeditor_link-0.5.3.dev0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.072714 django_ckeditor_link-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-21 13:57:19.072714 django_ckeditor_link-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/link_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/link_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/link_model/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/link_model/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.060714 django_ckeditor_link-0.5.3/ckeditor_link/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.060714 django_ckeditor_link-0.5.3/ckeditor_link/static/admin/ckeditor_link/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/static/admin/ckeditor_link/css/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/admin/ckeditor_link/css/link_admin.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/
--rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/
--rw-r--r--   0 runner    (1001) docker     (127)    53964 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
--rw-r--r--   0 runner    (1001) docker     (127)    35607 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
--rw-r--r--   0 runner    (1001) docker     (127)    18527 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
--rw-r--r--   0 runner    (1001) docker     (127)    15579 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.064714 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/
--rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/
--rw-r--r--   0 runner    (1001) docker     (127)    53964 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
--rw-r--r--   0 runner    (1001) docker     (127)    35607 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
--rw-r--r--   0 runner    (1001) docker     (127)    18527 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
--rw-r--r--   0 runner    (1001) docker     (127)    15579 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/templatetags/ckeditor_link_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.068714 django_ckeditor_link-0.5.3/ckeditor_link/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/settings_no_headless.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.072714 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.072714 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_link_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/test_templatetag.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.072714 django_ckeditor_link-0.5.3/ckeditor_link/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/utils/django_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/ckeditor_link/tests/utils/selenium_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:57:19.072714 django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-21 13:57:19.000000 django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-21 13:57:19.000000 django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:57:19.000000 django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:57:19.000000 django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 13:57:19.000000 django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 13:57:19.000000 django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:57:19.072714 django_ckeditor_link-0.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1266 2024-05-21 13:57:11.000000 django_ckeditor_link-0.5.3/setup.py
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

### Comparing `django_ckeditor_link-0.5.3/CHANGELOG.txt` & `django_ckeditor_link-0.5.3.dev0/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ==== 0.4.5 (under development) ===
 
 - ?
 
-==== 0.5.3 (2024-05-21) ===
+==== 0.5.2 (2024-05-21) ===
 
-- skip 0.5.2 due to github action / pypi troubles
 - no functional changes
 - REMOVE print statement
 - introduce pre-commit / ruff / black and other goodies
 - remove python 3.7 from test matrix
 
 
 ==== 0.5.1 (2023-06-28) ===
```

### Comparing `django_ckeditor_link-0.5.3/LICENSE` & `django_ckeditor_link-0.5.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/PKG-INFO` & `django_ckeditor_link-0.5.3.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditor-link
-Version: 0.5.3
+Version: 0.5.3.dev0
 Summary: Alternative link dialog for ckeditor 4, using django modeladmin forms.
 Home-page: http://github.com/bnzk/django-ckeditor-link
 Author: Ben Stähli
 Author-email: bnzk@bnzk.ch
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django_ckeditor_link-0.5.3/README.md` & `django_ckeditor_link-0.5.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/admin.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/admin.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/link_model/conf.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/link_model/conf.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/link_model/models.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/link_model/models.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/templatetags/ckeditor_link_tags.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/templatetags/ckeditor_link_tags.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/settings.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/admin.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/admin.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/0001_initial.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_app/models.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_app/models.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_editor.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_link_model.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_link_model.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/test_templatetag.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/test_templatetag.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/urls.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/ckeditor_link/tests/utils/selenium_utils.py` & `django_ckeditor_link-0.5.3.dev0/ckeditor_link/tests/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/PKG-INFO` & `django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditor-link
-Version: 0.5.3
+Version: 0.5.3.dev0
 Summary: Alternative link dialog for ckeditor 4, using django modeladmin forms.
 Home-page: http://github.com/bnzk/django-ckeditor-link
 Author: Ben Stähli
 Author-email: bnzk@bnzk.ch
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django_ckeditor_link-0.5.3/django_ckeditor_link.egg-info/SOURCES.txt` & `django_ckeditor_link-0.5.3.dev0/django_ckeditor_link.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/pyproject.toml` & `django_ckeditor_link-0.5.3.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_ckeditor_link-0.5.3/setup.py` & `django_ckeditor_link-0.5.3.dev0/setup.py`

 * *Files identical despite different names*

