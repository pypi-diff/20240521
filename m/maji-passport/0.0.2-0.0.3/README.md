# Comparing `tmp/maji_passport-0.0.2.tar.gz` & `tmp/maji_passport-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maji_passport-0.0.2.tar", last modified: Tue May 21 09:10:11 2024, max compression
+gzip compressed data, was "maji_passport-0.0.3.tar", last modified: Tue May 21 09:57:33 2024, max compression
```

## Comparing `maji_passport-0.0.2.tar` & `maji_passport-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.871580 maji_passport-0.0.2/
--rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-0.0.2/LICENSE
--rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 09:10:11.871580 maji_passport-0.0.2/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)       16 2024-05-20 12:56:48.000000 maji_passport-0.0.2/README.md
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.859581 maji_passport-0.0.2/maji_passport.egg-info/
--rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     1374 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/SOURCES.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/dependency_links.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/requires.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        9 2024-05-21 09:10:11.000000 maji_passport-0.0.2/maji_passport.egg-info/top_level.txt
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.863581 maji_passport-0.0.2/passport/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      401 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/admin.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/apps.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.863581 maji_passport-0.0.2/passport/authentication/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/authentication/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3032 2024-05-21 08:35:20.000000 maji_passport-0.0.2/passport/authentication/backend.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.863581 maji_passport-0.0.2/passport/management/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/management/__init__.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.863581 maji_passport-0.0.2/passport/management/commands/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/management/commands/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      532 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/management/commands/kafka_consumer.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      856 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/management/commands/kafka_producer_test.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      231 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/management/commands/migrate_all_users_to_passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.867581 maji_passport-0.0.2/passport/migrations/
--rw-rw-r--   0 teo       (1000) teo       (1000)     2229 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/0001_initial.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      521 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/0002_auto_20240418_1355.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      461 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/0004_alter_accesstoken_passport_user.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/migrations/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     1824 2024-05-21 08:45:40.000000 maji_passport-0.0.2/passport/models.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.867581 maji_passport-0.0.2/passport/serializers/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/serializers/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-0.0.2/passport/serializers/exchange.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     1847 2024-05-21 08:41:26.000000 maji_passport-0.0.2/passport/serializers/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/serializers/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.867581 maji_passport-0.0.2/passport/services/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/services/__init__.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     4485 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/services/auth.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     7013 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/services/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2977 2024-05-21 09:04:04.000000 maji_passport-0.0.2/passport/services/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      300 2024-05-21 08:41:26.000000 maji_passport-0.0.2/passport/services/passport.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-21 08:32:10.000000 maji_passport-0.0.2/passport/services/passport_migrate.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2254 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/tasks.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.867581 maji_passport-0.0.2/passport/tests/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/tests/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4005 2024-05-20 16:29:17.000000 maji_passport-0.0.2/passport/tests/test_exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3016 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/tests/test_kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      958 2024-05-20 16:29:16.000000 maji_passport-0.0.2/passport/urls.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:10:11.871580 maji_passport-0.0.2/passport/views/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.2/passport/views/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4796 2024-05-21 08:32:10.000000 maji_passport-0.0.2/passport/views/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3728 2024-05-21 08:32:10.000000 maji_passport-0.0.2/passport/views/passport.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-20 16:21:08.000000 maji_passport-0.0.2/pyproject.toml
--rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-21 09:10:11.871580 maji_passport-0.0.2/setup.cfg
--rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-20 17:54:37.000000 maji_passport-0.0.2/setup.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.542849 maji_passport-0.0.3/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-0.0.3/LICENSE
+-rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 09:57:33.542849 maji_passport-0.0.3/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)       16 2024-05-20 12:56:48.000000 maji_passport-0.0.3/README.md
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/maji_passport.egg-info/
+-rw-r--r--   0 teo       (1000) teo       (1000)     1091 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1374 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/SOURCES.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/dependency_links.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/requires.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)        9 2024-05-21 09:57:33.000000 maji_passport-0.0.3/maji_passport.egg-info/top_level.txt
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      401 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/admin.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/apps.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/authentication/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/authentication/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3036 2024-05-21 09:57:13.000000 maji_passport-0.0.3/passport/authentication/backend.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/management/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/management/__init__.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/management/commands/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/management/commands/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      532 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/management/commands/kafka_consumer.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      856 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/management/commands/kafka_producer_test.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      231 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/management/commands/migrate_all_users_to_passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/migrations/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2229 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/0001_initial.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      521 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/0002_auto_20240418_1355.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      461 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/0004_alter_accesstoken_passport_user.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/migrations/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     1824 2024-05-21 08:45:40.000000 maji_passport-0.0.3/passport/models.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.538849 maji_passport-0.0.3/passport/serializers/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/serializers/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-0.0.3/passport/serializers/exchange.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1852 2024-05-21 09:57:13.000000 maji_passport-0.0.3/passport/serializers/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/serializers/passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.542849 maji_passport-0.0.3/passport/services/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/services/__init__.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     4485 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/services/auth.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     7013 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/services/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2977 2024-05-21 09:04:04.000000 maji_passport-0.0.3/passport/services/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      300 2024-05-21 08:41:26.000000 maji_passport-0.0.3/passport/services/passport.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-21 08:32:10.000000 maji_passport-0.0.3/passport/services/passport_migrate.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2254 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/tasks.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.542849 maji_passport-0.0.3/passport/tests/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/tests/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4005 2024-05-20 16:29:17.000000 maji_passport-0.0.3/passport/tests/test_exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3016 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/tests/test_kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      958 2024-05-20 16:29:16.000000 maji_passport-0.0.3/passport/urls.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-21 09:57:33.542849 maji_passport-0.0.3/passport/views/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-0.0.3/passport/views/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4796 2024-05-21 08:32:10.000000 maji_passport-0.0.3/passport/views/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3728 2024-05-21 08:32:10.000000 maji_passport-0.0.3/passport/views/passport.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-21 09:57:32.000000 maji_passport-0.0.3/pyproject.toml
+-rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-21 09:57:33.542849 maji_passport-0.0.3/setup.cfg
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-21 09:57:32.000000 maji_passport-0.0.3/setup.py
```

### Comparing `maji_passport-0.0.2/LICENSE` & `maji_passport-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/PKG-INFO` & `maji_passport-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maji_passport
-Version: 0.0.2
+Version: 0.0.3
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
 Keywords: maji passport python
```

### Comparing `maji_passport-0.0.2/maji_passport.egg-info/PKG-INFO` & `maji_passport-0.0.3/maji_passport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maji-passport
-Version: 0.0.2
+Version: 0.0.3
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
 Keywords: maji passport python
```

### Comparing `maji_passport-0.0.2/maji_passport.egg-info/SOURCES.txt` & `maji_passport-0.0.3/maji_passport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/authentication/backend.py` & `maji_passport-0.0.3/passport/authentication/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from jwt import InvalidAlgorithmError, ExpiredSignatureError
 from rest_framework.exceptions import AuthenticationFailed
 
 from passport.models import AccessToken
 from passport.services.auth import RSAPassportService
 from rest_framework_jwt.authentication import JSONWebTokenAuthentication
 
-APPLICATION_AUTHENTICATION = settings.INHERITANCE_AUTHENTICATION if settings.get("APPLICATION_AUTHENTICATION") else JSONWebTokenAuthentication
+APPLICATION_AUTHENTICATION = settings.INHERITANCE_AUTHENTICATION if getattr(settings, "APPLICATION_AUTHENTICATION")else JSONWebTokenAuthentication
 
 
 class CommonPassportBackend(APPLICATION_AUTHENTICATION):
     def check_permission(self, access_token_obj):
         raise NotImplementedError
 
     def _authenticate_by_passport(self, request):
```

### Comparing `maji_passport-0.0.2/passport/management/commands/kafka_consumer.py` & `maji_passport-0.0.3/passport/management/commands/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/management/commands/kafka_producer_test.py` & `maji_passport-0.0.3/passport/management/commands/kafka_producer_test.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/migrations/0001_initial.py` & `maji_passport-0.0.3/passport/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/migrations/0002_auto_20240418_1355.py` & `maji_passport-0.0.3/passport/migrations/0002_auto_20240418_1355.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/migrations/0004_alter_accesstoken_passport_user.py` & `maji_passport-0.0.3/passport/migrations/0004_alter_accesstoken_passport_user.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/models.py` & `maji_passport-0.0.3/passport/models.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/serializers/exchange.py` & `maji_passport-0.0.3/passport/serializers/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/serializers/kafka.py` & `maji_passport-0.0.3/passport/serializers/kafka.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from rest_framework.serializers import Serializer
 
 from utils import clear_phone_number
 
 User = get_user_model()
 
-USER_DETAIL_SERIALIZER = settings.USER_DETAIL_SERIALIZER if settings.get("USER_DETAIL_SERIALIZER") else Serializer
+USER_DETAIL_SERIALIZER = settings.USER_DETAIL_SERIALIZER if getattr(settings, "USER_DETAIL_SERIALIZER") else Serializer
 
 
 class KafkaUpdateUserSerializer(USER_DETAIL_SERIALIZER):
     """
     Serializer for kafka update user messages
 
     phone and is_phone_verified is read_only_fields in ArgoUserDetailsSerializer
```

### Comparing `maji_passport-0.0.2/passport/serializers/passport.py` & `maji_passport-0.0.3/passport/serializers/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/services/auth.py` & `maji_passport-0.0.3/passport/services/auth.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/services/exchange.py` & `maji_passport-0.0.3/passport/services/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/services/kafka.py` & `maji_passport-0.0.3/passport/services/kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/services/passport_migrate.py` & `maji_passport-0.0.3/passport/services/passport_migrate.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/tasks.py` & `maji_passport-0.0.3/passport/tasks.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/tests/test_exchange.py` & `maji_passport-0.0.3/passport/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/tests/test_kafka.py` & `maji_passport-0.0.3/passport/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/urls.py` & `maji_passport-0.0.3/passport/urls.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/views/exchange.py` & `maji_passport-0.0.3/passport/views/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/passport/views/passport.py` & `maji_passport-0.0.3/passport/views/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-0.0.2/pyproject.toml` & `maji_passport-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maji_passport"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Viktor Ivanov", email="viktorteodorihivanov@gmail.com" },
 ]
 description = "Maji Passport With custom authorisation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `maji_passport-0.0.2/setup.py` & `maji_passport-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='maji_passport',
-  version='0.0.2',
+  version='0.0.3',
   author='ViktorTeodorih',
   author_email='viktorteodorihivanov@gmail.com',
   description='Maji Passport With custom authorisation',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://passport.maji.la/',
   packages=find_packages(),
```

