# Comparing `tmp/django_nextcloud_storage-2024.5.20.tar.gz` & `tmp/django_nextcloud_storage-2024.5.21a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nextcloud_storage-2024.5.20.tar", last modified: Mon May 20 19:15:11 2024, max compression
+gzip compressed data, was "django_nextcloud_storage-2024.5.21a1.tar", last modified: Mon May 20 20:13:53 2024, max compression
```

## Comparing `django_nextcloud_storage-2024.5.20.tar` & `django_nextcloud_storage-2024.5.21a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 abtinmiheban   (501) staff       (20)        0 2024-05-20 19:15:11.106928 django_nextcloud_storage-2024.5.20/
--rw-r--r--   0 abtinmiheban   (501) staff       (20)     1009 2024-05-20 19:15:11.106731 django_nextcloud_storage-2024.5.20/PKG-INFO
--rw-r--r--   0 abtinmiheban   (501) staff       (20)        0 2024-05-20 19:11:12.000000 django_nextcloud_storage-2024.5.20/README.md
-drwxr-xr-x   0 abtinmiheban   (501) staff       (20)        0 2024-05-20 19:15:11.105544 django_nextcloud_storage-2024.5.20/backend/
--rw-r--r--   0 abtinmiheban   (501) staff       (20)     5766 2024-05-20 18:39:42.000000 django_nextcloud_storage-2024.5.20/backend/storage.py
-drwxr-xr-x   0 abtinmiheban   (501) staff       (20)        0 2024-05-20 19:15:11.106551 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/
--rw-r--r--   0 abtinmiheban   (501) staff       (20)     1009 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/PKG-INFO
--rw-r--r--   0 abtinmiheban   (501) staff       (20)      282 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/SOURCES.txt
--rw-r--r--   0 abtinmiheban   (501) staff       (20)        1 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/dependency_links.txt
--rw-r--r--   0 abtinmiheban   (501) staff       (20)       43 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/requires.txt
--rw-r--r--   0 abtinmiheban   (501) staff       (20)        8 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/top_level.txt
--rw-r--r--   0 abtinmiheban   (501) staff       (20)     1360 2024-05-20 19:15:08.000000 django_nextcloud_storage-2024.5.20/pyproject.toml
--rw-r--r--   0 abtinmiheban   (501) staff       (20)       38 2024-05-20 19:15:11.106966 django_nextcloud_storage-2024.5.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:13:53.551893 django_nextcloud_storage-2024.5.21a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-20 20:13:53.551893 django_nextcloud_storage-2024.5.21a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:13:43.000000 django_nextcloud_storage-2024.5.21a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:13:53.551893 django_nextcloud_storage-2024.5.21a1/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-20 20:13:43.000000 django_nextcloud_storage-2024.5.21a1/backend/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:13:53.551893 django_nextcloud_storage-2024.5.21a1/django_nextcloud_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-20 20:13:53.000000 django_nextcloud_storage-2024.5.21a1/django_nextcloud_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-20 20:13:53.000000 django_nextcloud_storage-2024.5.21a1/django_nextcloud_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:13:53.000000 django_nextcloud_storage-2024.5.21a1/django_nextcloud_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 20:13:53.000000 django_nextcloud_storage-2024.5.21a1/django_nextcloud_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 20:13:53.000000 django_nextcloud_storage-2024.5.21a1/django_nextcloud_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-20 20:13:43.000000 django_nextcloud_storage-2024.5.21a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:13:53.551893 django_nextcloud_storage-2024.5.21a1/setup.cfg
```

### Comparing `django_nextcloud_storage-2024.5.20/PKG-INFO` & `django_nextcloud_storage-2024.5.21a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nextcloud-storage
-Version: 2024.5.20
+Version: 2024.5.21a1
 Summary: Django backend storage for nextcloud
 Author-email: Abtin MOHEBAN <abtin@riseup.net>
 License: MIT
 Project-URL: Homepage, https://github.com/abtinmo/django-nextcloud-storage
 Project-URL: Source, https://github.com/abtinmo/django-nextcloud-storage
 Keywords: django,nextcloud
 Classifier: Framework :: Django
```

### Comparing `django_nextcloud_storage-2024.5.20/backend/storage.py` & `django_nextcloud_storage-2024.5.21a1/backend/storage.py`

 * *Files identical despite different names*

### Comparing `django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/PKG-INFO` & `django_nextcloud_storage-2024.5.21a1/django_nextcloud_storage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nextcloud-storage
-Version: 2024.5.20
+Version: 2024.5.21a1
 Summary: Django backend storage for nextcloud
 Author-email: Abtin MOHEBAN <abtin@riseup.net>
 License: MIT
 Project-URL: Homepage, https://github.com/abtinmo/django-nextcloud-storage
 Project-URL: Source, https://github.com/abtinmo/django-nextcloud-storage
 Keywords: django,nextcloud
 Classifier: Framework :: Django
```

### Comparing `django_nextcloud_storage-2024.5.20/pyproject.toml` & `django_nextcloud_storage-2024.5.21a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 readme = "README.md"
-version = "2024.05.20"
+version = "2024.05.21-a1"
 keywords = [
   "django",
   "nextcloud",
 ]
 dependencies = [
     "Django>=4.2.0",
     "nc-py-api==0.13.0",
```

