# Comparing `tmp/maji_passport-0.0.3.tar.gz` & `tmp/maji_passport-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maji_passport-0.0.3.tar", last modified: Tue May 21 09:57:33 2024, max compression
+gzip compressed data, was "maji_passport-0.0.4.tar", last modified: Tue May 21 10:04:00 2024, max compression
```

## Comparing `maji_passport-0.0.3.tar` & `maji_passport-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.542849 maji_passport-0.0.3/
--rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-0.0.3/LICENSE
--rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 09:57:33.542849 maji_passport-0.0.3/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)       16 2024-05-20 12:56:48.000000 maji_passport-0.0.3/README.md
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/maji_passport.egg-info/
--rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     1374 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/SOURCES.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/dependency_links.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/requires.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        9 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/top_level.txt
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      401 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/admin.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/apps.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/authentication/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/authentication/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3036 2024-05-21 09:57:13.000000 maji_passport-0.0.3/passport/authentication/backend.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/management/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/management/__init__.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/management/commands/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/management/commands/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      532 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/management/commands/kafka_consumer.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      856 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/management/commands/kafka_producer_test.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      231 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/management/commands/migrate_all_users_to_passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/migrations/
--rw-rw-r--   0 teo       (1000) teo       (1000)     2229 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/0001_initial.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      521 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/0002_auto_20240418_1355.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      461 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/0004_alter_accesstoken_passport_user.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     1824 2024-05-21 08:45:40.000000 maji_passport-0.0.3/passport/models.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/serializers/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/serializers/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-0.0.3/passport/serializers/exchange.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     1852 2024-05-21 09:57:13.000000 maji_passport-0.0.3/passport/serializers/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/serializers/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.542849 maji_passport-0.0.3/passport/services/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/services/__init__.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     4485 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/services/auth.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     7013 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/services/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2977 2024-05-21 09:04:04.000000 maji_passport-0.0.3/passport/services/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      300 2024-05-21 08:41:26.000000 maji_passport-0.0.3/passport/services/passport.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-21 08:32:10.000000 maji_passport-0.0.3/passport/services/passport_migrate.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2254 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/tasks.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.542849 maji_passport-0.0.3/passport/tests/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/tests/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4005 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/tests/test_exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3016 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/tests/test_kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      958 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/urls.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.542849 maji_passport-0.0.3/passport/views/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/views/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4796 2024-05-21 08:32:10.000000 maji_passport-0.0.3/passport/views/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3728 2024-05-21 08:32:10.000000 maji_passport-0.0.3/passport/views/passport.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-21 09:57:32.000000 maji_passport-0.0.3/pyproject.toml
--rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-21 09:57:33.542849 maji_passport-0.0.3/setup.cfg
--rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-21 09:57:32.000000 maji_passport-0.0.3/setup.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.299294 maji_passport-0.0.4/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-0.0.4/LICENSE
+-rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 10:04:00.299294 maji_passport-0.0.4/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)       16 2024-05-20 12:56:48.000000 maji_passport-0.0.4/README.md
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.295294 maji_passport-0.0.4/maji_passport/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      406 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/admin.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-20 16:29:17.000000 maji_passport-0.0.4/maji_passport/apps.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.295294 maji_passport-0.0.4/maji_passport/authentication/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/authentication/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3046 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/authentication/backend.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.295294 maji_passport-0.0.4/maji_passport/management/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/management/__init__.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.295294 maji_passport-0.0.4/maji_passport/management/commands/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/management/commands/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      537 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/management/commands/kafka_consumer.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      861 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/management/commands/kafka_producer_test.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/management/commands/migrate_all_users_to_passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.299294 maji_passport-0.0.4/maji_passport/migrations/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2229 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/migrations/0001_initial.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      521 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/migrations/0002_auto_20240418_1355.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      461 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/migrations/0004_alter_accesstoken_passport_user.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/migrations/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     1824 2024-05-21 08:45:40.000000 maji_passport-0.0.4/maji_passport/models.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.299294 maji_passport-0.0.4/maji_passport/serializers/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/serializers/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-0.0.4/maji_passport/serializers/exchange.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1852 2024-05-21 09:57:13.000000 maji_passport-0.0.4/maji_passport/serializers/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/serializers/passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.299294 maji_passport-0.0.4/maji_passport/services/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/services/__init__.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     4490 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/services/auth.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     7023 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/services/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2977 2024-05-21 09:04:04.000000 maji_passport-0.0.4/maji_passport/services/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      305 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/services/passport.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-21 08:32:10.000000 maji_passport-0.0.4/maji_passport/services/passport_migrate.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.299294 maji_passport-0.0.4/maji_passport/tests/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/tests/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4010 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/tests/test_exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3026 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/tests/test_kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      968 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/urls.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.299294 maji_passport-0.0.4/maji_passport/views/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.4/maji_passport/views/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4806 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/views/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3753 2024-05-21 10:00:38.000000 maji_passport-0.0.4/maji_passport/views/passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 10:04:00.295294 maji_passport-0.0.4/maji_passport.egg-info/
+-rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 10:04:00.000000 maji_passport-0.0.4/maji_passport.egg-info/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1521 2024-05-21 10:04:00.000000 maji_passport-0.0.4/maji_passport.egg-info/SOURCES.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-21 10:04:00.000000 maji_passport-0.0.4/maji_passport.egg-info/dependency_links.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-21 10:04:00.000000 maji_passport-0.0.4/maji_passport.egg-info/requires.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)       14 2024-05-21 10:04:00.000000 maji_passport-0.0.4/maji_passport.egg-info/top_level.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-21 10:03:56.000000 maji_passport-0.0.4/pyproject.toml
+-rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-21 10:04:00.299294 maji_passport-0.0.4/setup.cfg
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-21 10:03:56.000000 maji_passport-0.0.4/setup.py
```

### Comparing `maji_passport-0.0.3/LICENSE` & `maji_passport-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/PKG-INFO` & `maji_passport-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maji_passport
-Version: 0.0.3
+Version: 0.0.4
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
 Keywords: maji passport python
```

### Comparing `maji_passport-0.0.3/maji_passport.egg-info/PKG-INFO` & `maji_passport-0.0.4/maji_passport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maji-passport
-Version: 0.0.3
+Version: 0.0.4
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
 Keywords: maji passport python
```

### Comparing `maji_passport-0.0.3/maji_passport.egg-info/SOURCES.txt` & `maji_passport-0.0.4/maji_passport.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+maji_passport/__init__.py
+maji_passport/admin.py
+maji_passport/apps.py
+maji_passport/models.py
+maji_passport/urls.py
 maji_passport.egg-info/PKG-INFO
 maji_passport.egg-info/SOURCES.txt
 maji_passport.egg-info/dependency_links.txt
 maji_passport.egg-info/requires.txt
 maji_passport.egg-info/top_level.txt
-passport/__init__.py
-passport/admin.py
-passport/apps.py
-passport/models.py
-passport/tasks.py
-passport/urls.py
-passport/authentication/__init__.py
-passport/authentication/backend.py
-passport/management/__init__.py
-passport/management/commands/__init__.py
-passport/management/commands/kafka_consumer.py
-passport/management/commands/kafka_producer_test.py
-passport/management/commands/migrate_all_users_to_passport.py
-passport/migrations/0001_initial.py
-passport/migrations/0002_auto_20240418_1355.py
-passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
-passport/migrations/0004_alter_accesstoken_passport_user.py
-passport/migrations/__init__.py
-passport/serializers/__init__.py
-passport/serializers/exchange.py
-passport/serializers/kafka.py
-passport/serializers/passport.py
-passport/services/__init__.py
-passport/services/auth.py
-passport/services/exchange.py
-passport/services/kafka.py
-passport/services/passport.py
-passport/services/passport_migrate.py
-passport/tests/__init__.py
-passport/tests/test_exchange.py
-passport/tests/test_kafka.py
-passport/views/__init__.py
-passport/views/exchange.py
-passport/views/passport.py
+maji_passport/authentication/__init__.py
+maji_passport/authentication/backend.py
+maji_passport/management/__init__.py
+maji_passport/management/commands/__init__.py
+maji_passport/management/commands/kafka_consumer.py
+maji_passport/management/commands/kafka_producer_test.py
+maji_passport/management/commands/migrate_all_users_to_passport.py
+maji_passport/migrations/0001_initial.py
+maji_passport/migrations/0002_auto_20240418_1355.py
+maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
+maji_passport/migrations/0004_alter_accesstoken_passport_user.py
+maji_passport/migrations/__init__.py
+maji_passport/serializers/__init__.py
+maji_passport/serializers/exchange.py
+maji_passport/serializers/kafka.py
+maji_passport/serializers/passport.py
+maji_passport/services/__init__.py
+maji_passport/services/auth.py
+maji_passport/services/exchange.py
+maji_passport/services/kafka.py
+maji_passport/services/passport.py
+maji_passport/services/passport_migrate.py
+maji_passport/tests/__init__.py
+maji_passport/tests/test_exchange.py
+maji_passport/tests/test_kafka.py
+maji_passport/views/__init__.py
+maji_passport/views/exchange.py
+maji_passport/views/passport.py
```

### Comparing `maji_passport-0.0.3/passport/authentication/backend.py` & `maji_passport-0.0.4/maji_passport/authentication/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import re
 
 from django.conf import settings
 from jwt import InvalidAlgorithmError, ExpiredSignatureError
 from rest_framework.exceptions import AuthenticationFailed
 
-from passport.models import AccessToken
-from passport.services.auth import RSAPassportService
+from maji_passport.models import AccessToken
+from maji_passport.services.auth import RSAPassportService
 from rest_framework_jwt.authentication import JSONWebTokenAuthentication
 
 APPLICATION_AUTHENTICATION = settings.INHERITANCE_AUTHENTICATION if getattr(settings, "APPLICATION_AUTHENTICATION")else JSONWebTokenAuthentication
 
 
 class CommonPassportBackend(APPLICATION_AUTHENTICATION):
     def check_permission(self, access_token_obj):
```

### Comparing `maji_passport-0.0.3/passport/management/commands/kafka_consumer.py` & `maji_passport-0.0.4/maji_passport/management/commands/kafka_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 
 from django.core.management.base import BaseCommand
 
-from passport.services.kafka import KafkaService
+from maji_passport.services.kafka import KafkaService
 
 
 class Command(BaseCommand):
     help = "Run Kafka consumer"
 
     def handle(self, *args, **options):
         """
```

### Comparing `maji_passport-0.0.3/passport/management/commands/kafka_producer_test.py` & `maji_passport-0.0.4/maji_passport/management/commands/kafka_producer_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import sys
 
 from django.core.management.base import BaseCommand
 
-from passport.services.kafka import KafkaService
+from maji_passport.services.kafka import KafkaService
 
 
 class Command(BaseCommand):
     help = "Execute test command to produce message to consumer"
 
     def handle(self, *args, **options):
         """
```

### Comparing `maji_passport-0.0.3/passport/migrations/0001_initial.py` & `maji_passport-0.0.4/maji_passport/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/migrations/0002_auto_20240418_1355.py` & `maji_passport-0.0.4/maji_passport/migrations/0002_auto_20240418_1355.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/migrations/0004_alter_accesstoken_passport_user.py` & `maji_passport-0.0.4/maji_passport/migrations/0004_alter_accesstoken_passport_user.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/models.py` & `maji_passport-0.0.4/maji_passport/models.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/serializers/exchange.py` & `maji_passport-0.0.4/maji_passport/serializers/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/serializers/kafka.py` & `maji_passport-0.0.4/maji_passport/serializers/kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/serializers/passport.py` & `maji_passport-0.0.4/maji_passport/serializers/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/services/auth.py` & `maji_passport-0.0.4/maji_passport/services/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import IntegrityError
 from django.conf import settings
 from jwt import InvalidAlgorithmError, ExpiredSignatureError
 from loguru import logger
 
-from passport.models import PassportUser, AccessToken, TargetAccess
+from maji_passport.models import PassportUser, AccessToken, TargetAccess
 
 User = get_user_model()
 
 
 class RSAManager:
     _instance = None
     file_data = None
```

### Comparing `maji_passport-0.0.3/passport/services/exchange.py` & `maji_passport-0.0.4/maji_passport/services/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import IntegrityError
 from loguru import logger
 from rest_framework import status
 from rest_framework.exceptions import AuthenticationFailed, PermissionDenied
 
-from passport.serializers.exchange import (
+from maji_passport.serializers.exchange import (
     TokenExchangeResponseSerializer,
     TokenExchangeCompleteSerializer,
     FullAccessTokenSerializer,
 )
-from passport.models import PassportUser, AccessToken, TargetAccess
+from maji_passport.models import PassportUser, AccessToken, TargetAccess
 
 User = get_user_model()
 
 
 class ExchangeTokenService:
     def __init__(self, email, user_uuid, user_auth_code, username, country_iso):
         self.email = email
```

### Comparing `maji_passport-0.0.3/passport/services/kafka.py` & `maji_passport-0.0.4/maji_passport/services/kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/services/passport_migrate.py` & `maji_passport-0.0.4/maji_passport/services/passport_migrate.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.3/passport/tests/test_exchange.py` & `maji_passport-0.0.4/maji_passport/tests/test_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pytest
 from django.utils import timezone
 from django.test import override_settings
 from rest_framework import status
 from rest_framework.test import APIClient
 
-from passport.models import PassportUser, AccessToken
+from maji_passport.models import PassportUser, AccessToken
 
 
 @pytest.mark.django_db
 @pytest.mark.passport
 @override_settings(
     PASSPORT_SERVICE_KEY="test_key",
     PASSPORT_EXCHANGE_URL="http://test.com/exchange/",
```

### Comparing `maji_passport-0.0.3/passport/tests/test_kafka.py` & `maji_passport-0.0.4/maji_passport/tests/test_kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import secrets
 import uuid
 
 import pytest
 from django.utils import timezone
 from django.test import override_settings
 
-from passport.models import PassportUser
-from passport.services.kafka import KafkaService
+from maji_passport.models import PassportUser
+from maji_passport.services.kafka import KafkaService
 
 
 @pytest.mark.django_db
 @pytest.mark.passport
 @override_settings(
     PASSPORT_SERVICE_KEY="test_key",
 )
```

### Comparing `maji_passport-0.0.3/passport/urls.py` & `maji_passport-0.0.4/maji_passport/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django.conf import settings
 from rest_framework.routers import DefaultRouter, SimpleRouter
 
-from passport.views.exchange import (
+from maji_passport.views.exchange import (
     ExchangeTokenViewSet,
     ServiceToken,
     UpdateUserInfo,
 )
-from passport.views.passport import (
+from maji_passport.views.passport import (
     UserPassportViewSet,
     PassportViewSet,
     ExpiredPassportViewSet,
 )
 
 if settings.DEBUG:
     router = DefaultRouter()
```

### Comparing `maji_passport-0.0.3/passport/views/exchange.py` & `maji_passport-0.0.4/maji_passport/views/exchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from rest_framework.decorators import action
 from rest_framework.exceptions import ValidationError
 from rest_framework.permissions import AllowAny
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 from rest_framework.viewsets import GenericViewSet
 
-from passport.serializers.exchange import (
+from maji_passport.serializers.exchange import (
     TokenExchangeRequestSerializer,
     ServiceKeySerializer,
     AccessTokenSerializer,
     UpdateUserInfoSerializer,
 )
-from passport.services.exchange import ExchangeTokenService
+from maji_passport.services.exchange import ExchangeTokenService
 
 User = get_user_model()
 
 
 class ExchangeTokenViewSet(GenericViewSet):
     serializer_class = TokenExchangeRequestSerializer
     permission_classes = [AllowAny]
```

### Comparing `maji_passport-0.0.3/passport/views/passport.py` & `maji_passport-0.0.4/maji_passport/views/passport.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from rest_framework import status
 from rest_framework.decorators import action
 from rest_framework.permissions import AllowAny
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 from rest_framework.viewsets import GenericViewSet
 
-from passport.authentication.backend import (
+from maji_passport.authentication.backend import (
     PassportExpireTokenBackend,
 )
-from passport.serializers.exchange import AccessTokenSerializer
-from passport.serializers.passport import (
+from maji_passport.serializers.exchange import AccessTokenSerializer
+from maji_passport.serializers.passport import (
     UserPassportSetPasswordSerializer,
     GetLoginUrlOutputSerializer,
 )
-from passport.services.exchange import ExchangeTokenService
-from passport.services.passport_migrate import PassportMigrateService
+from maji_passport.services.exchange import ExchangeTokenService
+from maji_passport.services.passport_migrate import PassportMigrateService
 
 User = get_user_model()
 
 
 class UserPassportViewSet(GenericViewSet):
     queryset = User.objects.all()
```

### Comparing `maji_passport-0.0.3/pyproject.toml` & `maji_passport-0.0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maji_passport"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Viktor Ivanov", email="viktorteodorihivanov@gmail.com" },
 ]
 description = "Maji Passport With custom authorisation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `maji_passport-0.0.3/setup.py` & `maji_passport-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='maji_passport',
-  version='0.0.3',
+  version='0.0.4',
   author='ViktorTeodorih',
   author_email='viktorteodorihivanov@gmail.com',
   description='Maji Passport With custom authorisation',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://passport.maji.la/',
   packages=find_packages(),
```

