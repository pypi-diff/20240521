# Comparing `tmp/django_webhook-0.0.8.tar.gz` & `tmp/django_webhook-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_webhook-0.0.8.tar", max compression
+gzip compressed data, was "django_webhook-0.0.9.tar", max compression
```

## Comparing `django_webhook-0.0.8.tar` & `django_webhook-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-07-03 15:49:26.008503 django_webhook-0.0.8/LICENSE
--rw-r--r--   0        0        0       22 2023-07-03 15:49:26.008503 django_webhook-0.0.8/django_webhook/__init__.py
--rw-r--r--   0        0        0     1130 2023-09-18 03:43:08.838398 django_webhook-0.0.8/django_webhook/admin.py
--rw-r--r--   0        0        0      698 2023-09-18 03:21:20.341116 django_webhook-0.0.8/django_webhook/apps.py
--rw-r--r--   0        0        0     1516 2023-07-10 14:34:51.663506 django_webhook-0.0.8/django_webhook/checks.py
--rw-r--r--   0        0        0      238 2023-09-17 01:57:09.005898 django_webhook-0.0.8/django_webhook/forms.py
--rw-r--r--   0        0        0     1412 2024-01-30 12:35:38.759617 django_webhook-0.0.8/django_webhook/http.py
--rw-r--r--   0        0        0     4203 2023-09-17 01:31:56.871387 django_webhook-0.0.8/django_webhook/migrations/0001_initial.py
--rw-r--r--   0        0        0     2460 2023-09-17 01:31:56.871387 django_webhook-0.0.8/django_webhook/migrations/0002_webhookevent.py
--rw-r--r--   0        0        0      556 2023-09-28 08:48:38.220003 django_webhook-0.0.8/django_webhook/migrations/0003_alter_webhook_created_alter_webhook_modified.py
--rw-r--r--   0        0        0      602 2024-01-30 12:35:38.759617 django_webhook-0.0.8/django_webhook/migrations/0004_alter_webhookevent_created_and_more.py
--rw-r--r--   0        0        0      408 2023-10-20 20:52:28.624557 django_webhook-0.0.8/django_webhook/migrations/0005_alter_webhook_url.py
--rw-r--r--   0        0        0        0 2023-07-10 14:34:51.663506 django_webhook-0.0.8/django_webhook/migrations/__init__.py
--rw-r--r--   0        0        0     3835 2024-01-30 12:35:22.175554 django_webhook-0.0.8/django_webhook/models.py
--rw-r--r--   0        0        0      197 2023-09-18 03:43:08.838398 django_webhook-0.0.8/django_webhook/settings.py
--rw-r--r--   0        0        0     3643 2024-01-30 12:35:22.175554 django_webhook-0.0.8/django_webhook/signals.py
--rw-r--r--   0        0        0        0 2023-07-03 15:49:26.008503 django_webhook-0.0.8/django_webhook/static/webhooks/css/.gitkeep
--rw-r--r--   0        0        0        0 2023-07-03 15:49:26.008503 django_webhook-0.0.8/django_webhook/static/webhooks/images/.gitkeep
--rw-r--r--   0        0        0        0 2023-07-03 15:49:26.008503 django_webhook-0.0.8/django_webhook/static/webhooks/js/.gitkeep
--rw-r--r--   0        0        0     2173 2024-01-30 12:35:22.175554 django_webhook-0.0.8/django_webhook/tasks.py
--rw-r--r--   0        0        0        0 2023-07-03 15:49:26.008503 django_webhook-0.0.8/django_webhook/templates/webhooks/.gitkeep
--rw-r--r--   0        0        0     1321 2023-09-17 01:57:09.005898 django_webhook-0.0.8/django_webhook/test_factories.py
--rw-r--r--   0        0        0       84 2023-07-10 14:34:51.667506 django_webhook-0.0.8/django_webhook/urls.py
--rw-r--r--   0        0        0      682 2023-09-28 01:09:05.572001 django_webhook-0.0.8/django_webhook/util.py
--rw-r--r--   0        0        0      684 2023-07-10 14:34:51.667506 django_webhook-0.0.8/django_webhook/validators.py
--rw-r--r--   0        0        0     1242 2024-01-30 12:35:38.759617 django_webhook-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 django_webhook-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-03 15:49:26.008503 django_webhook-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1486 2024-05-21 19:42:16.218882 django_webhook-0.0.9/README.md
+-rw-r--r--   0        0        0       22 2023-07-03 15:49:26.008503 django_webhook-0.0.9/django_webhook/__init__.py
+-rw-r--r--   0        0        0     1130 2023-09-18 03:43:08.838398 django_webhook-0.0.9/django_webhook/admin.py
+-rw-r--r--   0        0        0      698 2023-09-18 03:21:20.341116 django_webhook-0.0.9/django_webhook/apps.py
+-rw-r--r--   0        0        0     1516 2023-07-10 14:34:51.663506 django_webhook-0.0.9/django_webhook/checks.py
+-rw-r--r--   0        0        0      238 2023-09-17 01:57:09.005898 django_webhook-0.0.9/django_webhook/forms.py
+-rw-r--r--   0        0        0     1412 2024-01-30 12:35:38.759617 django_webhook-0.0.9/django_webhook/http.py
+-rw-r--r--   0        0        0     4203 2023-09-17 01:31:56.871387 django_webhook-0.0.9/django_webhook/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2460 2023-09-17 01:31:56.871387 django_webhook-0.0.9/django_webhook/migrations/0002_webhookevent.py
+-rw-r--r--   0        0        0      556 2023-09-28 08:48:38.220003 django_webhook-0.0.9/django_webhook/migrations/0003_alter_webhook_created_alter_webhook_modified.py
+-rw-r--r--   0        0        0      602 2024-01-30 12:35:38.759617 django_webhook-0.0.9/django_webhook/migrations/0004_alter_webhookevent_created_and_more.py
+-rw-r--r--   0        0        0      408 2023-10-20 20:52:28.624557 django_webhook-0.0.9/django_webhook/migrations/0005_alter_webhook_url.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:34:51.663506 django_webhook-0.0.9/django_webhook/migrations/__init__.py
+-rw-r--r--   0        0        0     3835 2024-01-30 12:35:22.175554 django_webhook-0.0.9/django_webhook/models.py
+-rw-r--r--   0        0        0      197 2023-09-18 03:43:08.838398 django_webhook-0.0.9/django_webhook/settings.py
+-rw-r--r--   0        0        0     3643 2024-01-30 12:35:22.175554 django_webhook-0.0.9/django_webhook/signals.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:49:26.008503 django_webhook-0.0.9/django_webhook/static/webhooks/css/.gitkeep
+-rw-r--r--   0        0        0        0 2023-07-03 15:49:26.008503 django_webhook-0.0.9/django_webhook/static/webhooks/images/.gitkeep
+-rw-r--r--   0        0        0        0 2023-07-03 15:49:26.008503 django_webhook-0.0.9/django_webhook/static/webhooks/js/.gitkeep
+-rw-r--r--   0        0        0     2173 2024-01-30 12:35:22.175554 django_webhook-0.0.9/django_webhook/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:49:26.008503 django_webhook-0.0.9/django_webhook/templates/webhooks/.gitkeep
+-rw-r--r--   0        0        0     1321 2023-09-17 01:57:09.005898 django_webhook-0.0.9/django_webhook/test_factories.py
+-rw-r--r--   0        0        0       84 2023-07-10 14:34:51.667506 django_webhook-0.0.9/django_webhook/urls.py
+-rw-r--r--   0        0        0      682 2023-09-28 01:09:05.572001 django_webhook-0.0.9/django_webhook/util.py
+-rw-r--r--   0        0        0      684 2023-07-10 14:34:51.667506 django_webhook-0.0.9/django_webhook/validators.py
+-rw-r--r--   0        0        0     1263 2024-05-21 19:42:36.598811 django_webhook-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 django_webhook-0.0.9/PKG-INFO
```

### Comparing `django_webhook-0.0.8/LICENSE` & `django_webhook-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/admin.py` & `django_webhook-0.0.9/django_webhook/admin.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/apps.py` & `django_webhook-0.0.9/django_webhook/apps.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/checks.py` & `django_webhook-0.0.9/django_webhook/checks.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/http.py` & `django_webhook-0.0.9/django_webhook/http.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/migrations/0001_initial.py` & `django_webhook-0.0.9/django_webhook/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/migrations/0002_webhookevent.py` & `django_webhook-0.0.9/django_webhook/migrations/0002_webhookevent.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/migrations/0003_alter_webhook_created_alter_webhook_modified.py` & `django_webhook-0.0.9/django_webhook/migrations/0003_alter_webhook_created_alter_webhook_modified.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/migrations/0004_alter_webhookevent_created_and_more.py` & `django_webhook-0.0.9/django_webhook/migrations/0004_alter_webhookevent_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/models.py` & `django_webhook-0.0.9/django_webhook/models.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/signals.py` & `django_webhook-0.0.9/django_webhook/signals.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/tasks.py` & `django_webhook-0.0.9/django_webhook/tasks.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/test_factories.py` & `django_webhook-0.0.9/django_webhook/test_factories.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/util.py` & `django_webhook-0.0.9/django_webhook/util.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/django_webhook/validators.py` & `django_webhook-0.0.9/django_webhook/validators.py`

 * *Files identical despite different names*

### Comparing `django_webhook-0.0.8/pyproject.toml` & `django_webhook-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "django-webhook"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Dani Hodovic <you@example.com>"]
 license = "MIT"
+readme = "README.md"
 
 [tool.black]
 skip_numeric_underscore_normalization = true
 exclude = ".*(venv|virtualenv|.poetry|migrations|node_modules)"
 
 [tool.isort]
 profile = "black"
```

