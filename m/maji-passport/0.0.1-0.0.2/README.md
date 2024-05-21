# Comparing `tmp/maji_passport-0.0.1.tar.gz` & `tmp/maji_passport-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maji_passport-0.0.1.tar", last modified: Mon May 20 15:23:39 2024, max compression
+gzip compressed data, was "maji_passport-0.0.2.tar", last modified: Tue May 21 09:10:11 2024, max compression
```

## Comparing `maji_passport-0.0.1.tar` & `maji_passport-0.0.2.tar`

### file list

```diff
@@ -1,58 +1,56 @@
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.423148 maji_passport-0.0.1/
--rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-0.0.1/LICENSE
--rw-r--r--   0 teo       (1000) teo       (1000)      751 2024-05-20 15:23:39.423148 maji_passport-0.0.1/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)       16 2024-05-20 12:56:48.000000 maji_passport-0.0.1/README.md
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.419148 maji_passport-0.0.1/maji_passport.egg-info/
--rw-r--r--   0 teo       (1000) teo       (1000)      751 2024-05-20 15:23:39.000000 maji_passport-0.0.1/maji_passport.egg-info/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     1410 2024-05-20 15:23:39.000000 maji_passport-0.0.1/maji_passport.egg-info/SOURCES.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-20 15:23:39.000000 maji_passport-0.0.1/maji_passport.egg-info/dependency_links.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)       17 2024-05-20 15:23:39.000000 maji_passport-0.0.1/maji_passport.egg-info/requires.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        9 2024-05-20 15:23:39.000000 maji_passport-0.0.1/maji_passport.egg-info/top_level.txt
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.419148 maji_passport-0.0.1/passport/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      406 2024-05-03 09:30:57.000000 maji_passport-0.0.1/passport/admin.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      241 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/apps.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.419148 maji_passport-0.0.1/passport/authentication/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/authentication/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2878 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/authentication/backend.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.419148 maji_passport-0.0.1/passport/management/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/management/__init__.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.419148 maji_passport-0.0.1/passport/management/commands/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/management/commands/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      537 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/management/commands/kafka_consumer.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      861 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/management/commands/kafka_producer_test.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/management/commands/migrate_all_users_to_passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.419148 maji_passport-0.0.1/passport/migrations/
--rw-rw-r--   0 teo       (1000) teo       (1000)     2229 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/migrations/0001_initial.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      521 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/migrations/0002_auto_20240418_1355.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      461 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/migrations/0004_alter_accesstoken_passport_user.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/migrations/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     1482 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/models.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.423148 maji_passport-0.0.1/passport/serializers/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/serializers/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-0.0.1/passport/serializers/exchange.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     1724 2024-05-06 13:34:14.000000 maji_passport-0.0.1/passport/serializers/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/serializers/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.423148 maji_passport-0.0.1/passport/services/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/services/__init__.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     4490 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/services/auth.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     7023 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/services/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     7607 2024-05-15 10:08:48.000000 maji_passport-0.0.1/passport/services/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      318 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/services/passport.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2844 2024-05-03 09:30:57.000000 maji_passport-0.0.1/passport/services/passport_migrate.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2259 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/tasks.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.423148 maji_passport-0.0.1/passport/tests/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/tests/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4025 2024-05-17 10:23:18.000000 maji_passport-0.0.1/passport/tests/test_exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3041 2024-05-03 09:30:57.000000 maji_passport-0.0.1/passport/tests/test_kafka.py
--rw-rw-r--   0 teo       (1000) teo       (1000)       60 2024-05-17 12:12:01.000000 maji_passport-0.0.1/passport/tests.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      968 2024-05-17 09:55:24.000000 maji_passport-0.0.1/passport/urls.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-20 15:23:39.423148 maji_passport-0.0.1/passport/views/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.1/passport/views/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4769 2024-05-17 10:23:18.000000 maji_passport-0.0.1/passport/views/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3716 2024-05-17 09:55:15.000000 maji_passport-0.0.1/passport/views/passport.py
--rw-rw-r--   0 teo       (1000) teo       (1000)       63 2024-05-17 12:12:01.000000 maji_passport-0.0.1/passport/views.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-20 14:48:36.000000 maji_passport-0.0.1/pyproject.toml
--rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-20 15:23:39.423148 maji_passport-0.0.1/setup.cfg
--rw-rw-r--   0 teo       (1000) teo       (1000)      749 2024-05-20 12:51:23.000000 maji_passport-0.0.1/setup.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.871580 maji_passport-0.0.2/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-0.0.2/LICENSE
+-rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 09:10:11.871580 maji_passport-0.0.2/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)       16 2024-05-20 12:56:48.000000 maji_passport-0.0.2/README.md
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.859581 maji_passport-0.0.2/maji_passport.egg-info/
+-rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1374 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/SOURCES.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/dependency_links.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/requires.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)        9 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/top_level.txt
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.863581 maji_passport-0.0.2/passport/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      401 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/admin.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/apps.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.863581 maji_passport-0.0.2/passport/authentication/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/authentication/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3032 2024-05-21 08:35:20.000000 maji_passport-0.0.2/passport/authentication/backend.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.863581 maji_passport-0.0.2/passport/management/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/management/__init__.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.863581 maji_passport-0.0.2/passport/management/commands/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/management/commands/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      532 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/management/commands/kafka_consumer.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      856 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/management/commands/kafka_producer_test.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      231 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/management/commands/migrate_all_users_to_passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.867581 maji_passport-0.0.2/passport/migrations/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2229 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/0001_initial.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      521 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/0002_auto_20240418_1355.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      461 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/0004_alter_accesstoken_passport_user.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     1824 2024-05-21 08:45:40.000000 maji_passport-0.0.2/passport/models.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.867581 maji_passport-0.0.2/passport/serializers/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/serializers/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-0.0.2/passport/serializers/exchange.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1847 2024-05-21 08:41:26.000000 maji_passport-0.0.2/passport/serializers/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/serializers/passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.867581 maji_passport-0.0.2/passport/services/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/services/__init__.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     4485 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/services/auth.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     7013 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/services/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2977 2024-05-21 09:04:04.000000 maji_passport-0.0.2/passport/services/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      300 2024-05-21 08:41:26.000000 maji_passport-0.0.2/passport/services/passport.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-21 08:32:10.000000 maji_passport-0.0.2/passport/services/passport_migrate.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2254 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/tasks.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.867581 maji_passport-0.0.2/passport/tests/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/tests/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4005 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/tests/test_exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3016 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/tests/test_kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      958 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/urls.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.871580 maji_passport-0.0.2/passport/views/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/views/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4796 2024-05-21 08:32:10.000000 maji_passport-0.0.2/passport/views/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3728 2024-05-21 08:32:10.000000 maji_passport-0.0.2/passport/views/passport.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-20 16:21:08.000000 maji_passport-0.0.2/pyproject.toml
+-rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-21 09:10:11.871580 maji_passport-0.0.2/setup.cfg
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-20 17:54:37.000000 maji_passport-0.0.2/setup.py
```

### Comparing `maji_passport-0.0.1/LICENSE` & `maji_passport-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.1/maji_passport.egg-info/SOURCES.txt` & `maji_passport-0.0.2/maji_passport.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 maji_passport.egg-info/requires.txt
 maji_passport.egg-info/top_level.txt
 passport/__init__.py
 passport/admin.py
 passport/apps.py
 passport/models.py
 passport/tasks.py
-passport/tests.py
 passport/urls.py
-passport/views.py
 passport/authentication/__init__.py
 passport/authentication/backend.py
 passport/management/__init__.py
 passport/management/commands/__init__.py
 passport/management/commands/kafka_consumer.py
 passport/management/commands/kafka_producer_test.py
 passport/management/commands/migrate_all_users_to_passport.py
```

### Comparing `maji_passport-0.0.1/passport/authentication/backend.py` & `maji_passport-0.0.2/passport/authentication/backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import datetime
 import re
 
+from django.conf import settings
 from jwt import InvalidAlgorithmError, ExpiredSignatureError
-from rest_framework.exceptions import AuthenticationFailed, PermissionDenied
+from rest_framework.exceptions import AuthenticationFailed
 
-from argo.passport.models import AccessToken
-from argo.passport.services.auth import RSAPassportService
-from argo.utils.drf_stuff import ArgoJSONWebTokenAuthentication
+from passport.models import AccessToken
+from passport.services.auth import RSAPassportService
+from rest_framework_jwt.authentication import JSONWebTokenAuthentication
 
+APPLICATION_AUTHENTICATION = settings.INHERITANCE_AUTHENTICATION if settings.get("APPLICATION_AUTHENTICATION") else JSONWebTokenAuthentication
 
-class CommonPassportBackend(ArgoJSONWebTokenAuthentication):
+
+class CommonPassportBackend(APPLICATION_AUTHENTICATION):
     def check_permission(self, access_token_obj):
         raise NotImplementedError
 
     def _authenticate_by_passport(self, request):
         """
         New authentication logic here
         Return the user object if authentication is successful, None otherwise"
```

### Comparing `maji_passport-0.0.1/passport/management/commands/kafka_consumer.py` & `maji_passport-0.0.2/passport/management/commands/kafka_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 
 from django.core.management.base import BaseCommand
 
-from argo.passport.services.kafka import KafkaService
+from passport.services.kafka import KafkaService
 
 
 class Command(BaseCommand):
     help = "Run Kafka consumer"
 
     def handle(self, *args, **options):
         """
```

### Comparing `maji_passport-0.0.1/passport/management/commands/kafka_producer_test.py` & `maji_passport-0.0.2/passport/management/commands/kafka_producer_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import sys
 
 from django.core.management.base import BaseCommand
 
-from argo.passport.services.kafka import KafkaService
+from passport.services.kafka import KafkaService
 
 
 class Command(BaseCommand):
     help = "Execute test command to produce message to consumer"
 
     def handle(self, *args, **options):
         """
```

### Comparing `maji_passport-0.0.1/passport/migrations/0001_initial.py` & `maji_passport-0.0.2/passport/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.1/passport/migrations/0002_auto_20240418_1355.py` & `maji_passport-0.0.2/passport/migrations/0002_auto_20240418_1355.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.1/passport/migrations/0004_alter_accesstoken_passport_user.py` & `maji_passport-0.0.2/passport/migrations/0004_alter_accesstoken_passport_user.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.1/passport/models.py` & `maji_passport-0.0.2/passport/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,35 @@
 from django.db.models import (
     SET_NULL,
     CharField,
     DateTimeField,
     ForeignKey,
     TextChoices,
     OneToOneField,
-    CASCADE,
+    CASCADE, Model,
 )
 from django.db.models.fields import UUIDField, TextField
 from django.utils import timezone
 
-from argo.common.models import BaseModel
-
+try:
+    from django.db.models import JSONField
+except ImportError:
+    from django.contrib.postgres.fields import JSONField
 User = get_user_model()
 
 
+class BaseModel(Model):
+    class Meta:
+        abstract = True
+
+    created_at = DateTimeField(auto_now_add=True, db_index=True)
+    updated_at = DateTimeField(auto_now=True, db_index=True)
+    extra = JSONField(default=dict, blank=True, null=True)
+
+
 class PassportUser(BaseModel):
     argo_user = OneToOneField(User, null=True, on_delete=SET_NULL)
     passport_uuid = UUIDField(null=False)
     user_auth_code = CharField(max_length=255, null=False)
     refresh_token = TextField()
 
     def __str__(self):
```

### Comparing `maji_passport-0.0.1/passport/serializers/exchange.py` & `maji_passport-0.0.2/passport/serializers/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.1/passport/serializers/kafka.py` & `maji_passport-0.0.2/passport/serializers/kafka.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from django.conf import settings
+from django.contrib.auth import get_user_model
 from rest_framework.fields import BooleanField, CharField
 
-from argo.common.models import Image
-from argo.common.utils import clear_phone_number
-from argo.users.api.serializers.auth import ArgoUserDetailsSerializer
-from argo.users.models import User
+from rest_framework.serializers import Serializer
 
+from utils import clear_phone_number
 
-class KafkaUpdateUserSerializer(ArgoUserDetailsSerializer):
+User = get_user_model()
+
+USER_DETAIL_SERIALIZER = settings.USER_DETAIL_SERIALIZER if settings.get("USER_DETAIL_SERIALIZER") else Serializer
+
+
+class KafkaUpdateUserSerializer(USER_DETAIL_SERIALIZER):
     """
     Serializer for kafka update user messages
 
     phone and is_phone_verified is read_only_fields in ArgoUserDetailsSerializer
     and here we must declare them read_only=False and required=False
     """
     phone = CharField(read_only=False, required=False, allow_blank=True)
@@ -28,12 +33,12 @@
         if "phone" in validated_data and validated_data["phone"]:
             old_users = User.objects.filter(phone=validated_data["phone"])
             old_users.update(phone="", is_phone_verified=False)
         # update avatar from kafka.
         # otherwise rise errors:
         # - ValueError: Cannot assign "3743": "User.avatar" must be a "Image" instance
         # - Incorrect type. Expected pk value, received Image.
-        if "avatar" in validated_data and validated_data["avatar"]:
-            avatar_id = validated_data.pop("avatar")
-            avatar = Image.objects.get(id=avatar_id)
-            instance.avatar = avatar
+        # if "avatar" in validated_data and validated_data["avatar"]:
+        #     avatar_id = validated_data.pop("avatar")
+        #     avatar = Image.objects.get(id=avatar_id)
+        #     instance.avatar = avatar
         return super().update(instance, validated_data)
```

### Comparing `maji_passport-0.0.1/passport/serializers/passport.py` & `maji_passport-0.0.2/passport/serializers/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.1/passport/services/auth.py` & `maji_passport-0.0.2/passport/services/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import IntegrityError
 from django.conf import settings
 from jwt import InvalidAlgorithmError, ExpiredSignatureError
 from loguru import logger
 
-from argo.passport.models import PassportUser, AccessToken, TargetAccess
+from passport.models import PassportUser, AccessToken, TargetAccess
 
 User = get_user_model()
 
 
 class RSAManager:
     _instance = None
     file_data = None
```

### Comparing `maji_passport-0.0.1/passport/services/exchange.py` & `maji_passport-0.0.2/passport/services/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import IntegrityError
 from loguru import logger
 from rest_framework import status
 from rest_framework.exceptions import AuthenticationFailed, PermissionDenied
 
-from argo.passport.serializers.exchange import (
+from passport.serializers.exchange import (
     TokenExchangeResponseSerializer,
     TokenExchangeCompleteSerializer,
     FullAccessTokenSerializer,
 )
-from argo.passport.models import PassportUser, AccessToken, TargetAccess
+from passport.models import PassportUser, AccessToken, TargetAccess
 
 User = get_user_model()
 
 
 class ExchangeTokenService:
     def __init__(self, email, user_uuid, user_auth_code, username, country_iso):
         self.email = email
```

### Comparing `maji_passport-0.0.1/passport/services/passport_migrate.py` & `maji_passport-0.0.2/passport/services/passport_migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import operator
 from typing import List
 
 import httpx
 import loguru
 import sentry_sdk
 from django.conf import settings
+from django.contrib.auth import get_user_model
 from httpx import Response
 from rest_framework import status
 
-from argo.users.models import User
+User = get_user_model()
 
 
 class PassportMigrateService:
     """
     Service for migrate users to passport
     """
```

### Comparing `maji_passport-0.0.1/passport/tasks.py` & `maji_passport-0.0.2/passport/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from django.contrib.auth import get_user_model
 from django.db.models import Q
 
-from argo.passport.services.passport_migrate import PassportMigrateService
+from passport.services.passport_migrate import PassportMigrateService
 from config import celery_app
 
 User = get_user_model()
 
 
 @celery_app.task
 def migrate_users_to_passport_task(ids: List[int]):
```

### Comparing `maji_passport-0.0.1/passport/tests/test_exchange.py` & `maji_passport-0.0.2/passport/tests/test_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pytest
 from django.utils import timezone
 from django.test import override_settings
 from rest_framework import status
 from rest_framework.test import APIClient
 
-from argo.passport.models import PassportUser, AccessToken
+from passport.models import PassportUser, AccessToken
 
 
 @pytest.mark.django_db
 @pytest.mark.passport
 @override_settings(
     PASSPORT_SERVICE_KEY="test_key",
     PASSPORT_EXCHANGE_URL="http://test.com/exchange/",
@@ -23,25 +23,25 @@
 def test_exchange(create_user, auth_fabric, faker, mocker):
     passport_user_uuid = uuid.uuid4()
     user_auth_code = secrets.token_hex(16)
     access_token = secrets.token_hex(32)
     access_token_expiration = datetime.now() + timedelta(hours=20)
     refresh_token = secrets.token_hex(32)
     mocker.patch(
-        "argo.passport.services.exchange.ExchangeTokenService._send_post_request",
+        "passport.services.exchange.ExchangeTokenService._send_post_request",
         return_value={
             "user_uuid": passport_user_uuid,
             "user_auth_code": user_auth_code,
             "access_token": access_token,
             "access_token_expiration": str(access_token_expiration),
             "refresh_token": refresh_token,
         },
     )
     mocker.patch(
-        "argo.passport.services.exchange.ExchangeTokenService.save_tokens",
+        "passport.services.exchange.ExchangeTokenService.save_tokens",
         return_value=True,
     )
 
     u_requester = create_user(
         email=faker.email(),
         registered_at=timezone.now(),
         is_registered=True,
@@ -63,15 +63,15 @@
     passport_user_uuid = uuid.uuid4()
     user_auth_code = secrets.token_hex(16)
     access_token = secrets.token_hex(32)
     refresh_token = secrets.token_hex(32)
     new_access_token = secrets.token_hex(32)
 
     mocker.patch(
-        "argo.passport.services.exchange.ExchangeTokenService.update_token_by_refresh",
+        "passport.services.exchange.ExchangeTokenService.update_token_by_refresh",
         return_value=new_access_token,
     )
 
     u_requester = create_user(
         email=faker.email(),
         registered_at=timezone.now(),
         is_registered=True,
```

### Comparing `maji_passport-0.0.1/passport/tests/test_kafka.py` & `maji_passport-0.0.2/passport/tests/test_kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import secrets
 import uuid
 
 import pytest
 from django.utils import timezone
 from django.test import override_settings
 
-from argo.passport.models import PassportUser
-from argo.passport.services.kafka import KafkaService
+from passport.models import PassportUser
+from passport.services.kafka import KafkaService
 
 
 @pytest.mark.django_db
 @pytest.mark.passport
 @override_settings(
     PASSPORT_SERVICE_KEY="test_key",
 )
@@ -21,15 +21,15 @@
         "action": "logout",
         "user_auth_code": user_auth_code,
         "description": "test_description",
         "service_key": "test_key",
     }
     return_value = json.dumps(return_value)
     mocker.patch(
-        "argo.passport.services.kafka.KafkaService._decode_message",
+        "passport.services.kafka.KafkaService._decode_message",
         return_value=return_value,
     )
 
     passport_user_uuid = uuid.uuid4()
 
     u_requester = create_user(
         email=faker.email(),
@@ -53,15 +53,15 @@
         "description": "test_description",
         "service_key": "test_key",
         "extra": {"username": new_username},
     }
     return_value = json.dumps(return_value)
 
     mocker.patch(
-        "argo.passport.services.kafka.KafkaService._decode_message",
+        "passport.services.kafka.KafkaService._decode_message",
         return_value=return_value,
     )
     service.process_message("")
     new_passport = PassportUser.objects.get(user_auth_code=user_auth_code)
     assert new_passport.argo_user.username == new_username
     assert new_passport.argo_user.display_name == new_username
 
@@ -86,15 +86,15 @@
             "phone": new_phone,
             "is_phone_verified": True,
         },
     }
     return_value = json.dumps(return_value)
 
     mocker.patch(
-        "argo.passport.services.kafka.KafkaService._decode_message",
+        "passport.services.kafka.KafkaService._decode_message",
         return_value=return_value,
     )
     service.process_message("")
     new_passport = PassportUser.objects.get(user_auth_code=user_auth_code)
     assert new_passport.argo_user.phone == new_phone
     assert new_passport.argo_user.is_phone_verified is True
```

### Comparing `maji_passport-0.0.1/passport/urls.py` & `maji_passport-0.0.2/passport/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django.conf import settings
 from rest_framework.routers import DefaultRouter, SimpleRouter
 
-from argo.passport.views.exchange import (
+from passport.views.exchange import (
     ExchangeTokenViewSet,
     ServiceToken,
     UpdateUserInfo,
 )
-from argo.passport.views.passport import (
+from passport.views.passport import (
     UserPassportViewSet,
     PassportViewSet,
     ExpiredPassportViewSet,
 )
 
 if settings.DEBUG:
     router = DefaultRouter()
```

### Comparing `maji_passport-0.0.1/passport/views/exchange.py` & `maji_passport-0.0.2/passport/views/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from urllib.parse import urlencode
 
 import httpx
 import loguru
 from django.conf import settings
+from django.contrib.auth import get_user_model
 from drf_yasg.utils import swagger_auto_schema
 from rest_framework import status
 from rest_framework.decorators import action
 from rest_framework.exceptions import ValidationError
 from rest_framework.permissions import AllowAny
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 from rest_framework.viewsets import GenericViewSet
 
-from argo.passport.serializers.exchange import (
+from passport.serializers.exchange import (
     TokenExchangeRequestSerializer,
     ServiceKeySerializer,
     AccessTokenSerializer,
     UpdateUserInfoSerializer,
 )
-from argo.passport.services.exchange import ExchangeTokenService
-from argo.users.models import User
+from passport.services.exchange import ExchangeTokenService
+
+User = get_user_model()
 
 
 class ExchangeTokenViewSet(GenericViewSet):
     serializer_class = TokenExchangeRequestSerializer
     permission_classes = [AllowAny]
 
     @swagger_auto_schema(
```

### Comparing `maji_passport-0.0.1/passport/views/passport.py` & `maji_passport-0.0.2/passport/views/passport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import datetime
 from urllib.parse import urlencode
 
 from django.conf import settings
+from django.contrib.auth import get_user_model
 from django.utils import timezone
 from drf_yasg.utils import swagger_auto_schema
 from rest_framework import status
 from rest_framework.decorators import action
 from rest_framework.permissions import AllowAny
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 from rest_framework.viewsets import GenericViewSet
 
-from argo.passport.authentication.backend import (
+from passport.authentication.backend import (
     PassportExpireTokenBackend,
 )
-from argo.passport.serializers.exchange import AccessTokenSerializer
-from argo.passport.serializers.passport import (
+from passport.serializers.exchange import AccessTokenSerializer
+from passport.serializers.passport import (
     UserPassportSetPasswordSerializer,
     GetLoginUrlOutputSerializer,
 )
-from argo.passport.services.exchange import ExchangeTokenService
-from argo.users.models import User
-from argo.passport.services.passport_migrate import PassportMigrateService
+from passport.services.exchange import ExchangeTokenService
+from passport.services.passport_migrate import PassportMigrateService
+
+User = get_user_model()
 
 
 class UserPassportViewSet(GenericViewSet):
     queryset = User.objects.all()
 
     @action(
         detail=False,
```

### Comparing `maji_passport-0.0.1/pyproject.toml` & `maji_passport-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maji_passport"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Viktor Ivanov", email="viktorteodorihivanov@gmail.com" },
 ]
 description = "Maji Passport With custom authorisation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

