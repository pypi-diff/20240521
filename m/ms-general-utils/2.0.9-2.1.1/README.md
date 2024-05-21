# Comparing `tmp/ms_general_utils-2.0.9.tar.gz` & `tmp/ms_general_utils-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_general_utils-2.0.9.tar", last modified: Wed Oct 25 12:00:28 2023, max compression
+gzip compressed data, was "ms_general_utils-2.1.1.tar", last modified: Tue May 21 14:12:58 2024, max compression
```

## Comparing `ms_general_utils-2.0.9.tar` & `ms_general_utils-2.1.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-10-25 12:00:28.952775 ms_general_utils-2.0.9/
--rw-rw-rw-   0        0        0     1091 2023-06-27 12:08:58.000000 ms_general_utils-2.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0      354 2023-10-25 12:00:28.951768 ms_general_utils-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      123 2023-06-27 12:08:58.000000 ms_general_utils-2.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-10-25 12:00:28.936146 ms_general_utils-2.0.9/ms_general_utils.egg-info/
--rw-rw-rw-   0        0        0      354 2023-10-25 12:00:28.000000 ms_general_utils-2.0.9/ms_general_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-10-25 12:00:28.000000 ms_general_utils-2.0.9/ms_general_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-25 12:00:28.000000 ms_general_utils-2.0.9/ms_general_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-10-25 12:00:28.000000 ms_general_utils-2.0.9/ms_general_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-10-25 12:00:28.000000 ms_general_utils-2.0.9/ms_general_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-25 12:00:28.948673 ms_general_utils-2.0.9/ms_utils/
--rw-rw-rw-   0        0        0      829 2023-10-20 14:33:14.000000 ms_general_utils-2.0.9/ms_utils/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-10-20 10:59:23.000000 ms_general_utils-2.0.9/ms_utils/abort.py
--rw-rw-rw-   0        0        0      406 2023-10-18 13:01:52.000000 ms_general_utils-2.0.9/ms_utils/abstract_model.py
--rw-rw-rw-   0        0        0     2770 2023-10-24 13:12:53.000000 ms_general_utils-2.0.9/ms_utils/authentication.py
--rw-rw-rw-   0        0        0     1073 2023-06-27 12:08:58.000000 ms_general_utils-2.0.9/ms_utils/binary_uuid.py
--rw-rw-rw-   0        0        0      629 2023-10-20 10:51:38.000000 ms_general_utils-2.0.9/ms_utils/deploy.py
-drwxrwxrwx   0        0        0        0 2023-10-25 12:00:28.950673 ms_general_utils-2.0.9/ms_utils/devops/
--rw-rw-rw-   0        0        0      718 2023-10-23 08:39:48.000000 ms_general_utils-2.0.9/ms_utils/devops/Dockerfile
-drwxrwxrwx   0        0        0        0 2023-10-25 12:00:28.950673 ms_general_utils-2.0.9/ms_utils/devops/deploy/
--rw-rw-rw-   0        0        0      185 2023-06-29 11:06:01.000000 ms_general_utils-2.0.9/ms_utils/devops/deploy/script.sh
--rw-rw-rw-   0        0        0      288 2023-06-29 08:11:09.000000 ms_general_utils-2.0.9/ms_utils/devops/docker-compose.yml
--rw-rw-rw-   0        0        0       48 2023-06-29 08:12:49.000000 ms_general_utils-2.0.9/ms_utils/devops/dockerfile.env
--rw-rw-rw-   0        0        0      727 2023-06-27 12:08:58.000000 ms_general_utils-2.0.9/ms_utils/func_date.py
--rw-rw-rw-   0        0        0     2679 2023-10-13 11:35:52.000000 ms_general_utils-2.0.9/ms_utils/generic_crud_class.py
--rw-rw-rw-   0        0        0      659 2023-09-15 11:57:39.000000 ms_general_utils-2.0.9/ms_utils/generic_pagination.py
--rw-rw-rw-   0        0        0     1527 2023-06-27 12:08:58.000000 ms_general_utils-2.0.9/ms_utils/model_utils.py
--rw-rw-rw-   0        0        0      357 2023-06-27 12:08:58.000000 ms_general_utils-2.0.9/ms_utils/prepare_json_response.py
--rw-rw-rw-   0        0        0      969 2023-10-25 10:48:33.000000 ms_general_utils-2.0.9/ms_utils/requests_utils.py
--rw-rw-rw-   0        0        0      616 2023-10-23 09:17:50.000000 ms_general_utils-2.0.9/ms_utils/schema_utils.py
--rw-rw-rw-   0        0        0      656 2023-10-25 11:59:45.000000 ms_general_utils-2.0.9/ms_utils/validation_utils.py
--rw-rw-rw-   0        0        0     7291 2023-10-25 11:59:45.000000 ms_general_utils-2.0.9/ms_utils/view_utils.py
--rw-rw-rw-   0        0        0       42 2023-10-25 12:00:28.952775 ms_general_utils-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-10-25 12:00:07.000000 ms_general_utils-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.247511 ms_general_utils-2.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2024-05-21 14:12:58.246511 ms_general_utils-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-09 14:38:49.000000 ms_general_utils-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.245510 ms_general_utils-2.1.1/ms_general_utils.egg-info/
+-rw-rw-rw-   0        0        0      354 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.242512 ms_general_utils-2.1.1/ms_utils/
+-rw-rw-rw-   0        0        0      829 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/abort.py
+-rw-rw-rw-   0        0        0      406 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/abstract_model.py
+-rw-rw-rw-   0        0        0     6714 2024-03-07 11:35:41.000000 ms_general_utils-2.1.1/ms_utils/authentication.py
+-rw-rw-rw-   0        0        0     1073 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/binary_uuid.py
+-rw-rw-rw-   0        0        0      629 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/deploy.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.244510 ms_general_utils-2.1.1/ms_utils/devops/
+-rw-rw-rw-   0        0        0      987 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/devops/Dockerfile
+-rw-rw-rw-   0        0        0     2051 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/devops/Jenkinsfile
+drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.244510 ms_general_utils-2.1.1/ms_utils/devops/deploy/
+-rw-rw-rw-   0        0        0      218 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/devops/deploy/script.sh
+-rw-rw-rw-   0        0        0      390 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/devops/docker-compose.yml
+-rw-rw-rw-   0        0        0      727 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/func_date.py
+-rw-rw-rw-   0        0        0      799 2024-02-09 13:56:55.000000 ms_general_utils-2.1.1/ms_utils/function_utils.py
+-rw-rw-rw-   0        0        0     2679 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/generic_crud_class.py
+-rw-rw-rw-   0        0        0      659 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/generic_pagination.py
+-rw-rw-rw-   0        0        0     1288 2024-02-09 13:56:52.000000 ms_general_utils-2.1.1/ms_utils/logger.py
+-rw-rw-rw-   0        0        0     1527 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/model_utils.py
+-rw-rw-rw-   0        0        0      357 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/prepare_json_response.py
+-rw-rw-rw-   0        0        0     2152 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/requests_utils.py
+-rw-rw-rw-   0        0        0      639 2024-01-12 12:24:21.000000 ms_general_utils-2.1.1/ms_utils/schema_utils.py
+-rw-rw-rw-   0        0        0      656 2023-12-04 12:35:36.000000 ms_general_utils-2.1.1/ms_utils/validation_utils.py
+-rw-rw-rw-   0        0        0     8910 2024-05-21 14:12:28.000000 ms_general_utils-2.1.1/ms_utils/view_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:12:58.247511 ms_general_utils-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-21 14:12:48.000000 ms_general_utils-2.1.1/setup.py
```

### Comparing `ms_general_utils-2.0.9/LICENSE.txt` & `ms_general_utils-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_general_utils.egg-info/SOURCES.txt` & `ms_general_utils-2.1.1/ms_general_utils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 ms_utils/__init__.py
 ms_utils/abort.py
 ms_utils/abstract_model.py
 ms_utils/authentication.py
 ms_utils/binary_uuid.py
 ms_utils/deploy.py
 ms_utils/func_date.py
+ms_utils/function_utils.py
 ms_utils/generic_crud_class.py
 ms_utils/generic_pagination.py
+ms_utils/logger.py
 ms_utils/model_utils.py
 ms_utils/prepare_json_response.py
 ms_utils/requests_utils.py
 ms_utils/schema_utils.py
 ms_utils/validation_utils.py
 ms_utils/view_utils.py
 ms_utils/devops/Dockerfile
+ms_utils/devops/Jenkinsfile
 ms_utils/devops/docker-compose.yml
-ms_utils/devops/dockerfile.env
 ms_utils/devops/deploy/script.sh
```

### Comparing `ms_general_utils-2.0.9/ms_utils/__init__.py` & `ms_general_utils-2.1.1/ms_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_utils/abort.py` & `ms_general_utils-2.1.1/ms_utils/abort.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_utils/binary_uuid.py` & `ms_general_utils-2.1.1/ms_utils/binary_uuid.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_utils/deploy.py` & `ms_general_utils-2.1.1/ms_utils/deploy.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_utils/func_date.py` & `ms_general_utils-2.1.1/ms_utils/func_date.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_utils/generic_crud_class.py` & `ms_general_utils-2.1.1/ms_utils/generic_crud_class.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_utils/generic_pagination.py` & `ms_general_utils-2.1.1/ms_utils/generic_pagination.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_utils/model_utils.py` & `ms_general_utils-2.1.1/ms_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/ms_utils/schema_utils.py` & `ms_general_utils-2.1.1/ms_utils/schema_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from flask import current_app
-import requests
+from .requests_utils import request_get
 
 
 def get_file(obj, f_key):
     """
     Get file from ms data file
     """
     obj_file = getattr(obj, f_key)
     try:
         if obj_file is None:
             return None
         url = f"{current_app.config.get('DATA_FILE_MS_URL')}/{current_app.config.get('DATA_FILE_MS_API')}/{obj_file}"
-        response = requests.get(url)
+        response = request_get(url)
         if response.status_code == 200:
             response = response.json()
             return f"{current_app.config.get('DATA_FILE_MS_URL')}{response['data']['path']}"
     except Exception:
         pass
     return None
```

### Comparing `ms_general_utils-2.0.9/ms_utils/validation_utils.py` & `ms_general_utils-2.1.1/ms_utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.0.9/setup.py` & `ms_general_utils-2.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ms_general_utils',
     packages=find_packages(),
     package_data={'ms_utils': ['devops/*', 'devops/deploy/*']},
     include_package_data=True,
-    version='2.0.9',
+    version='2.1.1',
     description='General functions for the implementation of microservices.',
     authors=[
         {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
         {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
     ],
     license="GPLv3",
     url="https://github.com/rgramos/ms-utils.git",
```

